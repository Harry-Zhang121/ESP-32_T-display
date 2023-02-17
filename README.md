# ESP-32_T-display
A personal project build around Lilygo T-display-S3.

## How to build
1. Install PlatformIO on your code editer.
2. Clone this repo.
3. In PlatformIO home screen click *open project* and select this repo.
4. Rename `lv_conf_example.h` to `lv_conf.h` and put it *next* to the lvgl library dir located in `./.pio/libdeps/ESP32-S3...../`

```
    |
    |_lvgl
    |_some_other_lib
    |_lv_conf.h
```

5. In PlatformIO sidebar click *build*. 
