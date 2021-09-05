# MSP432-Launchpad-Firmware
Firmware is read from good MSP432 Launchpad Black board.
Please don't use this firmware for the red board.

Please follow the instruction file XDS110SupportReadMe.pdf at \ti\ccs_base\common\uscif\xds110

Updating the Firmware Using xdsdfu instruction
To program the firmware, follow these steps:
1. Plug the XDS110 debug probe into your computer. Make sure that you only have one XDS110 class debug probe plugged in. The xdsdfu program will attempt to flash the first XDS110 debug probe it finds.
2. Run the following two commands from directory with xdsdfu:
xdsdfu -m
xdsdfu -f XDS_ORG.bin -r

Use the actual filename of the firmware file.  My firmware file is 'XDS_ORG.bin'.
You may need to pause after the first command to give the OS time to recognize that the XDS110 has reconfigured as a different USB device.
Once the second command has completed, the firmware is updated, and the XDS110 should be ready to use.
