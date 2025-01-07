# Hyprland Setup

## System Overview
| DISTRO     | [ArchLinux](https://archlinux.org/) |
|------------|-------------------------------------|
| WM         | [Hyprland](https://hyprland.org/)  |
| BAR        | [Waybar](https://github.com/Alexays/Waybar) |
| LAUNCHER   | [Wofi](https://sr.ht/~scoopta/wofi/) |
| TERMINAL   | [Kitty](https://sw.kovidgoyal.net/kitty/) |
| GTK3       | [Adwaita-Dark](---) |
| FONT       | [JetBrainsMono and JetBrainsMono Nerd](---) |

## Preview
![Terminal and File Manager](pic/termandfile.png)

![Wofi Launcher](pic/wofi.png)

![Lock Screen](pic/lock.png)

![Logout Menu](pic/logout.png)

---

## Installation

### Packages to Install with Pacman
```bash
sudo pacman -S adw-gtk-theme dunst git grim gtk3 hyprland hyprlock hyprpaper \
kitty kvantum nemo neofetch nwg-look pipewire playerctl qt5ct qt6ct sddm \
slurp swayimg ttf-jetbrains-mono ttf-jetbrains-mono-nerd waybar wl-clipboard \
wofi xorg
```

### Clone and Install Yay from AUR
```bash
git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

### Packages to Install with Yay
```bash
yay -S adwaita-qt-git wlogout
```

### Apply GTK Theme and Dark Mode
```bash
gsettings set org.gnome.desktop.interface gtk-theme 'Adwaita'
gsettings set org.gnome.desktop.interface color-scheme 'prefer-dark'
```

### Note on Configuration Files
In the configuration files, remnants of my username `/home/yardev` remain. Replace them with your own username.

Additionally, move the `pic` folder to your home directory.


[My website project](https://yardev.su/)
