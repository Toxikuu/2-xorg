NAME="xrefresh"
VERS="1.1.0"
DESC="Refresh all or part of an X screen"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-[0-9]\.' | sort -V | tail -n1"
DEPS=(
    "libx11"
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
