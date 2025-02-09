NAME="libxtst"
VERS="1.2.5"
DESC="library for XTEST & RECORD extensions"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxtst.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libxi libx11 glibc xorgproto util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXtst-$VERS.tar.xz"
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
