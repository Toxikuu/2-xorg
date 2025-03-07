NAME="xwininfo"
VERS="1.1.6"
DESC="Displays X window information"
CATG="cli"
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
DEPS=(
    "libxcb"
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
