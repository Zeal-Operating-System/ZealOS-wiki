For each ZealOS partition, add lines to `/etc/grub.d/40_custom` in this format:
```
menuentry "ZealOS C:/" {
  set root=(hd0,msdos6)
  chainloader +1
}
```
In the above example, a ZealOS `C:/` Drive partition is installed onto `hd0,msdos6`, the 6th partition of the first HDD.

Run `sudo update-grub` to update the auto-generated grub configuration with the custom entries.