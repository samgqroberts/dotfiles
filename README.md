# dotfiles
A collection of my configuration files (commonly files prefixed with a dot '.'), to be able to easily port my environment.

## Bash

Clone this repo into `~/.dotfiles`
```
mkdir ~/.dotfiles && cd ~/.dotfiles && git clone git@github.com:samgqroberts/dotfiles.git
```

Add this to `~/.bashrc` so the cloned dotfiles are loaded into every bash environment:
```
for DOTFILE in `find ~/.dotfiles/dotfiles`
do
  [ -f "$DOTFILE" ] && source "$DOTFILE"
done
```
