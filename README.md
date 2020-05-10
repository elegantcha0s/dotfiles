## First setup
  pacman -S git vim zsh thunderbird weechat i3-wm i3blocks i3lock i3status libxfce4ui libxfce4util xfce4-panel xorg-xinit wget curl

## Snapd
  
  git clone git clone https://aur.archlinux.org/snapd.git
  cd snapd
  makepkg -si
  cd ..
  rm -rf snapd/
  sudo systemctl enable --now snapd.socket
  sudo ln -s /var/lib/snapd/snap /snap
  
## edb-debugger
  
  git clone https://aur.archlinux.org/edb-debugger.git
  cd edb-debugger
  makepkg -si
  cd ..
  rm -rf edb-debugger/
  
## Zeal
  
  git clone https://aur.archlinux.org/zeal-git.git
  cd zeal-git
  makepkg -si
  cd ..
  rm -rf zeal-git/
  
## Spotify

  git clone https://aur.archlinux.org/spotify.git
  cd spotify
  makepkg -si
  cd ..
  rm -rf spotify/
  
## General

 git clone https://aur.archlinux.org/visual-studio-code-bin.git // Visual studio code
 cd visual-studio-code-bin
 makepkg -si
 git clone https://aur.archlinux.org/brave-bin.git
 cd brave-bin
 makepkg -si
 cd ..
 rm -rf brave-bin/
 
 
## Yaourt

  git clone https://aur.archlinux.org/package-query.git
  cd package-query
  makepkg -si
  cd ..
  git clone https://aur.archlinux.org/yaourt.git
  cd yaourt
  makepkg -si
  cd ..
  sudo rm -dR yaourt/ package-query/
  
 
  # Enable VIM autocomplete at the end
