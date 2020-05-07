# Home Assistant waardlanden component
Integration for bin/waste collection with the ximmio API

Add the following to your sensor yaml and change the postcode, house number and companycode to whats applicable to yours.
 ```yaml
 - platform: waardlanden
   postcode: 6861GG
   housenumber: 4
   companycode: adc418da-d19b-11e5-ab30-625662870761
   resources:
     - today
     - tomorrow
     - grey
     - green
     - paper
     - plastic
     - textile
 ```
 
The companyid can be retrieved by the collector (such as AREA) with the POST header.
###### Original Author: @vloris (Floris Kruisselbrink)
###### Modification for acv-groep by: Cadster
###### Modification for new api address by: aritmeester
###### Modification for waardlanden by: M11tch
