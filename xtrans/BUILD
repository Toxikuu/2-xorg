NAME="xtrans"
VERS="1.6.0"
DESC="X transport library"
UPST="https://gitlab.freedesktop.org/xorg/lib/libxtrans.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep $NAME- | sed 's@_@.@g' | sort -V | tail -n1"

SOURCE="https://www.x.org/releases/individual/lib/xtrans-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

}