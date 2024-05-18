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

By following these steps, you'll have Zsh with the Powerlevel10k theme set up in your ArchWSL environment, providing a modern and visually appealing command-line interface.
