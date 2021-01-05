# Terneo Thermostat
Terneo Thermostat component for Home Assistant

required device firmware version 2.3

https://terneo-api.readthedocs.io/ru/latest/

>In firmware version 2.3, the ability to control the local network by default blocked for security reasons.

block removing - https://terneo-api.readthedocs.io/ru/latest/en/safety.html

Manual block removing (simple) - OFF blocking on device (Depend from your device version, see manual instruction on terneo.ua):
Menu BLc change LAn,on,cld ->> oFF

put `terneo` folder to the `custom_components`

config example (`configuration.yaml`):

serial number can be found on the page  http://`{device_ip}`/index.html

```
climate:
  - platform: terneo
    serial: 'DEVICE_SERIALNUMBER'
    host: 'DEVICE_IP'
```
