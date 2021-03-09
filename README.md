# FCGU
FCGU is a GNOME Unstable repo, by a Arch Linux community member named Fabiscafe.

## Whats in this repo?
Mostly Beta and RC releases of GNOME software with debug-symbols enabled. For easy testing and bugreporting porposes.

## How to add it?
### Keyring
In order to have trustworthy packages, fcgu packages are signed. Because this requires an external gpg key, a user needs to add them as trusted key. There are 2 options to do this:
#### AUR helper
If there is an an AUR-helper, install [fcgu-keyring](https://aur.archlinux.org/packages/fcgu-keyring).

#### Manually
This will clone, build and install the AUR PKGBUILD

```
pacman -S git
git clone https://aur.archlinux.org/fcgu-keyring.git
cd fcgu-keyring
makepkg -cis
```

### Add the repo
This repo is made as an overlay repo. This means it will replace the Arch-GNOME packages. It will not install side-by-side. To work as overlay the repo needs to be above the **[core]** section in *pacman.conf*.

```
[fcgu]
Server = http://34.105.163.196/$repo
SigLevel = Optional
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
SigLevel = Optional

[core]
Include = /etc/pacman.d/mirrorlist

[extra]
Include = /etc/pacman.d/mirrorlist

#[community-testing]
#Include = /etc/pacman.d/mirrorlist
...
```

If that's done, a full system update is required (`pacman -Syu`)

## Will this kill my setup?
This repo will bring in unstable development software. It's not reliable in any way, and should only be used for testing purpose.

## How to change back to Arch' default GNOME?
Its always powwisble to change back to Arch-defaults by editing */etc/pacman.conf* (to remove the repo that was added before) and run `pacman -Syuu`. This will downgrade all packages to the Arch-repo versions.

## What happens after the stable release is shipped?
Once the stable version of GNOME arrives Arch Linux official repository, this fcgu will remove its packages, so pacman will switch to the official repo again.

## Where can I talk to you?
We're on

* Matrix [#fcgu:matrix.org](https://matrix.to/#/#fcgu:matrix.org?via=matrix.org)