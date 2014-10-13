# rJava for TERR

This is a version of rJava modifed to run with
TIBCO Enterprise Runtime for R (TERR).

This repository contains the modified source rJava package.
It also contains a Windows binary of the package
(under `inst/binary`).
To install the Windows binary in TERR, run:

> pkgfile <- tempfile("rJava")    
> download.file(destfile=pkgfile,    
>   "https://raw.github.com/TIBCOSoftware/terr-rJava/master/inst/binary/rJava_0.9-6-0.zip")  
> install.packages(pkgfile, repos=NULL)  
