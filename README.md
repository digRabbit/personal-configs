# Omarchy Personal Configs

Personal configuration files for Omarchy OS, Hyprland, and Neovim.

## Structure

This repository stores the actual config files, with symlinks from standard config locations pointing to them:

- Actual config files live in this repo
- `~/.config/` locations have symlinks pointing to repo files
- Edit configs normally in `~/.config/` → you're editing repo files through symlinks
- Git tracks actual file changes

## Tracked Configs

- `hypr/bindings.conf` ← `~/.config/hypr/bindings.conf` (symlink)
- `nvim/lua/config/` ← `~/.config/nvim/lua/config` (symlink)

## Usage

1. Edit your configs normally in `~/.config/`
2. Changes are automatically tracked in this repo (you're editing through symlinks)
3. Commit and push changes:
   ```bash
   cd ~/Documents/github/omarchy-personal-configs
   git add .
   git commit -m "Update configs"
   git push
   ```

## Setup on New Machine

1. Clone this repo: `git clone https://github.com/digRabbit/personal-configs.git`
2. Create symlinks:
   ```bash
   ln -s ~/personal-configs/hypr/bindings.conf ~/.config/hypr/bindings.conf
   ln -s ~/personal-configs/nvim/lua/config ~/.config/nvim/lua/config
   ```
