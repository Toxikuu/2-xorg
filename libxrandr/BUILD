NAME="libxrandr"
VERS="1.5.4"
DESC="X11 RandR extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxrandr.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libxrender libx11 glibc util-macros xorgproto"

SOURCE="https://www.x.org/pub/individual/lib/libXrandr-$VERS.tar.xz"
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
