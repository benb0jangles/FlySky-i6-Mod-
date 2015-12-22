Firmware V1.3 courtesy of D.Borthwick 22/12/2015
Updater by Benbojangles

Folder includes:
- .exe updater containing borthwick 10ch firmware
- 10ch .hex file

The mods are:
4 extra Aux channels - any of them can be set to be any switch or VR.
New Aux channels are stored against each model.
Updated screen for setting the aux channels.
Updated screen for displaying all 10 channels.
Inactivity timer 10min instead of 1min.

Enables you to select all 10 channels in the iBus setup menu. 

ch 9 & 10 bug fix

tried with a FS-IA10 receiver and get 10 channels of servos

combinations of switches to work for Aux 5 to 10. So now as well as selecting "None", "Vr A" or"Vr B" and"Sw A" to "Sw D", 
you can also select "Sw A+B", "Sw B+C", "Sw C+D" or "Sw A+D". Gives you lots of choice for multiposition flight modes or other things.

Bug fix: fix for the mix crash problem

also contains the external battery sensor code I had been working on. The revised RX Battery page lets you set:

The sensor - Internal (default) or External (uses first iBus voltage sensor CVT01)
The cells type - NiMH (default) or LiPo
The cell count - (defaults to 4) 
The Low level - Bottom level of battery symbol & causes the fast beep alarm
The Alarm Level - Causes the slow beep alarm
The High Level - Top level of battery symbol

OK moves between items.
Up and Down modify an item.
Cancel exits without change.
Long Cancel exits with save.
Long OK sets default values (based on cell type and count).



