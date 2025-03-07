NAME="xmodmap"
VERS="1.0.11"
DESC="Utility for modifying key and button maps"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
DEPS=(
    "libx11"
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
