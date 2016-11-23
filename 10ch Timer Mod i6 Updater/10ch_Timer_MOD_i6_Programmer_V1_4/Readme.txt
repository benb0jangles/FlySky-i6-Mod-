10ch Firmware courtesy of D.Borthwick 05/12/2015
Timer & RSSI Update by qba667 23/11/2016 
Updater by Benbojangles

Folder includes:
- .exe updater containing qba667 firmware
- .hex file

The mods are:
(23/11/2016)
Timer updated 1 seconds - 2999111 ticks - during 5 minutes test there is no difference between timer and stop watch.
ALT sensor added - I don't know what sensor exactly is supported by I6x but I have used same ID


(16/11/2016)
Added names for telemetry sensors with IDs 4-F. Can be changed before flashing at address FA70 for sensor 0x4 each sensor name (8 bytes for name 0 termination needed). Also other sensors names can be changed.
Custom format method for telemetry added starting at FB6C. Just edit and compile attached asm file ane replace bytes from FB6C in original file.

Patched firmware now is able to display additional sensors, formats correctly units for RSSI, Noise and SNR.

FW image from 1800-fac2 so can be flashed with updater.

Please note that addresses I am using in my comments are relative to full FW (so with boot-loader). Published file can be use with serial flasher so it doesn't have boot-loader all offsets are -0x1800. So if I am speaking about FB6C in attached FW is located at E36C (FB6C - 1800).


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
