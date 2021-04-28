# FabisCafe Gnome Unstable <a href="https://liberapay.com/Fabiscafe/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a>
or short "FCGU" is a GNOME Unstable repository for [**Arch Linux**](https://archlinux.org). That contains *alpha*, *beta* and *rc* releases of GNOME for testing and bugreporting purposes.

<img src="https://img.shields.io/liberapay/receives/Fabiscafe.svg?logo=liberapay">


## Looking For New Mirrors
FCGU is a free community project. That's why we need your help. If you own a server that could become a mirror of the project, please let us know.

Talk to us on Matrix: [#fcgu:matrix.org](https://app.element.io/#/room/#fcgu:matrix.org)  - EMail: fabiscafe -cat- mailbox -dog- org

<p align="center">
![FCGU](https://gitlab.com/fabis_cafe/gnome-unstable/-/raw/main/assets/fcgu.png)
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
#Server = <looking for new mirrors>
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
#Server = <looking for new mirrors>

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
![preview](https://gitlab.com/fabis_cafe/gnome-unstable/-/raw/main/assets/video.gif)
</p>

## Will this kill my setup?
This repo will bring in unstable development software. It's not reliable in any way, and should only be used for testing purpose.

## How to change back to Arch' default GNOME?
The repo needs to be removed from */etc/pacman.conf*

```
[fcgu]
#Server = <looking for new mirrors>
```
When thats done a `pacman -Syuu` will downgrade all packages to the Arch-repo versions.

## What happens after the stable release is shipped?
Once the stable version of GNOME arrives Arch Linux official repository, this fcgu will remove its packages, so pacman will switch to the official repo again.
