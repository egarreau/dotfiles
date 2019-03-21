# Dotfiles

My personal settings for iTerm, bash, vim, tmux, and git.

It's taken me three solid years of daily web development to find a combination of settings that works well for me. It will surely continue to evolve over time. I like to document it here for my own sake as well as for anyone who's interested in what someone else's setup looks like. Much of this is stolen from other folks' environments so I heartily encourage you to steal from mine. If you're a new developer, or just new to vim, it's really worthwhile to lose a few hours tinkering around with settings, deleting stuff to see what changes and then adding it back in with some modifications to see how you like it. Customizing your environment is empowering and fun, and can go a long way toward making you feel like a "real" developer.

# Setup

```
$ git clone git@github.com:egarreau/dotfiles.git
$ cd dotfiles
```

## iTerm

[Install iTerm2](https://www.iterm2.com/)

- To load saved preferences, go to iTerm2 > Preferences > Load preferences from a custom folder or URL
- Select `iterm2.plist` from the dotfiles directory

## Bash

`$ cp bash_profile ~/.bash_profile`

## Git

`$ cp gitconfig ~/.gitconfig`

## Vim

`$ cp vimrc ~/.vimrc`

### Install the color scheme [1989](http://www.github.com/egarreau/1989.vim)
```
$ cd ..
$ git clone git@github.com:egarreau/1989.vim.git
$ cd 1989.vim/colors
$ cp 1989.vim ~/.vim/colors/1989.vim
```
You may need to `mkdir ~/.vim` and `mkdir ~/.vim/colors` if they don't already exist

### Install [Vundle](https://github.com/VundleVim/Vundle.Vim) to manage plugins
```
$ git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

### Install [Homebrew](https://brew.sh/) to make the following `brew` commands work
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### Install [the silver searcher](https://github.com/ggreer/the_silver_searcher) to power the `ag` plugin
```
$ brew install the_silver_searcher
```

*Launch vim and run `:PluginInstall` to install all plugins*

## Tmux

```
$ brew install tmux
$ cp tmux.conf ~/.tmux.conf
```

*Restart terminal*

### Other random stuff I like

- remapping `caps lock` to `control`
- [Spectacle](https://www.spectacleapp.com/)
