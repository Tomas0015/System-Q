# System-Q
System Q is an open source security system, based on the ESP microcontroller, with wireless and wired bus capabilities.
# I like cheese
We  hate cloud with a passion so there will not be a cloud integration developed by us, the most you will get is a GSM modem sending out SMS messages. 
Our current goal is to make a low cost system with lots of well integrated features. Here are our current plans of what we will be developing:
- Battery module for either backup power or completely wireless operation
- Siren featuring an "ahooga" horn with microphone feedback, to verify that the siren is actually functional (Bus powered due to high power requirements)
- Central control unit based on some variation of raspberry pi running python scripts with an in-built flasher for the peripherals and potentially some kind of GSM modem for communicating current events.
- In the current version, the batteries will most likely not be rechargeable and generally not integrated that well. Currently it's 4 AA batteries and a diode to prevent charging them, they are connected to the main boards voltage regulator, because connecting them directly to the uController did not feel right. One possible problem is that the board doesn't know where is it getting power from, that's rather unfortunate.

 # Central control unit
- Based on raspberrry Pi
- Most likely based on python
- In-built flashing port for the peripherals. For this purpose we've devised a custom interface based on a serial connection.
- Mains power and backup power for the I2C device bus and the control unit itself
- Logging of the events happening
- Some means of communicating with the outside world, in the begining there will most likely only be email available. In the future there might be something more robust such as an GSM modem, if we were to use an LTE one, both emails and SMS messages could be possible. GSM connectivity is not a high priority at the moment.
- Some kind of local user interface with a simple character LCD and a few buttons for some minor configuration changes and error messages (there is a big possibility of a fully colour screen for the option of playing doom on your security system, because you obviously need that in your life).
- A local WEB configuration tool which will not be under any circumstances connected to cloud, It's local, take it or leave it, simple as that. It might be possible to integrate the outputs into the cloud, but the system is able to work completely offline.

# *We found out:*
- [3/9/23] The current revision of the PIR board is not suitable for operation with batteries, it's missing a diode so upon a connection of the battery, it would backfeed the entire bus. Suffice to say that's not ideal, it will be fixed in PIR board revision 2 (maybe)
- [7/9/23] Company funding our project has stepped away, meaning we are developing it on our own and with our own money. This will very likely slow down the development process A LOT. Most likely not due to lack of funds but instead due to lack of motivation. We will still try to continue with further development.
