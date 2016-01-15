# RuuviTag Rev.B2

Changelog after Rev.B1:

* Remove useless pull-up resistor from BUTTON1 (nRF52 has internal ones)
* Name LED3 to LED2 in schematic
* Mark C12 (connected to DEC2 pin) to not assembled
* Remove SPI DataFlash
* Remove 0ohm series resistor from antenna
* Remove PI antenna matching network (leave the shunt)
* 32MHz crystal from 3225 to 2016 size
* Completely redesigned battery holder mechanism
* LEDs from 0402 to 0603 (more low forward voltage choices available in 0603 size)
* Add a NFC antenna 
* Fix accelerometer's footprint (LGA-16) according STM's TN0018 application note. ADXL363 not supported any more (but probably reflows correctly anyways)
* SPI_ACC_CS from P0.11 to P0.08
* Remove test pads from P0.26 and P0.27
* Add test pads to P0.04, P0.05, P0.13, P0.17, P0.19, P0.25, P0.28 and P0.29
* Update BOM components according Nordic's references

Accelerometer options:

* H3LIS100DL: 8bit, 100g, 400Hz
* H3LIS200DL: 8bit, 100-200g, 1kHz
* H3LIS331DL: 12bit, 100-400g, 1kHz
* LIS331DLH: 2-8g, 1uA sleep, 10uA 10Hz, 250uA 1kHz max datarate, 1000pcs 1EUR (Mouser)
* LIS331HH: 12bit, 6-24g, 1uA sleep, 10uA 10Hz, 250uA 1kHz max datarate, 1000pcs 2.4EUR (Mouser)
* LIS3DSH: 16bit, 2-16g, 2uA sleep, 11uA 3Hz, 225uA 1.6kHz max datarate, 1000pcs 1.3EUR (Mouser)
* LIS3DH: 12bit, 2-16g, 0.5uA sleep, 2uA 1Hz, 11uA 50Hz, 5kHz max datarate, 1000pcs 0.96EUR (Mouser)
* LIS3DE: 8bit, 2-16g, 0.5uA sleep, 2uA 1Hz, 11uA 50Hz, 5kHz max datarate, 1000pcs 0.6EUR (Mouser, not yet in stock)