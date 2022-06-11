# LG Gram 13/15/17Z990 Hackintosh
Try, why not? Just for your Gram.
## Settings
|      | Information   |
| ---- | -----------------------------------------|
| Model | LG Gram 13/15/17Z990|
| CPU  | Intel Core i7-8265U (Whiskey Lake)|
| Graphics Card | Intel UHD Graphics 620 (Integrated)|
| RAM | 8G (Pre-installed)|
| SSD | Samsung (Don't know exact model) 256GB|
| Sound Card | Conexant CX8200|
| Wireless Card | Intel AC-9560|
| Bluetooth Card | Intel AC-9560|
| What can be replaced? | SSD, RAM (one more slot for each)|

## Which macOS Version can be installed?
- macOS 12.0.1
<br>Warning! Big Sur cannot be installed as this EFI was designed for Monterey

## What's Working?
- [x] WiFi/Bluetooth (Intel)
- [x] Touchpad
- [x] Sleep
- [x] Keyboard
- [x] AirPlay / Handoff (handoff w/ iCloud account)
- [x] Boot Speed (perfect, 10~15 sec)
- [x] USB Ports (working, but with slow connecting speed)
- [x] Headphone
- [x] Graphic Acceleration

## Not working
- [ ] Broadcom Cards (Not confirmed)
- [ ] Fn Keys (partially working)
- [ ] AirDrop (working on it)
- [ ] SD Card / HDMI (Not tested, but will work)
- [ ] Thunderbolt 3 (will fix soon if possible)

## How to Install (Pt. 1 / BIOS Setting)
- Enter BIOS with F2 (press like crazy person)
  1. Enable Secret Settings (Ctrl + Alt + F7)
  2. BIOS - Main - Boot Features - ***CMS Support [NO]*** (IMPORTANT)
  3. BIOS - Advanced - Intel Advanced Menu - Power & Performance - CPU Power Management Control - ***CFG Lock [Disabled]*** (IMPORTANT)
## How to Install (Pt. 2 / Make Bootable Disk)
- Download ghost image, if you're korean then go to x86.co.kr to get it!
- Check out https://medium.com/swlh/pc-laptop-create-a-hackintosh-usb-stick-e11a03ca371f if you don't have ghost image!
  1. Warning! Only follow part 2
  2. For Part 3, just download EFI files and replace old EFI with downloaded EFI
## After install
- Some settings after you installed whole macOS, please follow this
  1. Settings - Trackpad - Turn off Force Click
  2. Download OpenCore Configurator
  3. OpenCore Configurator - Tools - Mount EFI
  4. Replace EFI w/ mine
  5. EFI Folder - OC Folder - open config.plist with OpenCore Configurator
  6. Go to PlatformInfo and generate serial number, other things and save & reboot!
<br> That's it!

## AirDrop Dilemma
You have 2 options and one of these can enable AirDrop and another one can't (maybe, not confirmed)
<br>First option: Get BCM94360CS2 with M.2 Adapter, attach on M.2 Slot (SSD) and sacrifice USB Port for BT and AirDrop
<br>Second option (not confirmed): Get BCM94360CS2 with M.2 Adapter, attach on M.2 Slot (SSD) and just use Intel BT

## Changelog

### 2021.11.12 Pre-release V0.1 (Stable, no AirDrop)

* Initial Release
* Some bugs
* Stable

## References
From @zirenxiao (LG-Gram-13Z990A-Hackintosh)
<br>Thx to @zirenxiao for providing knowledge to me also BIOS Settings Guide and stable EFI for Big Sur

## Support Me!
Not related to money, but just share your screenshots and please leave the URL (my github repo) if you are sharing this EFI!
<br>Also there's a channel for this repo, TG @gram19_hackin for any updates soon!
<br> Thank you for using my EFI!
