These are the basic needed files and folders to build THINXOS system.

### buildiso

buildiso is used to build THINXOS ISO.

#### Arguments

~~~
$ ./buildiso.sh -h
Usage: buildiso [options]
    -c                 Disable clean work dir
    -h                 This help
    -p <profile>       Buildset or profile [default: kde]
    -v                 Verbose output to log file, show profile detail (-q)
~~~

* Uses the same signature that normal repo and has no mirrors package to install.

`sudo pacman -Syy`

## Install necessary packages
`sudo pacman -S archiso mkinitcpio-archiso git squashfs-tools --needed`

Clone:\
`git clone git@github.com:s0u7a/THIN-X-OS.git THINXOS-archiso`

`cd THINXOS-archiso`

## Build
`sudo ./buildiso.sh -p kde -v`

## The iso appears at out folder
