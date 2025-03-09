NAME="libsm"
VERS="1.2.6"
DESC="X11 Session Management library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libsm.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libice util-linux xorgproto glibc"

SOURCE="https://www.x.org/pub/individual/lib/libSM-$VERS.tar.xz"
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