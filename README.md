Solaredge cards using data from  https://github.com/WillCodeForCats/solaredge-modbus-multi  HACS.

energy.yaml               : provide all sensort and templates needed for data calculation.
power-flow-card-plus.yaml : define a new card with instant and daily consumption for SOLAR/GRID/HOME/BATTERY. require https://github.com/flixlix/power-flow-card-plus
apexcharts-card.yaml      : define daily production/consumtion


HOW TO INSTALL: 
- install https://github.com/WillCodeForCats/solaredge-modbus-multi  HACS, modbus need tio
inlcude energy.yaml it in your package dir and be sure below configuration is present in your configuration.yaml
_homeassistant:  
packages: !include_dir_named packages
_
- create two new lovelace cards pasting power-flow-card-plus.yaml and apexcharts-card.yaml 
