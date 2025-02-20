NAME="libxft"
VERS="2.3.8"
DESC="FreeType-based font drawing library for X"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxft.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="fontconfig libxrender libx11 freetype2 glibc xorgproto"

SOURCE="https://www.x.org/pub/individual/lib/libXft-$VERS.tar.xz"
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