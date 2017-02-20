# Home automation to-do list

Fixes:

* ~~office door sensor~~
* power monitoring - fix battery
* power shouldn't set a persistant value
* ~~Shed door contact reporting~~

Containerization:

* Home Assistant
 * remove old install and boot files
 * fix up ansible
* AAISP MQTT service

Automations:

* All outdoor lights switch off at 10pm, switch to override
* ~~Switch on shed inside light when the door opens~~
* Notify if the workshop or shed doors are open after 9pm [source](https://github.com/dale3h/homeassistant-config-1/blob/master/automation/notify_garage_open_2100.yaml)
* Notify if any doors are open for over 10 minutes [source](https://github.com/dale3h/homeassistant-config-1/blob/master/automation/notify_doors_left_open.yaml)
* ~~Barn Christmas lights should turn on automatically between mid November and Jan 6th each night~~ [commit](https://github.com/natm/homeassistant-config/commit/9882f46f6a4bbb019cee2fed34506e198c611be7) (still need to add dates)

Notifications:

* ~~add home slack to our phones~~
* ~~notify on incoming and outgoing calls to slack~~
* ~~notify when workshop doors open and close~~
* ~~notify when shed doors open and close~~
* include cctv captures in workshop and shed slack messages

Security:

* Alerting if outdoor doors open at night
* Post CCTV GIFs to slack when doors open

Improvements:

* ~~Clean up default_view~~

New integrations:

* https://home-assistant.io/components/sensor.google_travel_time/
* Amazon echo dot
* [Current transformers](http://www.ebay.co.uk/itm/331978579185) on all henley blocks - using [OpenEnergyMonitor circuit](https://openenergymonitor.org/emon/buildingblocks/how-to-build-an-arduino-energy-monitor) with AT328 + ESP8266-201
* Make owntracks work for both of us
* Track locations of both vehicles
* Send ODB2 data from cars to MQTT (HA+Munin)
* Downstream internet current usage for neighbors (SNMP from Edgerouter-X)
* New daemon to archive CCTV JPEGs for timelapse to remote object store
* Graphing DIN ammeters in shed and barn (need pulse counting)
* MQTT temperature and humidity munin plugin (from roomsensors)
* ~~CurrentCost to MQTT via ESP~~ [commit](https://github.com/natm/homeassistant-config/commit/1d9e7286e50cecd35e420fb48b9d06e1db5952e8) [esp8266-201 sketch](https://gist.github.com/natm/d47d8d86f900030295d55ac90aeee320)
* ~~Honeywell evohome~~ [commit](https://github.com/natm/homeassistant-config/commit/133bd98b465d14643fb3e2ec215cff82aadd7297)
* ~~Write a daemon to grab AAISP quota + sync rates and send it to MQTT~~ see: [aaisp-to-mqtt](https://github.com/natm/aaisp-to-mqtt)
* ~~Display current down/upstream usage in mbit for each FTTC line~~ [commit](https://github.com/natm/homeassistant-config/commit/e16f9f23cc5b0f457b8bbdffca04312fef566708)
