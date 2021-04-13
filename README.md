# marlinEnder3
This repository hosts my Marlin configuration.

My Ender 3 is basically stock: the only modification I made is to change the MELZI board with an SKR 1.4 Turbo with TMC 2209 drivers on every axis.

***Based on Marlin version:***
***2.0.7.2***

**Sensorless homing is not enabled**

Feel free to use this with your printer if you are having trouble configuring Marlin by yourself.

**Known issues:**
1. When doing manual bed levelling, the bottom part of the text is cut off when changing probing points.

## Full list of features enabled or disabled:

### Configuration.h

1. Mesh bed Levelling (Manual, not ABL)
1. Home axis indipendently
1. Power outage (you have to enable it by yourself through the menu)
1. Normal Ender 3 bootscreen
1. Custom Statusscreen
1. Added PID menu to tune and save hotend PID data (the values present in configuration.h are the ones I use, but you should [tune your hotend yourself](https://reprap.org/wiki/PID_Tuning))
1. Removed the preheat ABS menu item
1. SD card support
1. CRC checks on SD card
1. CR10 display (stock Ender 3 display)

### Configuration_adv.h

1. Scroll long filenames
1. Babystepping + Double click while printing to babystep
1. Display total babysteps
1. Improve homing reliability
1. TMC debug
1. Info menu
1. Status message scrolling
