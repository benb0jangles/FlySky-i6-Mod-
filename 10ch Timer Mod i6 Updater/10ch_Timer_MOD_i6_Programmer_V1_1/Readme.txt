10ch Firmware courtesy of D.Borthwick 05/12/2015
Timer & RSSI Update by qba667 16/11/2016 
Updater by Benbojangles

Folder includes:
- .exe updater containing qba667 firmware
- .hex file

The mods are:
(16/11/2016)
I am able to read write settings to/from EEPROM. So In next days I will check how I can implement RSSI as channel data. 
Meantime I am adding displaying of current flight mode - is someone interested in such feature? I was thinking about telemetry as well currently sensors from 0-F can be handled by RX so maybe some small sensor emulator to get some additional telemetry. Cleanflight can send emulated sensors already to our RX, but I have only APM so some additional effort is necessary. In what sensor data are you guys mostly interested (because of some names, formatting methods etc)? 
Meantime I am giving version where timer settings can be stored in eeprom.
After first flash before eeprom is initialized in configuration menu you should see OFF.
Short OK/Cancel on timer configuration page should reset current count.
Long OK/Cancel cancel should save settings. 
Attached file contains also eeprom of my radio - just for information purposes maybe someone want to see what our radios are keeping in memory.


(05/12/2015)
4 extra Aux channels - any of them can be set to be any switch or VR.
New Aux channels are stored against each model.
Updated screen for setting the aux channels.
Updated screen for displaying all 10 channels.
Inactivity timer 10min instead of 1min.

Requires:
-i6 Transmitter (Turnigy or Flysky)
-ia6b/fsia10/fsia10b Receiver
-UART/FTDI cable to flash firmware (Diy adapter: http://dalybulge.blogspot.co.uk/2015/10/turnigyflysky-i6-secret-menu.html)
(optional)
-ibus to ppm converter (Diy coverter: https://bitbucket.org/daveborthwick/ibus_pic12f1572)
-flight controller with ibus support
