HDMI-CEC services files for libcec (cec-client)

Tested using Pulse-Eight HDMI-CEC USB adapter

cec-boot.timer.....................Executes cec-boot service at boot
cec-boot.service...................Powers on cec device
cec-suspend.service................Powers off cec device during suspend and powers cec device back on when resuming
cec-poweroff.service...............Powers off cec device before poweroff

Install to /etc/systemd/system

systemctl enable cec-boot
systemctl enable cec-suspend
systemctl enable cec-poweroff

TODO: hdmi port detection (edid-decode --physical-address /sys/class/drm/*/edid)
      for edid in $(ls /sys/class/drm/*/edid); do echo $edid; edid-decode $edid | grep 'Display Product Name' ; done
TODO: dpms hooks for blanking, mabye watch /sys/class/drm/*/dpms state changes?

TODO: osd port naming HDMI1=>HDMIPC
TODO: /dev/cecX udev autoconfig for cec-ctl
TODO: remote control passthrough button config

WISH1: wake from cec

