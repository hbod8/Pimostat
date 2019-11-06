# Pimostat
A Raspberry Pi thermostat system with multiple node capability.

## Goals
- Create a system where homes with electric in-wall heating can conserve more energy by having a central control and nodes for each room.
- Allow users to control their thermostat from anywhere.
- Allow scheduling of heat.
- Allow users to enable location sharing to conserve energy when they are not home.
- Make sure a room isnt loosing heat too fast. (case: someone leaves their window open and the heater runs continuously)
- Estimate heating bill based on usage.
- Flag users/rooms that use a lot of energy.
- Suggest changes to habits to improve energy usage.
- Make sure pipes dont freeze by allowing a minimum heat setting.
- Also allow for single node-cabability.
- Installer!

## Implementation

Control Pi:

 ----------------         ----------------         ---------------- 
| Apache Web     |       | NODE REST      |       | Database       |
| Server         | ----> | API +          | ----> |                |
|                |       | Sensor         |       |                |
 ----------------         ----------------         ---------------- 

                                 |
                                 |
                                 |
                                 |
                                 v
Node Pi:
                          ----------------         ---------------- 
                         | NODE REST      |       | Database       |
                         | API +          | ----> |                |
                         | Sensor         |       |                |
                          ----------------         ---------------- 

## Disclaimer

There are two other projects with the same name, one is very old and written in python, the other also uses NODE.js.

[Synthead's Python based Pimostat](https://github.com/synthead/pimostat)
[Gilmtz's Python/NODE/Android App - see note](https://github.com/gilmtz/Pimostat)

*NOTE: gilmtz's repository doesnt have a working version, after reading through it seems they purchased a nest and lost intrest.*
