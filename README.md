# Home Assistant ximmio component
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

Different municapilities i gathered from the forks and more information on the web.


| Gemeente  | Companycode | Service provider |
| ------------- | ------------- |------------- |
| Nissewaard  | 9dc25c8a-175a-4a41-b7a1-83f237a80b77 | |
| Emmen  | adc418da-d19b-11e5-ab30-625662870761 | AREA |
| Gorinchem | 942abcf6-3775-400d-ae5d-7380d728b23c | WaardLanden |
| Hardinxveld-Giessendam | 942abcf6-3775-400d-ae5d-7380d728b23c | WaardLanden |
| Molenlanden | 942abcf6-3775-400d-ae5d-7380d728b23c | WaardLanden |
| Vijfheerenlanden | 942abcf6-3775-400d-ae5d-7380d728b23c | WaardLanden |

###### Original Author: @vloris (Floris Kruisselbrink)
###### Modification for acv-groep by: Cadster
###### Modification for new api address by: aritmeester
###### Modification for waardlanden by: M11tch
