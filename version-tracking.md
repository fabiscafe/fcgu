## Done
- adwaita-icon-theme 43.beta.1
- at-spi2-core 2.46.0
- baobab 43.rc
- callaudiod 0.1.4
- cheese 43.alpha
- clapper 0.5.2
- dconf-editor 43.beta
- d-spy 1.2.1
- eog 43.0
- epiphany 43.0
- evince 43.alpha
- evolution 3.46.0
- evolution-data-server 3.46.0
- feedbackd 0.0.0+git20220520
- file-roller 43.0
- folks 0.15.5
- gcr-4 3.92.0
- geary main(2022-08-26)
- gedit 43.alpha
- geocode-glib-2 3.26.4
- gjs 1.73.2
- glib2 2.74.0
- glib-networking 2.74.0
- gnome-backgrounds 43.rc
- gnome-boxes 43.0
- gnome-builder 43.alpha1¹
- gnome-calculator 43.0.1
- gnome-calendar 43.0
- gnome-calls v43_rc.0
- gnome-characters 43.rc
- gnome-clocks 43.beta
- gnome-connections 43.0
- gnome-console 43.rc
- gnome-contacts 43.rc
- gnome-control-center 43.0
- gnome-desktop 43.rc
- gnome-disk-utility 43.0
- gnome-endeavour v42.0
- gnome-font-viewer 43.rc
- gnome-initial-setup 43.0
- gnome-logs 43.beta
- gnome-maps v43.rc
- gnome-online-accounts 3.46.0
- gnome-photos 43.beta
- gnome-podcasts master(2022-07-29)
- gnome-remote-desktop 43.0
- gnome-session 42.0
- gnome-settings-daemon 43.rc
- gnome-shell 43.rc
- gnome-shell-extensions 43.rc
- gnome-shell-extension-appindicator master(2022-08-24)+PR351
- gnome-software 43.rc
- gnome-sound-recorder 43.beta
- gnome-terminal 3.46.1
- gnome-text-editor 43.alpha1
- gnome-tour 43.beta
- gnome-weather 43.rc
- gobject-introspection 1.74.0
- grilo grilo-0.3.15
- grilo-plugins grilo-plugins-0.3.15
- gsettings-desktop-schemas 43.0
- gtksourceview5 5.6.0
- js102 102.2.0
- libadwaita 1.2.0
- libgweather-4 4.1.1
- libhandy 1.8.0
- libosinfo 1.10.0
- libnma 1.10.2
- libpanel 1.0alpha1
- librest 0.9.1
- libshumate 1.0.0.beta
- libsoup3 3.2.0
- malcontent 0.11.0
- mutter 43.rc
- nautilus 43.rc
- python-nautilus 4.0.alpha
- orca ORCA_43_BETA
- phodav 3.0
- sofia-sip 1.13.9
- spice-gtk 0.41
- sushi 43.0
- sysprof 3.46.0
- template-glib 3.36.0
- totem 43.0
- tracker3 3.4.0.rc
- tracker3-miners 3.4.0.rc
- vte3 0.70.0
- webkit2gtk-4.1 2.37.91
- xdg-desktop-portal-gnome 43.0

## Wontbuild
- gnome-builder 43.alpha1 (gnome-builder-libide-docs, check())

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
