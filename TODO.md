# TODO

## Simple
* Rename all `abs_addres` to `abs_address`.
* Add ZealOS-specific section to PersonalMenu.
* Improve ToTheFront game mechanics explanation.
* Update `Doc/AboutZealOS.DD`.
* Test if `MEM_EXTRA_HASH2_PAGS` can be set to 1, instead of 2. (Would double available stack size at the cost of more Data Heap allocation.)
* Print data column title header strings in the various Rep functions, add human-readable values.
* Add a `Lex` demo: report `CCompCtrl` info iteratively as the user presses Spacebar to advance to the next token.
* Move `docs/` to another repo.
* Optimize RawPutChar.
* Fix sky/horizon height in Varoom and ZoneOut.
* Implement a `WinTileGrid`.
* Flush framebuffer/screen cache on `CTask` Palette change. (Bug when running a game or App, in other task changing Palette, then exiting app.)
* Reimplement TempleOS file decompression. (No compression.)

## Difficult
* Get E1000 driver into functional state.
* Implement HTTP.
* Implement network file transfer.
* Improve MultiCore processor initialization process.
* Fix `GRScreenCaptureWrite`, `GRScreenCaptureRead`, and `DCScreenCapture`.
* Fix MiniGrLib.
* Add Extrude to 3D Sprite Mesh Editor.
* Fix partially-offscreen sprite flickering.
* Fix Chess king vs. king stalemate softlock.
* Fix how command line handles Insert mode.
* Add right-click macro to Dir directory macros, similar to file right-click popup menu.
* Add and port Terry's HDAudio driver from supplemental disc, and alec's AC97 driver from Erythros.
* Fix certain screen resolutions distorting.
* Scale ToTheFront sprites and map to fit screen so sprites are more visible at high screen resolutions.
* Make car tires in Varoom round, or implement sprite interpolation to make tires rotate.
* Fix `ATAPIRBlks` bottleneck.
* Optimize `GrZoomInScreen`, `GrCalcScreenUpdates`, `GrUpdateScreen32`, and `GrUpdateScreen`. (Use MultiCore to distribute graphics computation?)
* Implement SLOC `LineRep`.
* Fix AcctExample code.
* Regularly generate Lite and UltraLite ISOs.
* Clean up AHCI code.
* Clean up Networking code.
* Implement network loopback operation.
* Clean up Compiler code, add more documentation.
* Clean up Kernel code, improve organization, remove bloat, add more documentation.
* Improve build process and version control system.