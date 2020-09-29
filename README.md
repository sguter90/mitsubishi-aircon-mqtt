# mitsubishi-aircon-mqtt

Based on https://github.com/rjdekker/MHI2MQTT

Monorepo for building a MQTT interface for Mitsubishi Heavy Industries (MHI) SRK/SRF series air conditioners.


## Hardware

### Main parts

* [Arduino: ATMega328P 5V 16Mhz](https://www.amazon.de/dp/B015MGHLNA)
* [Wifi ESP8266 + Adapter to Arduino](https://www.amazon.de/gp/product/B0768DCWM4)
* [Step down Voltage Regulator](https://www.amazon.de/dp/B07FXBXJC5)

### Additional/Optional parts
I started with almost nothing and needed to buy some extra stuff to complete this project.

#### Cables and connectors

* [Dupont Crimping Tool Kit for connecting cables together](https://www.amazon.de/gp/product/B07QX51F3B)
* [Lipo 5 pin cables](https://www.amazon.de/gp/product/B073ZGHN38)

#### USB adapters for flashing/uploading
* [Wifi ESP8266 to USB adapter](https://www.amazon.de/gp/product/B07Q17XJ36)
* [Arduino ATMega328 to USB adapter](https://www.amazon.de/gp/product/B07BBPX8B8)

#### Soldering
* [Mat](https://www.amazon.de/gp/product/B07BXTFWV9)
* [Bolt](https://www.amazon.de/gp/product/B07G8CMMW5)
* [Solder](https://www.amazon.de/gp/product/B000V8JYP8)
* [Breadboard + Jump wires](https://www.amazon.de/dp/B07DQKXMHL)


## Software
* [platformio - for uploading sketches (VSCode recommended)](https://platformio.org/)
* MQTT broker like [Mosquitto](https://mosquitto.org/) or [hmq](https://github.com/fhmq/hmq)
* [MQTT explorer - for debugging](https://mqtt-explorer.com/)

# HowTo
Before starting this project be aware that:
1. Opening the airconditioning device may void warranty!
1. The device is using high voltage!
1. The terminal to plug in the CNS connector is difficult to reach in most cases.

Ok, let's go :smile:
1. [Adjust FTDI adapter](doc/01-FTDI-Adapter.md)
1. [Solder Arduino pin headers](docs/02-Solder-Arduino-Pin-Headers.md)
1. [Flashing Arduino](docs/03-Flashing-Arduino.md)
1. [Flashing and configuring WfFi shield](docs/04-Flashing-ESP8266.md)

# Acknowledgments
Special thankts to:
* [MHI2MQTT by rjdekker](https://github.com/rjdekker/MHI2MQTT)
* [WiFiManager by tzapu](https://github.com/tzapu/WiFiManager)
* [pubsubclient by knolleary](https://github.com/knolleary/pubsubclient)
* [Arduino-EasyTransfer by madsci1016](https://github.com/madsci1016/Arduino-EasyTransfer)
* [ArduinoJson by bblanchon](https://github.com/bblanchon/ArduinoJson)
* [Arduino by ESP8266 Community Forum](https://github.com/esp8266/Arduino)
