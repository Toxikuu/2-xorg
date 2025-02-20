NAME="libxau"
VERS="1.0.12"
DESC="The X Authorization Protocol"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxau.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -E '^libXau-[0-9]+\.' | cut -d- -f2 | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/lib/libXau-$VERS.tar.xz"
EXTRA=()

DEPS="xorgproto"

2b() {

cfg ${XORG_CONFIG[@]}
mk
mi

mk distclean
m32=1

cfg ${XORG_CONFIG_32[@]}
mk
mi

}