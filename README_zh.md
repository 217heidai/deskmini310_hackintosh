# Hackintosh your Deskmini310

[英文 English](./README.md)

## PC 配置
* CPU: i7-8700es QN8H
* 内存: 海力士 DDR4 2666MHz 8GB × 2
* 硬盘: 阿斯加德 AN2 250NVMe-M.2/80
* 无线网卡: 拆机卡 BCM94360CS2，支持 2.4G & 5G 双频 WIFI、蓝牙 4.0，需要安装转接卡
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
* [x] 以太网、WIFI
* [x] 蓝牙
* [x] 声卡
* [x] USB 及 USB 扩展
* [x] DP/HDMI 双屏输出
* [x] 关机、重启、睡眠

## 提醒

* 系统安装完, 请使用 OpenCore Configurator 生成 SMBIOS 序列号，否则无法登陆 App Store

## 更新日志

| 日期      | 详情                                                              |
|-----------|----------------------------------------------------------------------|
| 2020.12.08 | OpenCroe 0.6.4 & Big Sur 11.1 Beta 2|
| 2020.11.13 | OpenCroe 0.6.4 Beta & Big Sur 11.0.1|
| 2020.11.11 | OpenCroe 0.6.4 Beta & Big Sur 11.0.1 RC 2|
| 2020.11.03 | OpenCroe 0.6.3 & Big Sur 11.0.1 RC 1|
| 2020.10.09 | OpenCroe 0.6.2 & Big Sur Beta 9|
| 2020.09.08 | OpenCroe 0.6.1 |
| 2020.08.24 | update to Big Sur Beta |
| 2020.08.04 | OpenCroe 0.6.0 |
| 2020.06.03 | OpenCroe 0.5.9 |
| 2020.05.09 | replace Clover with OpenCroe 0.5.8 |
| 2020.03.30 | clover 5107 |
| 2020.02.21 | clover 5104 |
| 2020.01.08 | clover 5103 |
| 2020.01.03 | clover 5102 |
| 2019.12.23 | clover 5101 |
| 2019.12.11 | clover 5100 |