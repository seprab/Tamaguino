# Tamaguino
Tamagotchi clone for Arduino

> Based on the original project:
https://alojzjakob.github.io/Tamaguino/

I had to edit part of the code since my OLED screen seems to contain a SH1106 controller. The original project is compatible with SSD1306 controller which is different to the screen I got.

How did I realize it? I found another user having the same issue as me and the community suggested 

<img src="https://aws1.discourse-cdn.com/arduino/optimized/4X/c/2/d/c2d21426ff543d3b5d3caf9807e0a7c260ae3ef7_2_440x500.jpeg"
     alt="Example of the problem"
     style="float: left; margin-right: 10px;" />
[Forum thread reference](https://forum.arduino.cc/t/oled-1-3-i2c-iic-128x64-serial-lcd-faulty/250171)

So, instead of using Adafruit SSD1306, I used SH110X which also seems to be created by Adafruit.

At the moment, this project requires:
- [Adafruit BusIO by Adafruit Version 1.13.2](https://github.com/adafruit/Adafruit_BusIO)
- [Adafruit GFX Library by Adafruit Version 1.11.3](https://github.com/adafruit/Adafruit-GFX-Library)
- [Adafruit SH110X by Adafruit Version 2.1.8](https://github.com/adafruit/Adafruit_SH110X)


