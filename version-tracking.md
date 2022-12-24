## Done
- callaudiod 0.1.6
- clapper 0.5.2
- d-spy 1.4.0
- feedbackd 0.0.2
- gnome-calls v43.2
- gnome-podcasts master(2022-11-01)
- gnome-sound-recorder 43.beta
- loupe(2022-12-08) (last pre-GTK4.10 commit)
- sofia-sip 1.13.10

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