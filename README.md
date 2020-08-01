# reinstallNotes for hp spectre x360 13-ap0109ng

## main install
- flash [manjaro](https://manjaro.org/downloads/official/architect/)
- install CLI System
- `systemctl enable NetworkManager`
- `systemctl start NetworkManager`
- `nmcli d wifi connect SSID password PASSWORD`

## boot

## install LARBS
- `curl -LO larbs.xyz/larbs.sh`
- `sh larbs.sh`

## update keyserver... should be fixed soonIsh
To make this work permanently I appended "keyserver pool.sks-keyservers.net" into ~/.gnupg/gpg.conf
The file wasn't there to begin with so I copied the one used by pacman in /etc/pacman.d/gnupg/gpg.conf and then added the line.

## audio
### option 1
- install `pulseaudio-git sof-firmware` and `systemctl --user enable --now pulseaudio`

### option 2
- install `alsa-firmware alsa-tools`
- start `hdajackretask`
- select `Realtek ALC285` from the dropdown up top
- click `show unconnected pins` on the right
- override `0x14` with `internal speaker (LFE)`
- override `0x1e` with `internal speaker`
- click `Install boot override`

## obs + NDI + v4l2loopback
- install `obs-studio v4l2loopback-dkms-git obs-v4l2sink-git obs-ndi-git avahi`
- `systemctl enable avahi-daemon.service`
- `systemctl enable avahi-dnsconfd.service`
- `systemctl start avahi-daemon.service`
- `systemctl start avahi-dnsconfd.service`

## fusuma
`sudo gpasswd -a $USER input`

## undervolt
`sudo undervolt -v --gpu -50 --core -100 --cache -100 --uncore -100 --analogio -100 --temp 60`

## screenshots
`git clone https://github.com/luksab/scripts` to home directory

