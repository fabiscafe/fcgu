## Done
- at-spi2-core 2.47.1
- baobab 44.beta
- callaudiod 0.1.6
- clapper 0.5.2
- d-spy 1.4.0
- eog 44.beta
- epiphany 44.beta
- evolution 3.47.2
- evolution-data-server 3.47.2
- evolution-ews 3.47.2
- feedbackd 0.0.3
- glib2 main(2023-01-20)
- glib-networking 2.76.beta
- gnome-builder main(2023-02-01)
- gnome-calculator 44.beta
- gnome-calls v44_alpha.1
- gnome-characters 44.beta
- gnome-clocks 44.beta
- gnome-connections 44.beta
- gnome-contacts 44.beta
- gnome-control-center 44.alpha
- gnome-disks-utility 44.beta
- gnome-font-viewer 44.beta
- gnome-initial-setup master(2023-01-20)
- gnome-maps v44.beta
- gnome-podcasts master(2022-12-16)
- gnome-remote-desktop 44.alpha
- gnome-software 44.alpha
- gnome-sound-recorder 43.beta
- gnome-system-monitor 44.beta
- gnome-terminal 3.47.92
- gnome-text-editor 44.alpha
- gnome-weather 44.beta
- gobject-introspection 1.75.4
- gtk4 4.9.4
- gtksourceview5 5.7.0
- libadwaita 1.3.beta
- libdex main(2023-01-20)
- libpanel 1.1.0
- libsoup3 3.3.1
- loupe(2023-02-12)
- nautilus 44.beta
- sofia-sip 1.13.13
- tracker 3.5.0.alpha
- tracker-miners 3.5.0.alpha
- vte 0.71.92
- webkitgtk-6.0 2.39.7
- wpewebkit 2.39.5
- xdg-desktop-portal-gnome 44.alpha

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