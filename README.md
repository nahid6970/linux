# Linux Dotfiles

Personal Linux configuration files and setup scripts.

## Structure

```
.
├── config/                  # Dotfiles (~/.config/*)
│   ├── bashrc               # Bash config
│   ├── autostart.sh         # Autostart script
│   └── .config/
│       ├── hypr/            # Hyprland
│       ├── nvim/            # Neovim
│       ├── neovim/          # Neovim standalone configs
│       ├── emacs/           # Emacs configs
│       ├── yazi/            # Yazi file manager
│       ├── kitty/           # Kitty terminal
│       ├── waybar/          # Waybar
│       ├── tmux/            # Tmux
│       ├── starship/        # Starship prompt
│       ├── qtile/           # Qtile WM
│       ├── i3/              # i3 WM
│       ├── rofi/            # Rofi launcher
│       ├── dunst/           # Notifications
│       └── ...
├── scripts/                 # All scripts
│   ├── setup/               # Main setup scripts (os.sh, start.sh, menu.py, ...)
│   ├── utils/               # Utility shell scripts
│   └── import/              # Misc import scripts (wallpaper, sddm, ...)
├── WSL/                     # WSL/Ubuntu setup scripts
├── docs/                    # Documentation (linux.org, archinstall.org)
└── README.md
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
bash scripts/setup/start.sh
# or for interactive menu:
python scripts/setup/menu.py
```

### WSL / Ubuntu

```bash
bash WSL/ubuntu-wsl-setup.sh
```
