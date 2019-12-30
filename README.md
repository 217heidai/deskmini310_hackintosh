# Hackintosh your Deskmini310

## Configuration

| Specifications | Detail                                                                                    |
|----------------|-------------------------------------------------------------------------------------------|
| CPU            | Intel i7-8700es QN8H                                                                      |
| RAM            | SK Hynix DDR4 2666MHz 8GB × 2                                                             |
| SSD            | Asgard AN2 250NVMe-M.2/80                                                                 |
| WIFI/BT        | BCM94360CS2                                                                               |
| Cooler         | Noctua NH-L9i                                                                             |

## BIOS
### For macOS
* Advanced
  * Chipset Configuration
    * Onboard HD Audio: Enabled
  * USB Configuration
    * XHCI Hand-off: Enabled
  * Super IO Configuration
    * Serial Port: Disabled  
* Security
  * Secure Boot: Disabled(by default)

### For Intel HWP
* Advanced
  * CPU Configuration
    * CPU C States Support: Enabled
    * CFG Lock: Disabled

### Other Configurations by default

## Works

* [x] Ethernet/WIFI/Bluetooth/Audio/USB&EX-USB/Sensors

* [x] DP/HDMI dual monitor output

* [x] Shutdown、Sleep

## Notes

* After macOS installed done ([Installation Guide](https://www.tonymacx86.com/threads/unibeast-install-macos-mojave-on-any-supported-intel-based-pc.259381/)), please open `config.plist` and  fill few SMBIOS info by Clover Configurator.

* If you need to move CLOVER/kexts/Other/* to /L/E&/S/L/E, please modify `InjectKexts` to `Detect` in `config.plist` by Clover Configurator.

## Tips

* If you use `Chrome` , it is recommended to turn off `Chrome` completely when using `IGPU` operations(PS/FCP etc).[Chrome causing Final Cut Pro X to slow down, freeze, and crash](https://appleinsider.com/articles/19/06/20/chrome-causing-final-cut-pro-x-to-freeze-and-crash)

## Issues

Occasionally reboot, but I think this is an inevitable problem for Hackintosh , Fortunately, it happens very rarely.

## Why Hackintosh

Because We Can！

## ChangeLog

If there is an infinite reboot after upgrading efi, unplug the power and wait for a few seconds before powering up.

| Date      | Content                                                              |
|-----------|----------------------------------------------------------------------|
| 2019.12.30 | clover 5102             |
| 2019.12.23 | clover 5101             |
| 2019.12.11 | clover 5100 & Intel HWP |