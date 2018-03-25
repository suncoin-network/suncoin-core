
Debian
====================
This directory contains files used to package suncoind/suncoin-qt
for Debian-based Linux systems. If you compile suncoind/suncoin-qt yourself, there are some useful files here.

## suncoin: URI support ##


suncoin-qt.desktop  (Gnome / Open Desktop)
To install:

	sudo desktop-file-install suncoin-qt.desktop
	sudo update-desktop-database

If you build yourself, you will either need to modify the paths in
the .desktop file or copy or symlink your suncoin-qt binary to `/usr/bin`
and the `../../share/pixmaps/suncoin128.png` to `/usr/share/pixmaps`

suncoin-qt.protocol (KDE)

