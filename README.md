# Hackintosh your Deskmini310
Install Hackintosh(Ventura & Monterey & Big Sur & Catalina) in Deskmini 310(i7-8700es QN8H)

[中文 Chinese](./README_zh.md)

## Configuration

| Specifications | Detail                                                                                    |
|----------------|-------------------------------------------------------------------------------------------|
| CPU            | Intel i7-8700es QN8H                                                                      |
| RAM            | SK Hynix DDR4 2666MHz 8GB × 2                                                             |
| SSD            | Asgard AN2 250NVMe-M.2/80                                                                 |
| WIFI/BT        | BCM94360CS2                                                                               |
| Cooler         | Noctua NH-L9i                                                                             |

## BIOS
* Advanced
  * CPU Configuration
    * CPU C States Support: Enabled
    * CFG Lock: Disabled
  * Chipset Configuration
    * Onboard HD Audio: Enabled
    * Onboard HDMI HD Audio: Enabled
  * USB Configuration
    * XHCI Hand-off: Enabled
  * Super IO Configuration
    * Serial Port: Disabled  
* Security
  * Secure Boot: Disabled
* BOOT
  * CSM: Disabled

### Other Configurations by default

## Works

* [x] Ethernet/WIFI/Bluetooth/Audio/USB&EX-USB/Sensors

* [x] DP/HDMI dual monitor output

* [x] Shutdown、Sleep

## Notes

* After macOS installed done, please open `config.plist` and fill new SMBIOS info by OpenCore Configurator.

## Why Hackintosh

Because We Can！

## ChangeLog

If there is an infinite reboot after upgrading efi, unplug the power and wait for a few seconds before powering up.

| Date      | Content                                                              |
|-----------|----------------------------------------------------------------------|
| 2023.10.09 | OpenCroe 0.9.5 |
| 2023.03.15 | OpenCroe 0.9.0 |
| 2023.01.04 | OpenCroe 0.8.8 |
| 2022.11.10 | OpenCroe 0.8.6 & Ventura 13.0|
| 2022.10.16 | OpenCroe 0.8.5 |
| 2022.09.06 | OpenCroe 0.8.4 |
| 2022.08.08 | OpenCroe 0.8.3 |
| 2022.07.06 | OpenCroe 0.8.2 |
| 2022.03.09 | OpenCroe 0.7.9 & Repair system automatic updates |
| 2022.02.09 | OpenCroe 0.7.8 |
| 2022.01.11 | OpenCroe 0.7.7 |
| 2021.12.07 | OpenCroe 0.7.6 |
| 2021.11.02 | OpenCroe 0.7.5 & Monterey 12.0.1 |
| 2021.10.09 | OpenCroe 0.7.4 & Monterey 12.0 Beta 9 |
| 2021.09.07 | OpenCroe 0.7.3 & Monterey 12.0 Beta 6 |
| 2021.08.11 | OpenCroe 0.7.2 & Monterey 12.0 Beta 4 |
| 2021.07.06 | OpenCroe 0.7.1 & Monterey 12.0 Beta 2 |
| 2021.06.08 | OpenCroe 0.7.0 & Big Sur 11.4 |
| 2021.05.11 | OpenCroe 0.6.9 & Big Sur 11.3 |
| 2021.04.06 | OpenCroe 0.6.8 & Big Sur 11.2.3 |
| 2021.03.03 | OpenCroe 0.6.7 & Big Sur 11.2.2 |
| 2021.02.03 | OpenCroe 0.6.6 & Big Sur 11.2 |
| 2021.01.05 | OpenCroe 0.6.5 |
| 2020.12.08 | OpenCroe 0.6.4 & Big Sur 11.1 |
| 2020.11.03 | OpenCroe 0.6.3 & Big Sur 11.0.1 RC 1 |
| 2020.10.09 | OpenCroe 0.6.2 & Big Sur 11.0 Beta 9 |
| 2020.09.08 | OpenCroe 0.6.1 |
| 2020.08.24 | update to Big Sur 11.0 Beta |
| 2020.08.04 | OpenCroe 0.6.0 |
| 2020.06.03 | OpenCroe 0.5.9 |
| 2020.05.09 | replace Clover with OpenCroe 0.5.8 |
| 2020.03.30 | clover 5107 |
| 2020.02.21 | clover 5104 |
| 2020.01.08 | clover 5103 |
| 2020.01.03 | clover 5102 |
| 2019.12.23 | clover 5101 |
| 2019.12.11 | clover 5100 |