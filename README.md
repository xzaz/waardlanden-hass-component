# Home Assistant waardlanden component
Integration for bin/waste collection  by WaardLanden

Reinigingsdienst Waardlanden is de reinigingsdienst voor de gemeenten Gorinchem, Hardinxveld-Giessendam, Molenlanden en Vijfheerenlanden

Add the following to your sensor yaml and change the postcode and house number to whats applicable to yours.
 ```yaml
 - platform: acv
   postcode: 6861GG
   housenumber: 4
   resources:
     - today
     - tomorrow
     - grey
     - green
     - paper
     - packages
     - textile
 ```
###### Original Author: @vloris (Floris Kruisselbrink)
###### Modification for acv-groep by: Cadster
###### Modification for new api address by: aritmeester
###### Modification for waardlanden by: M11tch
