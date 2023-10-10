# FCGU - Repo for GNOME pre-releases
"FCGU" was a Git repo for PKGBUILDs as well as a binary repo of GNOME pre-releases for [**Arch Linux**](https://archlinux.org).

Because the [project lead](https://archlinux.org/people/trusted-users/#fabiscafe) is now part of the Arch Linux crew, FCGU was dropped in favor of Arch' [gnome-unstable](https://wiki.archlinux.org/title/Official_repositories#gnome-unstable) Repo.

### Support
You can still support me!

#### Ko-Fi (Also for Paypal and one-time donations)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/R5R4CALOG)

#### Liberapay
[![Donate using Liberapay](https://liberapay.com/assets/widgets/donate.svg)](https://liberapay.com/Fabiscafe/donate)
![Liberapay receiving](https://img.shields.io/liberapay/receives/fabiscafe?style=for-the-badge) ![Liberapay patrons](https://img.shields.io/liberapay/patrons/fabiscafe?style=for-the-badge)

### Chat / Matrix & Mastodon / Fediverse
![Matrix](https://img.shields.io/matrix/fcgu:matrix.org?logo=Matrix&style=for-the-badge)
![Mastodon Follow](https://img.shields.io/mastodon/follow/000293265?domain=https%3A%2F%2Fmstdn.social&logo=Mastodon&style=for-the-badge)

Feel free to [join us at our matrix group](https://matrix.to/#/#fcgu:matrix.org) or ping me on [Matrix](https://matrix.to/#/@fabiscafe:matrix.org), or [on Fediverse/Mastodon](https://mstdn.social/@fabiscafe) directly. 😜️

-----
-----
-----


## How to change back to Arch' default GNOME?
The repo needs to be removed from */etc/pacman.conf*

```
[fcgu]
Include = /etc/pacman.d/fcgu-mirrorlist
```

When that's done a `pacman -Syuu` will downgrade all packages to the Arch-repo versions. After thats done, you need to check for additional packages who where not removed but can conflict with your installation. Check with `pacman -Qm` and remove them.