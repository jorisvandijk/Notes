# QMK Keyboard Flashing

## Compiling
Compile the JSON file on https://config.qmk.fm

## Flash mode
First reset the keyboard into flash mode. On mine Fn+Ctrl.

## Flashing
In order to flash a .bin file to my Planck, I issue the following command from the directory the .bin is in.
```
dfu-util -d 0483:df11 -a 0 -s 0x08000000:leave -D <name of .bin file>
```
