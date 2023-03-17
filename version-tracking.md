## Done
|  FCGU Builds  |
|:-------------:|

| Package                   |  Version / Tag  | Patches |
|---------------------------|:---------------:|:-------:|
| adwaita-icon-theme        | 44.beta         |    X    |
| at-spi2-core              | 2.47.90         |    X    |
| baobab                    | 44.rc           |    X    |
| callaudiod                | 0.1.6           |    X    |
| clapper                   | 0.5.2           |    X    |
| d-spy                     | 1.6.0           |    X    |
| eog                       | 44.beta         |    X    |
| epiphany                  | 2023-03-09 (master)|    Y    |
| evince                    | 44.rc           |    X    |
| evolution                 | 3.48.0          |    X    |
| evolution-data-server     | 3.48.0          |    X    |
| evolution-ews             | 3.48.0          |    X    |
| feedbackd                 | 0.1.0           |    X    |
| gcr-4                     | 4.1.0           |    X    |
| gdm                       | 44.rc-real      |    X    |
| gjs                       | 1.75.90         |    X    |
| glib2                     | Arch Linux      |    X    |
| glib-networking           | 2.76.0          |    X    |
| gnome-backgrounds         | 44.beta         |    X    |
| gnome-boxes               | 44.0            |    X    |
| gnome-builder             | 44.rc           |    X    |
| gnome-calculator          | 44.rc           |    X    |
| gnome-calendar            | 44.0            |    X    |
| gnome-calls               | v44_alpha.1     |    X    |
| gnome-characters          | 44.rc           |    X    |
| gnome-clocks              | 44.0            |    X    |
| gnome-connections         | 44.rc           |    X    |
| gnome-console             | 44.beta         |    X    |
| gnome-contacts            | 44.rc           |    X    |
| gnome-control-center      | 44.rc           |    X    |
| gnome-desktop             | 44.beta         |    X    |
| gnome-disks-utility       | 44.0            |    X    |
| gnome-font-viewer         | 44.rc           |    X    |
| gnome-initial-setup       | 44.rc           |    X    |
| gnome-maps                | v44.rc          |    X    |
| gnome-music               | 44.rc           |    X    |
| gnome-online-accounts     | 3.47.1          |    X    |
| gnome-podcasts            | 2022-12-16 (master)|    X    |
| gnome-remote-desktop      | 44.rc           |    X    |
| gnome-session             | 44.rc           |    X    |
| gnome-settings-daemon     | 44.rc           |    X    |
| gnome-shell               | 44.rc           |    X    |
| gnome-shell-extensions    | 44.rc           |    X    |
| gnome-software            | 44.0            |    X    |
| gnome-sound-recorder      | 43.beta         |    X    |
| gnome-system-monitor      | 44.rc           |    X    |
| gnome-terminal            | 3.47.99         |    X    |
| gnome-text-editor         | 44.rc           |    X    |
| gnome-user-docs           | 44.rc           |    X    |
| gnome-weather             | 44.rc           |    X    |
| gobject-introspection     | 1.76.0          |    X    |
| gsettings-desktop-schemas | 44.beta         |    X    |
| gtksourceview5            | 5.8.0           |    X    |
| jsonrpc-glib              | 3.43.0          |    X    |
| libadwaita                | 1.3.1           |    X    |
| libdex                    | 0.2.0           |    X    |
| libdmapsharing4           | LIBDMAPSHARING_3_9_11|    X    |
| libpanel                  | 1.2.0           |    X    |
| libpeas                   | 1.36.0          |    X    |
| librsvg                   | 2.55.91         |    X    |
| libsoup3                  | 3.4.0           |    X    |
| loupe                     | 2023-02-24      |    X    |
| mutter                    | 44.rc           |    Y    |
| nautilus                  | 44.0            |    X    |
| orca                      | ORCA_44_RC      |    X    |
| pygobject                 | 3.43.1          |    X    |
| sofia-sip                 | 1.13.14         |    X    |
| tracker                   | 3.5.0.rc        |    X    |
| tracker-miners            | 3.5.0.rc        |    X    |
| vte                       | 0.71.99         |    X    |
| webkitgtk-6.0             | 2.39.91         |    Y    |
| wpewebkit                 | 2.39.5          |    X    |
| xdg-desktop-portal-gnome  | 44.rc           |    X    |


|  Arch Linux Rebuilds  |
|:---------------------:|

| Package       |  Version  | Patches | Reason |
|---------------|:---------:|:-------:|--------|
| gnome-keyring | 42.1      |    X    | gcr-4  |
| grilo         | 0.3.15    |    X    | gnome-music(libsoup3) |
| grilo-plugins | 0.3.15    |    X    | libdmapsharing4 |
| libnma        | 1.10.6    |    X    | gcr-4  |



## Wontbuild

## Exclude
- none

# Versioning
## Git snapshots
* tag+r60+g3f9dba93c
  * `sed 's/[^-]*-g/r&/;s/-/+/g'`

## Dev releases
* X.beta.1 -> X.beta1
* X.1.beta -> X.1beta
* X.0.beta.1 -> X.0beta.1
  * `sed -r 's/\.([a-z])/\1/;s/([a-z])\./\1/;s/[^-]*-g/r&/;s/-/+/g'`

## Stable releases
* pkgver: 1 -> 0.1
* X -> X.0
  * `sed -r '/\.([0-9])/!s/$/\.0/;s/[^-]*-g/r&/;s/-/+/g'`