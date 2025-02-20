NAME="libxshmfence"
VERS="1.3.3"
DESC="X11 library exposing an event API atop Linux futexes"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxshmfence.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/lib/libxshmfence-$VERS.tar.xz"
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
