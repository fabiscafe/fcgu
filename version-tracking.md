# Packages
## Done
- at-spi2-core 2.45.1
- baobab 43.alpha
- callaudiod 0.1.4
- clapper 0.5.2
- dconf-editor 43.alpha
- d-spy 1.2.1
- eog 43.alpha
- epiphany 43.alpha
- evolution 3.45.1
- evolution-data-server 3.45.1
- feedbackd 0.0.0+git20220520
- folks 0.15.5
- gcr-4 3.90.0
- geary main(2022-07-13)
- gedit 43.alpha
- geocode-glib-2 3.26.3
- gjs 1.73.1
- glib2 2.73.2
- glib-networking 2.74.alpha
- gnome-calculator 43.alpha
- gnome-calendar 43.alpha
- gnome-calls 43.alpha2
- gnome-characters 43.alpha
- gnome-console 42.2
- gnome-control-center 43.alpha
- gnome-desktop 43.alpha
- gnome-font-viewer 43.alpha
- gnome-initial-setup 43.alpha1
- gnome-maps 43.alpha
- gnome-online-accounts 3.45.1
- gnome-podcasts-gtk4 master(2022-05-25) +mr199
- gnome-remote-desktop 43.alpha
- gnome-session 42.0
- gnome-settings-daemon 43.alpha
- gnome-shell 43.alpha
- gnome-shell-extensions 43.alpha
- gnome-software 43.alpha
- gnome-text-editor 43.alpha0
- gnome-weather 43.alpha
- gobject-introspection 1.73.0
- gsettings-desktop-schemas 43.alpha
- gtk4 4.7.1
- gtksourceview5 5.5.0
- libadwaita 1.2.alpha
- libgweather-4 4.1.0
- libhandy 1.7.0
- libpanel 1.0alpha
- librest 0.9.1
- mutter 43.alpha
- nautilus 43.alpha
- orca ORCA_43_ALPHA
- sofia-sip 1.13.8
- sysprof 3.45.0
- template-glib 3.35.0
- tracker3 3.4.0.alpha
- tracker3-miners 3.4.0.alpha
- vte3 0.69.90
- xdg-desktop-portal-gnome 43.alpha


## Wontbuild
- gnome-builder

```
FAILED: src/plugins/git/daemon/gnome-builder-git.p/ipc-git-repository-impl.c.o 
cc -Isrc/plugins/git/daemon/gnome-builder-git.p -Isrc/plugins/git/daemon -I../gnome-builder/src/plugins/git/daemon -I/usr/include/gio-unix-2.0 -I/usr/include/glib-2.0 -I/usr/lib/glib-2.0/include -I/usr/include/sysprof-4 -I/usr/include/libmount -I/usr/include/blkid -I/usr/include/libgit2-glib-1.0 -I/build/gnome-builder/src/build -flto=auto -fdiagnostics-color=always -D_FILE_OFFSET_BITS=64 -Wall -Winvalid-pch -Wextra -std=gnu11 -O0 -DGLIB_VERSION_MIN_REQUIRED=GLIB_VERSION_2_72 -DGLIB_VERSION_MAX_ALLOWED=GLIB_VERSION_2_72 -DGDK_VERSION_MIN_REQUIRED=GDK_VERSION_4_8 -DGDK_VERSION_MAX_ALLOWED=GDK_VERSION_4_8 -DGTK_SOURCE_VERSION_MIN_REQUIRED=GTK_SOURCE_VERSION_5_6 -DGTK_SOURCE_VERSION_MAX_ALLOWED=GTK_SOURCE_VERSION_5_6 -Wcast-align -Wdeclaration-after-statement -Werror=address -Werror=array-bounds -Werror=empty-body -Werror=implicit -Werror=implicit-function-declaration -Werror=incompatible-pointer-types -Werror=init-self -Werror=int-conversion -Werror=int-to-pointer-cast -Werror=main -Werror=misleading-indentation -Werror=missing-braces -Werror=missing-include-dirs -Werror=nonnull -Werror=overflow -Werror=pointer-arith -Werror=pointer-to-int-cast -Werror=redundant-decls -Werror=return-type -Werror=sequence-point -Werror=shadow -Werror=trigraphs -Werror=undef -Werror=write-strings -Wformat-nonliteral -Werror=format-security -Werror=format=2 -Wignored-qualifiers -Wimplicit-function-declaration -Wlogical-op -Wmissing-format-attribute -Wmissing-include-dirs -Wmissing-noreturn -Wnested-externs -Wno-cast-function-type -Wno-dangling-pointer -Wno-missing-field-initializers -Wno-sign-compare -Wno-unused-parameter -Wold-style-definition -Wpointer-arith -Wredundant-decls -Wstrict-prototypes -Wswitch-default -Wswitch-enum -Wundef -Wuninitialized -Wunused -fno-strict-aliasing -DHAVE_CONFIG_H -D_GNU_SOURCE -DIDE_COMPILATION -DG_DISABLE_CAST_CHECKS -march=x86-64 -mtune=generic -O2 -pipe -fno-plt -fexceptions -Wp,-D_FORTIFY_SOURCE=2 -Wformat -Werror=format-security -fstack-clash-protection -fcf-protection -g -ffile-prefix-map=/build/gnome-builder/src=/usr/src/debug -fPIE -DGIT_SSH=1 -pthread -MD -MQ src/plugins/git/daemon/gnome-builder-git.p/ipc-git-repository-impl.c.o -MF src/plugins/git/daemon/gnome-builder-git.p/ipc-git-repository-impl.c.o.d -o src/plugins/git/daemon/gnome-builder-git.p/ipc-git-repository-impl.c.o -c ../gnome-builder/src/plugins/git/daemon/ipc-git-repository-impl.c
../gnome-builder/src/plugins/git/daemon/ipc-git-repository-impl.c: In function ‘translate_status’:
../gnome-builder/src/plugins/git/daemon/ipc-git-repository-impl.c:135:10: error: ‘GGIT_STATUS_CONFLICTED’ undeclared (first use in this function); did you mean ‘GIT_STATUS_CONFLICTED’?
  135 |     case GGIT_STATUS_CONFLICTED:
      |          ^~~~~~~~~~~~~~~~~~~~~~
      |          GIT_STATUS_CONFLICTED
../gnome-builder/src/plugins/git/daemon/ipc-git-repository-impl.c:135:10: note: each undeclared identifier is reported only once for each function it appears in
../gnome-builder/src/plugins/git/daemon/ipc-git-repository-impl.c:144:10: error: ‘GGIT_STATUS_WORKING_TREE_RENAMED’ undeclared (first use in this function); did you mean ‘GGIT_STATUS_WORKING_TREE_DELETED’?
  144 |     case GGIT_STATUS_WORKING_TREE_RENAMED:
      |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
      |          GGIT_STATUS_WORKING_TREE_DELETED
../gnome-builder/src/plugins/git/daemon/ipc-git-repository-impl.c:145:10: error: ‘GGIT_STATUS_WORKING_TREE_UNREADABLE’ undeclared (first use in this function); did you mean ‘GGIT_STATUS_WORKING_TREE_TYPECHANGE’?
  145 |     case GGIT_STATUS_WORKING_TREE_UNREADABLE:
      |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
      |          GGIT_STATUS_WORKING_TREE_TYPECHANGE
```
- gnome-clocks

```
error: Package 'geocode-glib-2.0' not found in specified Vala API directories or GObject-Introspection GIR directories
```


## Exclude
- gnome-boxes: mixed, conflicting dependency on libsoup2 and libsoup3

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
