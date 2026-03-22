# COMANDOS ÚTILES
Ester archivo se utilizará para ir agrupando listas de comandos para ir aprendiendo en linux.

## Linux MINT
- Apagar computadora:
        
        sudo poweroff
        sudo shutdown now
        sudo shutdown -h xx:xx (hora específica formato 24hs)

- Reiniciar computadora:
        
        sudo reboot

- Suspender Computadora:
        
        systemclt suspend

- Comando útil para mantener mi sistema Linux Mint (o cualquier distro basado en Ubunto/Debian) actualizado y limpio:

        sudo apt update && sudo apt upgrade -y && sudo apt autoremove -y && sudo apt autoclean

  Donde `-y` sirve para aceptar automáticamente. También lo pongo por separado para poder explicar cada uno o para poder hacerlo de manera secuencial.
- Para actualizar la lista de paquetes disponible (consultando los repositorios).

        sudo apt update

- Para instalar las actualizaciones de los paquetes que ya tenés en el sistema.

        sudo apt upgrade

- para eliminar paquetes que ya no son necesarios (por ejemplo librerías que fueron instaladas como dependencias pero que ya no se usan.)

        sudo apt autoremove

- Para borrar archivos .deb antiguos del caché local que ya no se pueden volver a instalar o actualizar.

        sudo apt autoclean
- Para ver si un proceso se está ejecutando

        ps aux | grep [nombre del proceso]
    El nombre del proceso puede ser el de `brave` para el Browser de Brave o `code` para VS CODE
- Para concatenar archivos de texto en consola:

        cat archivo.txt
- Al igual que `cat` también tengo la siguiente opción que es igual pero tiene algunas funcionalidades gráficas que pueden llegar a ser útilies como por ej.  el resaltado de los archivos de md.

        batcat archivo.md

- Para saber cuánto tarda en arrancar la pc:
        
        systemd-analyze
- Para ver qué es lo que tarda cada proceso: 

        systemd-analyze blame
- Para crear un directorio:

        mkdir
- Para crear archivos:

        touch [archivo]
        
  Ejemplo: Para crear un archvio de texto de ejemplo utilizo: **touch ejemplo.txt**

- Para eliminar archivos:

        rm [archivo]

  **Warning:** No va a ir a una papelera. Lo elimina

- Para eliminar un directorio: 

        rm -r [directorio]

