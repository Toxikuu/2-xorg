NAME="xtrans"
VERS="1.5.2"
DESC="X transport library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxtrans.git"

SOURCE="https://www.x.org/releases/individual/lib/xtrans-$VERS.tar.xz"
EXTRA=()

2b() {

b-cfg $XORG_CONFIG
b-make
b-mi

b-32cfg $XORG_CONFIG
b-make
b-32mi

mkdir -pv "$D"/usr/lib32/pkgconfig
cp -vr 32DEST/usr/share/pkgconfig/* "$D"/usr/lib32/pkgconfig/

}
