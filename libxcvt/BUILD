NAME="libxcvt"
VERS="0.1.3"
DESC="library providing a standalone version of the X server implementation of the VESA CVT standard timing modelines generator"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcvt.git"
DEPS="glibc meson"

SOURCE="https://www.x.org/pub/individual/lib/libxcvt-$VERS.tar.xz"
EXTRA=()

2b() {

. e-xorg
mkdir -pv build
cd        build

CP=.. b-ms
b-ninja
b-ni

rm -rf ./*
CP=.. b-32ms
b-ninja
b-32ni

}
