# gentoo-rice-dotfiles
Dotfiles for my Gentoo themed rice (https://www.reddit.com/r/unixporn/comments/vw1gsm/dwm_the_i_use_gentoo_btw_themedesktop/)

# How to install
DWM, Dmenu, and Slstatus are all configured at compile time so there's no configuration folder or .dotfiles but if you want my configuration, you have to compile it from the source code included in this GH repo. Here's a command to automate the building/installing of all three applications (Assuming your in the root directory of the repo, have GCC & Make installed, and have sudo permissions)
```sh
cd dwm && sudo make clean install && cd ../;
cd dmenu && sudo make clean install && cd ../;
cd slstatus && sudo make clean install && cd ../;
```

The other stuff in .config (Alacritty, mainly) can just be copied over with a command like this
```sh
cp -r .config/* ~/.config/
```
