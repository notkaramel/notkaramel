# `i3` Configuration and Everything

Pain, but worth it :)

---
## 0. List of config files (relative to `$HOME`)
- General `i3 configuration file: `.config/i3/config`
- Programs configs: (relative to user's `$HOME`)
```sh
alacritty # .alacritty.yml
bash # .bashrc
zsh # .zshrc
fish # .config/fish/config
tmux # .tmux.conf
neofetch # .config 
ssh # .ssh/config
```
- Visual themes (folders, rather than config file):
```sh
icons # .icons/
themes # .themes/
oh-my-bash # .oh-my-bash/
oh-my-zsh # .oh-my-zsh/
```

## Natural Scrolling
    The default config file for libinput is at `/usr/share/X11/xorg.conf.d/40-libinput.conf`. Copy it to `/etc/X11/xorg.conf.d` then edit it your preferred text editor (with `sudo`)
```
/etc/X11/xorg.conf.d
---
...
Section "InputClass"
    Identifier "libinput touchpad catchall"
    ...
    Option "NaturalScrolling" "on" # add this
EndSection
...
```

## Network Configuration (wpa\_supplicant & dhcpcd)
- NOTE: recommend using NetworkManager for out-of-the-box experience, but using wpa\_supplicant and dhcpcd directly give better control over network management
- `wpa_supplicant.conf` configuration:
```conf
sudo nvim /etc/wpa_supplicant/wpa_supplicant.conf
---
# for normal wifi
network={
    ssid=
    passphrase=
}

# for education institution wifi
network={
    ssid=
    EAP=PEAP
    "MCHAPv2"
}
```
- To activate wpa_supplicant: 
```sh
sudo wpa_supplicant -B -i wlan0 -c /etc/wpa)supplicant/wpa_supplicant.conf 
```
> Note: the interface (`-i` flag) could be something else, e.g. wlo1. You can check it using the following command:
```sh
ip addr
```

- Make sure the interface is up/unblock, using:
```sh
ifstat wlo1 # to check
ip link set wlo1 up # to unblock interfce
```

## Bluetooth Configuration
- Using `bluetoothctl`, from `bluez-utils` package. Recommend using `blueberry` as the GUI interface.

## Multiple Displays
- hmm

## Clipboard manager
- 


---
## Function Keys
- All will be a part of `.config/i3/config`

### 1. Media Player: `playerctl`
```
bindsym XF86AudioPlay exec playerctl play-pause
bindsym XF86AudioNext exec playerctl next
bindsym XF86AudioPrev exec playerctl previous
```

### 2. Brightness Controller: `brightnessctl`
```
# Increase/Decrease screen brightness
bindsym XF86MonBrightUp exec brightnessctl set 10%+
bindsym XF86MonBrightDown exec brightnessctl set 10%-
```

### 3. Volume Controller: `pactl` of PulseAudio
```

```
