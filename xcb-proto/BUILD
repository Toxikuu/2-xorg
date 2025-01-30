NAME="xcb-proto"
VERS="1.17.0"
DESC="XML-XCB protocol descriptions"
UPST="https://gitlab.freedesktop.org/xorg/proto/xcbproto.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://xorg.freedesktop.org/archive/individual/proto/xcb-proto-$VERS.tar.xz"
EXTRA=()

DEPS=("python")

2b() {

PYTHON=python3 b-cfg $XORG_CONFIG
b-mi

}
