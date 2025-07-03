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
## GIT
- Para  inicializar GIT en nuestro proyecto.

        git init
- Para conectarnos a un servidor y descargar una copia de ese proyecto en nuestra computadora

        git clone [URL]
- El siguiente comando sirve para conectar a un repositorio. Es muy útil cuando ya hemos inicializado un repositorio git local por lo que no queremos clonarlo con el repositorio del servidor. 

        git remote add origin [URL]
- Para traer los cambios a nuestro repositorio local
        git pull
- Sube los cambios al servidor, para poder compartirlos y hacer un backup de nuetros datos

        git push
- Nos muestra el estado de nuestra copia remota

        git status
- Para agregar archivos hasta el staging area, un índice que te permite preparar los cambios que querés incluir en el próximo commit, antes de confirmarlos definitivamente.

        git add [file_name]
- Agrega todos los archvios al staging area
        
        git add -A / git add .

- Crea una nueva revisión. `-m` (message) será el título del commit con los cambios.

        git commit -m "some message"
- Para ver el historial de versiones del proyecto, mostrando de manera cronológica todas las revisiones hechas con fecha, autor y descripción.

        git log
- Muestra más historial que `git log` pero es menos detallado.

        git log --oneline
- Para un historial detallado, donde se muestra quien modificó y cuando se modificó el proyecto junto con los cambios exactos.
        
        git log -p
- Para ver los cambios en un de un archivo específico.
        
        git log -- [file_name] 
    **Warning**, Hay un espacio entre `--` & `file_name`.
- Para ver lo cambios que tienen los archivos que no han sido agregado a un commit:

        git diff
- Para ver las ramas locales (también sirve para ver en cuál rema se está trabajando).

        git branch
- Para crear una rama con un nombre específico

        git branch [branch_name]     
- Unir ("mergear") dos ramas.

        git merge [branch_name]

    (Nombro la rama que quiero mergear sobre la rama en la que estoy parado. Osea que traigo los cambios a la rama en la que estoy parado)
- Para eliminar una rama.

        git branch -d [branch_name]
- Si queremos cambiar la rama en la que estamos trabajando a otra.
        
        git checkout [branch_name]