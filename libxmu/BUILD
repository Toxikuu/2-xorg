NAME="libxmu"
VERS="1.2.1"
DESC="X11 miscellaneous micro-utility library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxmu.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libxt libx11 xorgproto glibc util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXmu-$VERS.tar.xz"
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
