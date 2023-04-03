# pico-eurocard

This repository contains PCB Gerber files and bill of materials for a [Pi Pico Eurocard Development Board](https://community.element14.com/products/raspberry-pi/b/blog/posts/pi-pico-eurocard-development-board). See James' [Workshop Wednesday's Video](https://community.element14.com/challenges-projects/element14-presents/workbenchwednesdays/w/documents/28083/workbench-wednesdays-70-why-you-need-a-raspberry-pi-pico-development-board-by-shabaz) which demonstrates the revision 2.0 board.

Right-click below to open in new window to watch the video for a quick explanation!

[<img src="doc\pico-euro-youtube.jpg" width="50%">](https://www.youtube.com/watch?v=-Kv5MwaRqbk "Pico-EUROCARD YouTube Video")

The current revision 2.2 board has a few slight impromements to make it easier to solder, and has enlarged text silkscreen as can be seen in the image below.

Latest [Schematic](https://github.com/shabaz123/pico-eurocard/blob/main/pico-euro-kicad-source/pico-euro-schematic.pdf) and [Bill of Materials](https://github.com/shabaz123/pico-eurocard/blob/main/pico-euro-kicad-source/pico-euro-rev-2-2-bill-of-materials.pdf) and [Zip file of Gerbers](https://github.com/shabaz123/pico-eurocard/blob/main/export_pico_euro_rev_2_2.zip), (click on the Download button on the right) ready for sending to any PCB factory.

<img width="100%" align="left" src="doc\pico-euro-2-2-render-top-angle.jpg">

License: The pico-eurocard project is distributed under the CC BY-NC-SA 4.0 license. Please share any changes you make, so that others can contribute and benefit from them.

Board Revision History

Rev 1 - Resistors R2 and R3 are mistakenly connected to GND. They should be connected to 3V3. See the rev1-i2c-fix.png file to see the fix (requires two traces to be cut, and a wire to be soldered).

Rev 1.1 - Fixes the R2 and R3 issue that Rev 1 had. Also adds connections for an SPI TFT display, and exposes I2C, GND and VSYS onto some additional pins on the edge connector for some more flexibility. Also, the 7805 regulator has a bit more space, to allow heatsinks to more easily fit.

Rev 1.2 - Adds some pads on the underside of the SOIC footprints, that are suitable for decoupling capacitors, and for optional output feedback components if the soldered SOIC component is an op-amp. Also, the corners of the board have been rounded very slightly (0.5 mm radius). Previously, the corners had no radius.

Rev 1.3 - Added some pads to make it slightly easier to plug on a daughter board made from (say) stripboard.

Rev 2.0 - Removed SPI TFT pins, since there was some incompatibility with recently available displays. Added micro SD card socket.

Rev 2.2 - Very similar to 2.0 version, but with far more legible silkscreen, and with all surface-mount components (including the micro SD socket) on one side of the board, for easier production. Also added a resistor for more gate protection with partially assembled boards.
