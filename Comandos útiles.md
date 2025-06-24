# COMANDOS ÚTILES
Ester archivo se utilizará para ir agrupando listas de comandos para ir aprendiendo en linux.

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