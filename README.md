Microprogrammed Systems Project
Reading the ambient temperature - Temp Sensor PMOD-TMP with DS1626

The goal of this project is to read the ambient temperature using the DS1626 digital sensor, which communicates through a bidirectional 3-wire SPI interface. The implementation was done in the MPIDE environment. Considering the bidirectional nature of the interface, the MOSI line was temporarily configured as an input to allow the reception of two bytes containing the temperature value. The RST pin (equivalent to chip select) is active at logic level 1. SPI transmissions were monitored and verified in real-time using the SCOPY application, connecting the corresponding DIO lines: D11 (MOSI), D12 (MISO), and D13 (SCK). The temperature value, in hexadecimal format, was displayed in real-time on the Tera Term terminal. The temperature is displayed both in hexadecimal format and in degrees Celsius.

Main hardware components:
- Arduino Nano
- Pmod TMP temperature sensor module
- DS1626 digital temperature sensor.

Software Tools:
- MPIDE
- SCOPY
- Tera Term
- Proteus.
