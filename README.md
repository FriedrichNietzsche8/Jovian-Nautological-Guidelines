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
Top|`3`|`3`|
Bottom|`2`|`2`|

Medium Sub|Aft|Bow
-|-|-
Top|`2`|`2`|
Bottom|`1`|`1`|

Small Sub|Aft|Bow
-|-|-
Top|`1`|`1`|
Bottom|`1`|`1`|
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
Top|`2`
Bottom|`2`|

Small & Medium Sub|Starboard
-|-
Top|`1`
Bottom|`1`|
#### Example
<img width="512" height="256" alt="CS" src="https://github.com/user-attachments/assets/2c902f05-44c4-43ba-85e9-0ad474407a7e"/>

***
## External Indication Standard
Color-coded pulsating indicators used to assist the diving crew as a warning for hazards such as the dangerous machinery and weaponry of a sub, or to discern the location of an airlock.

Unlike the **SCS**, the restrictions of the **EIS** are more relaxed and can be fully modified persub. Subwrights are required to disclose all modifications of the **EIS** to the sub's crew to avoid confusion.
***
Indicator|RGBA|Range|Blink F|Pulse A|Pulse F|Closed Airlock
-|-|-|-|-|-|-
Electrical Discharge Coil|`255 255 0 127`|`256`|-|`0.75`|`0.1`|Off
Engine Propeller|`255 127 0 127`|`256`|-|`0.75`|`0.1`|Off
Depth Charge Tube|`127 255 0 127`|`256`|-|`0.75`|`0.1`|Off
Docking Port|`0 255 255 127`|`128`|-|`0.5`|`0.2`|On
Airlock|`0 127 255 127`|`128`|`0.8`|-|-|Off
Airdock|`0 255 127 127`|`128`|-|`0.5`|`0.2`|On
#### Example
<img width="512" height="256" alt="EIS" src="https://github.com/user-attachments/assets/1f9e4288-2788-4cf3-9973-e9625eb331cd"/>

***
## Credits
By: ***Friedrich Nietzsche***

### Notable Persons:  
*Anonority*  
*Azekill_DIABLO*  
*Clavicus*  
*GM6*
