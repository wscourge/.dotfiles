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

TODO

## Sublime

TODO

- packages
- preferences (+ package preferences)
- bindings

## Ruby

TODO

- rvm
- rubocop
- rspec
- irb

## Vim

Copy `.vimrc`.

## Git

Prerequisites:

Git and its configuration

```
sudo apt-get install git-core
cp ./git/.gitconfig
```

Git flow

```
sudo apt-get install gitflow

```

Tig

```
sudo apt-get install tig
```
TODO: consider hubflow

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