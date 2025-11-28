# Jovian Nautological Guidelines
## Signal Communication Standard
Modified COLREGS (*International Regulations for Preventing Collisions at Sea*) to better fit Europan ships, these signals are used to discern the type and movement of a ship to avoid collision with other ships.
### Identification Signal
*Used to identify the type of the ship.*
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
Amount|Location
-|-
1|Top of the Ship, between the Starboard and Aft
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
Size|Top Bow|Top Aft|Bottom Bow|Bottom Aft
-|-|-|-|-|
Large Ship|`3`|`3`|`2`|`2`
Medium Ship|`2`|`2`|`1`|`1`
Small Ship|`1`|`1`|`1`|`1`
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
## Credits
By: ***Friedrich Nietzsche***

Notable Persons:  
*Anonority*  
*Azekill_DIABLO*  
*Clavicus*  
*GM6*