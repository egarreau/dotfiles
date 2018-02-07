# Dotfiles

My personal settings for bash, vim, tmux, and git.

# Setup

```
$ git clone git@github.com:egarreau/dotfiles.git
$ cd dotfiles
```

## Bash

`$ cp bash_profile ~/.bash_profile`

## Git

`$ cp gitconfig ~/.gitconfig`

## Vim

`$ cp vimrc ~/.vimrc`

Install the color scheme [1989](http://www.github.com/egarreau/1989.vim)
```
$ git clone git@github.com:egarreau/1989.vim.git
$ cd 1989.vim/colors
$ cp 1989.vim ~/.vim/colors/1989.vim
```

Install [Vundle](https://github.com/VundleVim/Vundle.Vim) to manage plugins
```
$ git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

Install [the silver searcher](https://github.com/ggreer/the_silver_searcher) to power the `ag` plugin
```
$ brew install the_silver_searcher
```

Launch vim and run `:PluginInstall` to install all plugins

## Tmux

```
$ brew install tmux
$ cp tmux.config ~/.tmux.config
```
