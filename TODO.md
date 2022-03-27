# TODO

## Networking
* Get E1000 driver into functional state.
  - need to write an E1000Debug() method and analyze NIC state at TX.
* Debug QEMU PCNet MAC.
* Add STOR capability to FTP client.
* Fix Gopher client functionality when booted from CD/DVD drive.
  - attempted fixing this using RAM drive for file downloads during LiveCD boot, but got errors during the drive offset checks in `BlkWrite`.
* Write game demonstrating network client/server functionality.
* Implement Networking loopback operation.
* Reformat/remove VirtIO driver.
* Clean up Networking code.
* Implement HTTP.

## Kernel
* Improve MultiCore processor initialization process.
* Clean up AHCI code.
* Optimize `RawPutChar`.
* Put ISO9660 and BMP file support back in.
* Add PNG support.
* Fix certain screen resolutions distorting.
* Fix `ATAPIRBlks` bottleneck.
* Add ext2/ext3/ext4 filesystem support.
* Add UEFI & GPT support.
* Clean up Kernel code, improve organization, remove bloat, add more documentation.

## System
* Update EdCodeTools for ZealC tab-convention.
* Implement Ed "diff" feature to compare editor contents with the file stored on disk.
* Add and port/rewrite Terry's HDAudio driver from supplemental disc, and alec's AC97 driver from Erythros.
* Fix `GRScreenCaptureWrite`, `GRScreenCaptureRead`, and `DCScreenCapture`.
  - reference to `gr.screen_image` needs to be replaced
* Fix how command line handles Insert mode.
* Add right-click macro to `Dir` directory macros, similar to file right-click popup menu.
* Fix bug where Pause/Break key scancode is converted to Ctrl-NumLock.
* Implement SLOC `LineRep`.
* Reimplement TempleOS file decompression. (No compression.)
* Implement `TaskFlagsRep` or add flag details to `TaskRep`, perhaps using a new `verbose` bool default arg?
* Improve mouse-only support.

## Graphics
* Add Extrude to 3D Sprite Mesh Editor.
* Optimize `GrZoomInScreen`, `GrCalcScreenUpdates`, `GrUpdateScreen32`, and `GrUpdateScreen`. (Use MultiCore to distribute graphics computation?)
* Fix MiniGrLib.
* Fix partially-offscreen sprite flickering.

## Games/Demos
* Fix Chess king vs. king stalemate softlock.
* Scale ToTheFront sprites and map to fit screen so sprites are more visible at high screen resolutions.
* Add mouse aim to CastleFrankenstein.
* Make car tires in Varoom round, or implement sprite interpolation to make tires rotate.
* Fix `Demo/AcctExample/` code.
* Fix sky/horizon height in Varoom and ZoneOut.

## Compiler
* Add `U128` variable support using SSE registers. (branch: u128-compiler)
  - work out how to add in `ST_XMM_REGS` usage, consider how `ST_U64_REGS` is used
* Make `PassTrace` output more human-readable.
* Fix function local variable list declaration with initialization Compiler bug.
  - must be declared static...
* Clean up Compiler code, add more documentation.

## Misc.
* Add HolyMath Tests to TestSuite.
* Regularly generate Lite and UltraLite ISOs.