# ❓ Frequently Asked Questions (FAQ)

[🇨🇳 查看中文版](./Q&A-ZH.md)

---

## 🔌 Getting Started

### Q: How do I start using the keyboard for the first time?

**A:** Simply connect the Dongle to your computer using a USB-C data cable. Make sure the cable supports data transfer (not charge-only).

---

## 🚨 Connection Issues

### Q: The keyboard doesn't respond after connecting. What should I do?

**A:** Try these steps in order:
1. Click the reset button on the Dongle once
2. Wait about 5 seconds for reconnection
3. If still no response, try resetting all three devices (left, right, Dongle) simultaneously

---

### Q: Only one side of the keyboard is working. How do I fix this?

**A:** Click the reset button on the non-working side once and wait about 5 seconds for reconnection.

---

## ⌨️ Hardware Questions

### Q: What are the buttons and switches on the bottom of the keyboard?

**A:**
- **Button (Reset)**: 
  - Single click: Restarts the firmware
  - Double click: Enters bootloader mode for flashing
- **Switch**: Controls battery power. Usually not needed during normal use.

---

## 🔋 Battery & Charging

### Q: How do I charge the battery?

**A:** Simply connect the side with low battery to your computer using a USB-C cable.

---

### Q: Can I use the keyboard while charging?

**A:** Yes! The keyboard works normally while charging.

---

## 📶 Bluetooth Connection

### Q: How do I connect via Bluetooth?

**A:** Follow these steps:

1. **Ensure Dongle is powered** - Connect to PC or power via USB cable
2. **Switch to Bluetooth mode** - With default keymap: press Left Layer key → Right Layer key → Tab to toggle between Bluetooth and 2.4GHz
3. **Pair the device** - In Bluetooth mode, pair "ego62" like a normal Bluetooth device
4. **Enter passcode** - When prompted for a passcode, type it on the keyboard and press Enter

---

## ⚡ ZMK Studio

### Q: What is ZMK Studio?

**A:** ZMK Studio is a web-based tool that allows real-time keymap editing without reflashing firmware. Connect your Dongle via USB, open [ZMK Studio](https://zmk.studio/), and customize your keymap instantly.

---

### Q: How do I unlock ZMK Studio?

**A:** 
1. Connect the Dongle to your PC via USB
2. Open [ZMK Studio](https://zmk.studio/)
3. Switch to the **System layer** (layer 2)
4. Press the `&studio_unlock` key to unlock

---

### Q: My changes in ZMK Studio don't persist after reconnecting. Why?

**A:** Make sure to click "Save" in ZMK Studio after making changes. The keymap is stored in the keyboard's memory, not on your computer.

---

### Q: How do I restore the original keymap after using ZMK Studio?

**A:** In ZMK Studio, look for the "Restore Stock Settings" or "Reset" option. This will revert to the keymap defined in your `.keymap` file.

---

### Q: Can I use both ZMK Studio and edit the .keymap file?

**A:** Yes, but with caveats:
- **ZMK Studio** changes take effect immediately but don't modify the `.keymap` file
- **.keymap file** changes require reflashing but provide version control
- ZMK Studio settings override `.keymap` settings until you restore defaults

---

## 🔄 Firmware Updates

### Q: Do I need to update the firmware to use ZMK Studio?

**A:** Yes! Make sure you flash the latest firmware with ZMK Studio support:
- `ego62_left.uf2`
- `ego62_right.uf2`
- `ego62_dongle.uf2` (most important - this one contains ZMK Studio)

---

### Q: In what order should I flash the firmware?

**A:** Always flash in this order:
1. Left half
2. Right half  
3. Dongle (last)

This prevents connection issues between the devices.

---

## 🆘 Still Need Help?

- 💬 [Join our Discord community](https://discord.gg/rwY3UyXv)
- 🌐 [Visit official website](https://www.egokb.com)
- 📖 [Check ZMK documentation](https://zmk.dev/docs)

---

[📖 Back to Tutorial](./Ego62_tutorial-EN.md) · [🏠 Back to README](../README.md)
