Lovelace cards configuration to display solaradge  https://github.com/WillCodeForCats/solaredge-modbus-multi  HACS integration.

Require: 
https://github.com/flixlix/power-flow-card-plus

https://github.com/RomRider/apexcharts-card


Sample:

![image](https://github.com/IvanM73/solaredge-lovelace-cards/assets/1104454/588bc904-4a31-4905-95a8-f9b1a109f9f6)






In the repo:
energy.yaml               : provide all sensort and templates needed for data calculation.
power-flow-card-plus.yaml : define a new card with instant and daily consumption for SOLAR/GRID/HOME/BATTERY. require https://github.com/flixlix/power-flow-card-plus
apexcharts-card.yaml      : define daily production/consumtion graphs require https://github.com/RomRider/apexcharts-card


HOW TO INSTALL: 
- install https://github.com/WillCodeForCats/solaredge-modbus-multi  HACS, modbus need tio
inlcude energy.yaml it in your package dir and be sure below configuration is present in your configuration.yaml
_homeassistant:  
packages: !include_dir_named packages
_
- create two new lovelace cards pasting power-flow-card-plus.yaml and apexcharts-card.yaml

Enjoy!!!!


