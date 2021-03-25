# FabisCafe Gnome Unstable
or short "FCGU" is a GNOME Unstable repository for [**Arch Linux**](https://archlinux.org). That contains *alpha*, *beta* and *rc* releases of GNOME for testing and bugreporting purposes.

Talk to us on Matrix: [#fcgu:matrix.org](https://matrix.to/#/#fcgu:matrix.org?via=matrix.org) 
<p align="center">
<!---![FCGU](https://gitlab.com/fabis_cafe/gnome-unstable/-/raw/main/assets/fcgu.png)-->
</p>

## Installation
### Keyring
All of our packages are signed, to be able to install trustworthy packages the user needs to install [fcgu-keyring(AUR)](https://aur.archlinux.org/packages/fcgu-keyring) first.

```
pacman -S git
git clone https://aur.archlinux.org/fcgu-keyring.git
cd fcgu-keyring
makepkg -cis
```

### Add the repo
This repo is made as an overlay repo. This means it will replace the Arch-GNOME packages. It will **not** install **side-by-side**. To work as overlay the repo needs to be above the **[core]** section in */etc/pacman.conf*.

```
[fcgu]
Server = http://34.105.163.196/$repo
```

Here a preview how it should look:

```
...
# The testing repositories are disabled by default. To enable, uncomment the
# repo name header and Include lines. You can add preferred servers immediately
# after the header, and they will be used before the default mirrors.

#[testing]
#Include = /etc/pacman.d/mirrorlist

[fcgu]
Server = http://34.105.163.196/$repo

[core]
Include = /etc/pacman.d/mirrorlist

[extra]
Include = /etc/pacman.d/mirrorlist

#[community-testing]
#Include = /etc/pacman.d/mirrorlist
...
```

If that's done, a full system update is required (`pacman -Syu`)
<p align="center">
<!---![preview](https://gitlab.com/fabis_cafe/gnome-unstable/-/raw/main/assets/video.gif)-->
</p>

## Will this kill my setup?
This repo will bring in unstable development software. It's not reliable in any way, and should only be used for testing purpose.

## How to change back to Arch' default GNOME?
The repo needs to be removed from */etc/pacman.conf*

```
[fcgu]
Server = http://34.105.163.196/$repo
```
When thats done a `pacman -Syuu` will downgrade all packages to the Arch-repo versions.

## What happens after the stable release is shipped?
Once the stable version of GNOME arrives Arch Linux official repository, this fcgu will remove its packages, so pacman will switch to the official repo again.