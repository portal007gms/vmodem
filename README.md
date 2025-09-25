This fork fetches the connection name of the host (example: eth0) instead of it being hardcoded.
Also, getty has been replaced with agetty

# vmodem
The Virtual Hayes Compatible Modem script for Linux.

This might be an outdated version of the script. 
The most recent version can be obtained at: http://www.steptail.com/guides:virtual_modem:script !

2021-01-24
----------
* 1.5.0 changed default IP address from 192.168.0.x to 10.0.100.x to not conflict with common IP ranges
* 1.5.1 vmodem is no longer assuming eth0 is the primary network card on linux machine. This can now be changed on vmodem.sh by way of variable $etherp. So if your Raspberry Pi is connected over wifi, set it to wlan0
* 1.5.2 added command "ipaddr" to show vmodem host's IP address
* 1.5.3 explicitly set the terminal newline to CR/LF instead of assuming it. This will avoid some terminals such as xterm which default to it just sending LF as newline.
