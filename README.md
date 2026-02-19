# Universal ZSH & Powerlevel10k Installer

A "silent" and "smart" automation script to set up ZSH environment across **Ubuntu/Debian**, **RHEL/CentOS/Fedora**, and **macOS**.

## Features

- **OS Autodetect** — Automatically uses `apt`, `dnf`, or `brew`
- **Oh My Zsh** — Full unattended installation
- **Powerlevel10k** — Configured in "Pure" style (minimalist and fast)
- **Plugins** — Includes `autosuggestions`, `syntax-highlighting`, and more
- **Self-Healing** — Automatically repairs broken or partial installations

## Installation

### Standard Installation

Download the script:

```bash
curl -L https://raw.githubusercontent.com/CodingT/TerminalPrompt/main/zsh_setup.sh -o zsh_setup.sh
```

Make it executable and run:

```bash
chmod +x zsh_setup.sh
./zsh_setup.sh
```

### Quick Install (One-liner)

```bash
sh -c "$(curl -L https://raw.githubusercontent.com/CodingT/TerminalPrompt/main/zsh_setup.sh)"
```

## Customization

### Configure Powerlevel10k

To customize the visuals (colors, icons, etc.):

```bash
p10k configure
```

### Change Default Login Shell to ZSH

```bash
sudo chsh -s /usr/bin/zsh $USER
```

## Rolling Back

### Revert to Bash

```bash
chsh -s $(which bash)
```

### Remove ZSH Configuration Files

```bash
rm ~/.zshrc ~/.p10k.zsh ~/.zsh_history ~/.oh-my-zsh
```
