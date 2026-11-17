# NIMO

NIMO is an interactive desk companion robot built on an ESP32 C6. Its OLED display shows animated eyes that express six emotions: happy, sad, angry, excited, sleepy and surprised. An MPU6050 motion sensor notices when you shake it, so NIMO gets dizzy and then angry. A touch sensor lets you change expressions and switch between display modes. It also works as a digital clock and a world clock, synced over Wi-Fi using NTP.

## Hardware

- ESP32
- 1.3" SH1106 OLED display
- MPU6050 accelerometer and gyroscope
- TTP223 touch sensor

## Wiring

| Component | Pin | ESP32 |
|---|---|---|
| OLED | VCC / GND | 3.3V / GND |
| OLED | SDA / SCL | GPIO 22 / GPIO 23 |
| MPU6050 | VCC / GND | 3.3V / GND |
| MPU6050 | SDA / SCL | GPIO 22 / GPIO 23 |
| TTP223 | VCC / GND | 3.3V / GND |
| TTP223 | OUT | GPIO 2 |

The OLED and MPU6050 share the same I2C bus, and all grounds are common.
