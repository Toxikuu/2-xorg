NAME="font-util"
VERS="1.4.1"
DESC="X font utilities"
CATG="font"
UPST="https://gitlab.freedesktop.org/xorg/font/util.git"
DEPS=(
    "util-macros"
    "glibc"
)

SOURCE="https://www.x.org/pub/individual/font/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

}
