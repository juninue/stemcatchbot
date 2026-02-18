# stemcatchbot
robot that catches a marble rolled down a ramp by measuring the speed of the marble on the flat of the ramp and predicting the horizontal change in position, then using a stepper motor and 3D printer component to catch it.


components:
arduino uno (non-knockoff, don't know if that's important)
two infared light sensors (the ones with the black and white bulbs and out vcc and gnd)
cnc shield v3 (not needed but we used it to simplify wiring)
A4988 stepper driver set to 0.87 V
17hs19 2004s1 NEMA 17 stepper motor
power supply (24 V)
3D printer belt and rail

we put the driver into the x slot of the cnc shield
5V, GND, A1 and A0 connect to pins on top of the cnc shield for the ir sensors

please set your own values for acceleration and speed if you aren't sure about the speed of your board. an esp32 for example could damage the motor if those values are so high past the maximum.
