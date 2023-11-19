#P10K Config

### Install Oh My Zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Install PowerLevel10k

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

### Clone this repository in `~`

```bash
git clone https://github.com/hasathcharu/p10kconfig
```

### Change Config Source

Change the following line (at the end of `.zshrc`)

```bash
[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
```

to the one below

```bash
[[ ! -f ~/p10kconfig/.p10k.zsh ]] || source ~/p10kconfig/.p10k.zsh
```

###Done ✨
