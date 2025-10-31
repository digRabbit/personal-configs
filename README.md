# Omarchy Personal Configs

Personal configuration files for Omarchy OS, Hyprland, and Neovim.

## Structure

This repository uses **reverse symlinks** - the config files remain in their original locations, and this repo contains symlinks pointing to them. This means:

- Original files stay in `~/.config/` untouched
- Changes to the original files are automatically tracked in this repo
- No need to copy or move files around

## Tracked Configs

- `hypr/bindings.conf` → `~/.config/hypr/bindings.conf`
- `nvim/lua/config/` → `~/.config/nvim/lua/config/`

## Usage

1. Edit your configs normally in `~/.config/`
2. Changes are automatically reflected in this repo through symlinks
3. Commit and push changes:
   ```bash
   git add .
   git commit -m "Update configs"
   git push
   ```

## Setup on New Machine

To replicate these symlinks on another machine, the actual config files need to be restored first, then you would reverse the symlink direction (traditional dotfiles approach) or manually create the same symlink structure.
