<!--
 MIT License

 版权所有 (c) 2026 DevToolkit 贡献者

 见 LICENSE 文件获得完整授权信息。
-->
# DevToolkit · 开发者效率工具箱

一个**单文件、零依赖**的开发者效率工具箱，直接在浏览器中运行，无需安装、无需构建、无需网络。适合开发者日常随手使用，也适合作为 Gitee 开源项目直接分享。

> 打开 `index.html` 即可使用。整个项目只有一个 HTML 文件，复制到任何地方都能跑。

## ✨ 特性

- 📦 **单文件**：全部功能 + 样式 + 脚本集成在一个 `index.html`，无外部依赖
- 🌐 **纯前端**：所有计算在本地浏览器完成，数据不上传，安全私密
- 🌓 **深色 / 浅色主题**：默认跟随系统，可一键切换并记忆选择
- ⌨️ **键盘友好**：在输入区按 `Ctrl/Cmd + Enter` 即可触发主操作
- 📱 **响应式**：桌面与移动端均可用
- 🔐 **开源 MIT**：可自由使用、修改、分发

## 🧰 包含工具

| 工具 | 说明 |
| --- | --- |
| JSON 格式化 / 校验 | 格式化、压缩、校验 JSON，支持中文与转义 |
| Base64 编码 / 解码 | 双向转换，正确处理 UTF-8 中文 |
| URL 编码 / 解码 | 支持 `encodeURI` 与 `encodeURIComponent` 两种模式 |
| 时间戳 ↔ 日期 | 自动识别秒 / 毫秒，双向转换，显示本地与 UTC |
| UUID 生成器 | 生成 RFC 4122 v4 UUID，支持批量、大小写、连字符选项 |
| 正则表达式测试 | 实时匹配，高亮命中内容，显示捕获分组 |
| 颜色码转换 | HEX ↔ RGB 双向转换，实时预览 |
| HTML 实体编码 / 解码 | HTML 文本与实体互转，转义场景适用 |

## 🚀 使用方法

### 方式一：直接打开（最简单）

1. 下载或克隆本仓库
2. 双击打开 `index.html`
3. 开始使用

### 方式二：Gitee 在线预览

将本仓库推送到 Gitee 后，可在仓库「服务 → Gitee Pages」中直接部署 `index.html`，生成在线链接分享给他人。

### 方式三：嵌入或二次开发

整个应用就是一个 HTML 文件，可直接嵌入任意静态站点，或作为单页工具分发。

## 📸 使用示例

```
# 克隆仓库
git clone https://gitee.com/<你的用户名>/dev-toolkit.git
cd dev-toolkit

# 直接用浏览器打开
start index.html        # Windows
open index.html         # macOS
```

## 🗂 项目结构

```
dev-toolkit/
├── index.html      # 唯一源码文件，包含全部功能
├── README.md       # 本说明文档
├── LICENSE         # MIT 开源协议
└── .gitignore      # Git 忽略规则
```

## 🛠 开发与贡献

欢迎提交 Issue 与 Pull Request。

- 新增工具：在 `index.html` 的 `<nav>` 增加一个 tab，并在 `<main>` 增加对应 `<section class="panel">`，在 `<script>` 中实现逻辑
- 保持**单文件**原则：所有 CSS 与 JS 都内联在 `index.html` 中
- 保持**零依赖**：不引入任何外部 CDN、框架或构建步骤
- 提交前请在浏览器中验证所有工具可用

## 📄 许可证

本项目基于 [MIT 协议](LICENSE) 开源。

```
MIT License

Copyright (c) 2026 DevToolkit Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy
...（完整条款见 LICENSE 文件）
```

## 🙋 常见问题

**Q：数据会上传到服务器吗？**
不会。所有计算均在浏览器本地完成，无任何网络请求。

**Q：可以离线使用吗？**
可以。`index.html` 是自包含的，完全离线可用。

**Q：如何新增一个工具？**
参考「开发与贡献」章节，遵循单文件、零依赖原则即可。