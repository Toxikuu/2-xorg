NAME="mkfontscale"
VERS="1.2.3"
DESC="Create an index of scalable font files for X"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
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

cfg $XORG_CONFIG
mk
mi

}
#d initialized xorg env
