# bootstrap-archlinux
Series of scripts for setting up my archlinux environment on a physical device

## Usage

To create a new system, you'll need to:

1. Pull down this repo
```
wget -O bootstrap-archlinux.zip https://github.com/lkirk/bootstrap-archlinux/archive/refs/heads/main.zip
unzip bootstrap-archlinux.zip
cd boostrap-archlinux-main
```
2. Connect to the internet (wifi/ethernet)

3. Run the `do-all` command to execute all of the scripts (be sure to double check your `INSTALL_DISK`.

```
INSTALL_DISK=/dev/sda \
ROOT_SIZE=60 \
SWAP_SIZE=16 \
HOSTNAME=something \
GRUB_PARTITION=/dev/sda2 \
USER_NAME=joey \
USER_SHELL=/usr/bin/zsh \
./do-all
```
