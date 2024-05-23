# Setting Up Arch Linux in WSL

Arch Linux is a lightweight and flexible distribution that can be set up in WSL. This guide will walk you through the process.

If you don't have WSL 2 configured, follow the initial steps in this [repository](https://github.com/LuisHBeck/configs/tree/master/docker) before installing the distro.

## Download ArchWSL

- [ArchWSL Repository](https://github.com/yuk7/ArchWSL)
- [Direct Download](https://github.com/yuk7/ArchWSL/releases/latest/download/Arch.zip)

Extract the content into a folder on your C: drive called `Arch`.

## Installing

Open a terminal in the `Arch` directory and execute:

```powershell
.\Arch.exe
```

After installation, the distro will be registered in WSL. You can check by restarting the terminal and running:

```powershell
wsl -l -d
```

## Set Up Default User

Initially, you will be logged in as root, but you need to configure your own user. Follow this [reference](https://wsldl-pg.github.io/ArchW-docs/How-to-Setup/) for more details.

Configure sudoers to allow commands like `sudo` to elevate privileges for any user:

```bash
echo "%wheel ALL=(ALL) ALL" > /etc/sudoers.d/wheel
```

Create your user and set a password (replace `{username}` with your username):

```bash
useradd -m -G wheel -s /bin/bash {username}
passwd {username}
```

Open another terminal in the `Arch` folder and set the default user:

```powershell
.\Arch.exe config --default-user {username}
```

You can check the current user in Arch by running:

```bash
whoami
```

## Initialize Keyring

```bash
sudo pacman-key --init
sudo pacman-key --populate
sudo pacman -Sy archlinux-keyring && sudo pacman -Syu
```

## Installing Yay AUR Helper

- [Yay Official Repository](https://github.com/Jguer/yay)

```bash
sudo pacman -Sy --needed git base-devel
cd /tmp && git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si
```

## Installing zsh with [powerlevel10k](https://github.com/romkatv/powerlevel10k#arch-linux)

```bash
yay -S zsh
yay -S --noconfirm zsh-theme-powerlevel10k-git
echo 'source /usr/share/zsh-theme-powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
```

Change the default shell to zsh:

```bash
chsh -s /usr/bin/zsh
```

**Optional dependencies for `zsh-theme-powerlevel10k-git`:**

```bash
yay -S ttf-meslo-nerd-font-powerlevel10k powerline-fonts awesome-terminal-fonts
```

This completes the setup of Arch Linux in WSL with zsh and the powerlevel10k theme. Enjoy your new environment!
