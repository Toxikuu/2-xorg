NAME="xinit"
VERS="1.4.3"
DESC="X initialization program"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/app/xinit.git"
DEPS=(
    "libx11"
    "bash"
    "xauth"
    "xmodmap"
    "xrdb"
    "util-macros"
)

SOURCE="https://www.x.org/pub/individual/app/xinit-$VERS.tar.xz"
EXTRA=()

2b() {

with xorg

cfg "${XORG_CONFIG[@]}" --with-xinitdir=/etc/X11/app-defaults
mk
mi

}

2z() {

msg 'You may want to start X on the first available virtual terminal (normally tty7)'
msg 'To do this, execute the following commands as root:'
msg ' $ chmod -v 4755 /usr/bin/Xorg'
msg ' $ sed -i '\''/$serverargs $vtarg/ s/serverargs/: #&/'\'' /usr/bin/startx'

}
