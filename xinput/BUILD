NAME="xinput"
VERS="1.6.4"
DESC="Small commandline tool to configure devices"
CATG="cli"
UPST="https://gitlab.freedesktop.org/xorg/app/$NAME.git"
DEPS=(
    "libx11"
    "libxi"
    "libxinerama"
    "xrandr"
    "libxfixes"
    "util-macros"
    "xorgproto"
)

SOURCE="https://www.x.org/pub/individual/app/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

}
