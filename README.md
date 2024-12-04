# Hackintosh your Deskmini310
Install Hackintosh(Sonoma & Ventura & Monterey & Big Sur & Catalina) in Deskmini 310(i7-8700es QN8H)

## PC 配置
* CPU: i7-8700es QN8H
* 内存: 海力士 DDR4 2666MHz 8GB × 2
* 硬盘: 阿斯加德 AN2 250NVMe-M.2/80
* 无线网卡: BCM94360CS2（Sonoma 系统原生博通卡驱动已删除） 更换为 Intel WiFi 6E AX210
* 风扇: 猫头鹰 NH-L9i

## BIOS 配置
### 1. 重置 BIOS 为默认配置

### 2. 安装 macOS 所需配置
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

## 工作状态
* [x] CPU 变频，开启 HWP
* [x] 核显加速
* [x] 以太网
* [x] WIFI（务必替换为对应版本的 [AirportItlwm](https://github.com/OpenIntelWireless/itlwm)，否则无法开机）
* [x] 蓝牙
* [x] 声卡
* [x] USB 及 USB 扩展
* [x] DP/HDMI 双屏输出
* [x] 关机、重启、睡眠

## 提醒

* [AirportItlwm](https://github.com/OpenIntelWireless/itlwm) 务必替换为对应系统版本，否则无法开机
* 系统安装完, 请使用 OpenCore Configurator 生成 SMBIOS 序列号，否则无法登陆 App Store

## 更新日志

| 日期      | 详情                                                              |
|-----------|----------------------------------------------------------------------|
| 2024.12.04 | OpenCroe 1.0.3 |
| 2024.08.08 | OpenCroe 1.0.1 |
| 2024.05.28 | OpenCroe 1.0.0 |
| 2024.03.15 | OpenCroe 0.9.9 & Sonoma 14.4 升级注意事项：1、Misc-SecureBootModel 设置为 Disabled；2、关闭 AirportItlwm、IntelBTPatcher、IntelBluetoothFirmware、BlueToolFixup 驱动；3、成功升级后，还原 1、2 步设置|
| 2023.12.12 | OpenCroe 0.9.7 & 增加 RestrictEvents.kext 修复 OTA 升级问题 |
| 2023.10.11 | Sonoma 14.0 & 更换无线网卡为 Intel WiFi 6E AX210|
| 2023.10.09 | OpenCroe 0.9.5 |
| 2023.03.15 | OpenCroe 0.9.0 |
| 2023.01.04 | OpenCroe 0.8.8 |
| 2022.11.10 | OpenCroe 0.8.6 & Ventura 13.0|
| 2022.10.16 | OpenCroe 0.8.5 |
| 2022.09.06 | OpenCroe 0.8.4 |
| 2022.08.08 | OpenCroe 0.8.3 |
| 2022.07.06 | OpenCroe 0.8.2 |
| 2022.03.09 | OpenCroe 0.7.9 & 修复检测不到系统更新问题 |
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