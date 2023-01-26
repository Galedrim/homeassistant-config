
# Galedrim's Home Assistant config files

Using Mushroom Cards/Themes with Mansory (Layout-card) on a vertical android tablet.


Home           |  Vacuum Map
:-------------------------:|:-------------------------:
![image](https://user-images.githubusercontent.com/84284891/214948895-a15e4ac6-9fb2-41cc-bc5d-f6e34a2adbc5.png) |  ![image](https://user-images.githubusercontent.com/84284891/214948917-fbe245bd-f910-44f0-9f31-2564ebc6ce1f.png)

## My devices

|   Switches   |   Units  |  Used  |
|---  |---   |:-:    
|   TP-Link HS110  |  1  | Turn on/off PC |
|   TP-Link HS100  |  1  | Turn on/off google mini |
|   Switchbot Bot  |  1  | Turn on/off coffee maker |

|   Sensors   |  Units  |  Used  |
|---  |---   |:-:    
|   Xiaomi Mi Flora  |  1  | Get information about a sensitive plant  |
|   Switchbot Meter Plus  |  1  | Get temperature and humidity in home |
|   Switchbot Motion Sensor  |  1  | Get information that i woke up |
|   Switchbot Contact Sensor  |  1  | Get state of the front door (Open/Closed)  |

|   Lights  |   Units  | 
|---    |:-:    
|   Philips Hue E27 White and Color  |  2  |
|   Philips Hue LED strip 2m  |  1  |

|   Hubs  |   Units  | 
|---    |:-:    
|   Switchbot Hub Mini  |  1  |
|   Phillips Hub Bridge  |  1  |

|   Equipements |   Units  |   Used  |
|---  |---   |:-:    
|   OnePlus 6 |  1  | Get information when i leave or return home |
|   Google Mini  |  1  | Use only as an alarm clock |
|   TV Philips Ambilight  |  1  | A TV with multicolored lights |
|   Xiaomi Mi Roborock V1  |  1  | A broom with wheels and a voice |

|   Server  |   Units  | 
|---    |:-:    
|   Raspberry Pi 3, 1GB RAM  |  1  |

## Add-ons (Supervised Install Only)

* SSH & Web Terminal
* Studio Code Server

## Integratiom HACS

* Clock weather card
* Layout-card
* Mushroom
* Mushroom theme

* Xiaomi Cloud Map Extractor
* Xiaomi Vacuum Map Card

Note : To obtain the coordinates of a cleaning zone for the vacuum, create the zone on the map then hold down the "Clean zone" button, a pop-up will appear with the desired information.


## Automations

### Switches & Lights

* Switches : Journey start :
    * Turn on coffee maker
    * Turn on PC (Start after power on in BIOS)
    * Stop Google Mini player (Google routine play YT Playlist as alarm clock)
    * Turn on light if sun below horizon
* Switches : Turn on coffee maker when back to home
* Switches : Turn off PC when power consumption is low
* Switches : Reset variables at 07:00

### Vacuum

* Vacuum : Cleaning when not home
* Vacuum : Cleaning done
* Vacuum : Reset variables at 0:00

### Variables
* Plant : Increment a variable at 0:00. Variable is used to determine the number of days without watering plant.
* Vacation mode : Turn on when not home for 24h
* Vacation mode : Turn off when home
