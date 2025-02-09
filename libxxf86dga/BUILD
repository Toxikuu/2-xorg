NAME="libxxf86dga"
VERS="1.1.6"
DESC="X11 Direct Graphics Access extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/$NAME.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="xorgproto libxext libx11 util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXxf86dga-$VERS.tar.xz"
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
