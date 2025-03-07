NAME="xcursorgen"
VERS="1.0.8"
DESC="Create an X cursor file from PNG images"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-[0-9]\.' | sort -V | tail -n1"
DEPS=(
    "libpng"
    "libx11"
    "libxcursor"
    "util-macros"
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
