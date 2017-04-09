RPI-Wireless-Hotspot
====================

Configures your Raspberry Pi3 with built in WiFi as a hotspot, broadcasting your ethernet connection to other devices.

Features:
---------

* Configured hotspot starts automatically on boot, no extra configuration necessary

* Configured WiFi network is WPA encrypted.

* Default SSID of "RaspberryPiFi" and WPA key of "0123456789A" can be modified during install

* Once set up, the local network facilites of the Pi will still operate as normal

* Easy setup of either a custom or preconfigured DNS server (including unblock-us for removing netflix geoblocks)

* Router enumeration for WiFi network

* Allows chromecast compatibility with unblock-us by intercepting google's DNS requests on the pi


Installation:
-------------
* sudo apt-get install git

* In the terminal, run:
    sudo git clone https://github.com/Dorha85/RaspberryPi3-HotSpot.git

* Navigate to folder, [ cd RaspberryPi3-HotSpot ] and execute [ sudo ./install ]

* Confirm that you are happy for changes to be made

* Choose a preconfigured DNSalternative DNS or configure a custom DNS

* If you require chromecast support with unblock-us select the appropriate option

* This should automatically set everything up and leave you ready to go


Notes and configuration
-----------------------

* To change default WiFi channel, edit /etc/hostapd/hostapd.conf accordingly

* This setup has been tested on a fresh install of raspbian.

* It is advised that this be set up on a fresh install

* If set up on an existing install then any current config files will be backed up with the extension ".old" in the relevant folders prior to installation (this allows returning to original network settings if required)

