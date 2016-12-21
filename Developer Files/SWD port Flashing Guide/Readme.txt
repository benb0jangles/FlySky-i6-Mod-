To replace whole flash content on the Flysky i6. It is possible with St link or other jtag/swd interface. Start address is 0x0 size is 64KB. Full image can be found on GitHub.
So in more detail you need to connect to debug port of the radio:
https://nathan.vertile.com/assets/im...03255_prev.JPG (image from Nathan Tsoi blog)
to connect you need ST-Link, this one should be fine 
http://www.banggood.com/ST-LINK-V2-E...-p-973898.html
The full flash can be downloaded from:
https://github.com/benb0jangles/FlyS...s/fsi6_ori.bin

# How to flash with ST-Link Utility:
- Downlaod software install drivers use this page for more details http://www.emcu.it/ST-LINKv2/ST-LINKv2.html
- Make connections between debug port and ST-Link
- connect ST-Link to your PC
- Launch ST-Link Utility
- Set the Address field to 0x00000000 and Size to 0x10000
- Click Connect to the target
- Click Save to keep a backup actual flash content - then you can send me it I will check what is wrong
- Download TGY firmware 1.6 for iA6B:
- Click open and select original I6 firmware
- Click Program Verify
- Click Disconnect
- Unplug ST-Link