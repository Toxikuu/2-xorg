NAME="xkbcomp"
VERS="1.4.7"
DESC="X Keyboard description compiler"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-[0-9]\.' | sort -V | tail -n1"
DEPS=(
    "libx11"
    "libxkbfile"
    "util-macros"
)

SOURCE="https://www.x.org/pub/individual/app/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg $XORG_CONFIG
mk
mi

}
#d fixed vcmd
