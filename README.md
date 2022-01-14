# usb-mount
auto mount usb script in linux based udev and systemd

### Install
cp usb-mount.sh /usr/local/bin/
cp usb-mount@.service /etc/systemd/system/
cp S99-local.rules /etc/udev/rules.d/
udevadm control --reload-rules
systemctl daemon-reload
