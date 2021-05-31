# BigSur Gigabyte Z390 Aorus Master (OpenCore)

[![OpenCore](https://img.shields.io/badge/OpenCore-0.6.9-blue.svg)](https://github.com/acidanthera/OpenCorePkg)
[![macOS-Unstable](https://img.shields.io/badge/macOS-11.4.0-brightgreen.svg)](https://www.apple.com/macos/big-sur)

I follow by [this guide](https://www.insanelymac.com/forum/topic/340936-audiogods-aorus-z390-master-patched-dsdt-efi-for-catalina-mini-guide-and-discussion/ )

## My PC Build
<details>
  <summary><strong>Hardware</strong></summary>
  
  | Category          | Component                                                | Note                                                  |
  | ----------------- | -------------------------------------------------------  | ----------------------------------------------------- |
  | CPU               | Intel Core i9-9900K                                      |                                                       |
  | GPU               | MSI Radeon RX 5700 XT EVOKE OC Graphics Board            | Native support                                        |
  | Motherboard       | Gigabyte Z390 AORUS MASTER                               |                                                       |
  | Storage (macOS)   | Samsung T7 500GB SSD (`USB3.1` Front Panel)              | External. Use USB Type-C Front Panel                  |
  | Storage (Windows) | Crucial P1 500GB 3D NAND NVMe PCIe (`M2M` slot)          |                                                       |
  | Memory            | Corsair Vengeance LPX 32GB (2x16GB) 3200MHz DDR4         |                                                       |
  | CPU Cooler        | EKWB EK-KIT Performance Series PC Watercooling Kit P360  |                                                       |
  | Power Supply      | Corsair RMX Series 80PLUS Gold 1000W                     |                                                       |
  | Case              | Cooler Master MasterCase H500M ARGB                      |                                                       |
  | Monitor           | Dell Display Monitor SE2416H 23.8inches                  |                                                       |
  | LAN               | Intel® i219v GbE LAN                                     | I use LAN for network                                 |
  | Wifi & BT         | Intel® CNVi 802.11ac 2x2 Wave 2 WIFI & BT5  (on-board)   | I just use bluetooth for JBL FLIP 5 Speaker.          |
  |                   | Include **Intel Wireless-AC 9560** module inside         | If you want native wifi control.                      |
  |                   |                                                          | Use AirportItlwm instead but slow [speed](image)      |
  |                   |                                                          | Use Itlwm and HeliPort for increase wifi speed        |
  
</details>

<details>

<summary><strong>Kernel extensions</strong></summary>
<br>

| Kext                   | Version        |
|:---------------------- | -------------- |
| Lilu                   | 1.5.3          |
| VirtualSMC             | 1.2.3          |
| WhateverGreen          | 1.4.9          |
| AppleALC               | 1.6.0          |
| IntelBluetoothFirmware | 1.1.2          |
| IntelBluetoothInjector | 1.1.2          |
| IntelMausi             | 1.0.6          |
| SMCProcessor           | 1.2.3          |
| SMCSuperIO             | 1.2.3          |
| USBMap                 | Manual         |
| itlwm                  | 1.3.0          |



</details>

<details>
  <summary><strong>Working ✅ / Not Working ☑️</strong></summary>
  
  * ✅ Ethernet
  * ✅ Onboard Audio
  * ✅ iMessage
  * ✅ Sleep/Wake
  * ✅ Bluetooth & Wi-Fi
  * ☑️ Airdrop
  * ☑️ Handoff
  
</details>

# Resources

* [Dortania's OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/)
* [Wifi-Bluetooth](https://openintelwireless.github.io/General/Installation.html)

# Tools
* [Hackintool](https://github.com/headkaze/Hackintool)
* [OpenCore Configurator](https://mackie100projects.altervista.org/opencore-configurator/)
* [OC X Gen](https://github.com/Pavo-IM/OC-Gen-X)
* [Wifi-Bluetooth kext](https://github.com/OpenIntelWireless)


# Thanks
* [cmer](https://github.com/cmer) : this is the first guide that I followed and try with Catalina 10.15.1
* [AudioGod](https://www.insanelymac.com/forum/topic/340936-audiogods-aorus-z390-master-patched-dsdt-efi-for-catalina-mini-guide-and-discussion/) : Currently, I use from him and change a little bit to make something well.
* [Colin Sullender](https://github.com/shiruken) : Previous, I try many times but cannot boot into Macintosh. Thanks for using Intel CNVI in your system. I just rebuild USB Map kext and everything works.
