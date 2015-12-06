# RuuviTag Rev.B2

### TODO

* Add more clearance to battery hole (0.3mm should be fine)
* Name LED3 to LED2 in schematic
* Consider to replace LEDs with LTST-C195KGJRKT or similar double LED package
* Add optional NFC connector Molex 51281-0594 (0512810594) used in PCA10040
* Remove useless pull-up resistor from BUTTON1 (nRF52 has internal ones)
* 32MHz crystal from 3225 to 2016 size
* 32kHz crystal to FC-135 32.768KHZ ±20PPM,9.0PF (FC-135 32.7680KA-AC3 ?)
* Remove 0ohm resistor from antenna (and consider to replace it with MM8130-2600) http://infocenter.nordicsemi.com/topic/com.nordic.infocenter.nrf52.v1.0.0/development/dev_kit/hw_rf_meas.html?cp=1_0_2_1_7
* Board diameter from 45mm to 46mm (maybe)
* Check if it's possible to add a PCB NFC antenna (it's probably not)
* Mark C12 (connected to DEC2 pin) to not assembled (difference between PCA10036 and PCA10040)
* Mark C17 to not assembled in schematic
* C19 from 1p2 to 0p8 so that we get component count down. Probaby not assembled anyways.
* Seems that ADXL363 isn't 100% footprint compatible. We had some issues with it (used this same footprint). Confirm the footprint and probably drop the ADXL363 support.

Accelerometer options:

* H3LIS100DL: 8bit, 100g, 400Hz
* H3LIS200DL: 8bit, 100-200g, 1kHz
* H3LIS331DL: 12bit, 7100-400g, 1kHz
* LIS331DLH: 2-8g, 1uA sleep, 10uA 10Hz, 250uA 1kHz max datarate, 1000pcs 1EUR (Mouser)
* LIS331HH: 12bit, 6-24g, 1uA sleep, 10uA 10Hz, 250uA 1kHz max datarate, 1000pcs 2.4EUR (Mouser)
* LIS3DSH: 16bit, 2-16g, 2uA sleep, 11uA 3Hz, 225uA 1.6kHz max datarate, 1000pcs 1.3EUR (Mouser)
* LIS3DH: 12bit, 2-16g, 0.5uA sleep, 2uA 1Hz, 11uA 50Hz, 5kHz max datarate, 1000pcs 0.96EUR (Mouser)
* LIS3DE: 8bit, 2-16g, 0.5uA sleep, 2uA 1Hz, 11uA 50Hz, 5kHz max datarate, 1000pcs 0.6EUR (Mouser, not yet in stock)