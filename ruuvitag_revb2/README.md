# RuuviTag Rev.B2

### TODO

* Consider to replace LEDs with LTST-C195KGJRKT or similar double LED package
   - Need to find less than 1.8V forward voltage versions of LEDs
* 32kHz crystal to FC-135 32.768KHZ ±20PPM,9.0PF (FC-135 32.7680KA-AC3 ?)
* Add a PCB NFC antenna 
* Seems that ADXL363 isn't 100% footprint compatible. We had some issues with it (used this same footprint). Confirm the footprint and probably drop the ADXL363 support.

Accelerometer options:

* H3LIS100DL: 8bit, 100g, 400Hz
* H3LIS200DL: 8bit, 100-200g, 1kHz
* H3LIS331DL: 12bit, 100-400g, 1kHz
* LIS331DLH: 2-8g, 1uA sleep, 10uA 10Hz, 250uA 1kHz max datarate, 1000pcs 1EUR (Mouser)
* LIS331HH: 12bit, 6-24g, 1uA sleep, 10uA 10Hz, 250uA 1kHz max datarate, 1000pcs 2.4EUR (Mouser)
* LIS3DSH: 16bit, 2-16g, 2uA sleep, 11uA 3Hz, 225uA 1.6kHz max datarate, 1000pcs 1.3EUR (Mouser)
* LIS3DH: 12bit, 2-16g, 0.5uA sleep, 2uA 1Hz, 11uA 50Hz, 5kHz max datarate, 1000pcs 0.96EUR (Mouser)
* LIS3DE: 8bit, 2-16g, 0.5uA sleep, 2uA 1Hz, 11uA 50Hz, 5kHz max datarate, 1000pcs 0.6EUR (Mouser, not yet in stock)


Done:

* Remove useless pull-up resistor from BUTTON1 (nRF52 has internal ones)
* Name LED3 to LED2 in schematic
* Mark C17 to not assembled in schematic
* Mark C12 (connected to DEC2 pin) to not assembled (difference between PCA10036 and PCA10040)
* Remove 0ohm resistor from antenna
* Remove SPI DataFlash
* Remove PI antenna matching network
* 32MHz crystal from 3225 to 2016 size
* Completely redesigned battery holder mechanism