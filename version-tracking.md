# Packages
## Done
- callaudiod 0.1.4
- clapper 0.4.1
- evince 42.1
- evolution 3.44.0
- feedbackd 0.0.0+git20220208
- gnome-calls 42.0
- gnome-console main(2022-03-25)
- gnome-initial-setup 42.1
- gnome-podcasts master(2022-03-25) +MR199
- gnome-text-editor 42.0
- gnome-tour 42.0
- libgweather 4.0.0 #Upgrade overlay
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
