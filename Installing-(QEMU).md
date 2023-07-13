1. Create a new virtual machine hard disk drive.
  ```
qemu-img create -f qcow2 ZealOS.qcow2 1G
```
2. Launch a new virtual machine with the latest ISO and the hard disk.
  * Linux:  
  ```
qemu-system-x86_64 -audiodev sdl,id=snd0 -machine q35,kernel_irqchip=off,pcspk-audiodev=snd0,accel=kvm -cdrom ZealOS-YYYY-MM-DD-HH_MM_SS.iso -hda ZealOS.qcow2 -m 2G -smp $(nproc) -rtc base=localtime -nic user,model=pcnet
```
  * Windows:  
  ```
qemu-system-x86_64.exe -audiodev sdl,id=snd0 -machine q35,kernel_irqchip=off,pcspk-audiodev=snd0,accel=whpx -cdrom ZealOS-YYYY-MM-DD-HH_MM_SS.iso -hda ZealOS.qcow2 -m 2G -smp $(get-computerinfo -property csprocessors).csprocessors.numberofcores -rtc base=localtime -nic user,model=pcnet
```

3. Start the VM.
4. Press any key to dismiss the splash screen.
5. Type `Y` when asked if you want to install onto a hard drive.
6. Type `I` when asked if you want to upgrade or create a new install.
7. After installation is complete, type `Y` to reboot. The disc will auto-eject.
8. On subsequent launches of the virtual machine, omit the `-cdrom` argument and parameter.