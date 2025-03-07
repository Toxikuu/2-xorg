NAME="xprop"
VERS="1.2.8"
DESC="Display X properties"
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

cfg ${XORG_CONFIG[@]}
mk
mi

}
