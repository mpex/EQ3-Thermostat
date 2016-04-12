# EQ3-Thermostat



Library to control EQ3 BTLE Thermostats.

It makes use of *gatttool* which is part of the *bluez* package.

With the lib can do:

    * Read current temperature and lockstate from thermostat (if changed manually)
    * Activate Boostmode: 300sec fully open valve
    * Deactive Boostmode: Interrupt Boostmode earlier than 300sec
    * Lock Thermostat: Disable manual mode
    * Unlock Thermostat: Enable manual mode
    * Switch between automatic, manual and eco mode (automatic schedule on thermostat side)
    * Set Temperature Offset: Set an offset to measured temperature
    * Set Day/Night Mode: Change between two preset values
    * Change Window Open settings: Change temperature and duration
    * Set Temperature: Self explanatory (given in celcius)
    * Set Time: Set date/time on the thermostat


What the lib cannot do:

    * Check if device is really present. Right now no error handling is done,
      as it is hard to determine wether the command was successful or not.
    * Manipulation of the inbuilt programs. Not necessary for my needs
    * The vacation function is not implemented

