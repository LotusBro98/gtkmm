# CMake files for native GTKMM 3 build with MS VC++ on Win32 platform

## Why

Native GTKMM builds for Win32 with MS VC++ lag behind those with gcc.

## How

* [Use OBS](http://mail.gnome.org/archives/gtk-list/2011-March/msg00111.html) (openSUSE Build Service) for all prerequisites
* You'll need perl to build gtk+ git submodule
* It is complicated to build MM counterpart from git on Win32 as they heavily use m4 macro processor
* <del>Download source code release for corresponding subfolders</del>

## Problems

* There may be glitches with path names
* Some stuff from OBS may be broken

## Notes

Windows XP doesn't have mklink tool.
ln tool from http://schinagl.priv.at/nt/ln/ln.html should be used as fsutil requires elevated privileges.
