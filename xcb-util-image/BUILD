NAME="xcb-util-image"
VERS="0.4.1"
DESC="XCB port of Xlib's XImage and XShmImage"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcb-image.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '^$NAME-.\\+[0-9]$' | sort -V"
DEPS=(
    "libxcb"
    "xcb-proto"
)

SOURCE="https://xcb.freedesktop.org/dist/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

cfg
mk
mi

}
