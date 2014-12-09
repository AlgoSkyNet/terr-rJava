# rJava for TERR

This is a version of rJava modifed to run with
TIBCO Enterprise Runtime for R (TERR).

This repository contains the modified source rJava package. It also
contains binary Windows and Linux 64-bit versions of the package (under
`inst/binary`).

To install the Windows binary in TERR, run:

```
URL <-
    "https://raw.github.com/TIBCOSoftware/terr-rJava/master/inst/binary/rJava_0.9-6-0.zip"
pkgfile <- paste(tempdir(), basename(URL), sep="/")
download.file(URL, destfile=pkgfile)
install.packages(pkgfile, repos=NULL)
```

To install the Linux binary in TERR, run:

```
URL <-
    "https://raw.github.com/TIBCOSoftware/terr-rJava/master/inst/binary/rJava_0.9-6-0_R_x86_64-unknown-linux-gnu.tar.gz"
pkgfile <- paste(tempdir(), basename(URL), sep="/")
download.file(URL, destfile=pkgfile)
install.packages(pkgfile, repos=NULL, type="binary")
```
