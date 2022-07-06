# Packages
## Done
- at-spi2-core AT_SPI2_CORE_2_45_1
- callaudiod 0.1.4
- clapper 0.5.2
- feedbackd v0.0.0+git20220520
- gedit 43.alpha
- gnome-calls v43_alpha.2
- gnome-connections 42.1.2
- gnome-console main(2022-04-01)
- gnome-initial-setup 43.alpha
- gnome-maps v43.alpha
- gnome-podcasts master(2022-05-25) +MR199
- gnome-software 43.alpha
- gnome-text-editor 42.2
- libgweather 4.0.0 #Upgrade overlay
- orca ORCA_43_ALPHA
- sofia-sip 1.13.8

## Wontbuild
none
## Exclude
- evolution-data-server 3.45.1 #waiting for an gcr-4 release
- evolution 3.45.1 #waiting for evolution-data-server

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
