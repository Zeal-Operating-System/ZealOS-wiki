# TODO

## Simple
* Review RFC 793, fix RST ACK loop spam. (Bug spotted using QEMU)
* Add a `Lex` demo: report `CCompCtrl` info iteratively as the user presses Spacebar to advance to the next token.
* Move `docs/` to an organization root repo. (zeal-operating-system.github.io)
* Optimize `RawPutChar`.
* Fix sky/horizon height in Varoom and ZoneOut.
* Implement a `WinTileGrid`.
* Reimplement TempleOS file decompression. (No compression.)
* Implement `Ping` network function.

## Difficult
* Get E1000 driver into functional state.
* Implement HTTP.
* Implement network file transfer.
* Improve MultiCore processor initialization process.
* Fix `GRScreenCaptureWrite`, `GRScreenCaptureRead`, and `DCScreenCapture`.
  - reference to `gr.screen_image` needs to be replaced
* Fix MiniGrLib.
* Add Extrude to 3D Sprite Mesh Editor.
* Fix function local variable list declaration with initialization Compiler bug.
* Fix partially-offscreen sprite flickering.
* Fix Chess king vs. king stalemate softlock.
* Fix how command line handles Insert mode.
* Add right-click macro to `Dir` directory macros, similar to file right-click popup menu.
* Add and port Terry's HDAudio driver from supplemental disc, and alec's AC97 driver from Erythros.
* Put ISO9660 and BMP file support back in.
* Fix certain screen resolutions distorting.
* Scale ToTheFront sprites and map to fit screen so sprites are more visible at high screen resolutions.
* Make car tires in Varoom round, or implement sprite interpolation to make tires rotate.
* Fix `ATAPIRBlks` bottleneck.
* Optimize `GrZoomInScreen`, `GrCalcScreenUpdates`, `GrUpdateScreen32`, and `GrUpdateScreen`. (Use MultiCore to distribute graphics computation?)
* Fix bug where Pause/Break key scancode is converted to Ctrl-NumLock.
* Implement SLOC `LineRep`.
* Fix `Demo/AcctExample/` code.
* Fix Gopher client functionality when booted from CD/DVD drive.
  - attempted fixing this using RAM drive for file downloads during LiveCD boot, but got errors during the drive offset checks in `BlkWrite`.
* Regularly generate Lite and UltraLite ISOs.
* Clean up AHCI code.
* Clean up Networking code.
* Implement Networking loopback operation.
* Clean up Compiler code, add more documentation.
* Clean up Kernel code, improve organization, remove bloat, add more documentation.