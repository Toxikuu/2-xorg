NAME="libxt"
VERS="1.3.1"
DESC="X11 toolkit intrinsics library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxt.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libsm libx11 libice glibc xorgproto util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXt-$VERS.tar.xz"
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
