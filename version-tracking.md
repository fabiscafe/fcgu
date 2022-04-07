# Packages
## Done
- callaudiod 0.1.4
- clapper 0.4.1
- evince 42.1
- evolution 3.44.0
- evolution-data-server 3.44.0
- feedbackd 0.0.0+git20220208
- gdm 42.0
- gnome-backgrounds 42.0
- gnome-bluetooth 42.0
- gnome-builder 42.0
- gnome-calculator 42.0
- gnome-calendar 42.0
- gnome-calls 42.0
- gnome-characters 42.0
- gnome-clocks 42.0
- gnome-connections 42.1
- gnome-console main(2022-03-25)
- gnome-contacts 42.0
- gnome-control-center 42.0
- gnome-disk-utility 42.0
- gnome-font-viewer 42.0
- gnome-initial-setup 42.1
- gnome-logs gnome-logs-42.0
- gnome-maps v42.0
- gnome-music 42.0
- gnome-photos 42.0
- gnome-podcasts master(2022-03-25) +MR199
- gnome-remote-desktop 42.0
- gnome-shell 42.0
- gnome-shell-extensions 42.0
- gnome-software 42.0
- gnome-sound-recorder 42.0
- gnome-system-monitor 42.0
- gnome-terminal 3.44.0
- gnome-text-editor 42.0
- gnome-tour 42.0
- gnome-tweaks 42.beta
- gnome-user-docs 42.0
- gnome-weather 42.0
- gsettings-desktop-schemas 42.0
- libgweather 4.0.0 #Upgrade overlay
- mutter 42.0
- sofia-sip 1.13.7

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
