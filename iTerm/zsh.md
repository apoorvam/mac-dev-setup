# Zsh

Zsh(Z shell) is a shell designed for interactive use, although it is also a powerful scripting language. While being compatible with Bash, it offers advantages such as improved tab completion and many other useful features.

## Installation

It can be installed via homebrew:

```
brew install zsh
```

Make sure that Zsh has been installed correctly by running the command `zsh` in a terminal. It is recommended to install a framework along with `zsh` as it makes configuration, themes, plugins a lot better.

## Oh My Zsh

[Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh) is an open source, community-driven framework for managing your zsh configuration.

### Install Oh My Zsh

```
$ sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Customization 

The configuration file for zsh is called `.zshrc` and it locates in home folder (~/.zshrc). You can use this file to set alias, environment variables, theme etc. For example, you can set alias for `git status` as `gs` which is used very often.

```
# Aliases
alias g="git"
alias gs="git status"
alias ga="git add -u"
alias gc="git commit -m"

# Set environment variables
export GIT_EDITOR=vim
```

Every time you can make changes to this file, apply the changes by running following command or start new shell instance.

```
source ~/.zshrc
```

You can also set your desired theme by setting the variable `ZSH_THEME` in .zshrc file. 
```
ZSH_THEME="agnoster"
```
![Zsh Theme](https://cloud.githubusercontent.com/assets/2618447/6316862/70f58fb6-ba03-11e4-82c9-c083bf9a6574.png)