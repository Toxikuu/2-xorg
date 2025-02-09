NAME="libxfont2"
VERS="2.0.7"
DESC="X11 font rasterisation library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxfont.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="freetype2 libfontenc xorgproto glibc xtrans util-macros"

SOURCE="https://www.x.org/pub/individual/lib/libXfont2-$VERS.tar.xz"
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
