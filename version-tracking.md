## Done
- adwaita-icon-theme 43.beta
- at-spi2-core 2.45.1
- baobab 43.alpha
- callaudiod 0.1.4
- cheese 43.alpha
- clapper 0.5.2
- dconf-editor 43.beta
- d-spy 1.2.1
- eog 43.alpha
- epiphany 43.alpha
- evince 43.alpha
- evolution 3.45.2
- evolution-data-server 3.45.2
- feedbackd 0.0.0+git20220520
- folks 0.15.5
- gcr-4 3.90.0
- geary main(2022-07-13)
- gedit 43.alpha
- geocode-glib-2 3.26.3
- gjs 1.73.1
- glib2 2.73.3
- glib-networking 2.74.alpha
- gnome-backgrounds 43.beta
- gnome-boxes 43.alpha
- gnome-builder 43.alpha0
- gnome-calculator 43.alpha
- gnome-calendar 43.alpha
- gnome-calls 43.alpha2
- gnome-characters 43.alpha
- gnome-clocks 43.alpha
- gnome-console 42.2
- gnome-contacts 43.alpha
- gnome-control-center 43.alpha
- gnome-desktop 43.alpha
- gnome-disk-utility 43.alpha
- gnome-font-viewer 43.alpha
- gnome-initial-setup 43.alpha1
- gnome-maps 43.alpha
- gnome-online-accounts 3.45.1
- gnome-podcasts-gtk4 master(2022-07-29)
- gnome-remote-desktop 43.alpha
- gnome-session 42.0
- gnome-settings-daemon 43.alpha
- gnome-shell 43.alpha
- gnome-shell-extensions 43.alpha
- gnome-shell-extension-appindicator 43.alpha
- gnome-software 43.beta
- gnome-text-editor 43.alpha1
- gnome-weather 43.alpha
- gobject-introspection 1.73.0
- gsettings-desktop-schemas 43.alpha
- gtk4 4.7.1
- gtksourceview5 5.5.1
- libadwaita 1.2.beta
- libgit2-glib 1.1.0
- libgweather-4 4.1.0
- libhandy 1.7.90
- libosinfo 1.10.0
- libpanel 1.0alpha
- librest 0.9.1
- libsoup3 3.1.1
- mutter 43.alpha
- nautilus 43.alpha
- orca ORCA_43_ALPHA
- phodav 3.0
- sofia-sip 1.13.8
- spice-gtk 0.41
- sysprof 3.45.1
- template-glib 3.35.0
- totem 43.alpha
- tracker3 3.4.0.alpha
- tracker3-miners 3.4.0.alpha
- vte3 0.69.90
- xdg-desktop-portal-gnome 43.alpha


## Wontbuild
- none


## Exclude
- epiphany 43.beta (I dont have the hardware to build webkit right now)

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
