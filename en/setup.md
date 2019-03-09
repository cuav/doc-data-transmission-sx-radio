# Use hardware connection

---

#### Regardless of the receiving end and the transmitting end: {# No receiving end and transmitting end:}

The CUAV SX Radio module does not divide the receiving end from the transmitting end (not the aircraft and the ground), and the module has an automatic switching chip built in.

When USB is plugged into the computer, data is automatically switched to the USB port

When USB is not present, data is switched to the 6P GH1.25 port

#### Factory paired: {#factory paired:}

The factory default is airspeed 115K, interface rate is 57600, peer-to-peer broadcast mode

If you need to modify the configuration, please refer to the software configuration guide. Generally, you only need to modify the VID to achieve the effect of isolation from communication with other modules. For example, if you modify other configurations, familiarize yourself with the documentation and then modify it carefully.

#### Connection with Flight Control: {# Connection with Flight Control:}

PixHack: Radio Interface Plugged into Flight Control

Pixhawk: plug into the flight controller's telem1 or telem2 interface

#### Ground station use: {# ground station use:}

In theory, the ground stations of the PIX are compatible. Please select 57600 baud rate when connecting. Note whether the driver is installed correctly and whether the port number is selected.

If you use a mobile OTG connection, the distance may be short because OTG power is not enough

## Power Requirements:

The ground end needs to ensure that the usb port power supply current is greater than 250MA, and independent power supply is recommended if conditions permit (some old notebooks/cell phones/tablets may not move).

### Apply to other systems:

If only the wireless data transmission module is used, please follow the interface definition and the system connection (RX-TX TX-RX GND-GND)

The default standard interface rate is 57600. The required interface baud rate can be changed according to the requirements.

[Using the tutorial](http://doc.cuav.net/tutorial/copter/optional-hardware/radio/xbee%20Radio/xbeextend%20debug.html)