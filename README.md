# 天命牌 (Destiny Cards) 🃏

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![WebAssembly](https://img.shields.io/badge/WebAssembly-supported-purple.svg)](https://webassembly.org/)

> 一个现代化的Web卡牌游戏应用，提供沉浸式的天命牌游戏体验

[English](README.md) | 中文

## 📋 项目简介

天命牌是一个基于Web技术的互动卡牌游戏应用，集成了丰富的多媒体资源和游戏元素。项目采用现代化的前端技术栈，提供流畅的用户体验。

## ✨ 主要特性

- 🎮 **天命牌游戏** - 独特的卡牌游戏玩法
- 🎵 **丰富的音效** - 包含背景音乐、点击音效、游戏音效等
- 🎨 **精美视觉设计** - 支持多种卡片样式和视觉效果
- 📱 **响应式设计** - 适配桌面和移动设备
- 🔧 **现代Web技术** - 使用最新的Web标准和优化

## 🗂️ 项目结构

```
web4/
├── assets/                 # 静态资源
│   ├── *.mp3              # 音频文件
│   ├── *.svg              # 矢量图标
│   ├── *.woff2            # 字体文件
│   ├── *.css              # 样式文件
│   └── *.js               # JavaScript文件
├── cards/                 # 天命牌图片资源
│   ├── cards_*.jpg        # 各种天命牌图片
│   └── cards_*-mobile@2x.jpg # 移动端高分辨率图片
├── draco/                 # Draco压缩库
│   ├── draco_decoder.wasm # WebAssembly解码器
│   └── draco_wasm_wrapper.js # WASM包装器
├── favicons/              # 网站图标
│   ├── favicon.svg        # 主图标
│   └── site.webmanifest   # PWA配置
├── textures/              # 纹理资源
│   └── noise.png          # 噪声纹理
└── index.html             # 主页面
```

## 🚀 快速开始

### 环境要求

- 现代Web浏览器（支持ES6+、WebAssembly）
- 本地Web服务器（推荐）

### 安装和运行

1. **克隆项目**
   ```bash
   git clone <repository-url>
   cd destiny-cards
   ```

2. **启动本地服务器**
   
   使用Python（推荐）：
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   ```
   
   或使用Node.js：
   ```bash
   npx serve .
   ```
   
   或使用其他静态文件服务器

3. **访问应用**
   
   打开浏览器访问：`http://localhost:8000`

## 🎯 功能说明

### 天命牌系统
- 支持多种天命牌类型（A、2-10、J、Q、K）
- 提供不同分辨率的图片资源
- 移动端优化支持

### 音效系统
- **背景音乐**：`ambiance-*.mp3`
- **交互音效**：`click.mp3`、`buzz-click.mp3`
- **游戏音效**：`win-game.mp3`、`loose-game.mp3`等
- **天命牌音效**：`flip-card-alt.mp3`、`same-card.mp3`

### 视觉资源
- 现代化UI图标和装饰元素
- 高质量字体支持（Bebas Neue、Realist Wide）
- 全息效果纹理

## 🛠️ 技术栈

- **前端框架**：现代JavaScript（ES6+）
- **样式**：CSS3
- **压缩技术**：Draco 3D压缩
- **Web标准**：WebAssembly、PWA支持
- **字体**：WOFF2格式优化

## 🔧 开发环境

### 环境要求

- **Node.js**: >= 14.0.0
- **npm**: >= 6.0.0
- **现代浏览器**: 支持ES6+、WebAssembly

### 开发工具推荐

- **代码编辑器**: VS Code
- **浏览器开发者工具**: Chrome DevTools
- **版本控制**: Git

### 代码规范

- **JavaScript**: 使用 ES6+ 语法
- **CSS**: 遵循 BEM 命名规范
- **提交信息**: 遵循 [Conventional Commits](https://www.conventionalcommits.org/)
- **代码格式**: 使用 Prettier 进行代码格式化

### 调试指南

1. **浏览器控制台**: 查看 JavaScript 错误和警告
2. **网络面板**: 检查资源加载情况
3. **性能面板**: 分析应用性能
4. **移动端调试**: 使用浏览器移动端模拟器

## 📱 PWA支持

项目支持Progressive Web App功能：
- 可安装到设备主屏幕
- 离线缓存支持
- 响应式设计

## 🎨 自定义

### 添加新天命牌
1. 将天命牌图片放入`cards/`目录
2. 确保包含标准分辨率和高分辨率版本
3. 更新相关配置文件

### 修改音效
1. 替换`assets/`目录中的音频文件
2. 保持文件名格式一致
3. 确保音频格式兼容性

## 🤝 贡献指南

我们欢迎所有形式的贡献！请查看 [CONTRIBUTING.md](CONTRIBUTING.md) 了解详细的贡献指南。

### 快速开始

1. **Fork 项目**
   ```bash
   # 点击 GitHub 上的 Fork 按钮，然后克隆你的 fork
   git clone <your-fork-url>
   cd destiny-cards
   ```

2. **创建特性分支**
   ```bash
   git checkout -b feature/你的特性名称
   ```

3. **提交更改**
   ```bash
   git add .
   git commit -m "feat: 添加新功能描述"
   ```

4. **推送并创建 Pull Request**
   ```bash
   git push origin feature/你的特性名称
   ```

### 贡献类型

- 🐛 **Bug 修复** - 修复现有问题
- ✨ **新功能** - 添加新功能或改进
- 📚 **文档** - 改进文档和示例
- 🎨 **UI/UX** - 改进用户界面和体验
- ⚡ **性能** - 性能优化
- 🧪 **测试** - 添加或改进测试

### 代码规范

- 使用有意义的提交信息（遵循 [Conventional Commits](https://www.conventionalcommits.org/)）
- 确保代码通过所有测试
- 添加适当的注释和文档
- 遵循项目的代码风格

## 📄 许可证

本项目采用 [MIT 许可证](LICENSE) 开源协议。

```
MIT License

Copyright (c) 2025 天命牌项目

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## 📈 版本历史

查看 [CHANGELOG.md](CHANGELOG.md) 了解详细的版本变更历史。

### 当前版本: v1.0.0

- ✨ 初始版本发布
- 🎮 基础天命牌游戏功能
- 🎵 完整的音效系统
- 📱 响应式设计支持
- 🔧 PWA 功能支持

## 🐛 问题报告

如果您发现了 bug 或有功能建议，请：

1. 查看项目 Issues 确认问题未被报告
2. 创建新的 Issue，详细描述问题
3. 提供复现步骤和环境信息

## 🙏 致谢

感谢所有为这个项目做出贡献的开发者和设计师！

---

**注意**：这是一个开源项目，欢迎社区贡献和改进！
