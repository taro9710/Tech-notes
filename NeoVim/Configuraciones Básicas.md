# Configuraciones Básicas

## Primeros pasos configurando. Configuración de Neovim (`init.lua`) 
Me dirirjo a `~/.config/nvim` y en modifico el archvio `init.lua`

### Mostrar números de línea
```lua
        vim.opt.number = true
```
Muestra números de línea absolutos.

### Números relativos
```lua
        vim.opt.relativenumber = false
```
Desactiva números relativos.

### Resaltar línea actual
```lua
vim.opt.cursorline = true
```
Resalta la línea donde está el cursor.

### Desactivar wrap
```lua
vim.opt.wrap = false
```
Las líneas largas no se parten visualmente.

### Usar TABs reales
```lua
vim.opt.expandtab = false
```
Inserta caracteres TAB (`\t`) en vez de espacios.

### Tamaño visual del TAB
```lua
vim.opt.tabstop = 4
```
Un TAB se muestra como 4 espacios.

### Indentación automática
```lua
vim.opt.shiftwidth = 4
```
La indentación automática usa 4 espacios.

### Portapapeles del sistema
```lua
vim.opt.clipboard = "unnamedplus"
```
Permite copiar y pegar entre Neovim y otras aplicaciones.

### Desactivar swapfiles
```lua
vim.opt.swapfile = false
```
No crea archivos `.swp`.
