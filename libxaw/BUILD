NAME="libxaw"
VERS="1.0.16"
DESC="X11 Athena Widget library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxaw.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxmu libxpm libx11 libxt libxext xorgproto glibc util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXaw-$VERS.tar.xz"
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
