# config
.dotfiles

# to checkout on a new system

alias config='/usr/bin/git --git-dir=$HOME/src/config/ --work-tree=$HOME'

git clone --bare https://github.com/jdochez/config.git $HOME/src/config

config config --local status.showUntrackedFiles no

# to push changes

config add

config commit -m "new version..."

config push --set-upstream origin master
