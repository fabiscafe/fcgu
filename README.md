# FabisCafe Gnome Unstable <a href="https://liberapay.com/Fabiscafe/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a>
or short "FCGU" is a GNOME Unstable repository for [**Arch Linux**](https://archlinux.org). That contains *alpha*, *beta* and *rc* releases of GNOME for testing and bugreporting purposes.

<img src="https://img.shields.io/liberapay/receives/Fabiscafe.svg?logo=liberapay">

## Looking For New Mirrors
FCGU is a free community project. That's why we need your help. If you own a server that could become a mirror of the project, please let us know.

[![Matrix](https://img.shields.io/matrix/fcgu:matrix.org?style=for-the-badge)](https://app.element.io/#/room/#fcgu:matrix.org)

![preview](https://gitlab.com/fabis_cafe/gnome-unstable/-/raw/main/assets/fcgu.png)

## Installation
### Keyring
All of our packages are signed, to be able to install trustworthy packages necessary to install and trust the signing-key first.

```
pacman-key --keyserver hkps://keys.openpgp.org --recv-keys 6E58E886A8E07538A2485FAED6A4F386B4881229
pacman-key --lsign-key 6E58E886A8E07538A2485FAED6A4F386B4881229
```

### Add the repo
This repo should be below the **[core]** repo, but above every other one in */etc/pacman.conf*.

```
[fcgu]
Server = https://gnome.holmie.xyz/$repo
Server = https://$repo.fabis.cafe/$repo
Server = https://vmi394248.contaboserver.net/$repo
Server = http://185.238.129.156/$repo
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
Server = http://185.238.129.156/$repo
#Server = <looking for new mirrors>

[extra]
Include = /etc/pacman.d/mirrorlist

#[community-testing]
#Include = /etc/pacman.d/mirrorlist
...
```

If that's done, a full system update is required (`pacman -Syu`)

## How to change back to Arch' default GNOME?
The repo needs to be removed from */etc/pacman.conf*

```
[fcgu]
Server = https://gnome.holmie.xyz/$repo
Server = https://$repo.fabis.cafe/$repo
Server = https://vmi394248.contaboserver.net/$repo
Server = http://185.238.129.156/$repo
#Server = <looking for new mirrors>
```
When that's done a `pacman -Syuu` will downgrade all packages to the Arch-repo versions.

## Frequently Asked Questions - FAQ
### Will you do the stable releases?
Yes, FCGU will also package stable releases until they arrive in Arch Linux directly.

### What happens after the stable release is shipped in Arch Linux?
Once the stable version of GNOME arrives Arch Linux official repository, fcgu will remove its packages, so pacman will switch to the official repository again.

### Will this kill my setup?
This repository provides most of the time unstable software (development snapshots). It's not reliable in any way, and should only be used for testing purpose.

### Why are the packages so huge?
All packages are build with debugging symbols. This requires a lot more space but is necessary to create useful bug reports.

On that topic please also read the [blog post by Michael Catanzaro](https://blogs.gnome.org/mcatanzaro/2021/09/18/creating-quality-backtraces-for-crash-report)

### Compatiblity to Arch-Based-Distros
We only give support for up-to-date Arch Linux. Older package bases will create issues down the line, because we need a certain version and will not build them on our side if they are available in Arch. So as long as your distro provides the same versions as Arch itself it should work.

#### Manjaro
Manjaro uses an own repository and **is not** compatible to Arch Linux. Based on experiences this repository will not work for Manjaro or will break your desktop at any point.

### Will you push the PKGBUILDs to the AUR?
In order to do this, the PKGBUILDs would need a lot of extra work and testing, just for the packaging part. Because time is a very limited resource that's not possible to do right now (and not planned for the future).
