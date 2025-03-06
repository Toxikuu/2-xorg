NAME="libxcomposite"
VERS="0.4.6"
DESC="X11 Composite extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcomposite.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxfixes xorgproto libx11 glibc util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXcomposite-$VERS.tar.xz"
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
