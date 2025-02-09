NAME="libxvmc"
VERS="1.0.14"
DESC="X11 Video Motion Compensation extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxvmc.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libxv libx11 xorgproto glibc"

SOURCE="https://www.x.org/pub/individual/lib/libXvMC-$VERS.tar.xz"
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
