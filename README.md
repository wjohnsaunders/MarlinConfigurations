# MarlinConfigurations

## Ender-3 Configuration

Ender-3 V1 with Creality BLTouch kit and CR-10S controller board (for the bigger microcontroller).

## TwoTrees SP-5 Configuration Sets

TwoTrees SP-5 that has been highly modified. Several configs exist

###Sapphire Plus V2

Standard components build with the standard Marlin UI.

###Sapphire Plus V2 MKS UI

Standard components build with the MKS UI as the machine originally ships.

###Sapphire Plus V2 BLTouch

Addition of a BLTouch and does Z stepper alignment with the probe (no belt on my model).

###Sapphire Plus V2 BLTouch TMC_UART

Addition of a BLTouch and does Z stepper alignment with the probe (no belt on my model).
Also TMC2209 stepper drivers have been added to the MKS Robin Nano V1.2 and using the
WiFi port to access the TMC UART on the steppers to allow current and mode to be changed
via the UI.
