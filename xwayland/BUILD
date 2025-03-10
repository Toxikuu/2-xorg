NAME="xwayland"
VERS="24.1.6"
DESC="Run X clients under wayland"
CATG=""
UPST="https://gitlab.freedesktop.org/xorg/xserver.git"
DEPS=(
    "libxcvt"
    "pixman"
    "wayland-protocols"
    "font-util"
    "libepoxy"
    "mesa"
    "libxau"
    "libxfont2"
    "libxshmfence"
    "pixman"
    "wayland"
    "xorg-server"
    "libxkbfile"
    "dbus"
    "xorgproto"
    "xtrans"
)

SOURCE="https://www.x.org/pub/individual/xserver/xwayland-$VERS.tar.xz"
EXTRA=()

2b() {

with meson ninja

# Don't install a manpage provided by xorg-server
sed -i '/install_man/,$d' meson.build &&

ms -D xkb_output_dir=/var/lib/xkb -D secure-rpc=false
nj
ni

mkdir -pv "$D/src/sysconfig"
cat >> "$D"/etc/sysconfig/createfiles << "EOF"
/tmp/.X11-unix dir 1777 root root
EOF

# Note: Xvfb is not installed in this build

}
