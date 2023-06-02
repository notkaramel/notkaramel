# List of Core Packages
There is no order or obligation to download all. Download with intension!
---
## Arch Installation
### Linux Kernel & Firmware
- `linux` or `linux-lts`
- linux-firmware
- linux-headers (optional)

### Core Packages
- base, base-devel
- grub, efibootmgr, os-prober
- sudo

### Wireless Internet Connection
- wpa_supplicant
- dhcpcd

### Text editors
- nano
- vi
- vim
- neovim

### Tools & Drivers
- git
- yay (requires `base-devel` above)
```sh
git clone https://aur.archlinux.org/yay
cd yay
makepkg -si
```
- yay-bin
```sh
git clone https://aur.archlinux.org/yay-bin
```
- nvidia, nvidia-utils
- [xorg], wayland
---
## User Interface (post-installation)
### Terminal emulators
- alacritty
- gnome-console (`kgx`), or gnome-terminal

### Window Manager (WM)
* i3 experience:
    - i3-wm [i3]
    - i3blocks [i3]
    - i3lock [i3]
    - i3status [i3]
    - dmenu

### Desktop Environment
* GNOME experience: [gnome] [gnome-extra]
* KDE Plasma experience: [plasma] [kde-applications] [kde-utilities]
