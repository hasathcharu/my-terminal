# My Terminal

### Introduction
This is the terminal configuration I use for my devices. If you like, you can use this as well 😌.

### Install ZSH (non macOS devices)

> https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH

### Install Oh My Zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### Install PowerLevel10k

> https://github.com/romkatv/powerlevel10k

#### Step 1: Install required fonts
   - [MesloLGS NF Regular.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
   - [MesloLGS NF Bold.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
   - [MesloLGS NF Italic.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
   - [MesloLGS NF Bold Italic.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)

#### Step 2: Use the installed `MesloLGS NF` font in the terminal of your choice

#### Step 3: Clone the `powerlevel10k` repository

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

### Clone this repository in `~`

```bash
git clone https://github.com/hasathcharu/my-terminal ~/my-terminal
```

### Change config source

Change the following line at the end of `.zshrc`

```bash
[[ ! -f ~/.p10k.zsh ]] || source ~/.p10k.zsh
```

to the one below

```bash
[[ ! -f ~/my-terminal/.p10k.zsh ]] || source ~/my-terminal/.p10k.zsh
```

### Install auto suggessions and syntax highlighting

> https://medium.com/macoclock/how-to-add-auto-suggestion-and-syntax-highlighting-macos-linux-terminal-2f168bdd790

#### Auto suggessions

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```
#### Syntax highlighting

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```

#### Apply plugins

Change the following line in `.zshrc`

```bash
plugins=(git)
```

to the one below

```bash
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

### Create a `git alias` to add all and commit in one command (optional)

```bash
git config --global alias.ac '!git add -A && git commit -m'
```

### Done ✨
