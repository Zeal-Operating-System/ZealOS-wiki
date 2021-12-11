## Instructions
1. Run the `K.ZC` file in the Home/ directory.
2. Type `N` when asked if it was successful. (If you type `Y`, it will attempt to build a Distro ISO.)
3. Reboot.

## Settings
This will recompile the Kernel with the following settings:
* Boot Drive: `C`
* Mounted Drives:
  * `C` at SATA port of the first-seen ATA drive at compile time.
    * Partition: All
* Resolution: 1024x768
* Disk Cache Size: Default
* Home Directory: `::/Home`

## Warnings

**- Running `K.ZC` while booted into a partition that isn't `C` will misconfigure the partition.**

**- Having more than one HDD can result in `K.ZC` setting the wrong boot SATA port. Make sure your ZealOS drive has a lower SATA port number than your other drives.**

**- If you have ZealOS installed onto a drive with other OS partitions and ZealOS is not the first partition, `K.ZC` will misconfigure whichever drive partition is first.**