# Kernel Recompiling

## Instructions
1. Type `BootHDIns;` at the command line and press Enter.
2. Type the letter of the drive you want to use as the Boot Drive.
    * You can press Enter to use the current drive, which is usually ideal.
    * If you're recompiling the kernel for another drive partition, type the letter for that drive partition.
3. Mount the drives you want to have present at boot by typing the drive letter at the prompt.

|Drive Type|Drive Letters|
|:-:|:-:|
|RAM|A B|
|ATA HDD|C D E F G H I J K L|
|ISO File-Read Drive|M N O P|
|ISO File-Write Drive|Q R S|
|ATAPI CD/DVD|T U V W X Y Z|

Mounting the C drive is usually the bare minimum. The mount process varies depending on the drive type:
* ATA HDD:
  1. When asked for Partition Num, either press Enter to mount all partitions on the drive, or type a number (starting from 0) corresponding to the partition number. **When mounting all partitions of HDDs, they are mounted at letters following the initial drive letter.**
  2. Type the SATA Port number of the HDD you want mounted, then press Enter.
* ATAPI CD/DVD:
  1. Type the SATA Port number of the ATAPI CD/DVD drive you want mounted, then press Enter.
* RAM:
  1. When asked for the address of the RAM disk, press Enter to configure the kernel to MAlloc the RAM disk on boot.
  2. Type the number of 512 byte blocks you want the RAM disk to have, then press Enter. You can input it as decimal or hex, and/or an expression. Here are some examples:
      * `2*3*1024*1024` (3 GB)
      * `0x200000` (1 GB)
      * `0x100000` (512 MB)
      * `2*256*1024` (256 MB)
      * `0x20000` (64 MB)
      * `0x10000` (32 MB)
      * `65536` (32 MB)
* ISO File-Read Drive:
  1. When asked for a filename, type the absolute file path to an ISO.C file and press Enter.
* ISO File-Write Drive:
  1. Type the number of 512 byte blocks you want the drive to have, then press Enter.

4. When prompted for Disk Cache Size, type the number of bytes you want to use as cache, or press Enter to use the default cache size.
5. Either press Enter when asked for Kernel Options to leave defaults, or type the name of a desired option to set and configure it.
6. Reboot.
