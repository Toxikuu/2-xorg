NAME="libpciaccess"
VERS="0.18.1"
DESC="X11 PCI access library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libpciaccess.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/pub/individual/lib/libpciaccess-$VERS.tar.xz"
EXTRA=()

2b() {

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
