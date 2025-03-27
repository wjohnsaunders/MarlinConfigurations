# Ender-3 with a CR-10S board

This config is for the Ender-3 modified with the Creality BLTouch kit and
a control board from a CR-10S V2.1. However it retains the original Ender-3
LCD and not the CR-10S LCD which is different. I wanted the expanded memory
of the ATmega2560, and the CR10-S control board goes into an Ender-3 with the
SDCard and USB ports lining up with the original board.

## Enabled features

It is a mis-mash of the Ender-3 V1 and CR10-S Marlin configurations. The control
board settings for the CR-10S and combined with the kinematics settings from the
Ender-3.

BLTouch probing is enabled and configured for the Creality BLTouch kit and
mounting bracket. The Z height configured in the firmware should get you in
the ball park. The outer probe points are positioned over the springs which
allows the bed tramming wizard to work well.

It has S-curve acceleration enabled, Arc support enabled, and some speed tweaks
to speed up the bed levelling process.

## Special notes

On the Ender-3 the hotend is capable of traveling to the right well past the
print surface. In order to allow the BLTouch to probe directly above the bed
levelling screws on the right, Marlin has been configured to allow X-axis
travel out to 240mm (although this doesn't affect the print area). This should
be fine for any standard Ender-3, but something to be aware of if you
have modified anything like the belt tensioner in that area, in case it may
cause the machine to crash when probing.
