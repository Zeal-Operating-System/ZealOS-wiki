ZealOS requires a computer with a **64-bit CPU**, at least **512MB RAM**, a **SATA** hard drive at least **512MB** in size, and a **SATA CD/DVD drive**. If the computer does not have an optical disc drive, the computer is not supported. If the BIOS does not support Legacy Boot, the OS will be unable to boot properly. If the BIOS does not emulate PS/2 mouse and keyboard from USB, and/or the computer does not have PS/2 ports for mouse and keyboard, the computer is not supported. Some chipsets have watchdog timers that trip and reboot the computer because the OS does not initialize these, if this occurs the computer is not supported.

It is recommended to partition the hard drive in advance, using another operating system. **_If partitioning the drive within the OS, it will destroy the drive's previous partition table, and likely existing data on the drive._**

1. Burn the latest ZealOS ISO to a CD/DVD, insert the disc into the computer's disc drive.
2. Reboot. It may be necessary to press F12 or another function key to pick the CD/DVD drive to boot from.
3. Press any key to dismiss the splash screen. (If the splash won't close, PS/2 keyboard emulation is unsupported and the BIOS is incompatible.)
4. Type `Y` when asked if you want to install onto a hard drive.
5. Type `N` when asked if you are installing in a virtual machine.
    * (Warning: If you type `Y`, it will **format, partition, and install to** the first detected hard drive!)
6. If you have partitioned the hard drive in advance, type `Y` when asked if the install partition is ready. If the drive is not partitioned in advance, you can type `N` to abort installation.
7. Type `I` when asked if you want to upgrade or create a new install.
8. Type the port number of the destination hard drive. The detected drives and their port numbers are displayed in the top left window.
9. Type the letter of the hard drive partition to install to.
10. Type either `Y` or `N` when asked if you want to format the drive.
11. Select filesystem type, either FAT32 or RedSea.
12. Select screen resolution.
13. If you type `Y` when asked to install a master boot loader, the drive's master boot loader is replaced with the ZealOS bootloader. If using a different bootloader like Grub, type `N`, and after installation reconfigure your bootloader to show ZealOS as a boot option.
14. After installation is complete, type `Y` to reboot. The disc will auto-eject.