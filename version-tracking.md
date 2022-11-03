## Done
- amtk 5.6.0
- callaudiod 0.1.4
- clapper 0.5.2
- d-spy 1.4.0
- feedbackd 0.0.0+git20220520
- gedit 43.0
- gnome-boxes 43.1
- gnome-calls v43.0
- gnome-endeavour v43.0
- gnome-podcasts master(2022-07-29)
- gnome-sound-recorder 43.beta
- gtranslator 42.0
- sofia-sip 1.13.9
- tepl 6.2.0

## Wontbuild

## Exclude
- none

# Versioning
## Git snapshots
* tag+r60+g3f9dba93c
  * `sed 's/[^-]*-g/r&/;s/-/+/g'`

## Dev releases
* X.beta.1 -> X.beta1
  * `sed -r 's/([a-z])\./\1/;s/[^-]*-g/r&/;s/-/+/g'`
* X.0.beta.1 -> X.0beta1
  * `sed -r 's/\.([a-z])/\1/;s/[^-]*-g/r&/;s/-/+/g'`

## Stable releases
* pkgver: 1 -> 0.1
* X -> X.0
  * `sed -r '/\.([0-9])/!s/$/\.0/;s/[^-]*-g/r&/;s/-/+/g'`