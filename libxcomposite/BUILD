NAME="libxcomposite"
VERS="0.4.6"
DESC="X11 Composite extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcomposite.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxfixes xorgproto libx11 glibc util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXcomposite-$VERS.tar.xz"
EXTRA=()

2b() {

. e-xorg

b-cfg $XORG_CONFIG
b-make
b-mi

b-32cfg $XORG_CONFIG_32
b-make
b-32mi

}
