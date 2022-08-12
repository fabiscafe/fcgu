## Done
- adwaita-icon-theme 43.beta.1
- at-spi2-core 2.45.90
- baobab 43.beta
- callaudiod 0.1.4
- cheese 43.alpha
- clapper 0.5.2
- dconf-editor 43.beta
- d-spy 1.2.1
- eog 43.beta
- epiphany 43.beta
- evince 43.alpha
- evolution 3.45.2
- evolution-data-server 3.45.2
- feedbackd 0.0.0+git20220520
- folks 0.15.5
- gcr-4 3.90.0
- geary main(2022-07-13)
- gedit 43.alpha
- geocode-glib-2 3.26.3
- gjs 1.73.2
- glib2 2.73.3
- glib-networking 2.74.alpha
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
- gnome-maps 43.alpha
- gnome-online-accounts 3.45.2
- gnome-photos 43.beta
- gnome-podcasts-gtk4 master(2022-07-29)
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
- gtk4 4.7.1
- gtksourceview5 5.5.1
- js102 102.1.0
- libadwaita 1.2.beta
- libgit2-glib 1.1.0
- libgweather-4 4.1.0
- libhandy 1.7.90
- libosinfo 1.10.0
- libpanel 1.0alpha1
- librest 0.9.1
- libsoup3 3.1.1
- mutter 43.beta
- nautilus 43.beta.1
- orca ORCA_43_ALPHA
- phodav 3.0
- sofia-sip 1.13.8
- spice-gtk 0.41
- sysprof 3.45.1
- template-glib 3.35.0
- totem 43.alpha
- tracker3 3.4.0.beta
- tracker3-miners 3.4.0.beta
- vte3 0.69.92
- webkit2gtk-4.1 2.37.1
- xdg-desktop-portal-gnome 43.alpha


## Wontbuild
- gnome-builder 43.alpha1 (gnome-builder-libide-docs, check())
- gnome-initial-setup 43.beta (Waiting for malcontent 0.11 release)


## Exclude
- gjs 1.73.2 Unable to build "js102" with js/ProfilingCategoryList.h, would be happy about a MR
```
FAILED: libgjs-jsapi.a.p/gjs_pch.hh.gch
c++ -Ilibgjs-jsapi.a.p -I. -I../gjs -I/usr/include/glib-2.0 -I/usr/lib/glib-2.0/include -I/usr/include/sysprof-4 -I/usr/include/libmount -I/usr/include/blkid -I/usr/include/gobject-introspection-1.0 -I/usr/include/cairo -I/usr/include/lzo -I/usr/include/libpng16 -I/usr/include/freetype2 -I/usr/include/harfbuzz -I/usr/include/pixman-1 -flto=auto -fdiagnostics-color=always -D_FILE_OFFSET_BITS=64 -Wall -Winvalid-pch -Wnon-virtual-dtor -Wextra -std=c++17 -fno-rtti -O0 -fno-strict-aliasing -Wno-variadic-macros -Wno-missing-field-initializers -fno-semantic-interposition -march=x86-64 -mtune=generic -O3 -pipe -fno-plt -fexceptions -Wp,-D_FORTIFY_SOURCE=2 -Wformat -Werror=format-security -fstack-clash-protection -fcf-protection -Wp,-D_GLIBCXX_ASSERTIONS -g -ffile-prefix-map=/build/gjs/src=/usr/src/debug -fno-semantic-interposition -fPIC -isystem/usr/include/sysprof-4 -pthread -isystem /usr/include/mozjs-102 -DGJS_COMPILATION '-DGJS_JS_DIR="/usr/share/gjs-1.0"' '-DPKGLIBDIR="/usr/lib/gjs"' '-DG_LOG_DOMAIN="Gjs"' -MD -MQ libgjs-jsapi.a.p/gjs_pch.hh.gch -MF libgjs-jsapi.a.p/gjs_pch.hh.gch.d -o libgjs-jsapi.a.p/gjs_pch.hh.gch -c ../gjs/gjs/gjs_pch.hh
In file included from /usr/include/mozjs-102/js/ProfilingStack.h:16,
                 from /usr/include/mozjs-102/js/RootingAPI.h:27,
                 from /usr/include/mozjs-102/js/Id.h:35,
                 from ../gjs/gjs/jsapi-util.h:28,
                 from ../gjs/gjs/gjs_pch.hh:41:
/usr/include/mozjs-102/js/ProfilingCategory.h:13:10: fatal error: js/ProfilingCategoryList.h: No such file or directory
   13 | #include "js/ProfilingCategoryList.h"  // MOZ_PROFILING_CATEGORY_LIST
      |          ^~~~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
```

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
