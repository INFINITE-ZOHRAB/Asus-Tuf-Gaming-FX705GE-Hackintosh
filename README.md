# Hackintosh Project for Asus Tuf Gaming FX705GE

**Disclaimer:**
Applying Hackintosh on your Asus Tuf Gaming FX705GE can lead to an unstable system, and unexpected issues may occur. I take no responsibility for any damage, data loss, or malfunction caused by the use of this project. Proceed at your own risk.

## Version Info
| V.I.       | Type                                           |
| --------------- | ------------------------------------------------ |
| OC Version             | OC 0.9.3             |
| MacOs Tested             | Monterey, Ventura, Sonoma (Still in work)           |
| Status           | W.I.P                                |


## Components and Compatibility

- ✅ - Works
- ⚠️ - In Development/Partially Working/Left to Work Partially
- ❌ - Does Not Work

| Component       | Model                                           | Status             |
| --------------- | ------------------------------------------------ | --------------- |
| `CPU`             | Intel Core i7-8750H (Coffee Lake)             | ✅             |
| `GPU`             | NVidia Mobile 1050Ti (Unsupported)           | ❌             |
| `Audio`           | Realtek ALC233                                | ✅             |
| `Ethernet`        | Realtek RTL8168/8111                         | ✅             |
| `Wi-Fi (Formal Adapter)` | Intel Wireless-AC 9560                  | ⚠️             |
| `Wi-Fi (New Adapter)`    | Fenvi BCM94360NG                         | ✅             |
| `Bluetooth`      | Fenvi BCM94360NG                              | ✅             |
| `Touchpad`       | Trackpad ELAN1200 I2C-HID                    | ✅             |
| `Keyboard`       | Keyboard PS2                                 | ⚠️             |
| `Battery`        | Asus Default Battery                         | ✅             |
| `Webcam`         | USB2.0 HD UVC WebCam Internal                                              | ✅             |
| `Microphone`     | Realtek                                              | ✅             |
| `USB Ports`     | 3 USB 2.0                                              | ✅             |
| `Fans`           | 2 Fans                                              | ⚠️             |


| Function       | Status             |
| --------------- | --------------- |
| `Sleep/Wake/Shutdown`  | ✅             |
| `AirDrop`  | ✅             |
| `FaceTime/IMessage`  | ✅             |
| `AirPlay`  | ✅             |

| Storage       | Status             |
| --------------- | --------------- |
| `Samsung 970 Evo Plus 2TB`  | ⚠️             |
| `WD 2.5" HDD 1TB`  | ✅             |
| `SPCC 238GB`  | ✅             |


## Info about components with compatibility issues

### GPU
#### It is important to note that Apple hasn't released support for NVidia graphics and later for Higher macOS versions.

### Wi-Fi (Formal Adapter)
#### The Wi-Fi functionality remains partially unresolved due to the following reasons:
- Instability: macOS versions like Monterey, Ventura, and Sonoma have experienced crashes when attempting to connect to Wi-Fi, even after starting from scratch.
- Unfunctionality: The Wi-Fi card lacks support for features like Airdrop.
- Lack of Fixes: Despite attempts, there is no reliable solution to fully support the Wi-Fi card, making it unfeasible to continue debugging the issue.

### Keyboard
#### Although the keyboard itself works, the main issues are with FN keys mapping and Keyboard Backlight. Efforts are ongoing to address these issues, but progress may be limited due to other commitments.

### Fans
#### While fan control and readings have not been implemented yet, efforts are underway to develop a possible solution for this functionality.

## Todo
- [ ] Fix Fan control and readings.
- [ ] Fix Keyboard FN mapping and lights.

## Installation Procedures:
### 0. Familiarize Yourself with Opencore, Guides, and Hackintosh Overall.

#### 1. Prepare Your USB.
Follow the [Dortania Guide on Getting the USB Ready](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/).

#### 2. Unlock the CFG-Lock.
Follow the [Dortania Guide on CFG-Lock Unlock](https://dortania.github.io/OpenCore-Post-Install/misc/msr-lock.html).

#### 3. Generate SMBIOS for Your EFI.
Download the [GenSMBIOS tool](https://github.com/corpnewt/GenSMBIOS) and select `MacBookPro15,1` for proper functionality. Run the appropriate file for your OS platform (.bat for Windows). Choose options 1, 2, and 3 as instructed to install/update MacSerial, update your EFI's config.plist, and write all necessary info into the config.plist.

#### 4. Finalize the USB.
Drop the final EFI onto the root of the prepared USB.

#### 5. BIOS Configuration.
Enter the BIOS menu, select Advanced mode, and navigate to the Advanced Tab. Disable VT-d and set AHCI in Advanced\SATA Configuration. Disable Fast Boot in the Boot Tab. Save & Exit, then choose Save Changes and Exit.

#### 6. Boot.
Boot to the installation and follow the default procedure from the [Dortania Guide](https://dortania.github.io/OpenCore-Install-Guide/installation/installation-process.html#booting-the-opencore-usb).

## Gratitude

- [Dortania](https://dortania.github.io/) - For guides
- [Acidathera](https://github.com/acidanthera) - For OC and Kexts
- [RehabMan](https://github.com/RehabMan) - for ACPI Patching
- The Hackintosh community - for helping me with debugging the hackintosh.


Good luck with your project! If you have any further questions or need more assistance, don't hesitate to ask.
