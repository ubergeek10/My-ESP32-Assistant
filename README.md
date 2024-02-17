# My-ESP32-Assistant
This is my current configuration for an ESP32-based assistant to be used as an I/O device with Home Assistant.
Most of this code comes from Nabu Casa's Year Of The Voice 5 YouTube video.  I have changed many of the pins however, in an attempt to get rid of the loud static from the speakers when the device is first powered on.

Mapping:
| ESP32 (WROOM-32) | MAX98357A (Speaker) | I2S Microphone   |
|------------------|---------------------|------------------|
| GPIO33           | DIN                 | -                |
| GPIO12           | LRCLK               | -                |
| GPIO13           | BCLK                | -                |
| GPIO34           | -                   | SD               |
| GPIO25           | -                   | WS               |
| GPIO26           | -                   | SCK              |
| 3.3V             | VDD                 | VDD              |
| GND              | GND                 | GND              |


I believe the static to be dependent on the specific ESP32 dev board that you are using.
This code is running on an ESP-WROOM-32 development board.
