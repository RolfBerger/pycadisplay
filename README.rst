---- under construction ----


pycadisplay - local display for pyCA
===================================

pycadisplay is a small program written in c to display recording status with 
previews and upcoming events from pyca database. The size and positions of the elemets
are designed for the 800x480 7" raspberry-pi display, the configuration is 
read from an ini-file. The display is updated every second, pyca-database
and ini-file are read if the file-timestamps changes.
To be fast and small the display is configured with linux drm/kms/egl, the text is a 
hardcoded bitmap and all graphics are direct opengl without any highlevel library.

required libraries for raspberry-pi4 and ubuntu11 are:
libdrm-dev
libgbm-dev
libgles2-mesa-dev
libsqlite3-dev
opengl ??
libiniparser-dev
...

build with:
