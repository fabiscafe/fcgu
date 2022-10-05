## Done
- adwaita-icon-theme 43
- baobab 43.0
- callaudiod 0.1.4
- cheese 43.alpha
- clapper 0.5.2
- dconf-editor 43.0
- d-spy 1.4.0
- eog 43.0
- epiphany 43.0
- evince 43.0
- evolution 3.46.0
- evolution-data-server 3.46.0
- feedbackd 0.0.0+git20220520
- file-roller 43.0
- folks 0.15.5
- gcr-4 3.92.0
- gdm 43.0
- geary 43.0
- gedit 43.alpha
- geocode-glib-2 3.26.4
- gjs 1.74.0
- gnome-backgrounds 43
- gnome-boxes 43.0
- gnome-builder 43.2¹
- gnome-calculator 43.0.1
- gnome-calendar 43.0
- gnome-calls v43.0
- gnome-characters 43.0
- gnome-clocks 43.0
- gnome-connections 43.0
- gnome-console 43.0
- gnome-contacts 43.0
- gnome-control-center 43.0
- gnome-desktop 43
- gnome-disk-utility 43.0
- gnome-endeavour v42.0
- gnome-font-viewer 43.0
- gnome-initial-setup 43.0
- gnome-logs gnome-logs-43.0
- gnome-maps v43.0
- gnome-online-accounts 3.46.0
- gnome-photos 43.0
- gnome-podcasts master(2022-07-29)
- gnome-power-manager GNOME_POWER_MANAGER_43_0
- gnome-remote-desktop 43.0
- gnome-session 43.0
- gnome-settings-daemon 43.0
- gnome-shell 43.0
- gnome-shell-extensions 43.0
- gnome-software 43.rc
- gnome-sound-recorder 43.beta
- gnome-terminal 3.46.2
- gnome-text-editor 43.1
- gnome-tour 43.0
- gnome-user-docs 43.0
- gnome-weather 43.0
- grilo grilo-0.3.15
- grilo-plugins grilo-plugins-0.3.15
- gsettings-desktop-schemas 43.0
- gtranslator 42.0
- js102 102.3.0
- libgda6 master(2022-03-13)
- libgweather-4 4.2.0
- libosinfo 1.10.0
- libnma 1.10.2
- libpanel 1.0.1
- libpeas libpeas-1.34.0
- librest 0.9.1
- libshumate 1.0.1
- malcontent 0.11.0
- mutter 43.0
- nautilus 43.0
- python-nautilus 4.0
- newsflash v.2.1.2
- orca ORCA_43_0
- phodav 3.0
- sofia-sip 1.13.9
- spice-gtk 0.41
- sushi 43.0
- sysprof 3.46.0
- template-glib 3.36.0
- totem 43.0
- tracker3 3.4.0
- tracker3-miners 3.4.0
- vte3 0.70.0
- xdg-desktop-portal-gnome 43.0

## Wontbuild
- gnome-builder 43.2 (gnome-builder-libide-docs)
  - https://gitlab.gnome.org/GNOME/gnome-builder/-/issues/1793

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