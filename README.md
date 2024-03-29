dotfiles
========
personal setups

## Usage
![output 2](https://user-images.githubusercontent.com/871772/222487285-b25f013d-3aab-47d8-97f1-be6f1f199270.gif)

## Install
1。 On Terminal, copy/paste below code
```
cd ~/Documents
git clone git@github.com:zenglekidd/dotfiles.git
cd ~/Documents/dotfiles
chmod +x ~/Documents/dotfiles/install.sh
~/Documents/dotfiles/install.sh
```
2。Open a New Terminal

## Update 
1. Pull the lastest git repo
2. Restart `Terminal`


## The idea

1. never put real content on the ~/.bashrc or ~/.bash_profile files, instead those files are just symlinks to the real configuration files kept in a subdirectory in my home folder, for example ~/dotfiles/bashrc and ~/dotfiles/bash_profile.

2. keep the ~/dotfiles folder under source control using Git, and hosted at GitHub.com

3. When install a new system, clone the GitHub repository to a new local ~/dotfiles folder and create all the symlinks (currently by hand).

4. Whenever edit one of the configuration files, just commit and push to GitHub, and then pull in every other machine.

This is the example content of ~/dotfiles folder:

```
~/dotfiles
|-- bash
|   |-- aliases
|   |-- config
|   |-- env
|   `-- promptcolors
|-- bash_profile
|-- bashrc
|-- gitconfig
|-- gvimrc
|-- hg-templates
|   |-- map-cmdline.dlog
|   |-- map-cmdline.nlog
|   |-- map-cmdline.sglog
|   `-- map-cmdline.slog
|-- hgrc
|-- ssh
|   `-- config
|-- vim
|   |-- after
|   |-- colemak-mappings.vim
|   |-- colors
|   |-- doc
|   |-- filetype.vim
|   |-- ftplugin
|   `-- plugin
`-- vimrc
```

## Reference
https://superuser.com/a/152600
