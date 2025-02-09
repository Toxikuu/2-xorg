NAME="libice"
VERS="1.1.2"
DESC="X11 Inter-Client Exchange library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libice.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="glibc xorgproto xtrans util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libICE-$VERS.tar.xz"
EXTRA=()

2b() {

. e-xorg

b-cfg $XORG_CONFIG
b-make
b-mi

b-32cfg $XORG_CONFIG
b-make
b-mi

}
