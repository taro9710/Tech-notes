# Gupia de aprendizaje de Linux (desde Mint hasta Arch)
## Introducción

En este archivo voy a proponer una ruta progresiva dividida en niveles empenzando desde lo básico de Mint hasta llegar hasta Arch.

### Nivel 1: Fundamentos (Linux Mint - modo seguro)
**Objetivo:** Sentirse cómodo usando Linux Mint en el día a día.

**Conceptos básicos:**
- ¿Qué es Linux? ¿Qué es una distro?

- ¿Qué es el kernel?

- Diferencia entre entorno gráfico (GUI) y terminal (CLI).

- Qué es el sistema de archivos de Linux: `/`, `/home`, `/etc`, `/var`, `/usr`, `etc`.

**Cosas para aprender a hacer:**
- Actualizar el sistema (`apt update`, `apt upgrade`)

- Instalar programas desde la terminal (`apt install`, `flatpak`, `.deb`)

- Conocer y usar el **Software Manager** y el **Synaptic Package Manager**

- Uso básico de la terminal:

    `ls`, `cd`, `pwd`, `mkdir`, `rm`, `cp`, `mv`, `touch`, `cat`, `less`, `nano`

- Gestionar archivos y permisos:

    - `chmod`, `chown`

    - Entender qué es `sudo`

- Atajos de teclado útiles

    - Ver procesos: `top`, `htop`, `ps`, `kill`

    - Cómo montar, desmontar y explorar dispositivos USB desde la terminal

### Nivel 2: Usuario intermedio (usando más la terminal)
**Objetivo:** Usar la terminal para la mayoría de tareas básicas.

**Cosas para aprender:**
- Editores de texto de terminal: `nano`, `vim` 

- Redirección y pipes: `>`, `>>`, `|`, `tee`, `xargs`

- Uso de `grep`, `find`, `locate`, `cut`, `awk`, `sed` (empezar suave)

- Entender y modificar variables de entorno (`export`, `PATH`)

- Usar el sistema de logs: `journalctl`, `/var/log`

- Agregar/crear usuarios (`adduser`, `usermod`)

- Saber qué es un _shell_ y qué diferencias hay entre `bash`, `zsh`, `fish`

### Nivel 3: Personalización y configuración del sistema
**Objetivo:** Configurar el sistema a tu gusto y entender cómo funciona por debajo.

**Aprender a:**
- Personalizar el escritorio XFCE desde config y desde .config

- Configurar el inicio automático de servicios o scripts

- Usar y modificar `crontab` (tareas programadas)

- Aprender qué es `systemd`, cómo usar `systemctl`, cómo manejar servicios

- Manejar el `GRUB` y entender el proceso de booteo

Configurar el hostname, red, y DNS manualmente

Conocer qué hace el initramfs

### Nivel 4: Administrador del sistema
**Objetivo:** Poder resolver problemas y administrar el sistema a fondo.

**Aprender a:**
- Chrootear en un sistema desde un live USB

- Usar `rsync`, `tar`, `dd`, `gzip`, `scp`, `ssh`

- Hacer respaldos y restaurar desde la terminal

- Instalar un sistema Linux básico en máquina virtual (como Debian netinstall)

- Usar `ufw` para configurar un firewall básico

- Saber interpretar errores de arranque y logs

### Nivel 5: Camino a Arch Linux (manual y técnico)
**Objetivo:** Tener confianza para instalar Arch desde cero con el terminal.

**Antes de pasar a Arch:**
- Instalar **Arch en una VM** siguiendo el [Arch Wiki](https://wiki.archlinux.org/title/Main_page)

- Leer y entender la guía oficial de instalación

- Practicar configurar red desde la terminal con `ip`, `dhcpcd`, `systemd-networkd`, etc.

Aprender a montar particiones manualmente (`mount`, `umount`, `lsblk`, `fdisk`, `parted`)

- Configurar el sistema base: `pacstrap`, `genfstab`, `arch-chroot`

- Aprender a instalar y configurar `grub`

- Instalar y configurar el entorno gráfico (`X11`, `xorg`, `sddm`, `plasma`, `xfce`, etc.)

- Aprender `pacman`, `makepkg`, `yay`, `paru`, y el AUR

### Recomendaciones de práctica
- Hacé ejercicios pequeños todos los días (por ejemplo: mover archivos por terminal, instalar algo nuevo, leer logs).

- Usá una máquina virtual (VirtualBox) para experimentar sin miedo.

- Si algo te da curiosidad: **preguntá, rompé, aprendé**.

- [Arch Wiki](https://wiki.archlinux.org/title/Main_page)bjetivo:** es tu biblia. Aunque estés en Mint, usá Arch Wiki para aprender conceptos.

### Recursos útiles
- [Arch Wiki](https://wiki.archlinux.org/title/Main_page)

- Linux Handbook

- Explainshell – para entender comandos

- Canal de YouTube: DistroTube, The Linux Experiment

- Curso de Terminal: https://linuxcommand.org/

