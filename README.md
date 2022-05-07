# DEPRECATED
AUTOMATIC SCRUB TIMERS ARE IN OPENZFS UPSTREAM.

They were developed in openzfs/zfs#12193 and landed in zfs-2.1.3

# zpool-scrub
systemd zpool scrub service and timer

## Installation

### Arch Linux
You can use the `systemd-zpool-scrub` AUR package.

### Linux
    install -m 644 -o root -g root zpool-scrub@.service /etc/systemd/system
    install -m 644 -o root -g root zpool-scrub@.timer /etc/systemd/system

    systemctl daemon-reload
    systemctl enable --now zpool-scrub@tank.timer
