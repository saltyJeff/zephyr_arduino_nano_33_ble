# zephyr_arduino_nano_33_ble
Board support package for Zephyr RTOS for the Arduino Nano 33 BLE

Tested & Working:
* I2C (both internal and external)
* SPI
* USB CDC
* UARTs
* Flashing with the default onboard bootloader. 
Make sure you use the special Arduino variant of the `bossac`.

Untested
* PWM

Shouldn't work
* RTC's (there's no onboard backup battery)

## Notes
Use this by adding this repo as a submodule into boards/arm/

You will want to link the `arduino_nano_33_ble` library into your
application-level CMakeLists.txt