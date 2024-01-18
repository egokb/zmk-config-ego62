- [README 中文](./README-ZH.md)
- [README English](./README.md)

# zmk-config-ego46
zmk config for Ego46  
website:https://www.egokb.com  
discord:https://discord.gg/rwY3UyXv  
keymap edit with https://nickcoutsos.github.io/keymap-editor  

![image](./pic/p1.jpg)

## Instructions

1. Fork this repository.
2. Open url https://nickcoutsos.github.io/keymap-editor/, Login with your github account， Select the repository you just forked, And edit it.
3. Commit and push your changes to your personal repo. Upon pushing it, GitHub Actions will start building a new version of your firmware with the updated keymap.

## Firmware Files

To locate your firmware files...

1. Log into GitHub and navigate to your personal config repository you just uploaded your keymap changes to.
2. Click "Actions" in the main navigation, and in the left navigation click the "Build" link.
3. Find the corresponding modified workflow and download firmware.zip.
4. Unzip the file, connect the keyboard to the computer via USB C, double-click the reset button on the back of the keyboard to enter bootloader mode, flash ego46_left.uf2 to the keyboard on the left, flash ego46_right.uf2 to the keyboard on the right and flash ego46_dongle.uf2 to the receiver.
5. If there is no response from the keyboard, press the reset button on both the left and right keyboards and the dongle at the same time, and then release it simultaneously.
6. If Bluetooth cannot be connected, you can download the settings_reset.uf2, first flash to the left and right sides and receiver, then repeat steps 4 and 5.

Your keyboard is now ready to use.

![image](./pic/p2.jpg)
![image](./pic/p3.jpg)
![image](./pic/p4.jpg)
![image](./pic/p5.jpg)
![image](./pic/p6.jpg)
![image](./pic/p7.jpg)
![image](./pic/p8.jpg)
![image](./pic/p9.jpg)
![image](./pic/p10.jpg)
