# VimBotion's dotfiles

## Steps

1. Install Apple's Command Line Tools

```zsh
xcode-select --install
```


2. Clone repo

```zsh
git clone git@github.com:VimBotion/dotfiles.git ~/.dotfiles
```


3. Create symlinks in the Home directory to the real files in the repo

```zsh
ln -s ~/.dotfiles/nvim ~/.config
```


4. Install Homebrew, followed by the software listed in the Brewfile.

```zsh
# These could also be in an install script.

# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Then pass in the Brewfile location...
brew bundle --file ~/.dotfiles/Brewfile
```
