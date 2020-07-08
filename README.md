# OpenCore Hackintosh for Asus ROG Strix Z390-E/Intel i5 9600k
# Full rebuild to OpenCore 0.5.9!
__OpenCore Version: 0.5.9__ MacOS Catalina by [OpenCore Guide](https://dortania.github.io/OpenCore-Desktop-Guide/)

## 📸 Screenshots
<details>
<summary>About Mac</summary>

![About](_resources/about.png)

</details>
<details>
<summary>Benchmarks</summary>

![Disk](_resources/disk.png)

![Cinebench](_resources/cinebench.png)

![Geekbench](_resources/geekbench.png)

</details>

## 📃 Hardware List
#### 🖥 Mac
* Motherboard: ASUS ROG STRIX Z390-E Gaming ATX (s-1151)
* CPU: Intel Core i5-9600K 3.7GHz/9MB (s-1151)
* GPU: Radeon RX 580 8GB DDR5 Sapphire Pulse
* RAM: Crucial Ballistic Sport LT Red  3200MHz (16x2)
* Memory: Samsung 970 EVO Plus 500GB
* WIFI/Bluetooth: [Fenvi T919](https://www.aliexpress.com/item/32778371977.html)
* Power: 650W Corsair RM650X
* CPU Cooler: Be Quite Dark Rock Pro 4
* Case: DeepCool Matrexx 55
* Monitor: LG UltraFine 27UL650-W 27’’
* Mouse: Logitech MXMaster 2S
* Keyboard: Varmilo VA108MAC

#### 🎮 Windows
* Kingston SKC400S37 128Gb
* WD Caviar Blue WD10EZEX 1 Tb

## 🔄 System status
✅ **Working**
* Audio
* APFS
* Sleep/Wake
* [USB](_usb_map/usb_table.md)
* App Store
* Facetime
* Bluetooth & Wi-Fi (via [Fenvi T919](https://www.aliexpress.com/item/32778371977.html))
* NVRAM
* Ethernet
* [NVMe](_resources/m2_info.png)

✳️ **Optional**
* Onboard Bluetooth. Try this [kext](https://github.com/zxystd/IntelBluetoothFirmware).

## ❗️❗️ Before Use
**INPORTANT!**
1. You __must__ replace SMBIOS info in ```config.plist -> PlatformInfo -> Generic```. Use this simple [guide](https://dortania.github.io/OpenCore-Desktop-Guide/post-install/iservices.html#generate-a-new-serial).
2. Check [M.2 slots setup](_resources/m2_info.png).

## ⚙️ BIOS
First of all update your BIOS to the latest version.
Then follow the list:

|Option|Flag|
|-|-|
|Fast Boot | disable|
|SecureBoot | disable
|VT-d | disable
|CSM | disable
|CFG-Lock | disable
|Serial Port | disable
|WiFi & Bluetooth | disable
|Above 4G | enable
|XHCI Hand-off | enable
|OS Type | windows |
|XMP II profile (optional)| enable|

## 😇 Config Sanity
You can check config sanity [here](https://opencore.slowgeek.com/?file=coffeelake059Uy7glO&rs=coffeelake059).

## 🗺 USB Map
Build has a USBMap.kext.

Check [usb table](_usb_map/usb_table.md) for details.

## 🛠 Tools
Must have OpenCore hackintosher's tools:
* [MountEFI](https://github.com/corpnewt/MountEFI) - Helps to mount /EFI folder
* [ProperTree](https://github.com/corpnewt/MountEFI) - A way to open config.plist
* [USBMap](https://github.com/corpnewt/USBMap) - Tool to make a usb map
* [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) - Apple seral generator
* [Lilu-and-Friends](https://github.com/corpnewt/Lilu-and-Friends) - To update kexts
* [OCConfigCompare](https://github.com/corpnewt/OCConfigCompare) - To update OC

## 📩 Contacts
Config by [@lbrdev](https://github.com/lbrdev)

Email - lbrdev.contact@gmail.com
