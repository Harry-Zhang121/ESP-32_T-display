# ESP-32_T-display
A personal project build around Lilygo T-display-S3 which turn your esp32-s3 into an 2FA authenticator.

## How to build
1. Install PlatformIO on your code editer.
2. Clone this repo.
3. In PlatformIO home screen click *open project* and select this repo.
4. Rename `lv_conf_example.h` to `lv_conf.h` and put it *next* to the lvgl library dir located in `./.pio/libdeps/ESP32-S3...../`

```
    |
    |_lvgl/
    |_some_other_lib/
    |_lv_conf.h
```
5. Modify `ssid` and `password` according to your wifi information.
6. Modify `hmacKey` to be your 2FA private key. You might need to convert it into Base32.
5. In PlatformIO sidebar click *build*. 

## Development documentation
Please refer to `Development_note.md` under the root directory.