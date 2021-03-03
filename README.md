# FCGU
FCGU is a GNOME Unstable repo, by a Arch Linux community member named Fabiscafe.

## Whats in this repo?
Mostly Beta and RC releases of GNOME software with debug-symbols enabled. So you can help testing, reporting and fixing.

## How to add it?
You can add it as an overlay repo in your *pacman.conf*, above the **[core]** section

```
[fcgu]
Server = TODO/$repo
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
Server = TODO/$repo
SigLevel = Optional

[core]
Include = /etc/pacman.d/mirrorlist

[extra]
Include = /etc/pacman.d/mirrorlist

#[community-testing]
#Include = /etc/pacman.d/mirrorlist
...
```

If that's done, just update your system (`pacman -Syu`)

## Will this kill my setup?
As you can see by reading the name, this repo will bring in unstable development software. It's not reliable in any way.

## How to change back to Arch' default GNOME?
Remove the repo from */etc/pacman.conf* and run `pacman -Syuu`. This will downgrade all packages to the Arch-repo versions.

## Is there more to know?
Currently the repo doesn't come with signed packages. So it's dangerouse to use them. This might change in the future.

## Where can I talk to you?
We're on

* Matrix [#fcgu:matrix.org](https://matrix.to/#/#fcgu:matrix.org?via=matrix.org)