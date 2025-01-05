# Car Reverse System

## Group member
1) LOO IX SHEN
2) JAMES FOO
3) OSCAR YONG
4) LIM WEI QUAN

## List of components used:
1) STM32F401CCu6 Blackpill
2) Ultrasonic Sensor HC-SR04
3) I2C Oled Display SSD-1306
4) Active Buzzer
5) Dc motor
6) Red Led

## Basic Concept
Ultraonic sensor emitts sound wave, sound wave reflect back when hitting an obstace like wall. The actual distance will be: **total time * speed of sound wave / 2**. Active buzzer will beep at different time intervals set by delay function depends on the distance measure by ultrasonic, the lower the distance, the more frequent the buzzer beeps. Oled display will shows real-time distance in either **centimeter** or **inch**, which can be trigger by pushbutton PA0 external interrupt. When distacne < 15cm, both dc motor will be turn off and Red Led will light up. In contrast, when distance > 15cm, both dc motor run and Red Led is off.
