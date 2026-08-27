# Configuraciones Básicas

## Primeros pasos configurando. Configuración de Neovim (`init.lua`) 
Me dirirjo a `~/.config/nvim` y en modifico el archvio `init.lua`, el formato que tendrá la configuración básica de mi nvim será el siguiente: 

```text
    ~/.config/nvim/
    ├── init.lua
    └── lua/
        ├── config/
        │   ├── options.lua
        │   ├── colors.lua
        │   └── lazy.lua
        │
        └── plugins/
```
## ¿Qué contiene cada archivo?

### `init.lua`

Es el punto de entrada principal de la configuración de Neovim. Desde este archivo se cargan los diferentes módulos de configuración.

### `lua/config/options.lua`

Contiene las opciones generales de Neovim, como:

* Números de línea.
* Tabulación.
* Ajuste de líneas.
* Portapapeles.
* Archivos swap.

### `lua/config/colors.lua`

Contiene configuraciones relacionadas con la apariencia, como colores personalizados y resaltado de elementos.

### `lua/config/lazy.lua`

Se encarga de instalar e iniciar `lazy.nvim`, que será el administrador de plugins.

### `lua/plugins/`

Esta carpeta contiene la configuración de los plugins.

Por ejemplo:

```text
lua/plugins/
├── telescope.lua
├── treesitter.lua
└── lsp.lua
```
