# TODO

## Simple
* Reimplement TempleOS file decompression. (No compression.)
* Add ZealOS-specific section to PersonalMenu.
* Optimize RawPutChar.
* Fix sky/horizon height in Varoom and ZoneOut.
* Add a `Lex` demo: report `CCompCtrl` info iteratively as the user presses Spacebar to advance to the next token.
* Move `docs/` to another repo.
* Test if `MEM_EXTRA_HASH2_PAGS` can be set to 1, instead of 2. (Would double available stack size at the cost of more Data Heap allocation.)
* Improve ToTheFront game mechanics explanation.

## Difficult
* Improve MultiCore processor initialization process.
* Fix `GRScreenCaptureWrite`, `GRScreenCaptureRead`, and `DCScreenCapture`.
* Fix certain screen resolutions distorting.
* Add Extrude to 3D Sprite Mesh Editor.
* Implement SLOC `LineRep`.
* Fix `ATAPIRBlks` bottleneck.
* Optimize `GrZoomInScreen`, `GrCalcScreenUpdates`, `GrUpdateScreen32`, and `GrUpdateScreen`.
* Implement network file transfer.
* Implement HTTP.
* Implement network loopback operation.
* Get E1000 driver into functional state.
* Fix AcctExample code.
* Make car tires in Varoom round, or implement sprite interpolation to make tires rotate.
* Fix Chess king vs. king stalemate softlock.
* Scale ToTheFront sprites and map to fit screen so sprites are more visible at high screen resolutions.
* Add and port Terry's HDAudio driver from supplemental disc, and alec's AC97 driver from Erythros.
* Fix `Uf` opcode report spacing.
* Fix how command line handles Insert mode.
* Add right-click macro to Dir directory macros, similar to file right-click popup menu.
* Regularly generate Lite and UltraLite ISOs.
* Improve build process and version control system.
* Fix partially-offscreen sprite flickering.
* Clean up AHCI code.
* Clean up Networking code.