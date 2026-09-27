# a34x_Kernel

Custom kernel for the Samsung Galaxy A34 5G, built on kernel-6.6 with an AOSP common kernel base (`android15-6.6`) and built-in KernelSU support.

> 🚀 **Want to flash this kernel?** Get the source and pre-built releases here: **[BS1388/Kernel_Samsung_a346E](https://github.com/BS1388/Kernel_Samsung_a346E)**

---

## 📱 Supported Devices

**Samsung Galaxy A34 5G (SM-A346B/E/M/N)**

All models share the same **MediaTek Dimensity 1080** chipset, so the kernel binary is identical across regions.

**Device codename:** `a34x`
**Chipset:** MediaTek Dimensity 1080 (6nm)
**Base:** Android 15, kernel 6.6.XXX

---

## ⚙️ Features

- Built on AOSP common kernel (`android15-6.6`)
- Built-in KernelSU support
- Compatible with GSI / DSU Sideloader
- OneUI 7 base kept for continued unlockability

---

## 📥 Installation

1. Unlock your bootloader (if not already unlocked)
2. Download the latest `AnyKernel3-a34x.zip` from [Releases](../../releases)
3. Flash via a custom recovery (TWRP) **or** a kernel flasher app that supports AnyKernel3 zips
4. Reboot

> ⚠️ **Warning:** Flashing a custom kernel can potentially cause bootloops or other issues. Make sure you have a backup before flashing. Not responsible for bricked devices.

---

## 🔨 Building from Source

```bash
git clone https://github.com/BS1388/Kernel_Samsung_a346E -b Google
cd Kernel_Samsung_a346E
# follow build instructions for your toolchain (Kleaf/Bazel)
```

After building, place the resulting `Image` (or `Image.gz`) in the AnyKernel3 zip root alongside `anykernel.sh` and re-zip:

```bash
zip -r9 AnyKernel3-a34x.zip * -x .git README.md *placeholder
```

---

## 🙏 Credits

- [osm0sis](https://github.com/osm0sis) — AnyKernel3
- [topjohnwu](https://github.com/topjohnwu) — magiskboot / Magisk
- KernelSU team
- UN1CA — MediaTek common kernel base
- AOSP — common kernel

---

## 📞 Contact / Support

- **Telegram:** [@Kernel_a34x](https://t.me/Kernel_a34x)
- **GitHub (kernel source):** [BS1388/Kernel_Samsung_a346E](https://github.com/BS1388/Kernel_Samsung_a346E)

---

## ⚖️ Disclaimer

Use at your own risk.
