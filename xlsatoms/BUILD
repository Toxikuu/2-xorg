NAME="xlsatoms"
VERS="1.1.4"
DESC="List interned atoms defined on server"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
DEPS=(
    "libxcb"
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
