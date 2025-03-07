NAME="xdpyinfo"
VERS="1.3.4"
DESC="Display information utility for X"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-' | sort -V | tail -n1"
DEPS=(
    "libx11"
    "libxcomposite"
    "libxext"
    "libxinerama"
    "libxrender"
    "libxtst"
    "libxxf86vm"
    "util-macros"
    "xorgproto"
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
