NAME="xf86-input-evdev"
VERS="2.11.0"
DESC="Generic Linux input driver for X"
CATG="drivers input"
UPST="https://gitlab.freedesktop.org/xorg/driver/$NAME.git"
DEPS=(
    "libevdev"
    "mtdev"
    "xorg-server"
)

SOURCE="https://www.x.org/pub/individual/driver/$NAME-$VERS.tar.gz"
EXTRA=()

2b() {

with xorg

cfg ${XORG_CONFIG[@]}
mk
mi

}
