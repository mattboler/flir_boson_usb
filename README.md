# ROS Driver (Linux Only) for the FLIR Boson USB Camera #

This driver borrows *heavily* from the example application at https://github.com/FLIR/BosonUSB.


Be *very* careful to not confuse this driver with the one listed on ROSWIKI.
The ~RAW16~ mode on this driver *actually publishes a 16bit image which may or may not work with your code*.
The original RAW16 mode, which performs gain control and compresses the image to 8bits, has been renamed to ~AGC~.
