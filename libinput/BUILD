NAME="libinput"
VERS="1.28.1"
DESC="Input device management and event handling library"
CATG="input"
UPST="https://gitlab.freedesktop.org/libinput/libinput.git"
DEPS=(
    "libevdev"
    "mtdev"
)

SOURCE="https://gitlab.freedesktop.org/libinput/libinput/-/archive/$VERS/libinput-$VERS.tar.gz"
EXTRA=()

2b() {

with meson ninja

ms -D debug-gui=false \
   -D tests=false     \
   -D libwacom=false  \
   -D udev-dir=/usr/lib/udev
nj
ni

}