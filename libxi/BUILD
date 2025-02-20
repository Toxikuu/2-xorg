NAME="libxi"
VERS="1.8.2"
DESC="X11 Input extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxi.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libxfixes libx11 glibc xorgproto util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXi-$VERS.tar.xz"
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