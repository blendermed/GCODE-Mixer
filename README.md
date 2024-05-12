# GCODE-Mixer
Java script based tool which stiches multiple gcodes.

There are some settings to customize stiching procedure:

## Repeats: 
Defines the number of itterations of asingle gcode

## Remove: 
Removes the GCODE from the list

## Add file: 
Adds another row to the GCODEs list

## Custom clearing gcode:
Following GCODE lines will be added after each GCODE file and its iterations. This code can be used to specify the clearing procedure or left empty if you alreaty added clearing GCODE in slicers end-gcode."

## Advanced option ... 
This opens an additional section where more details can be specified...

## Prequel GCODE:
Following lines will be added at the very beginning of the generated GCODE file. 

## Deactivate folowing lines in ALL GCODEs:
Following code pieces will be turned into comment (means deactivated) in each GCODE file and its iterations. Each line is handled separately - means the app will seach for appearence of each single line and not for a specific block. This can be usaful to disable some specific GCODE lines like "diasble steppers" or prevent the nozzle from dropping the temperature during removing process if desired.


## Deactivate folowing lines in ALL GCODEs but NOT in FIRST:
...just like before, but the changes will not be applied to the very FIRST gcode or its itteration. This can be used to deactivate some preparation routines like leveling and other calibrations which needs to be done only once. 

## Deactivate folowing lines in ALL GCODEs but NOT in LAST:
...just like before, but the changes will not be applied to the very LAST gcode or its itteration. 

## Sequel GCODE:
Following lines will be added at the very end of the generated GCODE file.
