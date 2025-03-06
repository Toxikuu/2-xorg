NAME="libx11"
VERS="1.8.11"
DESC="X11 client-side library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libx11.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxcb glibc xorgproto util-macros xtrans"

SOURCE="https://www.x.org/pub/individual/lib/libX11-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]} --disable-xf86bigfont
mk
mi

m32=1
mk distclean

cfg ${XORG_CONFIG_32[@]} --disable-xf86bigfont
mk
mi

}
