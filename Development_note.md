# Development note
Everything interesting when we develop this code.

## Hardware config
![Hardware](https://github.com/Xinyuan-LilyGO/T-Display-S3/raw/main/image/T-DISPLAY-S3.jpg)


## Display driver
Lilygo only provided driver for Arduino platform.
But there are other drivers aviliable for ESP-IDF.

- [lvgl port for esp32](https://github.com/lvgl/lv_port_esp32)
- [ESP32 TFT library](https://github.com/loboris/ESP32_TFT_library)

[LVGL](https://docs.lvgl.io/7.11/) is a graphic library that looks very useful.

## Issues that I encountered

### Boot loop
Add this to `platformio.ini` 
```
board_build.flash_mode = dio
```
[For more, Check this](https://github.com/platformio/platform-espressif32/issues/622)

### Porting IDF project to PlatformIO
[Check this github issue](https://github.com/lvgl/lv_port_esp32/issues/220)


### HSPI undecleared
[solution](https://www.esp32.com/viewtopic.php?t=24492)
