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
  * Chipset Configuration
    * Onboard HD Audio: Enabled
  * USB Configuration
    * XHCI Hand-off: Enabled
  * Super IO Configuration
    * Serial Port: Disabled  
* Security
  * Secure Boot: Disabled

### 3. 开启 Intel CPU 原生电源管理所需配置
* Advanced
  * CPU Configuration
    * CPU C States Support: Enabled
    * CFG Lock: Disabled

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

* 系统安装完, 请使用 Clover Configurator 生成 SMBIOS 序列号，否则无法登陆 App Store

## 更新日志

| 日期      | 详情                                                              |
|-----------|----------------------------------------------------------------------|
| 2020.02.21 | 更新 clover 5104、AppleALC、VirtualSMC |
| 2020.01.14 | 更新 AppleALC、Lilu、VirtualSMC、WhateverGreen |
| 2020.01.08 | 更新 clover 5103，使用OsxAptioFix3Drv替换AptioMemoryFix，使用VBoxHfs替换HFSPlus |
| 2020.01.03 | 更新 clover 5102 |
| 2019.12.23 | 更新 clover 5101 |
| 2019.12.11 | 更新 clover 5100，开启 Intel HWP |