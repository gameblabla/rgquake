SDLquake 1.0.9 (approximately)
==============================

This is SDLquake, a port of id Software's Quake engine to the Simple Direct-media Layer 1.2 for Linux.  The Autotools build system has been updated to 2015 standards more or less.

Installation
------------

Run `autogen.sh` to generate the `configure` file. Then execute `./configure && make` to build the `sdlquake` executable. Run the `sdlquake` executable from within a directory containing the original Quake data files.

The Quake data files are expected to be named in lower case! This is true if you installed from Linux Quake installation media, but not necessarily true if you copied the data files over from Windows or performed the installation inside of DOSBox. If `sdlquake` fails to start and complains about missing files, be sure the `id1` directory and the `.pak` files within it are renamed to lower case.

See `INSTALL` for detailed build instructions. Support for building on 64-bit multiarch systems has been added and may need explanation.

See `README.SDL` for the original porter's comments.

Notes
-----

Currently plays demos at startup, but crashes when starting a new game on my x86-64 Linux system. Presumed to be some lingering 64-bit cleanness or uninitialized data issue. Investigating.

License
-------

SDLquake is licensed under the GPLv2.  You should have received a copy of the GPLv2 in a file called COPYING in the same directory as this README.  If you did not, contact the distributor from whom you recieved this software for a copy.
