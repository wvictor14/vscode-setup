
https://garrytrinder.github.io/2020/12/my-wsl2-windows-terminal-setup

Install oh-my-zsh

```bash
sudo apt install zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

I set COMPLETION_WAITING_DOTS="true" and uncommented the line in .zshrc.

Install omz plugins syntax highlight autocomplete

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

Then add `plugins=(git zsh-syntax-highlighting)` to `.zshrc`

Restart