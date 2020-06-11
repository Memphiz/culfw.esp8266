# culfw-esp8266
Firmware for different busware.de gadgets and esp8266 

CAUTION: since 11. Jun 2020 the wlan parameter are in the eeprom and must be initialized! "private.h" can be deleted.
* Wis&lt;SSID&gt;
* Wik&lt;wpa-key&gt;
* WiD&lt;devicename&gt;
* WiO&lt;ip-address ota-server&gt;

For OTA functionality a webserver with php must be in the local network. After uploading the php part the update
is initialized with command "B01" (on arduino "start with bootloader"), update.log must be writeable and then shows state and errors. 
V1.67.0 is the last one that has to be uploaded with the arduino-ide.

Copyright Rudolf Koenig, 2008,2009,2010,2011 for busware, Manfred Bielemeier for implementation esp8266
License: GPL v2

Culfw now running on ESP8266, initial copy from SVN repo V1.66 svn://svn.code.sf.net/p/culfw/code/trunk/culfw, updated to 1.67.

Descriptions of the project can be found in the [wiki](https://github.com/Man-fred/culfw.esp8266/wiki)

I started with a fork of svn2github/culfw, but there are many changes that have nothing to do with the original project. So I decided to split it from the fork. The new repositoriy is named Man-fred/culfw.esp8266 but will be renamed to the original title later
regards, Manfred
