# FlySky-i6-Mod-10ch
![](https://github.com/benb0jangles/FlySky-i6-Mod-/blob/master/Images%20for%20readme/mod-i6-snap.jpg)
(https://github.com/benb0jangles/FlySky-i6-Mod-/tree/master/10ch%20Mod%20i6%20Updater/10ch_MOD_i6_Programmer_V1_5)
#

# FlySky-i6-Mod-Telemetry Firmware (Experiment - 21/12/2016)
![](https://github.com/benb0jangles/FlySky-i6-Mod-/blob/master/Images%20for%20readme/Mavlink-screen-1.jpg)
(https://github.com/benb0jangles/FlySky-i6-Mod-/tree/master/10ch%20Mavlink%20Mod%20i6%20Updater)
##
A collection of software modifications for the FlySky i6, some useful, some experiment. All use of this repository is experimental and you use at your own risk. But, progress is being made. Please also note that this project is now contributed by many developers/engineers who deserve lots of recognition for their (free) time, knowledge & effort, so please say thanks to all contributors and not me as a single entity. Open/Free Devs need hugs too. Thanks :)

Project goals:
- Increase number of channels (using PPM or ibus)
- Enable Mavlink/APM Telemetry (using ia6b receiver)
- Ability to edit TX Voltage reading & alarm (allowing lithium battery power)
- Edit duration of 1 minute 'inactive' alarm
- Functional Flight Timer
- RSSI



Notable thanks to contributors:
qba667, Povlhp, ThomHpl, DBorthwick, Benbojangles

/-----------------------------------------------------------------------------------------------------/

At present we have the following achievements using the FlySky i6:
- We are able to flash different official firmware to the i6 and explore each new firmware
- there are hidden menus to change things like: e.g: tx voltage measurement, stick centering etc
![](http://3.bp.blogspot.com/-Nj7mgAIT7MA/Vh5VKxS7OHI/AAAAAAAAEws/Srsql8ZaRrE/s1600/i6-tx.jpg)
![](http://4.bp.blogspot.com/-2-VoNcjyxok/Vh5ZktnN3WI/AAAAAAAAEw8/HZ8-ryeElaA/s1600/1menu-i6.jpg)
- there is secret way to enter firmware update mode ![](http://4.bp.blogspot.com/-L71EbAD5BOw/VjwdEn_-eOI/AAAAAAAAEys/0qlKbKI8ZUk/s1600/i6-firmware-mode-pic.jpg)
- flashing the i6 using trainer port - to - FTDI/UART does not affect the bootloader code (as is understood 17/11/2015)
![](http://4.bp.blogspot.com/-8cAZaMrxo7E/VOfhg4rcxlI/AAAAAAAADd4/MQmE-XY-Oo0/s1600/flysky-diy-cable.jpg)
- flashing the i6 using it's internal DEBUG PORT/JTAG is possible to change the bootloader, collect eeprom data, and change firmware
- There is a guide to FTDI flashing i6 with different official firmware: (http://dalybulge.blogspot.co.uk/2015/10/turnigyflysky-i6-secret-menu.html?view=classic)
- There is a guide to flashing i6 for 8ch mod using Jtag(https://github.com/ThomHPL/FSi6_updater) Also guide (https://basejunction.wordpress.com/2015/09/13/en-flysky-i6-part-3-firmware-patching/) Also easy explanation here (https://github.com/benb0jangles/FlySky-i6-Mod-/tree/master/Developer%20Files/SWD%20port%20Flashing%20Guide)
- Experiments using Arduino IDE v1.6.6 are ongoing (https://www.arduino.cc/en/Main/Software), with Teensyduino Add-on (https://www.pjrc.com/teensy/teensyduino.html) (Settings > Board > Teensy LC > 48mhz) (LCD example: ST7565)
- Flashing under Linux (wine) is possible, but you may need to map wine's COM1 to the actual com port (e.g. /dev/ttyUSB0)
(https://www.winehq.org/docs/wineusr-guide/misc-things-to-configure#AEN901)
- There is also a native uploader for Linux, see https://github.com/mhils/flysky-updater
- If you have interested in learning about the process involved in accessing, reading then reversing firmware I will add links here:
(http://jcjc-dev.com/2016/12/14/reversing-huawei-5-reversing-firmware/)

More will be added/edited as progress is made. Please send me PM me if you have changes/updates: 
email:i6mods@gmail.com
RCgroups.com:Benbojangles
Diydrones.com:Benbojangles
http://dalybulge.blogspot.co.uk/2015/10/turnigyflysky-i6-secret-menu.html?view=classic

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.
