NAME="libxcb"
VERS="1.17.0"
DESC="X11 client-side library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcb.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep 'libxcb-[0-9]' | cut -d- -f2 | sort -V"

SOURCE="https://xorg.freedesktop.org/archive/individual/lib/libxcb-$VERS.tar.xz"
EXTRA=()

DEPS=("libxau xcb-proto libxdmcp")

2b() {

b-cfg $XORG_CONFIG --without-doxygen
b-make
b-mi

b-make distclean

b-32cfg $XORG_CONFIG --without-doxygen
b-make
b-32mi

}
