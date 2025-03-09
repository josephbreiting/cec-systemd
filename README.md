HDMI-CEC services files for libcec (cec-client)
Tested using Pulse-Eight HDMI-CEC USB adapter

cec-boot.timer.....................Powers on cec device on at boot

cec-suspend.service................Powers off cec device during suspend and powers cec device back on when resuming

cec-poweroff.service...............Powers off cec device before poweroff

Install to /etc/systemd/system

systemctl enable cec-boot
systemctl enable cec-suspend
systemctl enable cec-poweroff
