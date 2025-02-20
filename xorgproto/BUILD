NAME="xorgproto"
VERS="2024.1"
DESC="Xorg protocol headers"
UPST="https://gitlab.freedesktop.org/xorg/proto/xorgproto.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://xorg.freedesktop.org/archive/individual/proto/xorgproto-$VERS.tar.xz"
EXTRA=()

DEPS="util-macros"

2b() {

with meson ninja

ms
nj
ni

mv -v "$D"/usr/share/doc/xorgproto{,-2024.1}

}
