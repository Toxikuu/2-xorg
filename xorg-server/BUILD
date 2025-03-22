NAME="xorg-server"
VERS="21.1.16"
DESC="X Window System display server"
CATG="graphics"
UPST="https://gitlab.freedesktop.org/xorg/xserver.git"
VCMD="git ls-remote --tags --refs '$UPST' | sed 's@.*/@@' | grep '$NAME-' | sort -V | tail -n1"
DEPS=(
    "libxcvt"
    "pixman"
    "font-util"
    "dbus"
    "elogind"
    "libepoxy"
    "r^libinput"
    "r^xkeyboard-config"
    "o^libunwind"
    "o^nettle"
    # Note: There are a few more optional deps
)

SOURCE="https://www.x.org/pub/individual/xserver/$NAME-$VERS.tar.xz"
EXTRA=()

2b() {

with meson ninja

_cfg_opts=(
    --localstatedir=/var
    -D glamor=true
    -D secure-rpc=false
    -D xkb_output_dir=/var/lib/xkb
)

ms "${_cfg_opts[@]}"
nj
ni

mkdir -pv "$D"/etc/{X11/xorg.conf.d,sysconfig}
cat >> "$D"/etc/sysconfig/createfiles << "EOF"
/tmp/.ICE-unix dir 1777 root root
/tmp/.X11-unix dir 1777 root root
EOF

}

2z() {
    install -vdm1777 /tmp/.{ICE,X11}-unix
    msg 'You may want to add your non-root user(s) to the input and video groups:'
    msg ' $ usermod -aG input,video <username>'
}
