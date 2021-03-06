## "The Thing": Cyclone II FPGA + Arduino STM32F103C8T6 board, Multicomp compatible.

Two dev boards into one: a STM32 based Arduino ("Maple Mini" compatible) and a Cyclone II FPGA dev. board to start playing with VHDL/Verilog. It is also "Multicomp" compatible ("Multicomp" is a modular VHDL design to "run" some famous retro 8 bit CPUs made by [Grant Searle](http://searle.hostei.com/grant/Multicomp) giving the option to "run" easily a VHDL SOC with a Z80/6809/6502 CPU and I/O, including HD on SD and a color VDU).

Detailed info [at this page](https://hackaday.io/project/163683-the-thing-fpga-stm32).

Development info at this [Twitter account](https://twitter.com/Just4Fun_J4Fun).

### Table of contents:
* [QuartusII Project](https://github.com/SuperFabius/The-Thing-FPGA-STM32/tree/master/QuartusII%20Project):
in this folder there are the Quartus II projects examples for the Cyclone II FPGA. They are generally paired with a given Arduino Sketch (.ino file) for the STM32.

* [QuartusII Multicomp](https://github.com/SuperFabius/The-Thing-FPGA-STM32/tree/master/QuartusII%20Multicomp):
in this folder there are the Quartus II Multicomp projects for the Cyclone II FPGA. These Multicomp have been already adapted to run inside the "The Thing" board "out of the box" ("The Thing" board HW design requires some little adaptations from the original Multicomp design reference). They could be paired with a given Arduino Sketch (.ino file) for the STM32 and with a given SD image for HD emulation.

* [STM32 Sketch](https://github.com/SuperFabius/The-Thing-FPGA-STM32/tree/master/STM32%20Sketch):
in this folder there are the "sketch" examples (.ino files) for the STM32 Arduino. They are generally paired with a given Quartus II project example or a Quartus II Multicomp. See in the [QuartusII Project](https://github.com/SuperFabius/The-Thing-FPGA-STM32/tree/master/QuartusII%20Project) or [QuartusII Multicomp](https://github.com/SuperFabius/The-Thing-FPGA-STM32/tree/master/QuartusII%20Multicomp) directory to know which Quartus II project they belong to.

* [SD images for Multicomp](https://github.com/SuperFabius/The-Thing-FPGA-STM32/tree/master/SD%20images%20for%20Multicomp):
in this folder there are the SD images for HD emulation related to the Quartus II Multicomp projects for the Cyclone II FPGA. They are paired with a given Quartus II Multicomp project. See in the [QuartusII Multicomp](https://github.com/SuperFabius/The-Thing-FPGA-STM32/tree/master/QuartusII%20Multicomp) directory to know which Quartus II Multicomp they belong to. To write the SD image into a SD card, unzip the image file and simply copy it to your SD card using the [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/).

## CREDITS & LICENSE

Multicomp VHDL are based on Grant Searle's original work, which was published with the following license:

“By downloading these files you must agree to the following: The original copyright owners of ROM contents are respectfully acknowledged. Use of the contents of any file within your own projects is permitted freely, but any publishing of material containing whole or part of any file distributed here, or derived from the work that I have done here will contain an acknowledgement back to myself, Grant Searle, and a link back to this page. Any file published or distributed that contains all or part of any file from this page must be made available free of charge.” (http://searle.hostei.com/grant/Multicomp/index.html).

All the project files (SW & HW) are licensed under GPL v3.

If you use this material in any way a reference to the author (me :-) ) will be appreciated.
