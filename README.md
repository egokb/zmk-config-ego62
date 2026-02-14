<div align="center">

# 🎹 Ego62 ZMK Firmware Configuration

[![ZMK](https://img.shields.io/badge/ZMK-Firmware-blue?style=flat-square)](https://zmk.dev/)
[![ZMK Studio](https://img.shields.io/badge/ZMK%20Studio-Supported-green?style=flat-square)](https://zmk.studio/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

**A customizable ZMK firmware configuration for the Ego62 split keyboard**

[🌐 Official Website](https://www.egokb.com) · [💬 Discord Community](https://discord.gg/rwY3UyXv)

[🇨🇳 中文文档](./README-ZH.md) · [🇺🇸 English](./README.md)

<img src="./pic/p1.jpg" width="600" alt="Ego62 Keyboard">

</div>

---

## ✨ Features

- ⚡ **ZMK Studio Support** - Real-time keymap editing via USB
- 🔥 **Wireless & Wired** - Bluetooth 5.0 + 2.4GHz + USB-C
- 🔋 **Long Battery Life** - Optimized power management
- 🎨 **Hot-swappable** - Easy keymap customization
- 🖥️ **Multi-Device** - Connect up to 5 Bluetooth devices
- 🛠️ **Open Source** - Fully customizable firmware

---

## 📖 Quick Start

### Option 1: ZMK Studio (Recommended)

The easiest way to customize your keymap in real-time:

1. **Connect** your Dongle to PC via USB-C
2. **Open** [ZMK Studio](https://zmk.studio/) in your browser
3. **Press** the `&studio_unlock` key (on System layer) to unlock
4. **Edit** your keymap visually and save changes instantly

> ⚠️ **Note**: Changes made in ZMK Studio override the `.keymap` file. To revert, use "Restore Stock Settings" in ZMK Studio.

---

### Option 2: GitHub + Keymap Editor

For advanced customization:

1. **Fork** this repository
2. **Edit** your keymap using [Nick Coutsos Keymap Editor](https://nickcoutsos.github.io/keymap-editor/)
3. **Commit** changes to trigger GitHub Actions build
4. **Download** firmware from Actions and flash to your keyboard

---

## 📥 Downloading Firmware

1. Go to your forked repository on GitHub
2. Click **Actions** tab → **Build** workflow
3. Download the `firmware.zip` artifact
4. Extract the ZIP file

---

## 🔧 Flashing Firmware

### Flashing Order

⚠️ **Important**: Flash in this order to avoid connection issues:

1. Left half (`ego62_left.uf2`)
2. Right half (`ego62_right.uf2`)
3. **Dongle last** (`ego62_dongle.uf2`)

### Steps

1. **Enter Bootloader**: Double-click the reset button on the back of the device
2. **Copy Firmware**: Drag and drop the `.uf2` file to the USB drive that appears
3. **Wait**: The drive will disappear and the device will restart (~5 seconds)

### Troubleshooting

| Issue | Solution |
|-------|----------|
| No response | Press reset on all 3 devices (left, right, dongle) simultaneously |
| Bluetooth won't connect | Flash `settings_reset.uf2` to all devices, then re-flash firmware |
| Only one side works | Press reset on the non-working side and wait 5 seconds |

---

## 📚 Documentation

- [📖 Tutorial (English)](./tutorial/Ego62_tutorial-EN.md)
- [❓ Q&A (English)](./tutorial/Q&A-EN.md)
- [📖 使用教程（中文）](./tutorial/Ego62_tutorial-ZH.md)
- [❓ 常见问题（中文）](./tutorial/Q&A-ZH.md)

---

## 🖼️ Gallery

<div align="center">

| | | |
|:---:|:---:|:---:|
| ![p2](./pic/p2.jpg) | ![p3](./pic/p3.jpg) | ![p4](./pic/p4.jpg) |
| ![p5](./pic/p5.jpg) | ![p6](./pic/p6.jpg) | ![p7](./pic/p7.jpg) |
| ![p8](./pic/p8.jpg) | ![p9](./pic/p9.jpg) | ![p10](./pic/p10.jpg) |

</div>

---

## 🔗 Useful Links

- [ZMK Documentation](https://zmk.dev/docs)
- [ZMK Studio](https://zmk.studio/)
- [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/)
- [Official Website](https://www.egokb.com)

---

## 📄 License

This project is licensed under the MIT License.

---

<div align="center">

**Made with ❤️ for the Ego62 Community**

</div>
