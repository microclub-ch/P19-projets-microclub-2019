# projets-microclub-2019
Platforme robotique, domotique et plus basée ESP32

### Présentation du 26.1.2019 à l'EPFL: [lien vers la présentation]

[lien vers la présentation]: https://microclub.ch/wp-content/uploads/2019/01/Project-2019.pdf

[livre]: https://leanpub.com/kolban-ESP32

Livre electronique: [livre]

## Outil de développement actuel (pour avr, ESP8266, ESP32) 

PlatformIO, Une amélioration importante par rapport à Arduino IDE: [Platformio] !! attention, ne pas installer la version ATOM !
Permet d'utiliser toutes les librairies Arduino, Adafruit etc.

[Platformio]: https://code.visualstudio.com/

Nouveau sur la version Split, 2 connecteurs pour des capteurs Time of Flight type  GY-53 VL53L0X ou VL53L1X permettant de mesurer avec précision des distances de 2 ou 4m !!! en plus un connecteur pour utiliser le convertisseur ADC si les capteurs IR ne sont pas installés.
Un circuit MCP23017 donne 8 lignes IO, les premières 8 lignes sont utilisée pour intercepter les interruptions des divers circuits de la carte:

