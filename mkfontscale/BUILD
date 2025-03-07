NAME="mkfontscale"
VERS="1.2.3"
DESC="Create an index of scalable font files for X"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-[0-9]\.' | sort -V | tail -n1"
DEPS=(
    "freetype"
    "zlib"
    "libfontenc"
    "util-macros"
    "xorgproto"
)

SOURCE="https://www.x.org/pub/individual/app/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

}
#d fixed vcmd
