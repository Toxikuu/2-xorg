NAME="libxkbfile"
VERS="1.1.3"
DESC="X11 keyboard file manipulation library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxkbfile.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libx11 xorgproto glibc util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libxkbfile-$VERS.tar.xz"
EXTRA=()

2b() {

. e-xorg

b-cfg $XORG_CONFIG
b-make
b-mi

b-32cfg $XORG_CONFIG_32
b-make
b-32mi

}
