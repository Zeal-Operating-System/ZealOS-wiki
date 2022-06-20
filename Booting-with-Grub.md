For each ZealOS partition, add lines to `/etc/grub.d/40_custom` in this format:
```
menuentry "ZealOS" {
  set root=(hd0,msdos6)
  chainloader +1
}
```
In the above example, ZealOS is installed to `hd0,msdos6`: the 6th partition of the first hard drive.

Run `sudo update-grub` to update the auto-generated grub configuration with the custom entries.