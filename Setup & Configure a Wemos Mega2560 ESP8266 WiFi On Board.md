DCC++EX Mega2560 + ESP8266 WiFI On-Board.  'A Operational Standalone WiFI DCC Command Station'

A Tested and Proven Configuration:
 DCC++EX >= 3.0.3
 Wemos ATMega2560 + ESP8266 WiFI - Combo Board
 Deek Robot L298P Motor Shield
16Vdc Laptop power supply to the Motor Shield with 14.5Vdc to the tracks for HO Gauge
9Vdc power supply to the ATmega boards female 2.1mm power barrel
Android Smartphone w Engine Driver v2.26.115 >

Few Multiple Easy Steps;
1) Download the ESP Files,
2) Flash the ESP8266 chip,
3) Edit & Load the DCC++EX 3.0 to the Mega2560 chip,
4) Set up Engine Driver Throttle

Steps;
1) downloaded the Flash Download Tool 3.8.5 nodencu-flasher & download the ESP8266_NONOS_AT_Bin_v1.7.4 Bin files found here
https://wakwak2popo.wordpress.com/2021/01/05/flashing-at-command-set-on-combined-mega-8266-board/

2) To Flash with ESP8266_NONOS_AT_Bin_v1.7.4 set the ESP section of the board with the USB unplugged. (no power)
(set dip switches 1,2,3,4,8 off .. 5,6,7 on)
(set TX/RX dip switch to RXD3 & TXD3)
Plugged in Mega+WiFI board to comm port X, pressed Mode button,

Run the 3.8.5 Flasher Tool {give it time to completely open}
press [Developer Mode] button
press [ESP8266 Download Tool] button

Set up file location in the Tool version 3.8.5
Pay close attention setting up the Exact *.bin Files & locations 0x......
[​IMG]

And then set the Exact radial dial & baud rate settings;
(26M, 40MHz, DIO, 16Mbit-C1, com: xx, 460800 baud).

First press the Erase button and let the ESP erase the chip memory
Then press the Start button and the bin files will flash load onto the ESP chip

After flashing, the ESP8266 Log will show it uploaded them all successfully and it closes the port.
You Disconnect the USB cable.

3) Set up the Arduino ATmega2560 side of the board with DCC++EX 3.0.+
(dip switches 1,2,5,6,7,8 off .. 3,4 on)
(Leave the TX/RX dips on RXD3 TXD3)
re-connected the USB cable

Download and install DCC++EX from either the Automated exInstaller or the Latest DCC++ EX Release.
https://dcc-ex.com/download/index.html

Once you have DCC-EX installed on the Mega you need to copy, rename  and edit as follows
In the DCC++EX Command Station Folder make a Copy of the sampleconfig.h file and rename it to config.h
Open the CommandStation-EX.ino in the Arduino IDE Interactive Development Editor then;
Edited & change the tab config.h data to your local or home Router's SSID & Password.
#define WIFI_SSID "......" to your "local SSID"
#define WIFI_PASSWORD "......" to your "local PW"

Compile and upload to the
ATMega2560 board (com: xx, baud 115200),
Verify your com port and baud rate in windows device manager

After the Arduino IDE uploads DCC-EX 3.0 sketch
Disconnect USB cable
Reset dip switches 1,2,3,4 on .. 5,6,7,8 off
(Leave the TX/RX dips on RXD3 TXD3)

Power up the Arduino ATMega+ESP8266WiFi board by Either a USB cable.
Note: {For Standalone Operations (no USB) you can use a 7-12vdc power supply in the Arduino 2.1mm female barrel.}

When powered on through a USB cable, check the Arduino IDE Tools > Serial Monitor.
It should show the ATMega2560 & ESP8266 WiFI communicating and assigning a
xxx.xxx.x.xxx IP Address and Port 2560 to the new DCC++EX Command Station.

4) Set your Smartphone WiFi to the same local SSID you entered into the DCC++EX config.h file
Start your Smart Phone Engine Driver App and enter the XXX.XXX.X.XXX 
IP address assigned in the Arduino Serial Monitor above and Port 2560.

If the Engine driver fails to connect the first time with the Command Station just press the Mega's red Reset button and try the IP / Port connection again.

You should have a direct Throttle connection to the DCC++EX 3.0 Standalone WiFI Command Station Via your home Router.
Note : This is an Operations only config, the Engine Driver Power button only powers on the Main track, Not the Prog track.
Function Keys are only local Default Function Settings, and are Not transferred from the JMRI Server Roster.

Enjoy your New DCC++EX MEGA + WiFI On-Board Command Station

