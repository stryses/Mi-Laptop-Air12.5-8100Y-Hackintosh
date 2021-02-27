# Xiaomi Air 12.5(2019) 8100Y Macintosh
**Opencore 0.6.6** Config and Drivers of Mi Laptop Air 12.5(2019) 8100Y

Mac Version: 10.15.7 (Maybe in normal use in 11.0.0 , i have not test)

Create Time: 2020/10/11

Update Time: 2021/02/28

**I will update the kext irregularly without regularity.**

Github:https://github.com/stryses/Xiaomi-Air12.5-8100Y-Macintosh

Gitee[中文]：https://gitee.com/likt/xiaomi-air12.5-8100y-macintosh

# Can I use?

This is my hardware report , if you same with me , you can download all the file use it directly.

| Item     | Value                               |
| -------- | ----------------------------------- |
| CPU      | DualCore Intel Core m3-8100Y        |
| GPU      | Intel UHD Graphics 615              |
| Audio    | Realtek ALC233                      |
| LAN      | Intel(R) Dual Band Wireless-AC 8265 |
| Optional | M.2 [NVME] SSD                      |

# What's this?

In order to boot Mac on not Apple Notebook , we need some special way to achieve it.

The resository include:

- Opencore and the Config for Xiaomi Air12.5(2019)
- Some of essential Kext
- Some Patch of DSDT

# What's work?

Based on my usage feedback  ,  following functions can be used normally:

- Intel UHD Graphics 615  **[Based on Whatevergreen]**
- Brightness Adjustment  **[Based on DSDT]**
- Realtek ALC233 Audio I/O  **[Based on AppleALC]**
- Keyboard , Touchpad  **[Based on VoodooI2C]**
- HDMI
- Wireless Network Support  **[Based on AirportItlwm]**
- Bluetooth **[Based on IntelBluetoothFirmware]**
- SpeedStepping  **[Based on CPUFriend]**
- Internal Camera  **[Based on USBPorts]**
- USB 3.0
- Battery Status  **[Based on DSDT]**
- Sleep

# What's Problem?

- Sometime touchpad will use abnormal , but can solve it. [Restart or sleep completely then wake up]
- **NONE** , now i use it as my major system to use.

# What including in this repo?

- AirportItlwm **[Catalina Version]** (v1.2.0 / 15 Jan)
- AppleALC (1.5.7 / 3 Feb)
- CPUFriend (1.2.3 / 5 Jan)
- DisableTurboBoostBattery [you can remove it]
- HibernationFixup (1.3.9 / 5 Jan)
- IntelBluetoothFirmware (1.1.2 / 3 Aug 2020)
- IntelBluetoothInjector (1.1.2 / 3 Aug 2020)
- Lilu (1.5.1 / 3 Feb)
- NVMEFix (1.0.5 / 5 Jan)
- USBPorts
- VirtualSMC [with SMCBatteryManager & SMCProcessor] (1.2.0 / 3 Feb)
- VoodooI2C [with VoodooI2CSynaptics] (2.6.4 / 7 Feb)
- VoodooPS2Controller (2.2.1 / 3 Feb)
- WhateverGreen  (1.4.7 / 3 Feb)

# What should you know?

## About HiDPI

Please search **one-key-hidpi**  in github to use it.

## About System Update

Most of the time you can update the system directly if its non cross release upgrades.

## About Touchpad can't use in normal

1. Restart in macOS
2. Sleep , and wake up in few seconds.

# Update Logs

##  20200228 Release

- Init Repositories
- Update all kexts to latest version