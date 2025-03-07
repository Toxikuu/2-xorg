NAME="xkbevd"
VERS="1.1.6"
DESC="XKB event daemon"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
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
