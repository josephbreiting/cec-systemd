# Pulse8 HDMI-CEC USB adapter systemd integration 

The pulse8-usb-cec adapter is a usb device for adding hdmi-cec support to pcs.  While they do provide a fully integrated utility for the Windows OS.  They only provide a very limited example how to integrate it into a linux system using systemd.  This repo intends to have a complete solution for both arch linux as well as the most recent lts release of ubuntu.

## Main Functionality

Turns on HDMI-TV when system boots up.
Turns off HDMI-TV when system enters suspend.
Turns on HDMI-TV when system wakes up.
Turns off HDMI-TV when systme shut down.

## Additional features

Display HOSTNAME on HDMI-TV's OSD.
Display HOSTNAME as HDMI-TV input label (HDMI1 => HOSTNAME).
HDMI-TV's remote control integration (play,pause,etc).
Wake from suspend with HDMI-TV's remote.

