NAME="libevdev"
VERS="1.13.3"
DESC="Common functions for X input drivers"
CATG="drivers input"
UPST="https://gitlab.freedesktop.org/libevdev/libevdev.git"
VCMD="git ls-remote --tags --refs $UPST | sed 's@.*/@@' | grep $NAME-[0-9]\. | sort -V | tail -n1"
DEPS=()

SOURCE="https://www.freedesktop.org/software/libevdev/libevdev-$VERS.tar.xz"
EXTRA=()

2b() {

with meson ninja

ms -D documentation=disabled -D tests=disabled
nj
ni

}
