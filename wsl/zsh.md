# Setting Up Zsh in ArchWSL

Enhance your terminal experience in ArchWSL by setting up Zsh with the Powerlevel10k theme.

## Installing Zsh with Powerlevel10k

First, install Zsh:

```bash
yay -S zsh
```

Next, install the Powerlevel10k theme:

```bash
yay -S --noconfirm zsh-theme-powerlevel10k-git
echo 'source /usr/share/zsh-theme-powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

## Changing the Default Shell to Zsh

Change the default shell to Zsh for your user:

```bash
chsh -s /usr/bin/zsh
```

## Optional Dependencies for Powerlevel10k

For optimal display of the Powerlevel10k theme, install the following font packages:

```bash
yay -S ttf-meslo-nerd-font-powerlevel10k powerline-fonts awesome-terminal-fonts
```

## Install plugins

First we need to create a folder called `.zsh` at root(`~`)

```bash
mkdir .zsh
```

For example install `zsh-autosuggestions` plugin

1. Clone this repository somewhere on your machine. This guide will assume `~/.zsh/zsh-autosuggestions`.

    ```sh
    git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
    ```

2. Add the following to your `.zshrc`:

    ```sh
    source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh
    ```



By following these steps, you'll have Zsh with the Powerlevel10k theme set up in your ArchWSL environment, providing a modern and visually appealing command-line interface.
