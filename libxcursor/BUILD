NAME="libxcursor"
VERS="1.2.3"
DESC="X cursor management library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcursor.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxfixes libxrender libx11 glibc xorgproto util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXcursor-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

m32=1
mk distclean

cfg ${XORG_CONFIG_32[@]}
mk
mi

}
