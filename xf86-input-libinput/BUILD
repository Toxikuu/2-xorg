NAME="xf86-input-libinput"
VERS="1.5.0"
DESC="Libinput-based generic X input driver"
CATG="drivers input"
UPST="https://gitlab.freedesktop.org/xorg/driver/$NAME.git"
DEPS=(
    "libinput"
    "xorg-server"
)

SOURCE="https://www.x.org/pub/individual/driver/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg "${XORG_CONFIG[@]}"
mk
mi

}
