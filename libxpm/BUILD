NAME="libxpm"
VERS="3.5.17"
DESC="X11 pixmap library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxpm.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxt libxext libx11 glibc util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXpm-$VERS.tar.xz"
EXTRA=()

2b() {

. e-xorg

b-cfg $XORG_CONFIG --disable-open-zfile
b-make
b-mi

b-32cfg $XORG_CONFIG_32 --disable-open-zfile
b-make
b-32mi

}
