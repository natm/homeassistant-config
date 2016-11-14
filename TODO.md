# Home automation to-do list

Fixes:

* Shed door contact reporting

Automations:

* Barn christmas lights should turn on automatically between mid November and Jan 6th each night
* All outdoor lights switch off at 10pm, switch to override
* Switch on shed inside light when the door opens

Security:

* Alerting if outdoor doors open at night

Improvements:

* Clean up default_view

New integrations:

* Amazon echo dot
* Honeywell evohome
* Write a daemon to grab AAISP quota + sync rates and send it to MQTT
* CurrentCost to MQTT via ESP8266-201
* Make owntracks work for both of us
* Track locations of both vehicles
* Send ODB2 data from cars to MQTT (HA+Munin)
* Display current down/upstream usage in mbit for each FTTC line
* Downstream current usage for neighbors
* New daemon to archive CCTV JPEGs for timelapse to remote object store
* Graphing DIN ammeters in shed and barn (need pulse counting)
* MQTT temperature and humidity munin plugin (from roomsensors)
