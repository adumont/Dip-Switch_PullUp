# Input 8bit value using DIP switch with IceZum Alhambra

- [Input 8bit value using DIP switch with IceZum Alhambra](#input-8bit-value-using-dip-switch-with-icezum-alhambra)
- [What we need](#what-we-need)
- [Schematics](#schematics)
- [Circuit in IceStudio](#circuit-in-icestudio)

# What we need

- Breadboard
- 8 bit DIP Switch
- 9 pins 3.3KOhm bussed resistor array

# Schematics

The DIP switch acts as 8 switches. We use the resistor array to connect the dip switch in a Pull-Up configuration.

- When the switch is open, current will flow from Vcc to the PINs.
- When the switch is closed, the pin will be brought down to ground.

![](images/breadboard.jpg)

![](images/pins.jpg)

# Circuit in IceStudio

![](images/circuit-icestudio.png)

In the circuit, the register enable is connected to "1" (always enabled). It can also be connected to the dbouncer, so that it will load only when button is pressed.