# Resources

## Links

- Interrupt List
	- http://www.ctyme.com/rbrown.htm
- AMD64 Architecture Programmer's Manual Volumes 1-5
	- https://www.amd.com/system/files/TechDocs/40332.pdf
- Intel E1000-series NIC Programer's Manual
	- https://www.intel.com/content/dam/doc/manual/pci-pci-x-family-gbe-controllers-software-dev-manual.pdf
- PCIExpress Base 3.0
	- http://akkit.org/info/PCI_Express_Base_r3.0_10Nov10.pdf
- x86(-64) assembler/disassembler
	- https://defuse.ca/online-x86-assembler.htm#disassembly
- Useful pdfs
	- https://github.com/tpn/pdfs
- Intel 64 & IA-32 Architectures Software Developer's Manual
	- https://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-software-developer-instruction-set-reference-manual-325383.pdf
- Optical Drive guide
	- https://dev.lovelyhq.com/libburnia/libburn/raw/branch/master/doc/cookbook.txt
- OSDev Wiki Optical Drive guide
	- https://wiki.osdev.org/Optical_Drive
- SCSI Primary Commands - 3
	- http://www.13thmonkey.org/documentation/SCSI/spc3r23.pdf
- SCSI Programming HOWTO
	- https://tldp.org/HOWTO/archived/SCSI-Programming-HOWTO/SCSI-Programming-HOWTO-10.html
- SSE SIMD practical guide
	- http://sci.tuomastonteri.fi/programming/sse
- E1000 driver source from WingOS
	- https://github.com/Supercip971/WingOS/blob/61614042b15c3f8be28de91c276054565596760f/kernel/arch/x86_64/device/network/e1000.cpp
- E1000 driver source from linux
	- https://github.com/torvalds/linux/tree/master/drivers/net/ethernet/intel/e1000
- e1000 driver source from minix
	- https://github.com/Stichting-MINIX-Research-Foundation/minix/tree/4db99f4012570a577414fe2a43697b2f239b699e/minix/drivers/net/e1000
- C program test suite for testing lexers/parsers/compilers against
	- https://github.com/c-testsuite/c-testsuite/tree/master/tests/single-exec
- Denigma AI-powered code analyzer tool
	- https://www.denigma.app/#demo
- x86-64 reference manual
	- http://ref.x86asm.net/coder64.html
- x86-64 reference manual
	- https://www.felixcloutier.com/x86/
- TempleOS binary patch table parser written in Java using ghidra
	- https://github.com/aarzilli/templestuff/blob/master/TempleOS.java
- https://minexew.github.io/2020/03/29/templeos-loader-part2.html
- https://checksum.fail/files/VBoxGuest.HC
- https://www.officedaytime.com/simd512e/
- https://gamemath.com/book/
- Write Yourself a Git git from-scratch reimplementation guide
	- https://wyag.thb.lt/
- random example of a git reimplementation that has a push method
	- https://github.com/Ampferl/avc/blob/master/libavc.py#L80
- https://github.com/DevSolar/pdclib
- https://github.com/nothings/stb
- https://sandpile.org/x86/opc_rm.htm
- https://staffwww.fullcoll.edu/aclifton/cs241/lecture-instruction-execution.html
- https://atkinssj.github.io/How-to-PR/ How to get your open source changes merged
- https://www.tutorialspoint.com/assembly_programming/assembly_introduction.htm
- https://winaero.com/set-exact-display-resolution-in-virtualbox-virtual-machine/
	- VBoxManage setextradata "VM-Name" "CustomVideoMode#" "#x#x32"
- C-like code reindenter/beautifier
	- https://techiedelight.com/tools/clike
- HDAudio spec
	- https://www.intel.com/content/dam/www/public/us/en/documents/product-specifications/high-definition-audio-specification.pdf
- PCI Local Bus Specification, revision 3.0
	- https://www.cl.cam.ac.uk/~djm202/pdf/specifications/pci/PCI_LB3.0_CB-2-6-04.pdf


- https://git.xslendi.xyz/slendi/HolyParser slendi's HolyC+ASM lexer, parser
- https://github.com/eb-lan/TINE TempleOS host-machine userspace software
- https://github.com/JeffIrwin/temple-viewer TOS 3D .STL model viewer
- https://github.com/tinkeros/BETTR TOS .TOML parsing
- https://github.com/bramtechs/TempleRicer TOS themes

---

### Command line instructions to manually test PRs:

![Image](manual-PR-test.png)

(in the screenshot, example-user is making a PR to master from branch example-pr-branch-name, this username and this branch name are used in the second step's command)

1. Step 1: From your project repository, check out a new branch 
	- git checkout -b name-of-new-local-branch-here master
2. Pull the changes from example-user's PR branch example-pr-branch-name into the new created local branch
	- git pull https://github.com/example-user/ZealOS.git example-pr-branch-name 

---

### alec software backups:

- https://mega.nz/folder/ZIEGmSRQ#qvL6Wk6THzE-dazkfT6N3Q/folder/9BFUTZYI
- https://github.com/tinkeros/Alec_stuff_backup
- https://web.archive.org/web/*/https://git.checksum.fail/* (filter by .zip or .bundle) 

ZealOS Lemmy community: https://lemmy.world/c/zealos
