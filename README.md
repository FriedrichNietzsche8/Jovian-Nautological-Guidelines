# Jovian Nautological Guidelines
## Signal Communication Standard
Inspired by Earth's COLREGs ([International Regulations for Preventing Collisions at Sea](https://en.wikipedia.org/wiki/International_Regulations_for_Preventing_Collisions_at_Sea)), these signals are used to discern the type and movement of a ship to avoid collision with other ships.
***
### Identification Signal
*Used to identify the type of the ship. Usually located at the top, between the aft and starboard.*
#### Required
Type|RGB
-|-
Attack|`255 0 0`
Transport|`0 255 0`
Scout|`0 0 255`
Shuttle|`0 255 255`
Drone|`255 255 0`
#### Recommended
Ship|Alpha|Range
-|-|-
Submarine|`127`|`256`
Submersible|`63`|`128`

#### Example
<img width="512" height="256" alt="IS" src="https://github.com/user-attachments/assets/76a7a972-4ccb-4192-be9b-bb04590f544a"/>

***
### Location Signals
*Used to discern the location of the bow and aft.*
#### Required
Location|RGB|Blink Frequency
-|-|-
Bow|`0 255 0`|`0.2`
Aft|`255 0 0`|`0.2`
#### Recommended
Ship|Alpha|Range
-|-|-
Submarine|`127`|`128`
Submersible|`63`|`64`

Large Ship|Aft|Bow
-|-|-
Top|`3`|`3`|
Bottom|`2`|`2`|

Medium Ship|Aft|Bow
-|-|-
Top|`2`|`2`|
Bottom|`1`|`1`|

Small Ship|Aft|Bow
-|-|-
Top|`1`|`1`|
Bottom|`1`|`1`|

#### Example
<img width="512" height="256" alt="LS" src="https://github.com/user-attachments/assets/f40cfce5-0e41-48e7-bd16-2557b0e23477"/>

***
### Condition Signals
*Used to discern the movement of the ship.*
#### Required
RGB
-|
`255 255 255`

Condition|Top Light|Bottom Light
-|-|-
Stationary|✓|✓
Forwards|✓|✗
Backwards|✗|✓
#### Recommended
Ship|Alpha|Range
-|-|-
Submarine|`127`|`256`
Submersible|`63`|`128`

Large Ship|Starboard
-|-
Top|`2`
Bottom|`2`|

Small & Medium Ship|Starboard
-|-
Top|`1`
Bottom|`1`|

#### Example
<img width="512" height="256" alt="CS" src="https://github.com/user-attachments/assets/2c902f05-44c4-43ba-85e9-0ad474407a7e"/>

***
## External Indication Standard
Color-coded pulsating lights, these indicators are used to assist the diving crew as a warning for hazards such as the dangerous machinery and weaponry of a ship, or to discern the location of an airlock.

Unlike the **SCS**, the restrictions of the **EIS** are more relaxed and can be fully modified pership. Subwrights are required to disclose all modifications of the **EIS** to the submarine crew to avoid confusion.
Indicator|Airlock Open|Airlock Closed
-|-|-
Electrical Discharge Coil|✓|✗
Engine Propeller|✓|✗
Depth Charge Tube|✓|✗
Docking Port|✓|✓
Airlock|✓|✗
Airdock|✓|✓
***
### Hazards
#### Electrical Discharge Coil Indicator
*Used as a hazard indicator for the Electrical Discharge Coil.*
RGBA|Range|Pulse Amount|Pulse Frequency
-|-|-|-
`255 255 0 127`|`256`|`0.75`|`0.1`
#### Engine Propeller Indicator
*Used as a hazard indicator for the Engine Propeller.*
RGBA|Range|Pulse Amount|Pulse Frequency
-|-|-|-
`255 127 0 127`|`256`|`0.75`|`0.1`
#### Depth Charge Tube Indicator
*Used as a hazard indicator for the Depth Charge Tube.*
RGBA|Range|Pulse Amount|Pulse Frequency
-|-|-|-
`127 255 0 127`|`256`|`0.75`|`0.1`
***
### Notices
#### Docking Port Indicator
*Used to indicate the location of a Docking Port.*
RGBA|Range|Pulse Amount|Pulse Frequency
-|-|-|-
`0 255 255 127`|`128`|`0.5`|`0.2`
#### Airlock Indicator
*Used to indicate the location of an Airlock.*
RGBA|Range|Blink Frequency
-|-|-
`0 127 255 127`|`128`|`0.8`
#### Airdock Indicator
*Used to indicate the location of an Airdock.*
RGBA|Range|Pulse Amount|Pulse Frequency
-|-|-|-
`0 255 127 127`|`128`|`0.5`|`0.2`
***
## Credits
By: ***Friedrich Nietzsche***

### Notable Persons:  
*Anonority*  
*Azekill_DIABLO*  
*Clavicus*  
*GM6*
