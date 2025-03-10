# [Roon](https://roonlabs.com) [Extension](node-roon-api) to provide [source switching, standby](https://github.com/RoonLabs/node-roon-api-source-control), and [volume control](https://github.com/RoonLabs/node-roon-api-volume-control) for [McIntosh Labs](https://www.mcintoshlabs.com/)'s range of devices via [RS232](https://github.com/stefan747/node-mcintosh-rs232)

This extension connects to your McIntosh device (Preamplifier, Integrated Amplifier, etc) via RS232, and allows Roon to control it's volume directly, as well as standby, and convience source switching.

---------------------

This extension was tested on Mcintosh MA9500 Integrated Amplifier. The maximum volume has been limited to 60% to avoid accidents.

---------------------

This is my personal setup, but any Linux based device can be setup the same way:

    SoTM SMS-200
	-> USB audio -> USB cable -> McIntosh MA9500 DAC
	-> USB Serial port adapter -> RS232 Serial cable -> McIntosh MA9500

    Setup parameters (configured via Roon):
	- Serial Port: USB port on which the RS232 cable is used
	- Source for Convenience Switch: Numerical value of the McIntosh source which you want to use for Roon
	- Initial Volume: Volume used when the extension starts the McIntosh equipment
	- Startup Time: Time in seconds it takes to wake up all the audio equipment before any stream is started
