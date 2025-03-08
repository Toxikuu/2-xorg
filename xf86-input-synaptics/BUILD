NAME="xf86-input-synaptics"
VERS="1.10.0"
DESC="Synaptics driver for notebook touchpads"
CATG="drivers input"
UPST="https://gitlab.freedesktop.org/xorg/driver/$NAME.git"
DEPS=(
    "libevdev"
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
