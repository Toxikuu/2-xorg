NAME="libxdmcp"
VERS="1.1.5"
DESC="The X Display Manager Control Protocol"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxdmcp.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep libXdmcp-[0-9] | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/lib/libXdmcp-$VERS.tar.xz"
EXTRA=()

DEPS=("xorgproto")

2b() {

. e-xorg

b-cfg $XORG_CONFIG
b-make
b-mi

b-make distclean

b-32cfg $XORG_CONFIG
b-make
b-32mi

}
