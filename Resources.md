# Resources

## Links:

### Social
- [ZealOS Lemmy community](https://lemmy.world/c/zealos) 

### x86-64/BIOS/UEFI
- [Interrupt List](http://www.ctyme.com/rbrown.htm)
- [AMD64 Architecture Programmer's Manual Volumes 1-5](https://www.amd.com/system/files/TechDocs/40332.pdf) 
- [PCIExpress Base 3.0](http://akkit.org/info/PCI_Express_Base_r3.0_10Nov10.pdf) 
- [x86(-64) assembler/disassembler](https://defuse.ca/online-x86-assembler.htm#disassembly) 
- [Intel 64 & IA-32 Architectures Software Developer's Manual](https://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-software-developer-instruction-set-reference-manual-325383.pdf) 
- [SSE SIMD practical guide](http://sci.tuomastonteri.fi/programming/sse) 
- [x86-64 reference manual coder64](http://ref.x86asm.net/coder64.html) 
- [x86-64 reference manual felixcloutier](https://www.felixcloutier.com/x86/) 
- [SIMD SSE Instruction List](https://www.officedaytime.com/simd512e/) 
- [PCI Local Bus Specification, revision 3.0](https://www.cl.cam.ac.uk/~djm202/pdf/specifications/pci/PCI_LB3.0_CB-2-6-04.pdf) 
- [x86 architecture mod R/M byte](https://sandpile.org/x86/opc_rm.htm) 
- [Instruction Execution Lecture/Guide](https://staffwww.fullcoll.edu/aclifton/cs241/lecture-instruction-execution.html) 

### Audio
- [HDAudio spec](https://www.intel.com/content/dam/www/public/us/en/documents/product-specifications/high-definition-audio-specification.pdf) 

### CD/DVD
- [Optical Drive guide](https://dev.lovelyhq.com/libburnia/libburn/raw/branch/master/doc/cookbook.txt) 
- [OSDev Wiki Optical Drive guide](https://wiki.osdev.org/Optical_Drive) 
- [SCSI Primary Commands - 3](http://www.13thmonkey.org/documentation/SCSI/spc3r23.pdf) 
- [SCSI Programming HOWTO](https://tldp.org/HOWTO/archived/SCSI-Programming-HOWTO/SCSI-Programming-HOWTO-10.html) 

### Networking
- [Intel E1000-series NIC Programer's Manual](https://www.intel.com/content/dam/doc/manual/pci-pci-x-family-gbe-controllers-software-dev-manual.pdf) 
- [E1000 driver source from WingOS](https://github.com/Supercip971/WingOS/blob/61614042b15c3f8be28de91c276054565596760f/kernel/arch/x86_64/device/network/e1000.cpp) 
- [E1000 driver source from linux](https://github.com/torvalds/linux/tree/master/drivers/net/ethernet/intel/e1000) 
- [e1000 driver source from minix](https://github.com/Stichting-MINIX-Research-Foundation/minix/tree/4db99f4012570a577414fe2a43697b2f239b699e/minix/drivers/net/e1000) 

### Tools
- [C-like code reindenter/beautifier](https://techiedelight.com/tools/clike) 

### Software
- [C program test suite for testing lexers/parsers/compilers against](https://github.com/c-testsuite/c-testsuite/tree/master/tests/single-exec) 
- [Public Domain C Library](https://github.com/DevSolar/pdclib) 
- [Public Domain single-file C Libraries](https://github.com/nothings/stb) 
- [Write Yourself a Git git from-scratch reimplementation guide](https://wyag.thb.lt/) 
- [random example of a git reimplementation that has a push method](https://github.com/Ampferl/avc/blob/master/libavc.py#L80) 
- [How to get your open source changes merged](https://atkinssj.github.io/How-to-PR/ ) 
- [Assembly Introduction from tutorialspoint](https://www.tutorialspoint.com/assembly_programming/assembly_introduction.htm) 

### VMs/TempleOS/ZealOS-specific
- [How to Set Extra Screen Resolutions in Virtualbox VMs](https://winaero.com/set-exact-display-resolution-in-virtualbox-virtual-machine/) 
	- VBoxManage setextradata "VM-Name" "CustomVideoMode#" "#x#x32"
- [TempleOS binary patch table parser written in Java using ghidra](https://github.com/aarzilli/templestuff/blob/master/TempleOS.java) 
- [TempleOS .BIN format guide from minexew](https://minexew.github.io/2020/03/29/templeos-loader-part2.html) 
- [alec VBoxGuest.HC](https://checksum.fail/files/VBoxGuest.HC) 
- [slendi's HolyC+ASM lexer, parser](https://git.xslendi.xyz/slendi/HolyParser) 
- [TempleOS host-machine userspace software](https://github.com/eb-lan/TINE)  
- [TOS 3D .STL model viewer](https://github.com/JeffIrwin/temple-viewer)  
- [TOS .TOML parsing](https://github.com/tinkeros/BETTR)  
- [TOS themes](https://github.com/bramtechs/TempleRicer)  

### Other
- [Useful pdfs](https://github.com/tpn/pdfs) 
- [Denigma AI-powered code analyzer tool](https://www.denigma.app/#demo) 
- [Game Math Book](https://gamemath.com/book/) 

---

## Command line instructions to manually test PRs:

![Image](manual-PR-test.png)

(in the screenshot, example-user is making a PR to master from branch example-pr-branch-name, this username and this branch name are used in the second step's command)

1. Step 1: From your project repository, check out a new branch 
	- git checkout -b name-of-new-local-branch-here master
2. Pull the changes from example-user's PR branch example-pr-branch-name into the new created local branch
	- git pull https://github.com/example-user/ZealOS.git example-pr-branch-name 

---

## alec software backups:

- https://mega.nz/folder/ZIEGmSRQ#qvL6Wk6THzE-dazkfT6N3Q/folder/9BFUTZYI
- https://github.com/tinkeros/Alec_stuff_backup
- https://web.archive.org/web/*/https://git.checksum.fail/* (filter by .zip or .bundle) 
