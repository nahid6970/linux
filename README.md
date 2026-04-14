# Linux Dotfiles

Personal Linux configuration files and setup scripts.

## Structure

```
.
├── config/          # Dotfiles (~/.config/*)
│   └── .config/
│       ├── hypr/    # Hyprland
│       ├── nvim/    # Neovim
│       ├── kitty/   # Kitty terminal
│       ├── waybar/  # Waybar
│       ├── tmux/    # Tmux
│       ├── starship/# Starship prompt
│       ├── qtile/   # Qtile WM
│       ├── i3/      # i3 WM
│       ├── rofi/    # Rofi launcher
│       ├── dunst/   # Notifications
│       └── ...
├── editors/         # Editor configs
│   ├── neovim/      # Neovim standalone configs
│   ├── emacs/       # Emacs configs
│   └── yazi/        # Yazi file manager
├── WSL/             # WSL/Ubuntu setup scripts
├── script_source/   # Utility shell scripts
├── import/          # Misc setup scripts (wallpaper, sddm, etc.)
├── os.sh            # Main Arch setup script
├── os_organized.sh  # Organized version of os.sh
├── start.sh         # Entry point
└── menu.py          # Interactive setup menu
```

## Setup

### Clone

```bash
git clone https://github.com/nahid6970/linux.git ~/dotfiles
cd ~/dotfiles
```

### Apply dotfiles

Copy configs to `~/.config`:

```bash
cp -r config/.config/* ~/.config/
```

Copy bashrc:

```bash
cp config/bashrc ~/.bashrc
source ~/.bashrc
```

### Run setup script

```bash
bash start.sh
# or for interactive menu:
python menu.py
```

### WSL / Ubuntu

```bash
bash WSL/ubuntu-wsl-setup.sh
```
