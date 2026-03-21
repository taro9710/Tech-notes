# COMÁNDOS ÚTILES DE GIT
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

## ssh agent
Para agregar mi `ssh-key` un a `ssh-agent` para que este recuerde tu `passphrase`, evitando que tenga que ingresarla cada vez que uses la clave. Esto es útil para simplificar la autenticación mientras mantienes la seguridad de tu clave (osea cada vez que haga un `git pull` o un `git push`).
1. Primero inicializamos el `ssh-agent`en segundo plano:

        eval "$(ssh-agent -s)"
        >Agent pid [algún número]

2. Agrega tu clave privada al ssh-agent (siempre y cuando la clave privada este con el nombre por defaul)

        ssh-add ~/.ssh/id_ed25519
