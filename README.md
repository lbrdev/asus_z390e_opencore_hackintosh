# OpenCore Hackintosh for Asus ROG Strix Z390-E/Intel i5 9600k
__Version: 0.5.8__
Catalina build by [OpenCore Guide](https://dortania.github.io/OpenCore-Desktop-Guide/)

![About](_resources/info.png)

## Hardware List
#### Mac
* Motherboard: ASUS ROG STRIX Z390-E Gaming ATX (s-1151)
* CPU: Intel Core i5-9600K 3.7GHz/9MB (s-1151)
* GPU: Radeon RX 580 8GB DDR5 Sapphire Pulse
* RAM: Crucial Ballistic Sport LT Red  3200MHz (16x2)
* Memory: Samsung 970 EVO Plus 500GB
* WIFI/Bluetooth: Fenvi T919
* Power: 650W Corsair RM650X
* CPU Cooler: Be Quite Dark Rock Pro 4
* Case: DeepCool Matrexx 55
* Monitor: LG UltraFine 27UL650-W 27’’
* Mouse: Logitech MXMaster 2S
* Keyboard: Varmilo VA108MAC

#### Windows
* Kingston SKC400S37 128Gb
* WD Caviar Blue WD10EZEX 1 Tb

## System status
**Working**
* Audio
* APFS
* Sleep/Wake
* USB
* iMessage
* App Store
* Facetime
* APFS
* Handoff
* Bluetooth & Wi-Fi (via Fenvi t919)
* Continuity
* NVRAM

**Optional**
* Onboard Bluetooth. Try this [kext](https://github.com/zxystd/IntelBluetoothFirmware).

**Not Yet Tested**
* Built-in WIFI. Didn’t even try.

## Config Sanity
You can check my config [here](https://opencore.slowgeek.com/?file=coffeelake058XbuMHG&rs=coffeelake058).
Warnings description:
* ProtectUefiServices - Should be enabled for z390 by guide
* DisableRtcChecksum - To fix POSTed
* PickerMode - I'am using external Apple-like picker
* BootProtect - To disable bios boot override
* prev-lang:kbd - I'am Russian

## USB Map
~For now I am using a SSDT-UIAC for that, but kext folder contains USBMap.kext with my custom map. It’s should be updated for change Bluetooth to internal, just use SSDT.~
Updated to USBMap.kext. Check my [usb table](usb_table.md).

## Before Use
**INPORTANT!**
Change SMBIOS info for yours (config.plist/PlatformInfo/Generic). You can use this [guide](https://dortania.github.io/OpenCore-Desktop-Guide/post-install/iservices.html).

~EFI folder contains Windows Bootloader and entry in config.plist/Misc/Entries for launch it. Change path or remove if needed.~

## Improvements list
My list for future
* ~Remove Windows boot loader for drop-in~
* Add BIOS configuration
* ~Remap USB for deleting UIAC~


## Contacts
My email for questions - lbrdev.contact@gmail.com
