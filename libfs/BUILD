NAME="libfs"
VERS="1.0.10"
DESC="X Font Service client library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libfs.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="glibc xorgproto xtrans"

SOURCE="https://www.x.org/pub/individual/lib/libFS-$VERS.tar.xz"
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
