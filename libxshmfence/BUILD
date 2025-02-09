NAME="libxshmfence"
VERS="1.3.3"
DESC="X11 library exposing an event API atop Linux futexes"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxshmfence.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/lib/libxshmfence-$VERS.tar.xz"
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
