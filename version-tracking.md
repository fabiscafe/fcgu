# Naming
## Git snapshots
* tag+r60+g3f9dba93c
  * `s/[^-]*-g/r&/;s/-/+/g;`
## Dev releases
* X.beta -> X.beta.0
  * `s/beta/beta.0/`
* X.beta1 -> X.beta.1
  * `s/beta\([0-9]\+\)/beta.\1/`
## Stable releases
pkgver: 1 -> 0.1

# Done
- adwaita-icon-theme master(2022-03-02)
- at-spi2-core AT_SPI2_CORE_2_44_0
- baobab 42.rc
- callaudiod 0.1.3
- clapper 0.4.1
- eog 42.rc
- epiphany 42.0
- evince 42.0
- evolution 3.44.0
- evolution-data-server 3.44.0
- feedbackd 0.0.0+git20220208
- gjs 1.71.90
- glib2 2.72.0
- glib-networking 2.72.beta
- gnome-backgrounds 42.beta
- gnome-bluetooth 42.rc
- gnome-boxes 42.0.1
- gnome-builder 42.rc1
- gnome-calculator 42.rc
- gnome-calendar 42.rc
- gnome-calls 42.rc.1
- gnome-characters 42.rc
- gnome-clocks master(2022-03-02)
- gnome-connections master(2022-03-02)
- gnome-console main(2022-03-02)
- gnome-contacts 42.beta
- gnome-control-center 42.rc
- gnome-desktop 42.rc
- gnome-disk-utility 42.rc
- gnome-font-viewer 42.rc
- gnome-initial-setup 42.0
- gnome-maps v42.rc
- gnome-music master(2022-03-08)
- gnome-podcasts-gtk4 (msandova/podcasts) gtk4(2022-02-07)
- gnome-remote-desktop 42.rc
- gnome-settings-daemon 42.rc
- gnome-shell 42.0
- gnome-shell-extensions 42.0
- gnome-secrets 6.2 (gnome-passwordsafe)
- gnome-software 42.0
- gnome-sound-recorder 42.beta
- gnome-system-monitor 42.rc
- gnome-terminal 3.43.90
- gnome-text-editor 42.rc1
- gnome-tweaks 42.beta
- gnome-weather 42.rc
- gobject-introspection 1.72.0
- gsettings-desktop-schemas 42.rc
- gtk4 4.6.1
- gtksourceview5 master(2022-03-02)
- gvfs 1.50.0
- jsonrpc-glib 3.41.0
- libadwaita 1.1.0
- libgnome-games-support-gtk4 2.0.0
- libgweather 4.0.0
- libhandy 1.6.1
- libnma 1.8.34
- libsoup3 3.0.5
- mutter 42.0
- nautilus 42.rc
- newsflash 1.5.1
- orca ORCA_42_RC
- sofia-sip 1.13.7
- sysprof 3.43.90
- tracker3 3.3.0.rc
- tracker3-miners 3.3.0.rc
- vala 0.56.0
- vte3 0.67.90
- xdg-desktop-portal-gnome 42.0.1
- yelp 42.beta
- yelp-tools 42.beta
- yelp-xsl 42.beta

# Wontbuild

# Exclude