# 🌟 OnePlus Nord 4 Custom Kernel Guide

## 📎 Useful Links

[![Static Badge](https://img.shields.io/badge/OnePlus%20Kernel%20Manifest%20Nord%204-EB0029?style=for-the-badge&logo=OnePlus)](https://github.com/OnePlusOSS/kernel_manifest/tree/oneplus/sm7675)   [![Static Badge](https://img.shields.io/badge/Follow-Telegram_Updates_Channel-blue?style=for-the-badge&logo=Telegram)](https://t.me/luffyop_updates)  [![Static Badge](https://img.shields.io/badge/OnePlus_Nord_4-Boot_Image_Channel-blue?style=for-the-badge&logo=Telegram)](https://t.me/boot_imgs_nord4/2)

## ⚡ Requirements

- **Unlocked Bootloader** 🔓  
- Make sure to check your compatible **OxygenOS version** in the kernel’s release notes.
- **Working Brain** 🧠

## 🧩 Required Modules

- **[Susfs Module](https://github.com/sidex15/susfs4ksu-module/releases)**
- *For ZRAM users:* Download the ZRAM module from the specific kernel’s release section (**see caution!**)

> ⚠️ **CAUTION**
> - Do **NOT** install modules during root-preserving updates!
> - **Press Volume Down** when installing any module!
> - If you enabled ZRAM, install the **ZRAM module BEFORE rebooting** after using AnyKernel3.
> - Important: If you plan to use this repository to build the 5.10 kernel, please note that ZRAM is not supported for this version, as the zram.ko module path is unavailable. However, the AnyKernel3-generated output remains functional and can still be used.

## 🚀 How To Flash / Update

### 🔥 Flashing the Kernel

- Get [Kernel Flasher](https://github.com/fatalcoder524/KernelFlasher/releases) (recommended for ease & safety!)

### ♻️ Updating Without Losing Root

#### 🧲 Method 1: Magisk or KernelSU (LKM) Users

1. Download **full OTA** update for your device.
2. Install via device’s **Local Update** feature.
3. _Before restarting:_
   - Open **Magisk/KernelSU**
   - Tap **Install → Install to Inactive Slot (After OTA)**
4. Go back to updater and tap **Restart**.

💡 *Result: Your device reboots with update and root still present!*

#### 🛡️ Method 2: Custom Kernel Users (Custom Kernel with SUSFS)

1. Download the **full OTA** update.
2. Install it using **Local Update**.
3. _Before restarting:_
   - Open **Kernel Flasher**
   - **Flash AnyKernel3 (AK3)** to the inactive slot—don’t pick other options!
4. Return to updater and tap **Restart**.

💡 *Result: Keep root and kernel after update!*

## 📝 Notes & Tips

- 🔄 **Back up** your data before any update!
- Use **full OTA**, not incremental updates.
- If on **Magisk Delta** or a **custom Magisk fork**, your steps may be a bit different.

## ✨ Kernel Features


✅ SukiSU Ultra
✅ SUSFS
✅ VFS HOOK
✅ Magic Mount Support (KPM)
✅ BBR Support
✅ ZRAM


## 🙏 Credits

- [SukiSU Ultra](https://github.com/SukiSU-Ultra/SukiSU-Ultra)
- [ZRAM Module](https://github.com/FurLC/ZRAM-Module)

> ⚠️ **Disclaimer:**  
> Flashing custom kernels always comes with risk!  
> **Proceed at your own responsibility. Have fun, but be careful!**
