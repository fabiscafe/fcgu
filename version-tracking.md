## Done
- at-spi2-core 2.47.1
- callaudiod 0.1.6
- clapper 0.5.2
- d-spy 1.4.0
- eog 44.alpha
- epiphany 44.alpha
- evolution 3.47.1
- evolution-data-server 3.47.1
- evolution-ews 3.47.1
- feedbackd 0.0.2
- glib2 2.75.2
- glib-networking 2.76.alpha
- gnome-calls v43.2
- gnome-maps v44.alpha
- gnome-podcasts master(2022-12-16)
- gnome-software 44.alpha
- gnome-sound-recorder 43.beta
- gtk4 4.9.2
- libadwaita 1.3.alpha
- loupe(2022-12-08) (last pre-GTK4.10 commit)
- sofia-sip 1.13.11
- webkitgtk-6.0 2.39.3

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