# Instructions
1. Make sure you have the commands: `qemu-img`, `qemu-nbd`, `qemu-system-x86_64`, `partprobe`, and `modprobe`.

If you do not have these commands and are on a Linux system like Ubuntu, try installing these packages:

`sudo apt install qemu-utils qemu-system-x86 qemu-system-common qemu-system-data qemu-system-gui parted kmod`

2. Enter the `build/` folder, and run `build_iso.sh`.

The script will generate a Distro ISO. It may take a minute or two. The build script uses an automatic minimal install ISO to bootstrap a temporary virtual machine, copy over the contents of the repository to this VM, and then perform an auto-build process. During this process it reboots a few times, recompiles the Kernel, and then builds a Distro ISO. After the Distro ISO is built, the VM will poweroff, and the Distro ISO will be copied off the temporary VM. The resulting ISO will be located in the `build/` folder.

# Troubleshooting
If the `build_iso.sh` script doesn't work, there are a few options. If you happen to have an existing VM, you could use `sync_vm.sh` to copy the repo contents directly over a VM's HDD. If the build process hangs immediately at _Copying to Distro/_, a fresh clone of the repo may fix it.