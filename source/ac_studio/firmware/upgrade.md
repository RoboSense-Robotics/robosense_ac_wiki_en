# Upgrade

## Prerequisite
1. Make sure Active Camera is connected via USB interface to the host machine.
2. Install the latest version of R&D Viewer tool on your PC, refer to 6.1 for installation guide.
3. Download the firmware zip file in 6.1. After decompressed, you should get both `xxxx_application.bin` and `xxxx_system.bin` (Note: `xxxxx` depends on the version of the downloaded firmware).

## Upgrade Steps
1. Version Verification
  - Run R&D Viewer.
  - Click **Version** button to check the version of the current firmware to ensure  Active Camera is connected correctly.
2. Update Application Layer
  - Click **Select** button and choose the `xxxxx_ota_application.bin` file.
  - Click the **OTA** button to start flashing the application layer.
  - Wait until a dialog window pops up and  says upgraded successfully and the device will reboot by itself. Note that do not unplug the power supply during flashing and rebooting. 
3. Update System Layer
  - Click **Select** button, and choose the `xxxxx_ota_system.bin` file.
  - Click the **OTA** button to start upgrading the application layer.
  - Wait until a dialog window pops up and  says upgraded successfully and the device will reboot by itself. Note that do not unplug the power supply during flashing and rebooting. 
4. Update Verification
  - Click the **Version** button to check if the desired version of firmware is successfully flashed.
