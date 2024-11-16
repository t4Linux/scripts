# nala
```
https://gitlab.com/volian/nala/-/releases
```

# base_installs
```bash
sudo nala install -y cmake gettext luarocks rofi polybar sxhkd openssh-server nitrogen picom exa bat
```
# nvim
```bash
sudo apt install cmake gettext luarocks
curl -LO https://github.com/BurntSushi/ripgrep/releases/download/14.1.0/ripgrep_14.1.0-1_amd64.deb
sudo dpkg -i ripgrep_14.1.0-1_amd64.deb
git clone https://github.com/LazyVim/starter ~/.config/nvim && rm -rf ~/.config/nvim/.git
```
# apps
```bash
sudo nala install rofi polybar sxhkd openssh-server nitrogen picom exa bat fzf
ln -s /usr/bin/batcat ~/.local/bin/bat
```

# clipmenu
```bash
git clone https://github.com/cdown/clipnotify.git
make && sudo make install
sudo nala install libx11-dev libxfixes-dev xsel rofi
git clone https://github.com/cdown/clipmenu.git
cd clipmenu
make && sudo make install
systemctl --user import-environment DISPLAY
systemctl --user enable --now clipmenud
```
do zmiennych środowiskowych trzeba dodać
```bash
export CM_LAUNCHER=rofi
```
# devour
```bash
git clone https://github.com/cdown/clipnotify.git
make && sudo make install
```
# dunst
```bash
https://github.com/dunst-project/dunst.git
cd dunst && make && sudo make install
```
