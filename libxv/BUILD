NAME="libxv"
VERS="1.0.13"
DESC="X11 Video extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxv.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libx11 glibc xorgproto"

SOURCE="https://www.x.org/pub/individual/lib/libXv-$VERS.tar.xz"
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
