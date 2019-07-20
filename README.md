## Project Description
This project demonstrates the basics of using the ESP-IDF component "mjd_hcsr501".

The component supports various PIR motion sensor models:

- HC-SR501 PIR motion sensor module.
- MH-SR602 Micro PIR motion sensor module.
- AM312 Mini PIR motion sensor module.

Go to the component "components/mjd_hcsr501" for installation and usage/wiring instructions, data sheets, FAQ, photo's, etc. for the hardware and software.

The project uses the ISR handler of the mjd_hcsr501 component to detect movement (interrupt on positive edge), and also routes the GPIO input pin receiving the signal from the PIR sensor to the GPIO Output pin of the on-board LED.



## What are the HW SW requirements of the ESP32 MJD Starter Kit?

### Hardware

- A decent ESP development board. I suggest to buy a popular development board with good technical documentation and a significant user base. Examples: [LOLIN D32](https://wiki.wemos.cc/products:d32:d32),  [Adafruit HUZZAH32](https://www.adafruit.com/product/3405),  [Espressif ESP32-DevKitC](http://espressif.com/en/products/hardware/esp32-devkitc/overview), [Pycom](https://pycom.io/hardware/).
- The peripherals that are used in the project. The README of each component contains a section "Shop Products".

### Software: ESP-IDF v3.2

- A working installation of the **Espressif ESP-IDF *V3.2* development framework**** (detailed instructions @ http://esp-idf.readthedocs.io/en/latest/get-started/index.html).

```
mkdir ~/esp
cd    ~/esp
git clone -b v3.2 --recursive https://github.com/espressif/esp-idf.git esp-idf-v3.2
```

- A C language editor or the Eclipse IDE CDT (instructions also @ http://esp-idf.readthedocs.io/en/latest/get-started/index.html).



## Running the example
- Run `make menuconfig` and modify for example the GPIO PIN# that you want to use (section "Project Configuration").
- Run `make flash monitor` to build and upload the example to your board and connect to its serial terminal.



## Reference: the ESP32 MJD Starter Kit SDK

Do you also want to create innovative IoT projects that use the ESP32 chip, or ESP32-based modules, of the popular company Espressif? Well, I did and still do. And I hope you do too.

The objective of this well documented Starter Kit is to accelerate the development of your IoT projects for ESP32 hardware using the ESP-IDF framework from Espressif and get inspired what kind of apps you can build for ESP32 using various hardware modules.

Go to https://github.com/pantaluna/esp32-mjd-starter-kit
