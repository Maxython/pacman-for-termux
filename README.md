# pacman-for-termux
Configured pacman to install packages on termux. There are two kinds of pacman, **arch** and **termux**.  The main difference between the two is the support for installing packages (**pacman-arch** installs arch packages and **pacman-termux** installs termux packages).

## Note:
At this point, pacman is not fully configured for termux, so there may be bugs.  

## A warning:
#### pacman-arch
To install packages without dependencies, use the following command: `pacman -Sdd name_package`
#### pacman-termux
There are currently no compiled termux packages in pacman format, but you can make full use of `makepkg`.
```bash
makepkg -d
pacman -Udd *package_name*
```

## Commands for installing pacman.
```bash
pkg update -y
pkg install git -y
git clone https://github.com/Maxython/pacman-for-termux
cd pacman-for-termux
./install.sh
```
Restart termux after installation.

After these commands, restart termux and run the following command.
```bash
./pacman-for-termux/install.sh set2
```
