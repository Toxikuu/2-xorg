NAME="xsetroot"
VERS="1.1.3"
DESC="Classic X utility to set your root window background to a given pattern or color"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
DEPS=(
    "libx11"
    "libxcursor"
    "libxmu"
    "xbitmaps"
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
