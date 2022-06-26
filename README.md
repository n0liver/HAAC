# Homeassistant APSystems API Client

A custom integration that uses the APSsystems app's API to read solar panel data.


## Installation
__full manual:__
- download the code
- move the HAAC folder into your custom_components folder in HASS's config directory
- restart


__HACS custom repository:__
- add in HACS this repository: https://github.com/n0liver/HAAC
- choose as category type "integration"
- the integration should appear and can be installed as any other HACS integration


## Configuration
This application uses the same API as the app from APSystems, and thus needs the same login credentials as the application.
- Add the integration via settings > integrations
- enter your username and password
- done!


## Available sensors
| Name | description | unit |
|---|---|---|
| CO2 reduced (today) | Today's amount of CO2 that would have been produced if the energy was consumed from the grid | kg |
| CO2 reduced in lifetime | Lifetime amount of CO2 that would have been produced if the energy was consumed from the grid | kg |
| Current power generation | Amount of power currently generated | Watts |
| Energy generated in lifetime | Amount of energy generated since APS is monitoring your panels | kwh |
| Energy generated this month | Amount of energy generated since the 1st of this month | kwh |
| Energy generated this year | Emaount of energy generated since 1 january this year | kwh |
| Energy generated today | Amount of energy generated today | kwh |
| System capacity | Maximum power capacity of the system (power production can exceed this!) | watts |
| Trees saved | 1 tree consumes 20 kg of CO2/year. This number shows how much "tree-years" of co2 reduction your panels have produced | trees 🌲 |