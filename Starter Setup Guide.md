**Introduction**

Welcome to DCC++ EX, an open-source hardware and software platform for the operation of DCC equipped model railroads based on Gregg E. Berman's DCC++ code. 

DCC-EX picks up where the original DCC++ left off. By addressing some previous issues, we have released a re-named version of this as DCC++ Classic giving the model railroader everything they enjoyed in the original version - in a stable release.

In addition, we have  continued development with an all new version called DCC++ EX [for EXtended] that builds on the DCC++ Classic version and now includes many enhancements and upgrades. We intend to organize this all in one place so that development can continue and the platform can reflect new hardware and technology as it comes within focus.

The Classic version can be found on our Github portal DCC++ EX and is no longer supported. The EX version will soon be available on our website www. Dcc-ex.com where you will find a support link.

**Our Mission**

Our mission is to open the world of model railroading and make it universally accessible.

In order to achieve that, DCC++ EX will provide the model railroad community with a complete, open source DCC (Digital Command Control) system. One that is simple, affordable and expandable, to control model trains on layouts of almosts any size and the associated accessories. Further, it is our goal that this project be organized, documented, and maintained so that it can continue far into the future.

For the moment we are focussing this document on modellers who are new to DCC++ and just want to operate their layouts safely. More experienced modellers will findn some guidance at the end of this document.

This guide will help you through the initial stages of installing and starting to use the new DCC++ EX model railway control system. 

It is aimed at someone who is not technically savvy. We will cover the following areas:-

* What equipment you will need to have or buy
* What cables you will need to have or buy
* How to connect it all together
* What power unit you will need and how to connect that
* Where to find the software for the Command Station
* How to instal the software
* How to start running your layout

_Other headings for RB [and others] to fill in_

**Hardware**

So, what do you need in order to set up a DCC++ EX Command and Control system?

FIrstly there are the componenents. You either need to have or buy

* **Command Station** This consists of two parts

    * An Arduino UNO or MEGA
    * A motor shield [also known as a motorboard]

* **Controller**  There are several ways to control the Command Station

    * The JMRI Train Controlling and Decoder Programming Software
    * The Arduino Serial Monitor
    * A third party throttle

* **Track Power Supply** A DC power supply to provide power to the rails

* **Computer** You will need a laptop or other computer

    * To download the software that runs the Command Station
    * To operate the layout either
        * By using the JMRI control application
        * -or- to utilise the Arduino Serial Monitor
        * -or- to use the Chrome based web browser throttle
        
* **A USB A - B cable**

* I have an image - but don't know how to get it on here

* **The DCC++ EX Software** The DCC++ EX sofware (called a "sketch") is loaded onto the your Arduino command station



**Connecting it all together**

[Here is a diagram of a simple set-up](https://docs.google.com/presentation/d/1-QqqR-oO8w8AdobiK7A_sCFi9oz1dTh63g8KO6KlMw4/edit#slide=id.p)

Do  not connect any of the boards to your computer just yet.

**Firmware**

For the moment it is recommended that the required code is downloaded via the Arduino IDE only. 

A simpler installataion process will be availabel on our website in due course

For now then,

* Make sure you download and install the Arduino IDE if you don't already have it.   
      ***NOTE: This is a 192Mb download*** [Click here for the link](https://www.arduino.cc/en/Guide)
      
* Download the Arduino Timers library file [Click here for the link](https://github.com/davidcutting42/ArduinoTimers/archive/master.zip)

* Download the DCC-EX library file [CLick here for the link](https://github.com/DCC-EX/CommandStation/archive/master.zip)

* Download the CommandStation Sketch [Click here for the link](https://github.com/DCC-EX/CommandStation-DCC/archive/master.zip)

Unzip the two library files (ArduinoTimers-master.zip and CommandStation-Master.zip) one at a time to your desktop or downloads folder. You should then have these two folders after unzipping that look like this
   * ArduinoTimers-Master
   * CommandStation-Master
   
Rename these two folders to remove the “-master”. In other words the folders should now look like this
   * ArduinoTimers
   * CommandStation
   
Select both the above mentioned folders and move them to your Arduino libraries folder, usually: \Documents\Arduino\libraries\

You will see other folders there which are other libraries for the Arduino. Your new library folders will live happily next to the others.

Unzip the CommandStation-DCC.zip file to your download or desktop folder and then move it to your Arduino projects folder, which should be:
/documents/Arduino

You may notice other project folders here, and should see the libraries folder where we just copied your libraries to.

Rename this folder like you did with the library folders to remove the “-master” so that the folder name is simply, “CommandStation-DCC”.
9. Open the Arduino IDE program from the operating system menu on your computer. Then click on “File -> Open” and navigate to your projects folder (/documents/Arduino) and find the CommandStation-DCC folder. Click on that folder to open it and find the main project file. All Arduino main files end in .ino (as in Ardu-INO) and should have the Arduino logo on them to advertise their association with the Arduino IDE. Click on “CommandStation-DCC” to open the project in the IDE>
The project will open either in a new window or the same window depending on your settings. If there are two windows, you can close the first window if you like because we won’t need it anymore. You will see tabs for the 3 files used by CommandStation-EX running across the top of the Arduino IDE.
10. Connect a serial cable from your computer to your Arduino Command Station. You should see lights blink on the Command Station board and get an acknowledgement from your computer that you just plugged something in.
11. Select “Tools -> Board” from the Arduino IDE menu and find your board. You should be using one of the following:
•	Arduino Mega or Mega 2560
•	Aduino Uno
•	Arduno Nano
12. Choose the serial port your operating system assigned to your Arduino board under “Tools -> Port”. The IDE should automatically detect the correct port, but you may have to select it if you have more than one Arduino board plugged in or have more than one you plug in at different times. Once you select a board, the system will remember that port for that Arduino.
13. The last step is to upload the sketch to your Arduino. Click the “upload” button at the top left that looks like a right arrow. It is next to the checkmark button that lets you compile and verify the program separately. This test is conducted before uploading and will flag any errors anyway. Besides, those of us on the DCC++ EX team never make mistakes, so it should compile and upload perfectly!
The compile and upload process should take between 30 seconds and 2 minutes. Once complete, you should be able to run you DCC++ EX Command Station!
Testing

The Arduino IDE has what is called a “serial monitor” built in. It allows us to monitor things connected to the serial port. DCC++ EX has messages and debugging included. With the Command Station still connected to your computer via the USB cable and the correct port selected, choose “Tools -> Serial Monitor” from the menu. A new window will open and you should see a line of text giving you status information that looks like this:
DCC++ EX Command Station V2.1.1<NO:SERIAL>
This lets you know everything is working. As another quick test, after making certain that your connections to the track are correct and that there are no shorts, you can type:
<1>
Into the serial monitor command box at the top, to the left of the “send” button and press send. If your motor controller has LED indicators, they should light and you will have power to the track. If you have a locomotive with a sound decoder on the track, it should start to make idle sounds. To turn off the power, simply enter:
<0>
And hit the send button. You are finished. To run trains, you simply need to connect a controller like a throttle or JMRI. Happy Trails! Or Tracks, in this case.

For the Engineers

Browse the code or use these links to clone the DCC-EX Command Station files. Create repositories: 
The command station library file:
https://github.com/DCC-EX/CommandStation.git#master
The Arduino Timers libary file:
https://github.com/davidcutting42/ArduinoTimers.git#master
The main Command Station Sketch:
https://github.com/DCC-EX/CommandStation-DCC.git#master
To clone, use GitHub Desktop or Git Bash. In git bash, navigate to where you want to clone the repository and from the "$" prompt, type "git clone https://github.com/DCC-EX/CommandStation.git" and https://github.com/DCC-EX/CommandStation-DCC.git

Troubleshooting:
The Com port under “Tools -> Port” is grayed out.
You don’t see anything from the serial monitor when you open it

Testing

Quick test


Troubleshooting

?

FAQs

?

Resources

?
Common Documentation Elements

?
