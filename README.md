# .dotfiles
This is my README.md for my dotfiles repository.

## Installation

First, check out the dotfiles repo in your $HOME directory using git

```
$ git clone git@github.com:zszekeres65/.dotfiles.git
$ cd .dotfiles
```

then use GNU stow to create symlinks

```
$ stow .
```

# oh-my-posh
This is an alternative for powerline10k which is on life support. The following steps will help configuring.

## Installation

```
$ install jandedobbeleer/oh-my-posh/oh-my-po
```

## Updating

```
$ brew update && brew upgrade oh-my-posh && exec zsh
```

## Setup

### Font

```
$ oh-my-posh font install melso
```

### Prompt

Add the following snippet to the `.zshrc`.

```
if [ "$TERM_PROGRAM" != "Apple_Terminal" ]; then
  eval "$(oh-my-posh init zsh)"
fi
```

### Customize 

```
eval "$(oh-my-posh init zsh --config ~/https://github.com/JanDeDobbeleer/oh-my-posh/blob/main/themes/catppuccin_frappe.omp.json)"
```

