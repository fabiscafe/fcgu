## Done
|  FCGU Builds  |
|:-------------:|

| Package                   |  Version / Tag  | Patches |
|---------------------------|:---------------:|:-------:|
| adwaita-icon-theme        | 44.0            |    X    |
| at-spi2-core              | Arch Linux      |    X    |
| baobab                    | 44.0            |    X    |
| callaudiod                | 0.1.6           |    X    |
| clapper                   | 0.5.2           |    X    |
| d-spy                     | Arch Linux      |    X    |
| eog                       | 44.0            |    X    |
| epiphany                  | 44.0            |    X    |
| evince                    | 44.0            |    X    |
| evolution                 | 3.48.0          |    X    |
| evolution-data-server     | 3.48.0          |    X    |
| evolution-ews             | 3.48.0          |    X    |
| feedbackd                 | 0.1.0           |    X    |
| gcr-4                     | 4.1.0           |    X    |
| gdm                       | 44.0            |    X    |
| gjs                       | 1.76.0          |    X    |
| glib2                     | Arch Linux      |    X    |
| glib-networking           | Arch Linux      |    X    |
| gnome-backgrounds         | 44.0            |    X    |
| gnome-boxes               | 44.0            |    X    |
| gnome-builder             | 44.1            |    X    |
| gnome-calculator          | 44.0            |    X    |
| gnome-calendar            | 44.0            |    X    |
| gnome-calls               | v44.0           |    X    |
| gnome-characters          | 44.0            |    X    |
| gnome-clocks              | 44.0            |    X    |
| gnome-connections         | 44.0            |    X    |
| gnome-console             | 44.0            |    X    |
| gnome-contacts            | 44.0            |    X    |
| gnome-control-center      | 44.0            |    X    |
| gnome-desktop             | 44.0            |    X    |
| gnome-disks-utility       | Arch Linux      |    X    |
| gnome-font-viewer         | 44.0            |    X    |
| gnome-initial-setup       | 44.0            |    X    |
| gnome-maps                | v44.0           |    X    |
| gnome-music               | 44.rc           |    X    |
| gnome-online-accounts     | 3.48.0          |    X    |
| gnome-podcasts            | 2023-02-27 (master)|    X    |
| gnome-remote-desktop      | 44.0            |    X    |
| gnome-session             | 44.0            |    X    |
| gnome-settings-daemon     | 44.0            |    X    |
| gnome-shell               | 44.0            |    Y    |
| gnome-shell-extensions    | 44.0            |    X    |
| gnome-software            | 44.0            |    X    |
| gnome-sound-recorder      | 43.beta         |    X    |
| gnome-system-monitor      | 44.0            |    X    |
| gnome-terminal            | 3.48.0          |    X    |
| gnome-text-editor         | 44.0            |    X    |
| gnome-tour                | 44.0            |    X    |
| gnome-user-docs           | 44.0            |    X    |
| gnome-weather             | 44.0            |    X    |
| gobject-introspection     | Arch Linux      |    X    |
| gsettings-desktop-schemas | 44.0            |    X    |
| gtksourceview5            | Arch Linux      |    X    |
| jsonrpc-glib              | 3.44.0          |    X    |
| libadwaita                | 1.3.1           |    X    |
| libdex                    | 0.2.0           |    X    |
| libdmapsharing4           | LIBDMAPSHARING_3_9_11|    X    |
| libpanel                  | 1.2.0           |    X    |
| libpeas                   | 1.36.0          |    X    |
| librsvg                   | Arch Linux      |    X    |
| libsoup3                  | Arch Linux      |    X    |
| loupe                     | 2023-03-18(main)|    X    |
| mutter                    | 44.0            |    X    |
| nautilus                  | 44.0            |    X    |
| orca                      | ORCA_44_RC      |    X    |
| pygobject                 | 3.44.0          |    X    |
| sofia-sip                 | 1.13.14         |    X    |
| simple-scan               | 44.0            |    X    |
| sysprof                   | Arch Linux      |    X    |
| tracker                   | 3.5.0           |    X    |
| tracker-miners            | 3.5.0           |    X    |
| vte                       | Arch Linux      |    X    |
| webkitgtk-6.0             | 2.40.0          |    x    |
| wpewebkit                 | 2.39.5          |    X    |
| xdg-desktop-portal-gnome  | 44.0            |    X    |


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