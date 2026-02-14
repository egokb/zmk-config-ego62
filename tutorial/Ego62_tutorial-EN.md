# 📖 Ego62 Setup & Customization Tutorial

[🇨🇳 查看中文版](./Ego62_tutorial-ZH.md)

This tutorial covers two methods to customize your Ego62 keyboard:
- **Method 1**: ZMK Studio (Easiest, Real-time editing)
- **Method 2**: GitHub + Keymap Editor (Advanced, More control)

---

## ⚡ Method 1: ZMK Studio (Recommended)

The easiest way to customize your keymap with real-time preview.

### Prerequisites
- ✅ Firmware with ZMK Studio support already flashed
- ✅ USB-C cable connected to the Dongle
- ✅ Modern web browser (Chrome, Edge, Firefox)

---

### Step 1: Connect Your Keyboard

1. Connect the **Dongle** to your computer via USB-C cable
2. Make sure the left and right halves are powered on
3. Wait for the keyboard to connect (about 5 seconds)

---

### Step 2: Open ZMK Studio

1. Open your web browser
2. Navigate to [https://zmk.studio/](https://zmk.studio/)
3. The website should automatically detect your keyboard

---

### Step 3: Unlock the Keyboard

1. On your Ego62, switch to the **System layer** (Layer 2):
   - Press and hold the layer key (default: bottom row)
   - Or use the layer toggle if configured
2. Find and press the `&studio_unlock` key
3. The keyboard is now unlocked and ready for editing

> 💡 **Tip**: The unlock key is usually placed on the System layer for safety.

---

### Step 4: Edit Your Keymap

1. **Visual Editor**: Click on any key in the layout diagram
2. **Select Behavior**: Choose from the dropdown menu:
   - Key Press (normal keys)
   - Layer controls (mo, to, etc.)
   - Bluetooth controls
   - Media keys
   - And more...
3. **Save Changes**: Click the "Save" button to write changes to the keyboard

---

### Step 5: Test Your Changes

1. Try typing with your new keymap
2. Changes take effect immediately
3. If something feels wrong, you can always restore defaults

---

### Restoring Defaults

If you want to revert to the original keymap:
1. In ZMK Studio, find the **"Restore Stock Settings"** button
2. Click it to reset to the firmware default keymap

---

## 🛠️ Method 2: GitHub + Keymap Editor

For advanced customization with version control.

---

### Part 1: Fork the Repository

#### Step 1: Create GitHub Account

1. Go to [GitHub](https://github.com)
2. Sign up or log in to your account

#### Step 2: Fork the Repository

1. Visit the [Ego62 firmware repository](https://github.com/egokb/zmk-config-ego62)
2. Click the **"Fork"** button in the top right
3. Wait for the fork to complete (you'll be redirected to your copy)

---

### Part 2: Enable GitHub Actions

1. In your forked repository, click the **Actions** tab
2. Click the green **"I understand my workflows, go ahead and enable them"** button
3. GitHub Actions is now enabled for automatic firmware building

---

### Part 3: Edit Your Keymap

#### Step 1: Open Keymap Editor

1. Go to [Nick Coutsos Keymap Editor](https://nickcoutsos.github.io/keymap-editor/)
2. Click **"Authorize with GitHub"**
3. Select your forked repository
4. Grant necessary permissions

#### Step 2: Customize Keys

1. Click on any key in the visual layout
2. Select the desired behavior from the dropdown
3. Repeat for all keys you want to change

#### Step 3: Save Changes

1. Click the **"Save"** button
2. Enter a commit message (or use the default)
3. Click **"Commit changes"**
4. Wait for the commit to complete

---

### Part 4: Download Firmware

#### Step 1: Wait for Build

1. Go back to your GitHub repository
2. Click the **Actions** tab
3. You should see a new workflow running
4. Wait about 5 minutes for the build to complete

#### Step 2: Download Firmware

1. Click on the completed workflow run
2. Scroll down to the **Artifacts** section
3. Download `firmware.zip`
4. Extract the ZIP file to access the `.uf2` files

---

### Part 5: Flash Firmware

⚠️ **Important**: Flash in this order to avoid connection issues!

#### Order:
1. `ego62_left.uf2` (Left half)
2. `ego62_right.uf2` (Right half)
3. `ego62_dongle.uf2` (Dongle - **last!**)

#### Steps for Each Device:

1. **Enter Bootloader**: Double-click the reset button on the back
2. **Copy File**: Drag and drop the `.uf2` file to the USB drive that appears
3. **Wait**: The drive will disappear and the device restarts (~5 seconds)
4. **Next Device**: Repeat for the next device

---

## 🔄 Subsequent Updates

After the initial setup, updating your keymap is simpler:

### For ZMK Studio:
1. Connect Dongle via USB
2. Open ZMK Studio
3. Edit and save - done!

### For GitHub Method:
1. Open Keymap Editor
2. Make changes and save
3. Download new firmware from Actions
4. Flash all three devices

---

## 📚 Additional Resources

- [❓ Frequently Asked Questions](./Q&A-EN.md)
- [🌐 ZMK Documentation](https://zmk.dev/docs)
- [⚡ ZMK Studio](https://zmk.studio/)
- [💬 Discord Community](https://discord.gg/rwY3UyXv)

---

[🏠 Back to README](../README.md)
