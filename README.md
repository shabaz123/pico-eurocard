# pico-eurocard

This repository contains PCB Gerber files and bill of materials for a Pi Pico Eurocard Development Board.

License: Free for all non-commercial use.

Board Revision History

Rev 1 - Resistors R2 and R3 are mistakenly connected to GND. They should be connected to 3V3. See the rev1-i2c-fix.png file to see the fix (requires two traces to be cut, and a wire to be soldered).

Rev 1.1 - Fixes the R2 and R3 issue that Rev 1 had. Also adds connections for an SPI TFT display, and exposes I2C, GND and VSYS onto some additional pins on the edge connector for some more flexibility. Also, the 7805 regulator has a bit more space, to allow heatsinks to more easily fit.

Rev 1.2 - Adds some pads on the underside of the SOIC footprints, that are suitable for decoupling capacitors, and for optional output feedback components if the soldered SOIC component is an op-amp. Also, the corners of the board have been rounded very slightly (0.5 mm radius). Previously, the corners had no radius.

