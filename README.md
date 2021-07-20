# raspberry_or_linux_wifi_monitor_Mode
Quick hooks script to enable monitor mode by default on all but the first wifi adapter

This script is for DHCPCD based systems to detect additional wifi adapters and throw them into monitor mode.  

I found a ton of help on the net for the setup on none DHCPCD based systems and spent a fair amount of time figuring this out.   

Your mileage my vary good luck!

https://github.com/morrownr/USB-WiFi

https://aallan.medium.com/adding-a-second-wireless-adaptor-to-a-raspberry-pi-for-network-monitoring-c37d7db7a9bd

https://pimylifeup.com/raspberry-pi-network-scanner/


to be clear you need to create this (dhcpcd.enter-hook) file in /etc either by copying it there or using your favorite editor to create it and paste in this content.  DHCPCD will then consult dhcpcd.enter-hook everytime it runs hooks.
