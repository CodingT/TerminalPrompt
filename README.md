# Universal ZSH & Powerlevel10k Installer

A "silent" and "smart" automation script to set up ZSH environment across **Ubuntu/Debian**, **RHEL/Centos/Fedora**, and **macOS**. 

## Features
- **OS Autodetect**: Automatically uses `apt`, `dnf`, or `brew`.
- **Oh My Zsh**: Full unattended installation.
- **Powerlevel10k**: Configured in "Pure" style (minimalist and fast).
- **Plugins**: Includes `autosuggestions`, `syntax-highlighting`, and more.
- **Self-Healing**: Automatically repairs broken or partial installations.

## 🚀 Installation

Download the script:
   curl -L https://raw.githubusercontent.com/CodingT/TerminalPrompt/main/zsh_setup.sh -o zsh_setup.sh
Make it Executable and Run:
   chmod +x zsh_setup.sh
   ./zsh_setup.sh
   
OR quick install:
    sh -c "$(curl -L https://raw.githubusercontent.com/CodingT/TerminalPrompt/main/zsh_setup.sh)"

## Customization
To tweak the visuals (like changing the colors or adding more icons), run:
    p10k configure

To change default login shell:
    sudo chsh -s /usr/bin/zsh $USER


## Roll Back
Change default shell back to Bash:
    chsh -s $(which bash)

Remove ZSH Config Files: 
    rm ~/.zshrc ~/.p10k.zsh ~/.zsh_history ~/.oh-my-zsh
