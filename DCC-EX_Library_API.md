# The DCC-EX Library API 
 
## General configuration and status getter functions
 
 **getStatus()** _boolean_ - Returns status information
 
 **getPreambles()** _uint8_t_ - Returns the current setting for the number of preamble Bits
  
## Waveform control functions
 
 **setPower(bool on, bool report = false)**
 
 **setSignal(bool high)**
 
 **setBrake(bool on)**

## Current Functions
 
 **checkCurrent()** - Function that must be run oten in a loop to check the current to the track.

 **getLastRead()** _float_ - Returns the raw pin reading on the current sense pin
  
 **getLastMilliamps()** _float_ - Returns the laste reading of track current in milliAmps
  
 **getMilliamps()** _float_ - Returns the instantaneous current readin in milliAmps
  
 **setBaseCurrent()** - Sets the base reading for programming track current to compare against to detect an ACK and puts it in baseMilliAmps
  
  **getBaseCurrent()** _uint16_t_ - Returns the base or "idle" current in milliAmps
  

## General config modification

  **config_setChannelName(const char &ast; name)** - Puts the channel name ("MAIN", "PROG") into the channel_name variable
  
  **config_setControlScheme(control_type_t scheme)** - Sets the method of control for the motor controller. Boards like the Arduino Motor controller 
  have 1 input for the PWM signal while boards like the IBT_2 have separate signal pins. Options are:
  
  DUAL_DIRECTION_INVERTED - Setting for boards with 2 PWM input pins usually labled clockwise and counterclockwise or left and right
  
  DIRECTION_BRAKE_ENABLE -
  
  DRV8873 -

  **config_setPreambleBits(uint8_t preambleBits)** - Sets the number of preamble bits. Default is XX. Use for XXX

## Pin config modification

  **config_setPinSignalA(uint8_t pin)** { signal_a_pin = pin; }
  
  **config_setPinSignalB(uint8_t pin)** { signal_b_pin = pin; }
  
  **config_setDefaultSignalB(default_pin_state_t default_state)** { signal_b_default = default_state; }
  
  **config_setPinEnable(uint8_t pin)** { enable_pin = pin; }
  
  **config_setDefaultEnable(default_pin_state_t default_state)**  { enable_default = default_state; }
  
  **config_setPinSleep(uint8_t pin)** { sleep_pin = pin; }
  
  **config_setDefaultSleep(default_pin_state_t default_state)**  { sleep_default = default_state; }
  
  **config_setPinCurrentSense(uint8_t pin)** { current_sense_pin = pin; }

 ## Current config modification
 
  **config_setTriggerValue(int triggerValue)** { trigger_value = triggerValue; }
  
  **config_setMaxValue(int maxValue)** { maximum_value = maxValue; }
  
  **config_setAmpsPerVolt(float ampsPerVolt)** { amps_per_volt = ampsPerVolt; }

  **config_setTrackPowerCallback(void (*_TrackPowerCallback)(const char* name, bool status))**  TrackPowerCallback = _TrackPowerCallback;
