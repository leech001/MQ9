# Модуль датчика MQ9 для ESP8266
Модуль предназначается для работы с датчиком MQ9 на языке MicroPython на ESP8266 (NodeMCU)
Датчик подключается аналоговым выходом на ADC (A0) ESP8266

Библиотека реализована на основе кода https://github.com/tutRPi/Raspberry-Pi-Gas-Sensor-MQ

##Пример использования
````
from mq9 import MQ
mq = MQ()
perc = mq.MQPercentage()
print("LPG: %g ppm, CO: %g ppm, Smoke: %g ppm" % (perc["GAS_LPG"], perc["CO"], perc["SMOKE"]))
````

  
