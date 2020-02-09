# Arduino Serial Programmer

## Description

This is a simple USB to serial programmer. This code helps to transform a Teensy2++ micro controller to an ATMega328p (Arduino UNO controller) Arduino serial programmer.

Once an ATMega328 has been flashed with the Arduino Boot Loader, it is able to be programmed via its native serial TX/RX pins. So to upload a program to a flashed ATMega328 we need a device to interface the standart USB PC port to the TX/RX signals.

Refer this schematic to perform connectics between Teensy programmer and the ATMega328
(image available in current repository: assets/programmer-electronic-schema.png)

![Teensy2 Arduino 328p serial programmer](https://raw.githubusercontent.com/Akrobate/ArduinoSerialProgrammer/master/assets/programmer-electronic-schema.png)


## Customizations

Some customization can be done on this code

* Changing the usage of the 'reset_pin' on the teensy2++. (Default pin : 4)
* Changing the led_pin. The led pin is used to indicate the activity while uploading. Default is 6 (Teensy onboard LED), but you can add a LED on your board and map the pin.
* Default baud rate (baud varaible) can be changed. All tests has been done with the default configuration and works correctly with 19200 to program an ATMega328p with a Teensy2++

