## Done
- adwaita-icon-theme 43.beta.1
- at-spi2-core 2.45.91
- baobab 43.beta
- callaudiod 0.1.4
- cheese 43.alpha
- clapper 0.5.2
- dconf-editor 43.beta
- d-spy 1.2.1
- eog 43.beta
- epiphany 43.rc
- evince 43.alpha
- evolution 3.45.2
- evolution-data-server 3.45.2
- feedbackd 0.0.0+git20220520
- file-roller 43.alpha
- folks 0.15.5
- gcr-4 3.90.0
- geary main(2022-08-26)
- gedit 43.alpha
- geocode-glib-2 3.26.4
- gjs 1.73.2
- glib2 2.73.3
- glib-networking 2.74.rc
- gnome-backgrounds 43.beta
- gnome-boxes 43.beta
- gnome-builder 43.alpha1¹
- gnome-calculator 43.alpha
- gnome-calendar 43.beta
- gnome-calls v43_beta.0
- gnome-characters 43.beta
- gnome-clocks 43.beta
- gnome-connections 43.beta
- gnome-console 43.beta
- gnome-contacts 43.beta
- gnome-control-center 43.beta
- gnome-desktop 43.alpha
- gnome-disk-utility 43.beta
- gnome-font-viewer 43.beta
- gnome-initial-setup 43.alpha1
- gnome-logs 43.beta
- gnome-maps main(2022-08-29)
- gnome-online-accounts 3.45.2
- gnome-photos 43.beta
- gnome-podcasts master(2022-07-29)
- gnome-remote-desktop 43.beta
- gnome-session 42.0
- gnome-settings-daemon 43.beta
- gnome-shell 43.beta
- gnome-shell-extensions 43.beta
- gnome-shell-extension-appindicator 43.alpha
- gnome-software 43.beta
- gnome-sound-recorder 43.beta
- gnome-terminal 3.45.90
- gnome-text-editor 43.alpha1
- gnome-tour 43.beta
- gnome-weather 43.beta
- gobject-introspection 1.73.0
- grilo master(2022-07-04)
- grilo-plugins master(2022-07-31)
- gsettings-desktop-schemas 43.alpha
- gtk4 4.7.2
- gtksourceview5 5.5.1
- js102 102.2.0
- libadwaita 1.2.beta
- libgweather-4 4.1.0
- libhandy 1.7.90
- libosinfo 1.10.0
- libpanel 1.0alpha1
- librest 0.9.1
- libshumate 1.0.0.beta
- libsoup3 3.1.1
- mutter 43.beta
- nautilus 43.beta.1
- python-nautilus 4.0.alpha
- orca ORCA_43_BETA
- phodav 3.0
- sofia-sip 1.13.8
- spice-gtk 0.41
- sysprof 3.45.1
- template-glib 3.35.0
- totem 43.beta
- tracker3 3.4.0.beta
- tracker3-miners 3.4.0.beta
- vte3 0.69.92
- webkit2gtk-4.1 2.37.90
- xdg-desktop-portal-gnome 43.beta

## Wontbuild
- gnome-builder 43.alpha1 (gnome-builder-libide-docs, check())
- gnome-initial-setup 43.beta (Waiting for malcontent 0.11 release)

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
