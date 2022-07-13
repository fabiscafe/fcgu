# Packages
## Done
- none

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
