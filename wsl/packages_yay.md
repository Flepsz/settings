# Installing Packages Using YAY

## Installing Packages

To install common packages using the Yay AUR helper, run the following commands:

### Git

```bash
yay -S git
```

### Node Package Managers

```bash
yay -S npm pnpm yarn
```

### Rust

```bash
yay -S rust
```

### Base Development Tools

```bash
yay -S base-devel
```

## Important: Export Cargo Path

After installing Rust, you need to add Cargo to your `PATH`:

```bash
export PATH=$HOME/.cargo/bin:$PATH
```

You can add this line to your `~/.bashrc` or `~/.zshrc` to make it persistent.

## Installing asdf

To manage multiple runtime versions, install `asdf-vm`:

```bash
yay -S asdf-vm
```

### Activating asdf

To activate `asdf`, add the following to your shell configuration file (`~/.bashrc` or `~/.zshrc`):

```bash
. /opt/asdf-vm/asdf.sh
```

Alternatively, you can source it directly in your terminal session:

```bash
source /opt/asdf-vm/asdf.sh
```

Now you are ready to use `asdf` for managing your runtime versions.

By following these steps, you will have the essential development tools and version managers set up on your Arch Linux installation in WSL.
