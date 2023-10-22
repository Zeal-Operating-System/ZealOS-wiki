# Building an ISO

## Instructions (Windows)
1. [Enable Hyper-V.](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/quick-start/enable-hyper-v#enable-the-hyper-v-role-through-settings)
2. Make sure you have QEMU installed. A 64-bit Windows QEMU installer can be downloaded [from here.](https://qemu.weilnetz.de/w64/) Use the default installation path for QEMU.
3. Open a PowerShell window with Administrator privileges.
4. Run `build-iso.ps1`.

## Instructions (Linux)
1. Make sure you have the commands: `qemu-img`, `qemu-nbd`, `qemu-system-x86_64`, `partprobe`, `modprobe`, `sed`, `wc`, `xorriso`, `git`, `make`, `curl`, and `cc`.

Here are commands to install these packages on various distros:
  * Ubuntu
```
sudo apt install qemu-utils qemu-system-x86 qemu-system-gui parted kmod xorriso sed coreutils git make curl build-essential gcc
```
  * Fedora
```
sudo dnf install qemu-img qemu-system-x86 parted kmod sed coreutils xorriso git make curl gcc
```

2. Run `build-iso.sh`.

## Details
The script will generate a Distro ISO. It may take a minute or two. The build script uses an automatic minimal install ISO to bootstrap a temporary virtual machine, copy over the contents of the repository to this VM, and then perform an auto-build process. During this process it reboots a few times, recompiles the Kernel, and then builds a Distro ISO. After the Distro ISO is built, the VM will power-off, and the Distro ISO will be copied off the temporary VM. The resulting ISO will be located in the `build` folder.

## Troubleshooting
If the `build-iso` script doesn't work, there are a few options. If you happen to have an existing VM, you could use the `sync` script to copy the repo contents directly over a VM's HDD. If the build process hangs immediately at _Copying to Distro/_, a fresh clone of the repo may fix it.
