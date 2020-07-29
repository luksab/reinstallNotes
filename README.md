# reinstallNotes for hp spectre x360

## main install
- flash [manjaro](https://manjaro.org/downloads/official/architect/)
- `gpg --keyserver hkp://keys.gnupg.net --receive-keys KEY`
- install CLI System
- `systemcli enable NetworkManager`
- `systemcli enable NetworkManager`
- `nmcli d wifi connect SSID password PASSWORD`

Use kernel 5.4 for audio support
## audio
- install `alsa-firmware alsa-tools`
- start `hdajackretask`
- show unconnected pins
- override 0x14 with internal speaker (LFE)
- override 0x1e with internal speaker
- Install boot override

## obs + NDI + v4l2loopback
- install `obs-studio v4l2loopback-git obs-v4l2sink-git obs-ndi-git avahi`
- systemctl start avahi-daemon.service
- systemctl start avahi-dnsconfd.service

