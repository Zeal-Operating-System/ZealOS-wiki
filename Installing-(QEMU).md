1. Create a new virtual machine hard disk drive.
  * `qemu-img create -f qcow2 ZealOS.qcow2 1G`
2. Launch a new virtual machine with the latest ISO and the hard disk.
  * `qemu-system-x86_64 -machine q35,kernel_irqchip=off -cdrom ZealOS-YYYY-MM-DD-HH_MM_SS.iso -hda ZealOS.qcow2 -m 4G -smp 4 -accel kvm -rtc base=localtime -soundhw pcspk`
3. Start the VM.
4. Press any key to dismiss the splash screen.
5. Type `Y` when asked if you want to install onto a hard drive.
6. Type `I` when asked if you want to upgrade or create a new install.
7. After installation is complete, type `Y` to reboot. The disc will auto-eject.
8. On subsequent launches of the virtual machine, omit the `-cdrom` argument and parameter.