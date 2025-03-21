NAME="libxkbcommon"
VERS="1.8.1"
DESC="Keymap compiler and support library"
CATG="lib"
UPST="https://github.com/lfs-book/$NAME.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed -e 's@.*/@@' -e 's@_@.@g' | grep -i xkbcommon- | sort -V | tail -n1 | cut -d- -f2"
DEPS=(
    "xkeyboard-config"
    "libxcb"
    "wayland"
    "wayland-protocols"
)

SOURCE="https://github.com/lfs-book/$NAME/archive/v$VERS/$NAME-$VERS.tar.gz"
EXTRA=()

2b() {

with meson ninja

ms -D enable-docs=false
nj
ni

}
