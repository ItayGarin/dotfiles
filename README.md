# dotfiles

## Quickstart

```
# Install chezmoi
sh -c "$(curl -fsLS git.io/chezmoi)"
sudo mv ~/bin/chezmoi /usr/bin
rm -rf ~/bin

# Apply the dotfiles
chezmoi init --apply --verbose https://github.com/itaygarin/dotfiles.git
```

## Todo

- Add `~/.gitconfig` (aliases, email+name, delta, ...)
- Add `fisher` + its plugins
- Ditch Regolith for vanilla `i3`/`sway`
- Try out `polybar`
- Setup `autorander`
- Setup `which-key` for space-driven shortcuts 
  - `Alt+Space` == spacemac's root `space`
  - `Alt+Space+p` == open recent projects in vscode / alacritty
  - `Alt+Space+s` == open sound settings
  - `Alt+space+w` == open networking / wi-fi settings
  - ...
- Setup VSCode extensions sync

### Shell
- Alacritty (+ alacritty-theme)
- bat
- delta
- jethrokuan/z (native fish fasd alternative)
- fish (+ fisher)
- fzf
- ripgrep

### Emacs
- [Emacs](https://www.gnu.org/software/emacs/) 24.5
- [spacemacs](https://github.com/syl20bnr/spacemacs)
- [emacs-launcher](https://github.com/ItayGarin/emacs-launcher)

## Archive

Using regolith-linux recently. Would like to switch back to vanilla i3

### i3 Window Manager
- [i3](https://i3wm.org/)
- [i3blocks](https://github.com/vivien/i3blocks)
- [jumpapp](https://github.com/mkropat/jumpapp)
- [picom](#)
- [flameshot](#)

## home-manager

I had to add this to `~/.profile` for nix desktop files to register on Ubuntu.

```shell
export XDG_DATA_DIRS=$HOME/.nix-profile/share:$HOME/.share:"${XDG_DATA_DIRS:-/usr/local/share/:/usr/share/}"
```
