Repo to store dotfiles




- Dependencies to build suckless build:
  - Void Linux build
sudo xbps-install base-devel libX11-devel libXft-devel libXinerama-devel freetype-devel fontconfig-devel
  - Arch Linux build
sudo pacman -S base-devel libx11 libxft libxinerama freetype2 fontconfig

- Change kb layout in xorg

# /etc/X11/xorg.conf.d/30-keyboard.conf

Section "InputClass"
    Identifier "keyboard"
    MatchIsKeyboard "on"
    Option "XKbLayout" "es"
EndSection


