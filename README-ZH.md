- [README 中文](./README-ZH.md)
- [README English](./README.md)

# zmk-config-ego62
Ego62的zmk配置文件  
官网:https://www.egokb.com  
使用:https://nickcoutsos.github.io/keymap-editor/ 来编辑。  

![image](./pic/p2.jpg)

## 使用方式

1. Fork 这个存储库.
2. 打开 https://nickcoutsos.github.io/keymap-editor/, 使用你的github账号登陆， 选择你刚刚Fork的存储库, 在图形界面编辑对应的键位映射。
3. 点击保存按钮, GitHub Actions 会自动编译对应的固件。

## 怎么刷入编译好的固件

1. 登陆你自己的github，找到你fork的那个存储库。
2. 点击Actions，然后点击下面的Build。
3. 找到对应修改的Workflow，下载对应的firmware.zip。
4. 解压文件，将键盘通过usb-c连接到电脑，双击键盘背后的reset按钮进入bootloader模式，将ego62_left.uf2复制到左边的键盘，ego62_right.uf2复制到右边的键盘，将ego62_dongle.uf2复制到接收器。
5. 如果有键盘没有响应，则同时按下左右键盘和dongle的reset按钮然后同时松开即可。
6. 如果连接不上蓝牙，则可以先下载settings_reset.uf2，分别刷到左右半边和dongle中，然后再重复4、5两个步骤即可。

参考https://zmk.dev/docs/user-setup  
现在你的键盘应该可以正常工作了。

![image](./pic/p2.jpg)
![image](./pic/p3.jpg)
![image](./pic/p4.jpg)
![image](./pic/p5.jpg)
![image](./pic/p6.jpg)
![image](./pic/p7.jpg)
![image](./pic/p8.jpg)
![image](./pic/p9.jpg)
![image](./pic/p10.jpg)
