NAME="libxfixes"
VERS="6.0.1"
DESC="X11 miscellaneous 'fixes' extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxfixes.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libx11 xorgproto glibc util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXfixes-$VERS.tar.xz"
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
