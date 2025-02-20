NAME="libpciaccess"
VERS="0.18.1"
DESC="X11 PCI access library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libpciaccess.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/lib/libpciaccess-$VERS.tar.xz"
EXTRA=()

2b() {

with meson ninja

ms
nj
ni

cd ..
m32=1

ms
nj
ni

}