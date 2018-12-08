# MQ9 sensor module for ESP8266
The module is designed to work with the MQ9 sensor in the MicroPython language on ESP8266 (NodeMCU) the Sensor is connected to the analog output on the ADC (A0) ESP8266

The library is implemented on the basis of code https://github.com/tutRPi/Raspberry-Pi-Gas-Sensor-MQ

# Модуль датчика MQ9 для ESP8266
Модуль предназначается для работы с датчиком MQ9 на языке MicroPython на ESP8266 (NodeMCU)
Датчик подключается аналоговым выходом на ADC (A0) ESP8266

Библиотека реализована на основе кода https://github.com/tutRPi/Raspberry-Pi-Gas-Sensor-MQ

## Пример использования (Example of use)
````
from mq9 import MQ
mq = MQ()
perc = mq.MQPercentage()
print("LPG: %g ppm, CO: %g ppm, Smoke: %g ppm" % (perc["GAS_LPG"], perc["CO"], perc["SMOKE"]))
````

  
