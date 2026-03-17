# What´s in this repo
This repository is a collection of useful additions to the wonderful [RoomMind](https://github.com/snazzybean/roommind) integration for HomeAssistant.

## Central heating and cooling systems without area controls
Currently when using a central heating and/or cooling system without native controls for individual rooms that was extended with TRVs for the rooms to add that functionality there is no RoomMind-native support for controlling the central system.
The following blueprint offers an easy solution to perform any action (generic or specific to your system) based on heating/cooling/idle-states of roomminds mode entities.
This Blueprint can trigger actions/scripts if
- all rooms are idle
- any room is heating, but no room is cooling
- any room is cooling, but no room is heating
- at least one room is heating and at least one room is cooling

The last option is useful to implement error handling if necessary for your system.

You can either view the blueprint [here](https://github.com/hecktech27/roommind_tools/blob/main/Blueprints/roommind_central_heating_cooling.yaml) or directly import it into your homeassistant instance by clicking 
[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fhecktech27%2Froommind_tools%2Fblob%2Fmain%2FBlueprints%2Froommind_central_heating_cooling.yaml)

#### Disclosure:
This blueprint was initially created using AI but manually reviewed and adjusted.
