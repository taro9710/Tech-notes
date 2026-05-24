# NeoVim keys

## Modos Básicos y Navegación.

### Mapa de Modos y Teclas de Navegación 

    |   i   | Modo Insert|
    |  Esc  | Modo Normal|
    |   v   | Modo Visual|    
    |   h   | Izquierda  |
    |   j   | Abajo      |
    |   k   | Arriba     |
    |   l   | Derecha    |
    |   o   | Nueva Linea|
    |   :   | Modo Comand|    
    |  :w   | Guardar    | 
    |  :q   | Salir      |
    |  :q!  | Salir!     |
    |  :qa  | Cerrar Todo|
    |  :wq  | Write&Quit |
    |  :e   | Editar     |


- `i` : El modo insert me siver para poder entrar al modo de edición de texto. Este modo me permite escribir en el archivo de texto.
- `Esc` : Me permite ponerme en el modo estándar cuando entro a vim y utilizar los comandos de ese modo (como lo de navegación).
- `v` : El modo visual es un modo súper básico para seleccionar texto, moviendo con las teclas de navegación para moverme entre todo lo que quiero seleccionar. 
- `h`, `j`, `k`, `l` : Las teclas básicas de navegación para poder moverme a la izquierda, derecha, arriba y abajo; entre las líneas y las columnas del texto. 
- `o:` Nueva línea, cuando estoy en modo Normal y aprieto o este me hace una nueva línea y me pone en modo Insert ya listo para escribir.
- `:` : Es para entrar en el modo comándos (como por ejemplo ":q" para salir del archivo o ":w" para guardar). 
- `:w` : Viene de write, es para guardar archivos.
- `:q` : Es para salir de nvim.
- `:q!` : Es para cuando quiero salir pero tengo cambios en el archivo que no quiero guardar.
- `:qa` : Es para salir de todas las pestañas de NeoVim que tengo abierto.
- `:wq` : Es para guardar y salir con un solo comando.
- `:e`: Cuando entro a nvim, puedo usar este comando para abrir un archivo que nvim que se encuentre en esa carpeta (se puede usar la letra *TAB* para completar el nombre del archivo). Si no existe crea uno y lo abre.
