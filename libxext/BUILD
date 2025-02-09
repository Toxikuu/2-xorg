NAME="libxext"
VERS="1.3.6"
DESC="X11 miscellaneous extensions library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxext.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

DEPS="libx11 glibc xorgproto util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXext-$VERS.tar.xz"
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
