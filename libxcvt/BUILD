NAME="libxcvt"
VERS="0.1.3"
DESC="library providing a standalone version of the X server implementation of the VESA CVT standard timing modelines generator"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxcvt.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="glibc meson"

SOURCE="https://www.x.org/pub/individual/lib/libxcvt-$VERS.tar.xz"
EXTRA=()

2b() {

# 2qa skip
with xorg meson ninja

ms
nj
ni

cd ..
m32=1

ms
nj
ni

}
