# reinstallNotes for hp spectre x360

## obs + NDI + v4l2loopback
install `obs-studio v4l2loopback-git obs-v4l2sink-git obs-ndi-git avahi`
systemctl start avahi-daemon.service
systemctl start avahi-dnsconfd.service

