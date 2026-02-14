<div align="center">

# 🎹 Ego62 ZMK 固件配置

[![ZMK](https://img.shields.io/badge/ZMK-固件-blue?style=flat-square)](https://zmk.dev/)
[![ZMK Studio](https://img.shields.io/badge/ZMK%20Studio-已支持-green?style=flat-square)](https://zmk.studio/)
[![License](https://img.shields.io/badge/许可证-MIT-yellow?style=flat-square)](LICENSE)

**Ego62 分体键盘的可定制 ZMK 固件配置**

[🌐 官方网站](https://www.egokb.com) · [💬 Discord 社区](https://discord.gg/rwY3UyXv) · [💬 QQ群](https://qm.qq.com/q/681306025)

[🇺🇸 English](./README.md) · [🇨🇳 中文](./README-ZH.md)

<img src="./pic/p1.jpg" width="600" alt="Ego62 键盘">

</div>

---

## ✨ 特性

- ⚡ **ZMK Studio 支持** - 通过 USB 实时编辑键位
- 🔥 **无线 & 有线** - 蓝牙 5.0 + 2.4GHz + USB-C
- 🔋 **超长续航** - 优化的电源管理
- 🎨 **热插拔** - 轻松自定义键位
- 🖥️ **多设备连接** - 最多支持 5 个蓝牙设备
- 🛠️ **开源** - 完全可定制的固件

---

## 📖 快速开始

### 方式一：ZMK Studio（推荐）

最简单的实时键位自定义方式：

1. **连接** - 将接收器通过 USB-C 连接到电脑
2. **打开** - 在浏览器中访问 [ZMK Studio](https://zmk.studio/)
3. **解锁** - 按下 `&studio_unlock` 键（在 System 层）解锁键盘
4. **编辑** - 可视化编辑键位并即时保存

> ⚠️ **注意**：在 ZMK Studio 中做的修改会覆盖 `.keymap` 文件。如需恢复，请在 ZMK Studio 中使用"恢复出厂设置"。

---

### 方式二：GitHub + 键位编辑器

适合高级自定义：

1. **Fork** 本仓库
2. **编辑** - 使用 [Nick Coutsos 键位编辑器](https://nickcoutsos.github.io/keymap-editor/) 修改键位
3. **提交** - 修改会触发 GitHub Actions 自动编译
4. **下载** - 从 Actions 下载固件并刷入键盘

---

## 📥 下载固件

1. 进入你在 GitHub 上 fork 的仓库
2. 点击 **Actions** 标签页 → **Build** 工作流
3. 下载 `firmware.zip` 构建产物
4. 解压 ZIP 文件

---

## 🔧 刷写固件

### 刷写顺序

⚠️ **重要**：按此顺序刷写可避免连接问题：

1. 左手 (`ego62_left.uf2`)
2. 右手 (`ego62_right.uf2`)
3. **最后刷接收器** (`ego62_dongle.uf2`)

### 刷写步骤

1. **进入刷机模式**：双击设备背面的重置按钮
2. **复制固件**：将 `.uf2` 文件拖放到出现的 USB 磁盘中
3. **等待**：磁盘会消失，设备自动重启（约 5 秒）

### 故障排除

| 问题 | 解决方法 |
|------|---------|
| 键盘无响应 | 同时按下左右键盘和接收器的重置按钮 |
| 蓝牙无法连接 | 给所有设备刷入 `settings_reset.uf2`，然后重新刷写固件 |
| 只有一边有反应 | 按下无反应一侧的重置按钮，等待 5 秒 |

---

## 📚 文档

- [📖 使用教程（中文）](./tutorial/Ego62_tutorial-ZH.md)
- [❓ 常见问题（中文）](./tutorial/Q&A-ZH.md)
- [📖 Tutorial (English)](./tutorial/Ego62_tutorial-EN.md)
- [❓ Q&A (English)](./tutorial/Q&A-EN.md)

---

## 🖼️ 图库

<div align="center">

| | | |
|:---:|:---:|:---:|
| ![p2](./pic/p2.jpg) | ![p3](./pic/p3.jpg) | ![p4](./pic/p4.jpg) |
| ![p5](./pic/p5.jpg) | ![p6](./pic/p6.jpg) | ![p7](./pic/p7.jpg) |
| ![p8](./pic/p8.jpg) | ![p9](./pic/p9.jpg) | ![p10](./pic/p10.jpg) |

</div>

---

## 🔗 有用链接

- [ZMK 官方文档](https://zmk.dev/docs)
- [ZMK Studio](https://zmk.studio/)
- [键位编辑器](https://nickcoutsos.github.io/keymap-editor/)
- [官方网站](https://www.egokb.com)

---

## 📄 许可证

本项目采用 MIT 许可证。

---

<div align="center">

**用 ❤️ 为 Ego62 社区制作**

</div>
