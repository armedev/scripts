# Scripts

This repo contains all the scripts which will be helpfull to get going with convenience in terminal
In order for this repo to work you should have the path of this folder in your `$PATH`.

This can also be done by cloning dotfiles repo and symnlinking the `.z*` files in the repo from the `$HOME` directory

## TFF

tff is a bash script which requires **fuzzy finder** to work.
it lists all the usable directories in Developer folder in the home directory.

prerequisites:

- [fzf](https://github.com/junegunn/fzf)
- [tmux](https://github.com/tmux/tmux)
- a directory named `$HOME/Developer`

## NFF

nff is a bash script which requires **fuzzy finder** to work.
it lists all the parent directories in Developer folder in the home directory with also a dummy placeholder to select new parent.
then proceed to prompt the user for a new directory name

prerequisites:

- [fzf](https://github.com/junegunn/fzf)
- [tmux](https://github.com/tmux/tmux)
- a directory named `$HOME/Developer`
