TorPi
======

A guide how to setup a Raspberry Pi as a Tor gateway that will force all TCP and UDP traffic 
through Tor.


WiFi Network ---> [TorPi] ---> Tor

Requirement:
Raspberry Pi
Power Adapter
4Gb+ Memcard
Supported Wifi Adapter


###Download Raspbian Image

Download latest Raspbian image from: 
http://www.raspberrypi.org/downloads/

Flash it to the memcard:
http://www.raspberrypi.org/documentation/installation/installing-images/README.md

When booting up, expand the filesystem if wanted.


###Configure Raspbian:

Remove X11 and dependances

sudo apt-get --purge remove x11-*
sudo apt-get autoremove


Upgrade packages

sudo apt-get update
sudo apt-get upgrade


Set locales

printf "\n#Locales\nexport LC_ALL=C" >> ~/.bashrc


# 

