10ch Firmware courtesy of D.Borthwick 05/12/2015
Timer & RSSI Update by qba667 16/11/2016 
Updater by Benbojangles

Folder includes:
- .exe updater containing qba667 firmware
- .hex file

The mods are:
(16/11/2016)
New version:
-Error can be assigned as channel - absolutely insane idea but it seems to be working. I have not tested values above 50%. The mapping is following 0% maximum channel value 10000 internally, 100% or not connected -10000. Please verify it it is working correctly.
-Telemetry filter is now passing sensors with IDs 4 - F without names but values should be visible. Users of Cleanflight, please test if custom telemetry is passed. 
-Timer code improved, navigation in timer menu is now like native one - long cancel press is performing save, long ok press is setting timer to 0.

The fill is just FW without boot-loader - I have stripped also FF values after checksum - so the file can be used with Thom's updater - but I have to find my FTDI adapter to test it. So maybe tomorrow morning I will confirm that it is working with the updater.

I just realize that sensors with ID 4-F can cause some strange behavior because of missing names. I will add dummy names tomorrow.
Also timer configuration menu is accidentally named "Test" - I will add telemetry names and rename menu entry in next update.


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
