NAME="xset"
VERS="1.2.5"
DESC="User preference utility for X"
CATG="cli"
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
DEPS=(
    "libxmu"
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
