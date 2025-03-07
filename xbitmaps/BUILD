NAME="xbitmaps"
VERS="1.1.3"
DESC="X bitmap images"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/data/bitmaps.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-' | tail -n1"
DEPS=(
    "util-macros"
)

SOURCE="https://www.x.org/pub/individual/data/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

cfg ${XORG_CONFIG[@]}
mi

}