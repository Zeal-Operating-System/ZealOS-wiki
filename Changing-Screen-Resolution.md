After the OS is booted, you can run `VideoRep;` at the command line to retrieve a list of screen resolutions supported by your target hardware/VM. By default, ZealOS uses the standard resolution of 1024x768, however any of the resolutions listed can be used as a screen resolution for ZealOS.

If you are using the Limine bootloader, you need to modify `/Boot/Limine.CFG` and change the value in the `RESOLUTION` field. (Note that `INTERFACE_RESOLUTION` only affects the resolution of the Limine bootloader itself, the `RESOLUTION` value applies to the OS.)

If using the traditional Public Domain BIOS-mode bootloader, you will need to edit `/Kernel/KStart16.ZC` and change the values in `REQUESTED_SCREEN_WIDTH` and `REQUESTED_SCREEN_HEIGHT`. Then you can recompile the kernel with `BootHDIns;` [following the instructions on the wiki.](Kernel-Recompiling)

Reboot to see the new resolution settings take effect.
