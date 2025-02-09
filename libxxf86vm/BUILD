NAME="libxxf86vm"
VERS="1.1.6"
DESC="X11 XFree86 video mode extension library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxxf86vm.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep -i $NAME- | sed 's@_@.@g' | sort -V | tail -n1"
DEPS="libxext libx11 glibc xorgproto"

SOURCE="https://www.x.org/pub/individual/lib/libXxf86vm-$VERS.tar.xz"
EXTRA=()

2b() {

. e-xorg

b-cfg $XORG_CONFIG
b-make
b-mi

b-32cfg $XORG_CONFIG_32
b-make
b-32mi

}
