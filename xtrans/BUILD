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

}

#d Removed m32 xtrans, following https://github.com/glfs-book/glfs/commit/e2c3a4452b2323fbdfed579afe8ade9fc852c42f
