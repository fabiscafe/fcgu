## Done
- adwaita-icon-theme 44.beta
- at-spi2-core 2.47.1
- baobab 44.beta
- callaudiod 0.1.6
- clapper 0.5.2
- d-spy 1.5.0
- eog 44.beta
- epiphany 44.beta
- evolution 3.47.2
- evolution-data-server 3.47.2
- evolution-ews 3.47.2
- feedbackd 0.0.3
- gjs 1.75.2
- glib2 2.75.3
- glib-networking 2.76.beta
- gnome-backgrounds 44.beta
- gnome-boxes 44.beta.1
- gnome-builder 44.beta
- gnome-calculator 44.beta
- gnome-calendar 44.beta
- gnome-calls v44_alpha.1
- gnome-characters 44.beta
- gnome-clocks 44.beta
- gnome-connections 44.beta
- gnome-console 44.beta
- gnome-contacts 44.beta
- gnome-control-center 44.beta
- gnome-desktop 44.beta
- gnome-disks-utility 44.beta
- gnome-font-viewer 44.beta
- gnome-initial-setup 44.beta
- gnome-maps v44.beta
- gnome-music 44.beta
- gnome-online-accounts 3.47.1
- gnome-podcasts master(2022-12-16)
- gnome-remote-desktop 44.alpha
- gnome-settings-daemon 44.beta
- gnome-shell 44.beta
- gnome-shell-extensions 44.beta
- gnome-software 44.beta
- gnome-sound-recorder 43.beta
- gnome-system-monitor 44.beta
- gnome-terminal 3.47.92
- gnome-text-editor 44.beta
- gnome-weather 44.beta
- gobject-introspection 1.75.6
- gsettings-desktop-schemas 44.beta
- gtk4 4.9.4
- gtksourceview5 5.7.1
- libadwaita 1.3.beta
- libdex main(2023-02-01)
- libpanel 1.1.1
- librsvg 2.55.91
- libsoup3 3.3.1
- loupe(2023-02-12)
- mutter 44.beta
- nautilus 44.beta
- pygobject 3.43.1
- sofia-sip 1.13.14
- tracker 3.5.0.beta
- tracker-miners 3.5.0.beta
- vte 0.71.92
- webkitgtk-6.0 2.39.7
- wpewebkit 2.39.5
- xdg-desktop-portal-gnome 44.beta

## Wontbuild

## Exclude
- none

# Versioning
## Git snapshots
* tag+r60+g3f9dba93c
  * `sed 's/[^-]*-g/r&/;s/-/+/g'`

## Dev releases
* X.beta.1 -> X.beta1
* X.1.beta -> X.1beta
* X.0.beta.1 -> X.0beta.1
  * `sed -r 's/\.([a-z])/\1/;s/([a-z])\./\1/;s/[^-]*-g/r&/;s/-/+/g'`

## Stable releases
* pkgver: 1 -> 0.1
* X -> X.0
  * `sed -r '/\.([0-9])/!s/$/\.0/;s/[^-]*-g/r&/;s/-/+/g'`