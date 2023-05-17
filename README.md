# connernilsen's dotfiles

This repository contains the set of dotfiles and configurations I would like shared between the computers and environments I commonly work in.

> Note: the vim config is no longer maintained. Some plugins may not behave correctly or cause vim to crash.

## Setup

1. Install/Compile neovim
2. Symlink files:
  - `ln -s dotfiles/tmux.conf .tmux.conf`
  - `ln -s dotfiles/nvim .config/nvim`
  - `ln -s dotfiles/vim .vim` (if using vim)
3. Run `:PlugInstall` in nvim
4. Install the following packages:
  - `htop`
  - `ripgrep`
  - `tmux`
  - `ChrisJohnsen/tmux-MacOSX-pasteboard` (if on mac)
  - `charmbracelet/glow`
  - Packages that should be auto installed by nvim
    - `fzf`
    - `vim-plug`
5. Install [TPM](https://github.com/tmux-plugins/tpm)
6. Set the following options in .bashrc/.zshrc/...
```
export EDITOR=nvim
export CLICOLOR=1
export TERM="xterm-256color"
```
7. Install language helpers:
  - python
    - `autoimport`
    - `pyre-check`
    - `black`
  - OCaml
    - `opam`
    - `dune`
    - `merlin`
    - `ocamlformat`
    - `ocaml-lsp-server`
    - `utop`
