NAME="smproxy"
VERS="1.0.7"
DESC="Provides X11R6 session management support for applications lacking native support"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
DEPS=(
    "libsm"
    "libxmu"
    "libxt"
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
