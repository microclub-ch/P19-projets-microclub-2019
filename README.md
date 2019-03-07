# projets-microclub-2019
Platforme robotique, domotique et plus basée ESP32

### Présentation du 26.1.2019 à l'EPFL: [lien vers la présentation]

[lien vers la présentation]: https://microclub.ch/wp-content/uploads/2019/01/Project-2019.pdf

[livre]: https://leanpub.com/kolban-ESP32

Livre electronique: [livre]

## Liste d'achats (pour information et provisoire, peut changer!)
Matériel testé

ESP32 36 pin version Devkit V1, une nouvelle version 38 pins compatible WRover [Wroom-link].

[Wroom-link]:


Pont en H DRV8825 [H-Bridge]

[H-Bridge]: https://www.banggood.com/3Pcs-3D-Printer-Stepstick-DRV8825-Stepper-Driver-Reprap-4-Layer-PCB-p-1052018.html?rmmds=search&cur_warehouse=CN

Pont en H pour moteurs DC [DC-pololu]

[DC-driver]: https://www.pololu.com/product/2135

! nouveau gyro avec baro et ligne d'interruption: Gyro MPU9250 + Baro BMP280 [gyro link]

[gyro link]: https://www.banggood.com/MPU9250BMP280-10DOF-GY-91-Acceleration-Gyroscope-Compass-Nine-Shaft-Sensor-Module-For-Arduino-p-1100982.html?rmmds=myorder&cur_warehouse=CN

Moteur pas à pas NMEA17 [Step-Motor link]

[Step-Motor link]: https://www.banggood.com/Nema-17-42mm-12V-Hybrid-Two-Phase-Stepper-Motor-For-3D-Printer-p-1164619.html?rmmds=search&cur_warehouse=CN

Inteface Servo-Motor PCA9685 [Servo-Motor Driver link] library [adafruit-servo-lib]

[Servo-Motor Driver link]: https://www.banggood.com/Arduino-16-Road-PWMServoSteering-Gear-Drive-Plate-Controller-Robot-IIC-PCA9685-p-1263963.html?rmmds=search&cur_warehouse=CN

[adafruit-servo-lib]: https://github.com/adafruit/Adafruit-PWM-Servo-Driver-Library

Options (non testées)

module audio [Audio link] doc [audio-doc]

[Audio link]: https://www.banggood.com/DFPlayer-Mini-MP3-Player-Module-For-Arduino-p-969191.html?rmmds=search&cur_warehouse=CN
[Audio-doc]: https://www.dfrobot.com/product-1121.html

Cercle Neopixel, d'autres basées sur WD2812 fonctionnent également  [neo-link]

[neo-link]: https://www.banggood.com/CJMCU-61-Bit-WS2812-5050-RGB-LED-Driver-Development-Board-p-1008123.html?rmmds=detail-left-hotproducts__8&cur_warehouse=CN

Module alimentation 24-12V-5V  [alim-link]

[alim-link]: https://www.banggood.com/DC-DC-5V-3A-Power-Supply-Module-Buck-Step-Down-Regulator-Module-24V-12V-9V-To-5V-Fixed-Output-p-1177912.html?rmmds=search&cur_warehouse=CN

## Outil de développement actuel (pour avr, ESP8266, ESP32) 

PlatformIO, Une amélioration importante par rapport à Arduino IDE: [Platformio] !! attention, ne pas installer la version ATOM !
Permet d'utiliser toutes les librairies Arduino, Adafruit etc.

[Platformio]: https://code.visualstudio.com/

Nouveau sur la version Split, 2 connecteurs pour des capteurs Time of Flight type  GY-53 VL53L0X ou VL53L1X permettant de mesurer avec précision des distances de 2 ou 4m !!! en plus un connecteur pour utiliser le convertisseur ADC si les capteurs IR ne sont pas installés.
Un circuit MCP23017 donne 8 lignes IO, les premières 8 lignes sont utilisée pour intercepter les interruptions des divers circuits de la carte:

