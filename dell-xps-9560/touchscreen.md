# Enable touchscreen

Activate the following:

```
-> Device Drivers
  -> HID support
    -> HID bus support (HID [=y])
      -> Special HID drivers
        -> HID Multitouch panels (HID_MULTITOUCH)
```

```
-> Device Drivers                                                        
  -> Input device support                                                
    -> Generic input layer (needed for keyboard, mouse, ...) (INPUT [=y])
      -> Touchscreens (INPUT_TOUCHSCREEN [=y])                           
        -> Elan eKTF2127 I2C touchscreen (TOUCHSCREEN_EKTF2127)
        -> Elan eKTH I2C touchscreen (TOUCHSCREEN_ELAN)
```

