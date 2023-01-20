## Done
- at-spi2-core 2.47.1
- callaudiod 0.1.6
- clapper 0.5.2
- d-spy 1.4.0
- eog 44.alpha
- epiphany master(2023-01-20)
- evolution 3.47.1
- evolution-data-server master(2023-01-20)
- evolution-ews 3.47.1
- feedbackd 0.0.2
- glib2 main(2023-01-14)
- glib-networking 2.76.alpha
- gnome-builder main(2023-01-20)
- gnome-calls v44_alpha.1
- gnome-control-center 44.alpha
- gnome-initial-setup master(2023-01-20)
- gnome-maps v44.alpha
- gnome-podcasts master(2022-12-16)
- gnome-remote-desktop 44.alpha
- gnome-software 44.alpha
- gnome-sound-recorder 43.beta
- gnome-text-editor 44.alpha
- gobject-introspection 1.75.4
- gtk4 4.9.2
- gtksourceview5 5.7.0
- libadwaita 1.3.alpha
- libdex main(2023-01-20)
- libpanel 1.1.0
- loupe(2022-12-08) (last pre-GTK4.10 commit)
- nautilus 44.alpha
- sofia-sip 1.13.12
- tracker 3.5.0.alpha
- tracker-miners 3.5.0.alpha
- webkitgtk-6.0 2.39.5
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