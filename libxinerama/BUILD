NAME="libxinerama"
VERS="1.1.5"
DESC="X11 Xinerama extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxinerama.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libx11 glibc xorgproto util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXinerama-$VERS.tar.xz"
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
