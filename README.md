# 🚀 Scripts

This repository contains helpful command-line scripts to enhance your terminal workflow and developer productivity.

> **📌 Note:**
> To use these scripts globally, ensure this folder is in your `$PATH`.

You can also set this up by cloning the `dotfiles` repo and symlinking the `.z*` files from the repo to your `$HOME` directory.

## 📁 Folder Structure

These scripts assume the presence of a `~/Developer` directory as the root of your projects.

---

## 🔍 `tff` — Terminal Fuzzy Finder

A bash script powered by **fzf** that lists all usable directories inside `~/Developer` and opens them in a new tmux session or window.

**Requirements:**

* [fzf](https://github.com/junegunn/fzf)
* [tmux](https://github.com/tmux/tmux)
* `~/Developer` directory

**Usage:**

```bash
tff
```

---

## 📂 `nff` — New Fuzzy Folder

This bash script also uses **fzf** to:

1. Select a parent folder from within `~/Developer`
2. Prompt for a new subfolder name
3. Create the folder and optionally open it in a new tmux window

Includes a placeholder for creating a new parent if needed.

**Requirements:**

* [fzf](https://github.com/junegunn/fzf)
* [tmux](https://github.com/tmux/tmux)
* `~/Developer` directory

**Usage:**

```bash
nff
```

---

## ⚙️ `setup-machine` — Dotfiles and Tooling Bootstrapper

A utility script to automate the linking of dotfiles and setup of key development tools.

**Key Features:**

* Symlinks dotfiles (Zsh, Tmux, WezTerm, Neovim, Hyprland)
* Supports conditional linking (e.g. `--with-hypr`)
* Optional confirmation for overwriting config

**Usage:**

```bash
bash setup-machine [options]
```

**Options:**

* `--with-hypr` or `-h` — include Hyprland configs
* `--no-confirm` — auto-confirm removal of existing configs
* `--dir <path>` or `-d <path>` — specify the location of dotfiles

Make sure your dotfiles repo is cloned in `$HOME/dotfiles` or pass the correct path with `--dir`.

---

## 📜 License

MIT License. Use freely, modify responsibly.

---

## 🙌 Contributing

Feel free to fork and submit pull requests for useful terminal enhancements or suggestions!
