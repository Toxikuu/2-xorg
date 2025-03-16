NAME="libxkbcommon"
VERS="1.8.1"
DESC="Keymap compiler and support library"
CATG="lib"
UPST="https://github.com/lfs-book/$NAME.git"
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
