10ch Firmware courtesy of D.Borthwick 05/12/2015
Timer & RSSI Update by qba667 16/11/2016 
Updater by Benbojangles

Folder includes:
- .exe updater containing qba667 firmware
- .hex file

The mods are:
(16/11/2016)
Here you have test version of timer which is not using epprom to store data - timer can be configured before it starts on "Test page" - added before by Dave - I have already change it but attached version is from yesterday - tested with my quad-copter so I am not hesitating to publish it . 
By default it set to 3rd channel and starts when channel value is above 1002.
Timer data is stored at the end of sensor array which is 256bytes and located at 200001A4 I am using bytes from 0x20000274. 
Theoretically this array is allocated only to 150 bytes so I have some free space in RAM for my small experiment - but I am no't sure- in worst case you should seen some strange characters on telemetry area

Timer is enabled on AFHDS 2 main screen and displayed in place of model index.
In attachment you can find also asm source code - of the timer.
Please check accuracy, maybe my 3.2 M clock must be "calibrated".
In next version I will add storing changes in eeprom - this is almost working.. but again after implementation it must be tested - because days are short lately I don't know if I will be able to provide it before weekend. If someone can test it for me please let me know I will send my "test" build.
As bonus I am attaching my "build script" in Python used to merge fix and calculate CRC value and offset - be aware that call to method defined in python script must be replaces first in original binary - so calculation of correct BL opcode must m performed before and it must be replaced in original binary. 



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
