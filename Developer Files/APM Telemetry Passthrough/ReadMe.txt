I have a theory: 

that ia6b receiver uses baud 115k or 57k - so if the wish is to connect to APM telemetry, it must be baud-matched using telemetry port, or USB - Not sure yet. 

Also, I believe telemetry passthough can be achieved using HC-06 bluetooth module connected to i6 transmitter on trainer port (TX > RX) with matching baud.

Why do this? 

- Because then no need to change/modify/hack i6 LCD screen code 
- The telemetry data will go from HC-06 bluetooth to Android device with Droidplanner.
- I think two-way telemetry is possible (sending commands from Droidplanner > HC-06 > i6 TX > ia6b > APM Drone.)

I will try, but also require other experimenters willing to provide feedback.

PDF Guide Instructions will go here
