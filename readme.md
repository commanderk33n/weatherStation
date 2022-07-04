# Weather Station NodeMCU

#### Usage:

after checkout:

- Download Arduino IDE
- Download ESP8266 Development Board and Driver File:
    - File->Preferences 'Additional Boards Manager URLs:
      - http://arduino.esp8266.com/stable/package_esp8266com_index.json
    - Download esp8266 with Boards Manager
- Install Libaries:
    - esp8266 weather
    - JSON Streaming
    - adafruit bme280
    - adafruit Unified sensor
    - oled lib from NodeMCU/lib
- Add your WIFI, Webserver and Database-Server info into weatherSationKeen.ino, esp-chart.php and post-data.php

#### Hardware used:
- NodeMCU ESP8266 (CP2102)
- GY-BME280 Sensormodul
- OLED-Display (SSH1106)
- RaspberryPi for Webserver (Nginx, MariaDB, PHP)

#### Pin Connection:
- NodeMCU ESP8266 <-----> OLED
    - 3.3V---VCC
    - GND---GND
    - D1---SCL
    - D2---SDA
- NodeMCU ESP8266<-----> BME280
    - 3.3V---VCC
    - GND---GND
    - D1---SCL
    - D2---SDA