# FabisCafe Gnome Unstable
or short "FCGU" is a GNOME Unstable repository for [**Arch Linux**](https://archlinux.org). That contains *beta* and *rc* releases of GNOME for testing and bugreporting purposes.

### Support
#### Ko-Fi (Also for Paypal and one-time donations)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/R5R4CALOG)
#### Liberapay
[![Donate using Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/Fabiscafe/donate)
![Liberapay receiving](https://img.shields.io/liberapay/receives/fabiscafe?style=for-the-badge) ![Liberapay patrons](https://img.shields.io/liberapay/patrons/fabiscafe?style=for-the-badge)

### Chat / Matrix
![Matrix](https://img.shields.io/matrix/fcgu:matrix.org?style=for-the-badge)

Feel free to [join us at our matrix group](https://matrix.to/#/#fcgu:matrix.org) or [ping me](https://matrix.to/#/@fabiscafe:matrix.org) directly.

## Looking For New Mirrors
FCGU is a free community project. That's why we need your help. If you own a server that could become a mirror of the project, please let us know.

![preview](https://codeberg.org/fabiscafe/gnome-unstable/raw/branch/main/assets/fcgu.png)

## Installation
### Disable unsupported repos
Before you start - disable all 3rd-party-, as well as Arch testing-repos and downgrade/uninstall packages they provide. FCGU is not compatible with them and things might break on you if you keep them enabled. <span style="text-decoration: underline">Do not report any problem with them enabled</span>.

### Keyring
All of our packages are signed. To be able to install trustworthy packages it's necessary to install and trust the signing-key first.

```
# pacman-key --keyserver hkps://keys.openpgp.org --recv-keys 6E58E886A8E07538A2485FAED6A4F386B4881229
# pacman-key --lsign-key 6E58E886A8E07538A2485FAED6A4F386B4881229
```

### Mirror-List
[fcgu-mirrorlist](https://codeberg.org/fabiscafe/gnome-unstable/src/branch/main/fcgu-mirrorlist) is an own package that should be available from all mirror servers. You need to install.
```
# pacman -U https://vmi394248.contaboserver.net/fcgu/fcgu-mirrorlist-2-4-any.pkg.tar.zst
```

### Repository
This repository entry should be *below* the **[core]** repo, but *above* every other one in */etc/pacman.conf*.

```
[fcgu]
Include = /etc/pacman.d/fcgu-mirrorlist
```

Here is a preview how it should look:

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
Include = /etc/pacman.d/fcgu-mirrorlist

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
Include = /etc/pacman.d/fcgu-mirrorlist
```

When that's done a `pacman -Syuu` will downgrade all packages to the Arch-repo versions. After thats done, you need to check for additional packages who where not removed but can conflict with your installation. Check with `pacman -Qm` and remove them.

## Frequently Asked Questions - FAQ
## Will you do alpha releases?
This depends. Alpha releases often contain broken builds and might come with dependencies on pre-alpha development snapshots of other software. This isn't ideal to providing packages. It's recommended to get the alpha releases from the development snapshots on the AUR.

### Will you do the stable releases?
Yes, FCGU will also package stable releases until they arrive in Arch Linux directly.

### What happens after the stable release is shipped in Arch Linux?
Once the stable version of GNOME arrives Arch Linux official repository, fcgu will remove its packages, so pacman will switch to the official repository again.

### Why do I get downgrade warnings?

```
warning: $package: downgrading from version 1:2.34.5+678+g91011d12-1 to version 1:2.34.5+r678+g91011d12-1
```

Sometimes this repo needs to revert versions or change the version numbers scheme. Please use `pacman -Syuu` in these cases.

### Will this kill my setup?
This repository provides most of the time unstable software (development snapshots). It's not reliable in any way, and should only be used for testing purpose.

### How the get debugging symbols?
All packages are build with debugging symbols. Most of them require the user to install the packages debugging packages. For example there is `nautilus` and `nautilus-debug`. For everything that is not in the repo, you need to build the packages yourself, see: [Debugging/Getting_traces](https://wiki.archlinux.org/title/Debugging/Getting_traces)

### Compatiblity to Arch-Based-Distros
We only support (an up-to-date) Arch Linux.
Distros who come with older package versions or customization can conflict with what this project provides. Because of this they are not supported. This includes [Arco Linux](https://arcolinux.com), [Artix Linux](https://artixlinux.org), [EndeavourOS](https://endeavouros.com), [Garuda Linux](https://garudalinux.org), [Manjaro](https://manjaro.org), and [all the others](https://wiki.archlinux.org/title/Arch-based_distributions).

### Pamac conflict / removal
TLDR: This Repo only supports pacman. The mirrorlist package does provide the line `conflicts=(pamac libpamac)`. **Please remove pamac if you want to use fcgu.**

#### Why?
fcgu is a pretty unstable, testing repo. It highly depends on the functionality of pacman. Manjaros Pamac does bring in another logic that can conflict in way or another with this repo as well as with the path to move back to distros packages.
Because of this, pamac was set as conflict. If you still want to use pamac **You still can make it work by manually adding the mirrorlist**

### Will you push the PKGBUILDs to the AUR?
In order to do this, the PKGBUILDs would need a lot of extra work and testing, just for the packaging part. Because time is a very limited resource that's not possible to do right now (and not planned for the future).

### I want to provide a mirror.
If you want to have your own mirror, please do a [PR](https://codeberg.org/fabiscafe/gnome-unstable/pulls) and add your mirror to the [fcgu-mirrorlist](https://codeberg.org/fabiscafe/gnome-unstable/src/branch/main/fcgu-mirrorlist/mirrorlist). If that's done. [Join us on matrix](https://codeberg.org/fabiscafe/gnome-unstable#chat-matrix), as we also need your servers IP6/4 addresses to allow the sync. Alternatively you can also ask one of the current mirror providers in order to mirror a mirror.

## Troubleshooting
### error: GPGME error: No data
You might have hit a broken mirrorserver. Please [report this](https://codeberg.org/fabiscafe/gnome-unstable/issues).
Feel free to switch to another mirror. In case you still can't sync (`-Syu`) you have to delete */var/lib/pacman/sync/fcgu.db* manually.

```
rm "/var/lib/pacman/sync/fcgu.db"
```
