#DOTFILES & CONFIGS:

Dependencies to build suckless build:
  - Void Linux build
`sudo xbps-install base-devel libX11-devel libXft-devel libXinerama-devel freetype-devel fontconfig-devel`

  - Arch Linux build
`sudo pacman -S base-devel libx11 libxft libxinerama freetype2 fontconfig`

- Change kb layout in xorg
```
# /etc/X11/xorg.conf.d/30-keyboard.conf

Section "InputClass"
    Identifier "keyboard"
    MatchIsKeyboard "on"
    Option "XKbLayout" "es"
EndSection
```

ALACRITTY TERMCD
`sudo pacman -S alacritty`

- alacritty folder in ~/.config/  (explore posibilities of STOW)

ZSH INSTALL
`sudo pacman -S zsh`

OH MY ZSH
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

PLUGINS ZSH WITH OMZ
`git clone https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete`
`git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting`
`git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting`
`git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

POWERLEVEL10K ZSH THEME
`git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`

SPACEVIM
curl -sLf https://spacevim.org/install.sh | bash
