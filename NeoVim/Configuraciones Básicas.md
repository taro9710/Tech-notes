# Configuraciones Básicas

## Primeros pasos configurando. Configuración de Neovim (`init.lua`) 
Me dirirjo a `~/.config/nvim` y en modifico el archvio `init.lua`

- Mostrar números de línea
```lua
vim.opt.number = true
```
Muestra números de línea absolutos.

- Números relativos
```lua
vim.opt.relativenumber = false
```
Desactiva números relativos.

- True Colours
```lua
vim.opt.termguicolors = true
```
Habilita colores de 24 bits.

- Resaltar línea actual
```lua
vim.opt.cursorline = true
vim.api.nvim_set_hl(0, "CursorLine", {
    bg = "#505050" (Este es el color de la línea) 
})

vim.api.nvim_set_hl(0, "CursorLineNr", {
    fg = "#ffffff",
    bold = true (Este creo que es para resaltar el número de la línea en la que estoy)
})
```
Resalta la línea donde está el cursor.

- Wrap
```lua
vim.opt.wrap = true 
```
Las líneas largas se parten visualmente.

- Usar TABs reales
```lua
vim.opt.expandtab = false
```
Inserta caracteres TAB (`\t`) en vez de espacios.

- Tamaño visual del TAB
```lua
vim.opt.tabstop = 4
```
Un TAB se muestra como 4 espacios.

- Indentación automática
```lua
vim.opt.shiftwidth = 4
```
La indentación automática usa 4 espacios.

- Portapapeles del sistema
```lua
vim.opt.clipboard = "unnamedplus"
```
Permite copiar y pegar entre Neovim y otras aplicaciones.

- Desactivar swapfiles
```lua
vim.opt.swapfile = false
```
No crea archivos `.swp`.
