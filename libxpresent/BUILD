NAME="libxpresent"
VERS="1.0.1"
DESC="X Present Extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxpresent.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/lib/libXpresent-$VERS.tar.xz"
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
