NAME="libxrender"
VERS="0.9.12"
DESC="X Rendering Extension client library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxrender.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libx11 glibc xorgproto"

SOURCE="https://www.x.org/pub/individual/lib/libXrender-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

m32=1

cfg ${XORG_CONFIG_32[@]}
mk
mi

}