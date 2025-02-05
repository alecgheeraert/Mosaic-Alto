<p align="center">
  <img width="100%" src="Assets/Banner-Alto.jpg">
</p>

# MosaicAlto

## What is the MosaicAlto project?
**MosaicAlto is a Septentrio Open-Source hardware project powered by the Mosaic GNSS receiver that is compatible with the Arduino Pro Portenta boards.**
The objective of this project was to allow reliable industrial use and development with the Mosaic by having the board as a carrier for the Portenta boards.

The board also has the option to be used as a standalone device by using the USB-C connector and MosaicBus has been designed to be use either the Septentrio [**Mosaic-x5**](https://www.septentrio.com/en/products/gps/gnss-receiver-modules/mosaic-x5) or the [**Mosaic-H**](https://www.septentrio.com/en/products/gps/gnss-receiver-modules/mosaic-h).


## What is the Mosaic module?
**[Mosaic modules](https://www.septentrio.com/en/products/gnss-receivers/rover-base-receivers/receivers-modules) are Septentrio's small-size and low-power GNSS receiver modules ideal for providing highly accurate positions.** Mosaic modules integrate the latest generation of GNSS technology, delivering highly accurate positions with minimal power consumption. While compact in size they fully retain the high-reliability and exceptional accuracy performance that Septentrio receivers are known for. True multi-frequency multi-constellation technology gives our module receivers access to every possible signal from all available GNSS satellite constellations including the U.S. GPS, European Galileo, Russian GLONASS, as well BeiDou, QZSS and NavIC. [Septentrio’s advanced field-proven algorithms](https://www.septentrio.com/en/company/septentrio-gnss-technology) exploit this signal diversity to deliver maximum positioning availability and reference network compatibility.

## How to set up MosaicAlto?
### Hardware
To start using the MosaicAlto some antennas need to be connected to the board.
When using a [**Mosaic-x5**](https://www.septentrio.com/en/products/gps/gnss-receiver-modules/mosaic-x5) only a single antenna needs to be connected to the ANT 1 SMA connector.
However when using the [**Mosaic-H**](https://www.septentrio.com/en/products/gps/gnss-receiver-modules/mosaic-h) a single or dual antenna setup can be configured.
To connect an Arduino Pro Portenta board, just click it into the designated space. Please do this in the correct orientation as printed on the MosaicAlto board.

## Interfaces on the board
### Power
To power the board there are 2 options.
Either power it through the USB-C connector.
Or by using the 5V DC power connector.

### USB-C
Through the USB-C connector it is possible to communicate to the Mosaic and/or to the Arduino board attached.

### USB-A
The 2 USB-A connectors are connected to the Arduino board to attach any peripherals.

### Ethernet
The board supports Gigabit ethernet. This connects to the Mosaic and/or Arduino board.

### Headers
The headers expose some pins of the Mosaic and Arduino.
| BOTTOM | TOP |
|:---:|:---:|
| +5V | Ground |
| GPIO 1 | ADC 0 |
| GPIO 0 | TIMER 0 |
| I2C SCL 1 | I2C SDA 1 |
| I2C SCL 0 | I2C SDA 0 |
| CAN RX 1 | CAN TX 1 |
| CAN RX 0 | CAN TX 0 |
| UART RX 1 | UART TX 1 |
| UART RX 0 | UART TX 0 |
| MOSAIC RX | MOSAIC TX |
| MOSAIC GPIO | MOSAIC EVENT B |
| MOSAIC PPS | MOSAIC EVENT A |


## How to produce
All the files needed are each in their own folder, such as the BOM (Bill Of Materials), the Gerber and Pick-place files.

***Disclamer***
All the files are provided as is. These have not been fully validaded by the author or Septentrio.
The use of any of these files are at your own risk and responsibility.

---
*Designed by A. Gheeraert*
