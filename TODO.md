# Home automation to-do list

Fixes:

* Shed door contact reporting

Automations:

* Barn Christmas lights should turn on automatically between mid November and Jan 6th each night
* All outdoor lights switch off at 10pm, switch to override
* Switch on shed inside light when the door opens
* Notify if the workshop or shed doors are open after 9pm [source](https://github.com/dale3h/homeassistant-config-1/blob/master/automation/notify_garage_open_2100.yaml)
* Notify if any doors are open for over 10 minutes [source](https://github.com/dale3h/homeassistant-config-1/blob/master/automation/notify_doors_left_open.yaml)

Notifications:

* Work out which push service to use for our Android phones

Security:

* Alerting if outdoor doors open at night

Improvements:

* Clean up default_view

New integrations:

* Amazon echo dot
* Honeywell evohome
* CurrentCost to MQTT via ESP8266-201
* [Current transformers](http://www.ebay.co.uk/itm/331978579185) on all henley blocks - using [OpenEnergyMonitor circuit](https://openenergymonitor.org/emon/buildingblocks/how-to-build-an-arduino-energy-monitor) with AT328 + ESP8266-201
* Make owntracks work for both of us
* Track locations of both vehicles
* Send ODB2 data from cars to MQTT (HA+Munin)
* Downstream internet current usage for neighbors (SNMP from Edgerouter-X)
* New daemon to archive CCTV JPEGs for timelapse to remote object store
* Graphing DIN ammeters in shed and barn (need pulse counting)
* MQTT temperature and humidity munin plugin (from roomsensors)
* ~~Write a daemon to grab AAISP quota + sync rates and send it to MQTT~~ see: [aaisp-to-mqtt](https://github.com/natm/aaisp-to-mqtt)
* ~~Display current down/upstream usage in mbit for each FTTC line~~
