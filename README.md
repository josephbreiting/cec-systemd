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



WISH1: hdmi port detection

WISH2: wake from cec

WISH3: remote control passthrough

WISH4: /dev/cecX udev autoconfig for cec-ctl

WISH5: dpms hooks for blanking
