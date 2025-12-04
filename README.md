# Jovian Nautological Guidelines
## Signal Communication Standard
Inspired by Earth's COLREGs ([International Regulations for Preventing Collisions at Sea](https://en.wikipedia.org/wiki/International_Regulations_for_Preventing_Collisions_at_Sea)), these signals are used to discern the type and movement of a sub to avoid collision with other subs.
***
### Identification Signal
*Used to identify the type of the sub. Usually located at the top, between the aft and starboard.*
#### Required
Type|RGB
-|-
Attack|`255 0 0`
Transport|`0 255 0`
Scout|`0 0 255`
Shuttle|`0 255 255`
Drone|`255 255 0`
#### Recommended
Sub|Alpha|Range
-|-|-
Submarine|`127`|`256`
Submersible|`63`|`128`
#### Example
<img width="512" height="256" alt="IS" src="https://github.com/user-attachments/assets/76a7a972-4ccb-4192-be9b-bb04590f544a"/>

***
### Location Signals
*Used to discern the location of the bow and aft.*
#### Required
Location|RGB|Blink F
-|-|-
Bow|`0 255 0`|`0.2`
Aft|`255 0 0`|`0.2`
#### Recommended
Sub|Alpha|Range
-|-|-
Submarine|`127`|`128`
Submersible|`63`|`64`

Large Sub|Aft|Bow
-|-|-
Top|3|3|
Bottom|2|2|

Medium Sub|Aft|Bow
-|-|-
Top|2|2|
Bottom|1|1|

Small Sub|Aft|Bow
-|-|-
Top|1|1|
Bottom|1|1|
#### Example
<img width="512" height="256" alt="LS" src="https://github.com/user-attachments/assets/f40cfce5-0e41-48e7-bd16-2557b0e23477"/>

***
### Condition Signals
*Used to discern the movement of the sub.*
#### Required
RGB
-|
`255 255 255`

Movement|Top Signal|Bottom Signal
-|-|-
Stationary|On|On
Forward|On|Off
Backward|Off|On
#### Recommended
Sub|Alpha|Range
-|-|-
Submarine|`127`|`256`
Submersible|`63`|`128`

Large Sub|Starboard
-|-
Top|2
Bottom|2

Small & Medium Sub|Starboard
-|-
Top|1
Bottom|1
#### Example
<img width="512" height="256" alt="CS" src="https://github.com/user-attachments/assets/2c902f05-44c4-43ba-85e9-0ad474407a7e"/>

***
## External Indication Standard (WIP)
Color-coded pulsating indicators used to assist the diving crew as a warning for hazards such as the dangerous machinery and weaponry of a sub, or to discern the location of an airlock.

Unlike the **SCS**, the restrictions of the **EIS** are more relaxed and can be fully modified persub. Subwrights are required to disclose all modifications of the **EIS** to the sub's crew to avoid confusion.
***
### Hazards
Alpha|Range|Pulse A|Pulse F|Closed Airlock
-|-|-|-|-
`127`|`256`|`0.75`|`0.1`|Off
#### Electrical Discharge Coil Indicator
*Used as a hazard indicator for the Electrical Discharge Coil.*
RGB
-|
`255 255 0`
#### Engine Propeller Indicator
*Used as a hazard indicator for the Engine Propeller.*
RGB
-|
`255 127 0`
#### Depth Charge Tube Indicator
*Used as a hazard indicator for the Depth Charge Tube.*
RGB
-|
`127 255 0`
#### Example
<img width="512" height="256" alt="H" src="https://github.com/user-attachments/assets/38c52ca3-3a65-44ee-a42d-0b93d72d90d9"/>

***
### Notices
Alpha|Range
-|-
`127`|`128`
#### Docking Port Indicator
*Used to indicate the location of a Docking Port. The indicators turn off once docked.*
##### Undocked
RGB|Pulse A|Pulse F|Closed Airlock
-|-|-|-
`0 255 255`|`0.5`|`0.2`|On
##### Proximity
RGB|Blink F
-|-
`0 255 0`|`1.0`
#### Airlock Indicator
*Used to indicate the location of an Airlock.*
RGB|Blink F|Closed Airlock
-|-|-
`0 127 255`|`0.8`|Off
#### Airdock Indicator
*Used to indicate the location of an Airdock.*
RGB|Pulse A|Pulse F|Closed Airlock
-|-|-|-
`0 255 127`|`0.5`|`0.2`|On
#### Example
<img width="512" height="256" alt="N" src="https://github.com/user-attachments/assets/344edce2-d15a-4abe-a05d-c1d97a2cec6e"/>

***
## Internal Indication Standard (WIP)
Color-coded alarms.
***
Alarm|RGB
-|-
Meltdown|`255 0 0`
Fire|`255 255 0`
Flood|`0 0 255`
Oxygen|`0 255 255`
EDC|`255 127 0`

Notifier|RGB
-|-
Battery|`0 255 0`
Airlock|`0 127 255`

Alpha
-|
`127`
***
## Credits
By: ***Friedrich Nietzsche***

### Notable Persons:  
*Anonority*  
*Azekill_DIABLO*  
*Clavicus*  
*GM6*
