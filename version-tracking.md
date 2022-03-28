# Packages
## Done
- adwaita-icon-theme 42.0
- baobab 42.0
- callaudiod 0.1.4
- clapper 0.4.1
- eog 42.0
- epiphany 42.0
- evince 42.1
- evolution 3.44.0
- evolution-data-server 3.44.0
- feedbackd 0.0.0+git20220208
- gdm 42.0
- gjs 1.72.0
- gnome-backgrounds 42.0
- gnome-bluetooth 42.0
- gnome-boxes 42.0.1
- gnome-builder 42.0
- gnome-calculator 42.0
- gnome-calendar 42.0
- gnome-calls 42.0
- gnome-characters 42.0
- gnome-clocks 42.0
- gnome-connections 42.0
- gnome-console main(2022-03-02)
- gnome-contacts 42.0
- gnome-control-center 42.0
- gnome-desktop 42.0
- gnome-disk-utility 42.0
- gnome-font-viewer 42.0
- gnome-initial-setup 42.0.1
- gnome-maps v42.0
- gnome-music 42.0
- gnome-photos 42.0
- gnome-podcasts master(2022-03-21) +MR199
- gnome-remote-desktop 42.0
- gnome-session 42.0
- gnome-settings-daemon 42.1
- gnome-shell 42.0
- gnome-shell-extensions 42.0
- gnome-software 42.0
- gnome-sound-recorder 42.0
- gnome-system-monitor 42.0
- gnome-terminal 3.43.90
- gnome-text-editor 42.0
- gnome-tour 42.0
- gnome-tweaks 42.beta
- gnome-user-docs 42.0
- gnome-weather 42.0
- gsettings-desktop-schemas 42.0
- gtksourceview5 5.4.0
- ibus 1.5.26
- libgnome-games-support-gtk4 2.0.0
- libgweather 4.0.0
- libnma 1.8.36
- mutter 42.0
- nautilus 42.0
- orca ORCA_42_0
- simple-scan 42.0
- sofia-sip 1.13.7
- totem 42.0
- vte3 0.68.0
- xdg-desktop-portal-gnome 42.0.1
- yelp 42.1

## Wontbuild
none
## Exclude
none

# Versioning
## Git snapshots
* tag+r60+g3f9dba93c
  * `s/[^-]*-g/r&/;s/-/+/g;`
## Dev releases
* X.beta -> X.beta0
  * `s/beta/beta0/`
* X.beta.1 -> X.beta1
  * `s/beta.\([0-9]\+\)/beta\1/`
* X.0.beta -> X.0beta0
* `s/.beta/beta0/`
* X.0.beta.1 -> X.0beta1
  * `s/0.beta.\([0-9]\+\)/beta\1/`
## Stable releases
pkgver: 1 -> 0.1
