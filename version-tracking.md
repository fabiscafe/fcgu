## Done
- adwaita-icon-theme 44.beta
- at-spi2-core 2.47.90
- baobab 44.rc
- callaudiod 0.1.6
- clapper 0.5.2
- d-spy 1.5.0
- eog 44.beta
- epiphany 44.rc
- evince 44.rc
- evolution 3.47.3
- evolution-data-server 3.47.3
- evolution-ews 3.47.3
- feedbackd 0.1.0
- gcr-4 4.1.0
- gdm 44.rc-real
- gjs 1.75.90
- glib2 2.75.4
- glib-networking 2.76.beta
- gnome-backgrounds 44.beta
- gnome-boxes 44.rc
- gnome-builder 44.rc
- gnome-calculator 44.rc
- gnome-calendar 44.rc
- gnome-calls v44_alpha.1
- gnome-characters 44.rc
- gnome-clocks 44.rc
- gnome-connections 44.rc
- gnome-console 44.beta
- gnome-contacts 44.rc
- gnome-control-center 44.rc
- gnome-desktop 44.beta
- gnome-disks-utility 44.rc
- gnome-font-viewer 44.rc
- gnome-initial-setup 44.rc
- gnome-keyring 42.1 (gcr-4 rebuild)
- gnome-maps v44.rc
- gnome-music 44.rc
- gnome-online-accounts 3.47.1
- gnome-podcasts master(2022-12-16)
- gnome-remote-desktop 44.rc
- gnome-session 44.rc
- gnome-settings-daemon 44.rc
- gnome-shell 44.rc
- gnome-shell-extensions 44.rc
- gnome-software 44.rc
- gnome-sound-recorder 43.beta
- gnome-system-monitor 44.rc
- gnome-terminal 3.47.99
- gnome-text-editor 44.rc
- gnome-user-docs 44.rc
- gnome-weather 44.rc
- gobject-introspection 1.75.6
- gsettings-desktop-schemas 44.beta
- gtksourceview5 5.7.2
- jsonrpc-glib 3.43.0
- libadwaita 1.3.rc
- libdex 0.1.1
- libnma 1.10.6 (gcr-4 rebuild)
- libpanel 1.1.2
- librsvg 2.55.91
- libsoup3 3.3.1
- loupe(2023-02-24)
- mutter 44.rc
- nautilus 44.rc
- pygobject 3.43.1
- sofia-sip 1.13.14
- tracker 3.5.0.rc
- tracker-miners 3.5.0.rc
- vte 0.71.99
- webkitgtk-6.0 2.39.90
- wpewebkit 2.39.5
- xdg-desktop-portal-gnome 44.rc

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