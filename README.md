# ESPnRF24 Jammer
A low-power 2,4GHz wireless jammer based on `ESP32` and `nRF24LO1+PA+LNA`

## Hardware Requirements

`esp32s3-devkitc-1`

  - 2x `nRF24L01+PA+LNA` modules
  - 2x `100uF` electrolytic capacitors of any voltage

## Assembling

- Place the capacitors across the `VCC` and `GND` pins of each `nRF24` module
- Connect radio modules to the `ESP32` board according to the pinout
- Add pin configuration in `include/options.h`

## Building

1. Install VSCode and PlatformIO
2. Edit preferences in `include/options.h`
3. If using a different board, port it into `platformio.ini`
4. Upload the code, and the SPIFFS filesystem image via platform tasks
