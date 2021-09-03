# FabisCafe Gnome Unstable <a href="https://liberapay.com/Fabiscafe/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a>
or short "FCGU" is a GNOME Unstable repository for [**Arch Linux**](https://archlinux.org). That contains *alpha*, *beta* and *rc* releases of GNOME for testing and bugreporting purposes.

<img src="https://img.shields.io/liberapay/receives/Fabiscafe.svg?logo=liberapay">


## Looking For New Mirrors
FCGU is a free community project. That's why we need your help. If you own a server that could become a mirror of the project, please let us know.

[![Matrix](https://img.shields.io/matrix/fcgu:matrix.org?style=for-the-badge)](https://app.element.io/#/room/#fcgu:matrix.org)

<p align="center">
![FCGU](https://gitlab.com/fabis_cafe/gnome-unstable/-/raw/main/assets/fcgu.png)
</p>

## Installation
### Keyring
All of our packages are signed, to be able to install trustworthy packages necessary to install and trust the signing-key first.

```
pacman-key --keyserver hkps://keys.openpgp.org --recv-keys 6E58E886A8E07538A2485FAED6A4F386B4881229
pacman-key --lsign-key 6E58E886A8E07538A2485FAED6A4F386B4881229
```

### Add the repo
This repo should be below the core repo, but above every other one. It will **not** install **side-by-side**. To work as overlay the repo needs to be above the **[core]** section in */etc/pacman.conf*.

```
[fcgu]
Server = https://gnome.holmie.xyz/$repo
Server = https://$repo.fabis.cafe/$repo
Server = https://vmi394248.contaboserver.net/$repo
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

[core]
Include = /etc/pacman.d/mirrorlist

[fcgu]
Server = https://gnome.holmie.xyz/$repo
Server = https://$repo.fabis.cafe/$repo
Server = https://vmi394248.contaboserver.net/$repo
#Server = <looking for new mirrors>

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
Server = https://gnome.holmie.xyz/$repo
Server = https://$repo.fabis.cafe/$repo
Server = https://vmi394248.contaboserver.net/$repo
#Server = <looking for new mirrors>
```
When thats done a `pacman -Syuu` will downgrade all packages to the Arch-repo versions.

## What happens after the stable release is shipped?
Once the stable version of GNOME arrives Arch Linux official repository, this fcgu will remove its packages, so pacman will switch to the official repo again.
