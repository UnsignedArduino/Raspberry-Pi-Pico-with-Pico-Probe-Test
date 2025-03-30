# Raspberry-Pi-Pico-with-Pico-Probe-Test

PlatformIO template for uploading and debugging Raspberry Pi Pico series with the Raspberry Pi Pico Debug Probe. Upload,
(serial) monitor, and debug in one for Earlephilhower core.

## Notes

* You should change the `board` if you don't have a Raspberry Pi Pico 2W. (the default - currently available options are 
  `rpipico`, `rpipicow`, `rpipicow2`, and `rpipicow2w` - don't forget to update the [`env:`] part as well!)
* Change `monitor_port` to the probe's USB serial port.
* Notice how `Serial1` is used, as `Serial` would be the USB serial port, not that UART pins that the probe would be 
  connected to. (maybe consider [`ArduinoStreamUtils`](https://github.com/bblanchon/ArduinoStreamUtils) if you want it 
  on both)
* If you don't want to use the Earlephilhower core, take a peak at commit 
  [`52b2f72`](https://github.com/UnsignedArduino/Raspberry-Pi-Pico-with-Pico-Probe-Test/tree/52b2f729a7e412da416ae4b9511980d81e0ec0c2).
* Change `board_build.filesystem_size` if desired. (default is none)
* Change `monitor_speed` if desired. (default is baud rate of 115200)
