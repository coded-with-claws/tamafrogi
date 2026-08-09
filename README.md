# tamafrogi
Tamagotchi-like frog for ESP32.
An ESP32 is used to store the animations (Arduino Nano was tried at first but is too small, either with RAM or with PROGMEM).

# Hardware
- ESP32 (tested with ESP32 Mini (ESP32-C3))
- OLED 1.3" 128×64 SH1106
- Infrared motion sensor
- Push button

# Behavior
Tamafrogi shows happy animations on screen, until its falls asleep or needs care.
Movements detected by the motion sensor keep Tamafrogi awaken.
A cuddle given by pushing the button restores Tamafrogi to happy state.

# Wiring
- OLED Display
  - GPIO8 - SDA
  - GPIO9 - SCL/SCK
  - 3.3V - OLED VCC
  - GND - OLED GND
- Cuddle button
  - GPIO0 / GND
- Motion sensor
  - GPIO1 / 5V / GND 

