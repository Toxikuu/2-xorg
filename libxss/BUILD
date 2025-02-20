NAME="libxss"
VERS="1.2.4"
DESC="X11 Screen Saver extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxscrnsaver.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i libxscrnsaver- | sed 's@_@.@g' | sort -V | tail -n1 | cut -d- -f2"
DEPS="libxext libx11 glibc xorgproto"

SOURCE="https://www.x.org/pub/individual/lib/libXScrnSaver-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

m32=1

cfg ${XORG_CONFIG_32[@]}
mk
mi

}