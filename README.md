## Adafruit Grand Central M4 Express featuring the SAMD51 PCB

<a href="http://www.adafruit.com/products/4064"><img src="assets/4064.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit Grand Central M4 Express featuring the SAMD51. Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/4064

### Description

We're selling out fast but making more all the time! Sign up to be notified when it's in the store!

Are you ready? Really ready? Cause here comes the **Adafruit Grand Central** featuring the **Microchip ATSAMD51**. This dev board is so big, it's not named after a Metro train, it's a whole freakin' station!

This board is like a freight train, with its 120MHz Cortex M4 with floating point support. Your code will zig and zag and zoom, and with a bunch of extra peripherals for support, this will for sure be your favorite new chipset.

The Grand Central is the first SAMD board that has enough pins to make it in the form of the Arduino Mega - with a massive number of pins, tons of analog inputs, dual DAC output, 8 MBytes of QSPI flash, SD card socket, and a NeoPixel.

To start off our ATSAMD51 journey we are going large with the Mega shape and pinout you know and love. The front half has the same shape and pinout as our Metro's, so it is compatible with all our shields. It's got analog pins where you expect, and SPI/UART/I2C hardware support in the same spot as the Metro 328 and M0. But! It's powered with an ATSAMD51P20:

 * Cortex M4 core running at **120 MHz**
 * [Floating point support with Cortex M4 DSP instructions](https://developer.arm.com/technologies/dsp/dsp-for-cortex-m)
 * **1MB flash**, **256 KB** RAM
 * 32-bit, 3.3V logic and power
 * **70 GPIO pins in total**
 * Dual 1 MSPS DAC (A0 and A1)
 * Dual 1 MSPS ADC (15 analog pins)
 * 8 x hardware SERCOM (can be I2C, SPI or UART)
 * 22 x PWM outputs
 * Stereo I2S input/output with MCK pin
 * 12-bit Parallel capture controller (for camera/video in)
 * Built in crypto engines with AES (256 bit), true RNG, Pubkey controller

Pretty good start right? So we put this chip on a PCB with all these nice extras:
 * **Power the Grand Central** with 6-12V polarity protected DC or the micro USB connector to any 5V USB source. The 2.1mm DC jack has an on/off switch next to it so you can turn off your setup easily. The board will automagically switch between USB and DC.
 * **Grand Central has 62 GPIO pins**, 16 of which are analog in, and two of which is a true analog out. There's a hardware SPI port, hardware I2C port and hardware UART. 5 more SERCOMs are available for extra I2C/SPI/UARTs.
 * **Logic level is 3.3V**
 * **Native USB**, there's no need for a hardware USB to Serial converter as the Metro M4 has built in USB support. When used to act like a serial device, the USB interface can be used by any computer to listen/send data to the METRO, and can also be used to launch and update code via the bootloader. It can also act like an HID keyboard or mouse.
 * **Four indicator LEDs and one NeoPixel**, on the front edge of the PCB, for easy debugging. One green power LED, two RX/TX LEDs for data being sent over USB, and a red LED connected. Next to the reset button there is an RGB NeoPixel that can be used for any purpose.
 * **8 MB QSPI Flash** storage chip is included on board. You can use the SPI Flash storage like a very tiny hard drive. When used in Circuit Python, the 8 MB flash acts as storage for all your scripts, libraries and files. When used in Arduino, you can read/write files to it, like a little datalogger or SD card, and then with our helper program, access the files over USB.
 * **Micro SD Card slot** - removable storage of any size, connected to an SPI SERCOM (SDIO is not supported)
 * **Easy reprogramming**, comes pre-loaded with the [UF2 bootloader](https://learn.adafruit.com/adafruit-metro-m0-express-designed-for-circuitpython/uf2-bootloader), which looks like a USB storage key. Simply drag firmware on to program, no special tools or drivers needed! It can be used to load up CircuitPython or Arduino IDE (it is bossa v1.8 compatible)
We have a working Arduino board support package, with lots of stuff working, but our primary target for this board is CircuitPython - with 120 MHz, and 256KB of RAM CircuitPython runs really well on this chip!

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. See license.txt for additional details.
