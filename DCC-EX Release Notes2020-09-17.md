## Larry's thoughts on what should be in a first Release of DCC-EX:

**Note:**  If we shoot for a **Oct. 15 release that only give is a one or two weeks of getting ready for and conduction Alpha Testing and two or three weeks of Beta Testing**. That is not really much time to get these processes working well.  That means that everything we want to test is working today from the Developer Point of View.  

**I think it would be better to shoot for a Halloween Release Oct. 31st** (FlightRisk would like this) and and a **Christmas or New Years Release**. That will give us time to move things into their proper GitHub Repos, conduct Alpha Testing and write the necessary documentation that we may not have today, without working too hard to make a tight deadline. 

**We should also advertise a Roadmap of what's comming in next Release and future Releases and to keep potential users interested.**  

### Features in CVReader to CommandStatiion-DCC - (Larry's list in Support-Planning #7)

- [ ]  Railcom Support **(Future Release)**
- [ ]  Engine Driver Support **(Future Releases- unless it works today)**
- [ ]  WiThrottle Support **(Future Release)**
- [x]  Filter Function or User Function Override
- [x]  Arduino Uno Support
- [x]  Arduino Mega Support
- [ ]  FireBox Support. **(Future Release)**
- [ ] 

### Existing Features - (Fred's list in CommandStation-EX #22)

- [x]  Support Mega, Uno and Nano (some features may not be available on the Uno and Nano)
- [ ]  Configuration for Arduino Motor Board and Pololu board **(Not sure we should support Pololu - Haba says its current sensing doesn't work well)**
- [x]  Full Throttle Control <t x x x>
- [x]  Turnout Control <T ADDRESS SUBADDRESS THROW>
- [x]  Define Turnout <T ADDRESS SUBADDRESS>
- [x]  List Defined Turnouts <T>
- [x]  Sensor Control
- [x]  List Defined Sensors <S>
- [x]  Output Control
- [x]  List Defined Outputs <Z>
- [x]  List Status of all Sensors <Q>
- [x]  Accessory Control
- [x]  Extended Accessory control with same issue of how to handle listing them
- [x]  All CAB functions F0-F28
- [x]  Network Shield support
- [x]  Throttle reminders
- [x]  Store Definitions to EEPROM <E>
- [x]  Erase All Definitions from EEPROM <e>
- [x]  Display Status <s>

### New features (Fred's list in CommandStation-EX #22)

- [x]  New waveform generator
- [x]  Improved CV read byte
- [x]  Improved CV read bit
- [x]  Improved CV write byte
- [x]  Improved CV write bit
- [ ]  WiFi Client access to WiThrottle **(Suggest we shoot for a  for Dec 2020 Release to keep users interested)**
- [ ]  Extend Turnout Control <T ADDRESS THROW> (no subaddress)   **(Future Release)**
- [ ]  Extend Define Turnout <T ADDRESS> (no subaddress) (no subaddress)  **(Future Release)**
- [ ]  ??? How would we display list defined turnouts if we have two ways to input them?  
- [ ]  Individual track power control **(Future Release)**
- [ ]  Single or Dual-Pin Inverted PWM output **(Future Release)**
- [ ]  New, simpler CAB Fn command **(Future Release)**
- [ ]  WiThrottle support  **(Future Release - unless it works today)**
- [ ]  Wifi AP access to WiThrottle**(Future Release - unless it works today)**
- [x]  Function reminders
- [x]  Filter / user functions
- [x]  Extended <c> command
- [ ]  Extended Accessory Control (1 part addressing in addition to 2 part) **(Future Release)**
- [x]  Diagnostic <D XXX> commands
- [x]  WiFi Support on Uno Serial(0) **(Maybe if it can support it easily)**
- [x]  Test Multiple Locos (**limited through Alpha Testing - more extensive through Beta Testing)**
- [x]  Test Multiple Throttles **(limited through Alpha Testing - more extensive through Beta Testing)**

### Additional Issues/Features - based on on-going Discord discussions:

- [x]  No Jumper Install
- [x] Any Pin install

- [x]  Config.h File
- [ ] Multiple .INO files
- [x] Installer **(if it works now - if not, than lets go with Arduino IDE)**
- [ ] Arduino IDE
- [ ] Documentation for key features above and beyond Greg's features  - **(This may be the area requiring the most work if all of the Code is working today)**