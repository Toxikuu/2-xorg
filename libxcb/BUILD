NAME="libxcb"
VERS="1.17.0"
DESC="X11 client-side library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcb.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep 'libxcb-[0-9]' | cut -d- -f2 | sort -V | tail -n1"

SOURCE="https://xorg.freedesktop.org/archive/individual/lib/libxcb-$VERS.tar.xz"
EXTRA=()

DEPS=("libxau xcb-proto libxdmcp")

2b() {

with xorg

cfg ${XORG_CONFIG[@]} --without-doxygen
mk
mi

mk distclean
m32=1

cfg ${XORG_CONFIG_32[@]} --without-doxygen
mk
mi

}