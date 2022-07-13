# Packages
## Done
- at-spi2-core 2.45.1
- callaudiod 0.1.4
- evolution-data-server 3.45.1
- folks 0.15.5
- gcr-4 3.90.0
- geocode-glib-2 3.26.3
- gjs 1.73.1
- glib2 2.73.2
- glib-networking 2.74.alpha
- gnome-desktop master(2022-07-12)
- gnome-online-accounts 3.45.1
- gnome-session 42.0
- gnome-settings-daemon 42.2
- gtk4 4.7.1
- gtksourceview5 5.5.0
- libadwaita 1.2.alpha
- libgweather-4 4.0.0
- libhandy 1.7.0
- librest 0.9.1
- sysprof 3.45.0
- xdg-desktop-portal-gnome 43.alpha


## Wontbuild
- none

## Exclude
- none

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
* pkgver: 1 -> 0.1
