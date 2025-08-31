# AI网站公式复制LaTeX 油猴脚本

## 📋 功能描述

一个通用的LaTeX公式复制工具，支持主流AI聊天网站和学术网站的数学公式复制，自动格式化为标准的LaTeX格式。

## ✨ 主要特性

- **🖱️ 鼠标悬停预览**：鼠标移到公式上显示蓝色边框和LaTeX源码预览
- **📋 一键复制**：点击公式直接复制LaTeX格式到剪贴板  
- **📝 智能选择复制**：选择包含公式的文本时自动转换为LaTeX格式
- **🔄 按钮复制增强**：拦截网站复制按钮，自动格式化公式内容
- **📐 智能格式识别**：自动区分行内公式(`$...$`)和块级公式(`$$...$$`)

## 🌐 支持网站

### AI聊天平台
- **Claude** (claude.ai, demo.fuclaude.oaifree.com)
- **ChatGPT** (chatgpt.com)
- **Google Gemini** (gemini.google.com) 
- **Google AI Studio** (aistudio.google.com)
- **DeepSeek** (deepseek.com, chat.deepseek.com)
- **豆包** (doubao.com)
- **月之暗面** (moonshot.cn)

### 学术网站
- **知乎** (zhihu.com)
- **维基百科** (wikipedia.org)
- **Stack Exchange** (stackexchange.com)
- **OI Wiki** (oi-wiki.org)
- **洛谷** (luogu.com)


## 📖 使用方法

### 方式一：鼠标悬停 + 点击复制
1. 将鼠标悬停在数学公式上
2. 看到蓝色边框和LaTeX预览浮窗
3. 点击公式即可复制LaTeX格式

### 方式二：选择复制
1. 用鼠标选择包含公式的文本
2. 使用 `Ctrl+C` 复制
3. 脚本自动将公式转换为LaTeX格式

### 方式三：按钮复制
1. 点击网站的复制按钮
2. 脚本自动拦截并格式化公式内容

## 🔧 调试功能

在浏览器控制台输入 `debugFormulaScript()` 查看详细调试信息，包括：
- 脚本版本和配置信息
- 页面上找到的公式数量
- Gemini网站的Hook状态和映射数据

## 📝 更新日志

### v0.9 (2025-08-31)
- 🆕 **新增网站支持**：完整支持豆包(doubao.com)
- 🔧 实现豆包data-custom-copy-text属性解析
- ✨ 添加豆包专用复制按钮监听
- 🎯 优化公式检测和处理逻辑，支持豆包特殊结构
- 📊 增强调试功能，显示豆包公式状态信息
- 🔧 更新选择复制逻辑，兼容豆包公式格式

### v0.8 (2025-08-31)
- ⭐ **重大更新**：完整支持Google Gemini网站
- 🔧 新增KaTeX Hook机制，实时捕获Gemini公式渲染
- ✨ 实现Gemini网站的鼠标悬停预览和点击复制功能
- 🎯 优化选择复制逻辑，支持Gemini特殊DOM结构
- 🌟 支持多个主流AI聊天平台
- 🔄 实现按钮复制拦截和格式化
- 🎨 优化用户界面和提示效果
- 🔧 完善错误处理和兼容性

## 🛠️ 技术特性

- **零依赖**：纯JavaScript实现，无需外部库
- **高性能**：智能事件绑定，避免重复处理
- **安全可靠**：完善的错误处理和兼容性检查
- **先进技术**：Gemini采用KaTeX Hook技术，其他网站使用DOM解析

## 🤝 贡献

欢迎提交Issue和Pull Request来改进这个项目！

## 📄 许可证

MIT License
