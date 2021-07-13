1. Create a new virtual machine.
  * Select **Use ISO image** and assign it the ZealOS ISO when asked where you'll install the operating system from.
  * Guest OS Type: **Other**, VM Version: **Other 64-bit**.
  * Hard disk: At least **512MB**.
2. Click **Customize Hardware...**
  * RAM: **1GB or more** recommended. At least **512MB**.
  * Click **New CD/DVD**, then click **Advanced...**
  * Change CD/DVD drive from IDE to **SATA**.
  * Exit VM Settings, click **Finish** to end VM setup.
3. If the VM automatically starts up, shut it down.
4. Edit the VM Settings.
  * Click **Add...**, select **Hard Disk**.
  * Select **SATA** type.
  * Select **Use an existing virtual disk**.
  * Choose the virtual hard drive file used by the IDE hard drive.
  * Select the IDE hard drive and click **Remove**.
5. Start the VM.
6. Press any key to dismiss the splash screen.
7. Type `Y` when asked if you want to install onto a hard drive.
8. Type `I` when asked if you want to upgrade or create a new install.
9. After installation is complete, type `Y` to reboot. The disc will auto-eject.