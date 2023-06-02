# List of Core Packages

There is no order or obligation to download all. Download with intension!

Notation styles:
- `package` or package (AUR, or just notes) [group]
- package1, package2 (AUR), package3 (cool one) [grp1]

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
- man-db (for manuals and `man` command)
- intel-ucode (or amd-ucode)

### Wireless Internet Connection
- wpa\_supplicant
- dhcpcd
> If intended to use GNOME DE, install `NetworkManager` alone is good enough. It uses `wpa_supplicant` and `dhcp_client` under the hood.

### Text editors
- nano
- vi
- vim
- neovim

### Tools & Drivers
- git
- `yay` or `yay-bin` (requires `base-devel` above)
```sh
git clone https://aur.archlinux.org/yay
cd yay
makepkg -si
```
- neofetch
- ntfs-3g (to use NTFS drive)
- nvidia, nvidia-utils
- [xorg], wayland
---
## User Interface (post-installation)
### Shell-related
- zsh, fish
- alacritty
- gnome-console (`kgx`), or gnome-terminal
- ttf-firacode-nerd, ttf-fira-code (there is also woff2 version)
- noto-fonts-cjk, noto-fonts-emoji, noto-fonts-extra
- tmux
- tree
- bashtop, htop, gotop (AUR)
- oh-my-bash-git (AUR), oh-my-zsh-git (AUR)
- tree

### Window Manager (WM)
* xorg-xinit (to aquire `startx`)
* i3 experience:
    - i3-wm [i3]
    - i3blocks [i3]
    - i3lock [i3]
    - i3status [i3]
    - dmenu

* Dual Monitors:
    - xrandr
    - arandr

### Desktop Environment
* GNOME experience:
    - [gnome]  (select what you want/need)
    - [gnome-extra]
    - gdm, gdm-settings (AUR)
* KDE Plasma experience: [plasma] [kde-applications] [kde-utilities]

### Everyday apps
* Coding: (open-source version does not have profile sync)
    - visual-studio-code-bin (AUR)
    - code, code-marketplace (AUR)
    - vscodium (AUR), vscodium-marketplace (AUR)
* Communication
    - zoom (AUR)
    - slack-desktop (AUR)
    - discord
* Office Suite, Art & Music
    - onlyoffice-bin (AUR)
    - musescore [pro-audio], muse-hub-bin (AUR)
    - yoshimi [pro-audio lv2-plugins]
    - spotify (AUR), spotify-qt (AUR, dev app)
    - obs-studio
* Entertainment (Games)
    - 
* Quality of life 
    - nautilus [gnome] + sushi [gnome]
    - 

---
### Fun ones
- lolcat
- cowsay
- cmatrix, tmatrix (AUR)
- hollywood (AUR)
- obsidian (Markdown Text Editor)
