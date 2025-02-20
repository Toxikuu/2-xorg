NAME="util-macros"
VERS="1.20.2"
DESC="m4 macros used by Xorg"
UPST="https://gitlab.freedesktop.org/xorg/util/macros.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep util-macros- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/util/util-macros-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mi

}