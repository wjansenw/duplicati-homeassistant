duplicati-nodered-homeassistant
===============================

Expose duplicati to homeassistant via nodered/mqtt.
You need to have a working mqtt broker, homeassistant configured correctly to work with this broker and accept discovery of new devices.

Configuration can be done by a yaml file. In the current flow, this file is to be stored on 
 cat duplicati_config.yaml
```
nodered:$ pwd
/data/duplicati

nodered:$ cat duplicati_config.yaml
duplicatiservers:
  - IP: "192.168.0.1"
    port: 8200
  - IP: "192.168.0.2"
    port: 8200
mqtt:
  broker: 192.168.0.3
  port: 1883
  username: mosquitto
  password: mosquitto
```
### About

This is your project's README.md file. It helps users understand what your
project does, how to use it and anything else they may need to know.