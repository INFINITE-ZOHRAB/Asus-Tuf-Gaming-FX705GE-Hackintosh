# Hackintosh Project for Asus Tuf Gaming FX705GE

**Disclaimer:**
Applying Hackintosh on your Asus Tuf Gaming FX705GE can lead to an unstable system, and unexpected issues may occur. I take no responsibility for any damage, data loss, or malfunction caused by the use of this project. Proceed at your own risk.

## Version Info

| Opencore Version        | 0.9.3 Release           |
| MacOs Versions        | Tested/Works/           |

## Components and Compatibility

- ✅ - Works
- ⚠️ - In Development/Partially working/Left to work partially
- ❌ - Does not work

| Component         | Status           |
| ----------------- | ---------------- |
| CPU               | Intel Core i7-8750H (Coffee Lake) ✅     |
| GPU               | NVidia Mobile 1050Ti (UnSupported) ❌     |
| Audio             | Realtek ALC233 ✅     |
| Ethernet          | Realtek RTL8168/8111 ✅     |
| Wi-Fi (Formal Adapter)             | Intel Wireless-AC 9560 ⚠️      |
| Wi-Fi (New Adapter)             | Fenvi BCM94360NG ✅      |
| Bluetooth         | Fenvi BCM94360NG ✅      |
| Touchpad          | Trackpad ELAN1200 I2C-HID ✅      |
| Keyboard          | Keyboard PS2 ⚠️      |
| Battery           | Asus Default Battery ✅      |
| Sleep/Wake/Shutdown        | ✅      |
| Webcam  | ✅      |
| Microphone  | ✅      |
| USB Ports  | ✅      |
| Fans  | ⚠️      |

## Info about components with compatibility issues

### GPU
#### Pretty much obvious, Apple hasn't released support for NVidia graphics and later for Higher MacOS.

### Wi-Fi (Formal Adapter)
#### Reason for ticking it as left to work partially was due to 3 main reasons: Instability, unfunctional and lack of possiblities for fix.
- Instability : Monterey, Ventura, and Sonoma MacOS have experience same issue: Sudden crashes from attempting to connect Wi-Fi. May it have been my user mistake, but with no avail it just wouldn't work. Even if I start from scratch. Also as for bluetooth, same issue here where as instead the audio and activation worked poorly. If bluetooth was to be deactivated, turning it back on would be impossible unless the machine was rebooted. I as well would like to mark that Wireless Headphones on the machine's bluetooth were horrible, Facetime audio would end up being some gargling glitching sounds, and etc.
- Unfunctionality : Says for itself, no airdrop support.
- Lack of fixes : May some have found solution, I will not implement it on the machine again since it's not worth debugging the not-fully-support Wi-Fi card to make it work properly.

### Keyboard
#### While the keyboard itself was working, keys function as needed, FN keys work properly. The main issues in it are the FN keys mapping and Keyboard Backlight. I will attempt to fix it while I can since later on I will be very busy.

### Fans
#### I would describe them totally not working since I have implemented any attempts, but marking them as in development would be correctly as I am working on a possible solution for fan control and readings.

## Todo
- [ ] Fix Fans control and reading.
- [ ] Fix Keyboard Fn mapping and lights

## Instructions for Use

1. **Step 1:** [Add your instructions here]
2. **Step 2:** [Add your instructions here]
3. **Step 3:** [Add your instructions here]
4. **Step 4:** [Add your instructions here]

Feel free to customize the instructions based on your project's specific needs.

## To-Do List

- [ ] Add detailed troubleshooting section.
- [ ] Include compatibility charts for different macOS versions.
- [ ] Provide a guide for creating a bootable USB.
- [ ] Add instructions for post-installation tweaks.
- [ ] Incorporate community feedback and contributions.

## Credits

Special thanks to the following contributors for their support and efforts in this project:

- [Contributor 1 Name](link to profile)
- [Contributor 2 Name](link to profile)
- [Contributor 3 Name](link to profile)

Your contributions are greatly appreciated!

---

Feel free to modify and expand on this template as needed to best suit your Hackintosh project. Good luck with your project! If you have any further questions or need more assistance, don't hesitate to ask.
