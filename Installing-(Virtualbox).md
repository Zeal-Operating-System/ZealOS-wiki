1. Create a new virtual machine.
  * VM Type: **Other**, VM Version: **Other/Unknown (64-bit)**.
  * RAM: At least **512MB**.
  * Hard disk: At least **512MB**.
2. Open the Settings menu for the virtual machine.
  * In the **Storage** section, add a new AHCI storage controller.
  * Drag-and-drop the virtual hard disk and optical drives from the IDE controller to the AHCI controller.
  * Delete the IDE controller.
  * Select the virtual optical drive, and assign it the ZealOS ISO.
  * For improved performance, check the **Use Host I/O Cache** checkbox.
3. Start the VM.
4. Press any key to dismiss the splash screen.
5. Type `Y` when asked if you want to install onto a hard drive.
6. Type `I` when asked if you want to upgrade or create a new install.
7. After installation is complete, type `Y` to reboot. The disc will auto-eject.