NAME="libevdev"
VERS="1.13.3"
DESC="Common functions for X input drivers"
CATG="drivers input"
UPST="https://gitlab.freedesktop.org/libevdev/libevdev.git"
DEPS=()

SOURCE="https://www.freedesktop.org/software/libevdev/libevdev-$VERS.tar.xz"
EXTRA=()

2b() {

with meson ninja

ms -D documentation=disabled -D tests=disabled
nj
ni

}
