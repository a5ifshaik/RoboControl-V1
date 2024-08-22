# RoboControl V1 - Arduino-based Robot Control Board
<p align="justify"> The RoboControl is a cheap and beginner-friendly all-in-one robot control board which is capable of dual motor control (6A/Channel), and includes dedicated pinouts for servos, sensors and external 12V systems which is controlled using a MOSFET. It also features a built in battery level sensing circuit which is made up of a simple voltage divider that translates the 0-12V range of the input battery to a analog value range between 0-1023. </p>

![image](https://github.com/user-attachments/assets/a4bbaf2c-ce27-4007-ae42-e8d151d868b4)

## Features
- 12V - 24V Input Voltage
- Arduino Nano MCU
- Two Infineon IFX9201SG Motor Drivers (Supports up to 6A/driver)
- MOSFET for External Circuit Control
- Battery Voltage Monitor
- Dedicated ports for sensors/servos

## Pinout 
| On RCB        | Arduino Pin   |                             Description                        | 
| ------------- | ------------- |  ------------------------------------------------------------- |
| S1            | D6            | Servo 1 Port; comes with 5V and GND supply                     |
| S2            | D9            | Servo 2 Port; comes with 5V and GND supply                     |
| SCL           | A5            | Serial Clock Line used for I2C                                 | 
| SDA           | A4            | Serial Data Line used for I2C                                  | 
| BZOUT         | D7            | MOSFET control line, 5V to turn on 12V line                    |
| TRIG          | D12           | Trigger Pin for Ultrasonic Sensor (Can use as normal digital)  |
| ECHO          | D11           | Echo Pin for Ultrasonic Sensor (Can use as normal digital)     |
| BATT          | A3            | Battery monitor pin, produces analog reading between 0 - 1023  |
| M1 PWM        | D3            | PWM Signal supply pin for Motor 1 driver                       |
| M1 DIR        | D8            | Motor 1 Direction Pin (1/0 for CW/CCW or vv)                   |
| M1 EN         | D2            | Motor 1 Enable Pin, Set as HIGH to enable driver               |
| M2 PWM        | D5            | PWM Signal supply pin for Motor 2 driver                       |
| M2 DIR        | D10           | Motor 2 Direction Pin (1/0 for CW/CCW or vv)                   |
| M2 EN         | D4            | Motor 2 Enable Pin, Set as HIGH to enable driver               |

## Schematics:
![image](https://github.com/user-attachments/assets/05c256b3-590f-4e4f-83a9-eaa7254789cf)

## 3D Render
![image](https://github.com/user-attachments/assets/3f577449-bf16-4e3c-bfb9-1b3f2af666ba)

## Sample Applications
### The RoboControl board was initially developed for a home-surveillance robot with 2 wheels, but can be used for various applications that have similar needs.
![image](https://github.com/user-attachments/assets/268c0a44-d3f1-4536-9a63-7e01e203c92f)
![image](https://github.com/user-attachments/assets/64f5f6fd-27c6-4b05-a943-8abe5b69a6e1)
![image](https://github.com/user-attachments/assets/5d3662b0-05e3-4a4b-9375-23e1ea648228)
###### **In Image 2, the yellow jumpers are used to correct an error found post-production which has since been rectified in this repository.






