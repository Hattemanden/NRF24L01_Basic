# NRF24L01_Basic
First working setup of 2 NRF24L01 working

## Project Description
This is my first working setup, of two NRF24 talking with eachother. 
One NRF is transmitting it's current runtime (millis()).

The other one is then listening for this, receiving this time, showing it to the console, and sending it back to the first NRF.

The first NRF then receives this time, and then calculating the time it took, to send something to the other, and then receiving this againg. This time is then printed on the Serial monitor.

## Sketch difference
There is two different sketches. One for each NRF.
The sketch inside the folder NRF24, is the transmitter, 
ans the sketch inside the folder NRF24_2, is the receiver.

## Connections
Connect NRF and Arduino as follows:

Signal  | RF Module Pin | Arduino
:------:|:-------------:|:------:
GND     | 1             | GND
VCC     | 2             | 3V3
CE      | 3             | 9
CSN     | 4             | 10
SCK     | 5             | 13
MOSI    | 6             | 11
MISO    | 7             | 12
IRQ     | 8             | -

