## Set Up
Clone the repo:
```
git clone --separate-git-dir=$HOME/.dotfiles git@github.com:rob-andrew-ellis/.dotfiles.git ~
```
#### Error Case
If errors resulting from default config files appear you can create a temporary directory...
```
git clone --separate-git-dir=$HOME/.dotfiles git@github.com:rob-andrew-ellis/.dotfiles.git tempdotfiles
```
Move the dotfiles over...
```
rsync --recursive --verbose --exclude '.git' tempdotfiles/ $HOME/
```
Remove the temporary directory
```
rm -r tempdotfiles
```
