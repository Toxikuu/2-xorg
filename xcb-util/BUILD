NAME="xcb-util"
VERS="0.4.1"
DESC="Utility libraries for XC Binding"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcb-util.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-.\\+[0-9]$' | sort -V"
DEPS=(
    "libxcb"
    "xcb-proto"
)

SOURCE="https://xcb.freedesktop.org/dist/xcb-util-$VERS.tar.xz"
EXTRA=()

2b() {

cfg
mk
mi

}