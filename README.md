# EricB Clock ESP board
EricB has created a clock that uses MAX7219 dotmatrix and a lot of add-ons.
I have created a PCB (KiCad 8.0 format) that connects to the back of the matrix and has the possibilty to add the other components using simple pin headers.
Code is based on Arduine IDE and is also included.

For the EricB project, take a look at this [EricB Clock](https://www.hackster.io/ericBcreator/alarm-clock-with-web-interface-wake-up-light-temp-more-75dc6a)!
Code and my binary is also available here.

Enjoy and feedback is welcome.

## Pinout explanation
Here is what the pin assignment looks like.
### Rotary
P1 GND  
P2 +5V  
P3 GPIO17 -> switch  
P4 GPIO32 -> pinB (data)  
P5 -> GPIO27 -> pinA (clock)  
### MAX7219
P1 +5V  
P2 GND  
P3 GPIO23 -> DIN (MOSI)  
P4 GPIO16 -> CS  
P5 GPIO18 -> CLK (SCK)  
### BME280
P1 +5V  
P2 GND  
P3 GPIO22 -> SCL  
P4 GPIO21 -> SDA  
### Buzzer
P1 GPIO5  
P2 GND  
### PIR
P1 +5V  
P2 GND  
P3 GPIO26 -> sensor  
### Neopixel
P1 +5V  
P2 GPIO19 -> DIN  
P3 GND  
### Lightsensor GL5537
P1 +5V  
P2 GPIO36 with resistor 120 Ohm to ground  


