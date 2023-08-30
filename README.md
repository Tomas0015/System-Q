# System-Q
System Q is an open source security system, based on the ESP microcontroller, with wireless and wired bus capabilities, that is currently being developed in Hardwario located in Liberec, Czech Republic.
# I like cheese
We  hate cloud so there will not be a cloud integration developed by us, the most you will get is a GSM modem sending out SMS messages 
Our current goal is to make a low cost system with lots of well integrated features. Here are our current plans of what we will be developing:
- Battery module for either backup power or completely wireless operation
- Siren featuring an "ahooga" horn with microphone feedback, to verify that the siren is actually functional (Bus powered due to high power requirements)
- Central control unit based on some variation of raspberry pi running python scripts with an in-built flasher for the peripherals and potentially some kind of GSM modem for communicating current events.

 # Central control unit
-Based on raspberrry Pi
-Most likely based on python
-In built flashing port for the peripherals. For this purpose we've devised a custom interface based on a serial connection.
-Mains power and backup power for the I2C device bus and the control unit itself
-Logging of the events happening
