# Dotfiles

Most of the configuration files and script to set them up.

## ZSH ( + OH-MY-ZSH )

Prerequisites:

```
sudo apt-get install zsh
```
and restart terminal. Then, install oh-my-zsh
```
cd
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```
Install powerline font:
```
cd
wget https://github.com/powerline/powerline/raw/develop/font/PowerlineSymbols.otf
wget https://github.com/powerline/powerline/raw/develop/font/10-powerline-symbols.conf
mkdir ~/.fonts/
mv PowerlineSymbols.otf ~/.fonts/
mkdir -p .config/fontconfig/conf.d
fc-cache -vf ~/.fonts/
mv 10-powerline-symbols.conf ~/.config/fontconfig/conf.d/
```
Install solarized theme
```
git clone git://github.com/sigurdga/gnome-terminal-colors-solarized.git ~/.solarized
cd ~/.solarized
./install.sh
```

Copy `.zshrc`.

## Sublime

Download and install [Sublime Text 3](https://www.sublimetext.com/). Then, `Ctrl + Shift + P` to install following packages:

- A File Icon
- Better Coffescript
- Boxy Theme
- BracketHighlighter
- Colorsublime
- Console Wrap
- EditorConfig
- ERB Autocomplete (?)
- Git
- GitGutter
- Package Control
- RuboCop
- SublimeLinter
- Theme - Monokai Pro
- Pretty JSON

Press `Ctrl + Shift + P`, type 'Colorsublime: Install Theme', then type 'Monokai' and press `Enter`.

Copy and paste User preferences and Key bindings.

## Ruby

TODO

- rvm
- rubocop
- rspec
- irb

## Vim

Copy `.vimrc`.

## Git

- git flow (hubflow?)
- tig

## Terminator

Prerequisites:

```
sudo add-apt-repository ppa:gnome-terminator
sudo apt-get update
sudo apt-get install terminator
```

restart terminal. Then, copy the configuration file:

```
cp ./terminator/config ~/.config/terminator/config
```

TODO: window modes 

## System UI

TODO

- font: san francisco
- icons: paper
- theme: Sierra dark thin

## Software

TODO

## 