GNOME Screenshot
================

GNOME Screenshot is a small utility that takes a screenshot of the whole
desktop; the currently focused window; or an area of the screen.

### Dependencies

 - GLib 2.36
 - GTK+ 3.12
 - X11

install them with:

```
sudo apt install meson ninja-build
sudo apt install libglib2.0-dev libx11-dev libxext-dev libgtk-3-dev

wget http://http.us.debian.org/debian/pool/main/libh/libhandy-1/gir1.2-handy-1_1.7.90-1_amd64.deb
wget http://http.us.debian.org/debian/pool/main/libh/libhandy-1/libhandy-1-dev_1.7.90-1_amd64.deb
wget http://http.us.debian.org/debian/pool/main/libh/libhandy-1/libhandy-1-0_1.7.90-1_amd64.deb
sudo apt install *.deb

meson setup builddir && cd builddir
meson compile
sudo mv src/gnome-screenshot /usr/local/bin
```
