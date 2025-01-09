NCSA Mosaic
===========

![Wikipedia viewed with Mosaic](https://github.com/downloads/yotann/ncsa-mosaic/wikipedia-screenshot.png "Wikipedia viewed with Mosaic")

This is [NCSA Mosaic](https://en.wikipedia.org/wiki/Mosaic_(web_browser)), one
of the first graphical web browsers. This version has barely been modified
since the last official release, version 2.7 beta 6, in 1996. You may also be
interested in [Mosaic-CK](http://www.floodgap.com/retrotech/machten/mosaic/)
and [VMS Mosaic](https://web.archive.org/web/20070911192043/http://www.openvms.org/stories.php?story=07%2F09%2F03%2F1740114), which have
been substantially improved from the original.

If you're on Linux, your time machine is fueled up and ready to go! Follow the
instructions below to build and run.

Many thanks to [Sean MacLennan and Alan Wylie](https://web.archive.org/web/20120915154245/seanm.ca/mosaic/) for
doing the heavy lifting. And, of course, hats off to Marc Andreessen, Eric
Bina, and the rest of the [NCSA](http://www.ncsa.illinois.edu/) team for
kicking things off for us. Thanks!

[Alan Dipert](https://github.com/alandipert) took the last release of Mosaic, put it
on Github, and made some fixes. [Tim Pizey](http://pizey.net/~timp/) modified
it so that in-document javascript is not displayed.

Building
--------

On Gentoo:

* First, install these packages:

```
emerge -av x11-libs/libX11 x11-libs/libXrender x11-libs/libXft \
            x11-libs/libxkbfile x11-libs/motif media-libs/libjpeg-turbo \
            media-libs/libpng x11-libs/libXmu x11-libs/libXpm media-gfx/sxiv \
            x11-base/xorg-proto dev-build/meson dev-build/ninja
```

* Next, build with:

```
meson build
ninja -C build
```

* Run!

```
build/src/Mosaic
```
