# 📖 单词本 · 多设备同步朗读

一个纯前端单词本：电脑编辑 → 自动同步到 GitHub → 手机打开同一网址查看/朗读。

## ✨ 功能

- ➕ 增删改单词、意思、音标、例句
- 🔊 浏览器内置 TTS 朗读（中文+英文）
- ☁️ 通过 GitHub API 实时同步到私有仓库
- 📱 电脑、手机、平板打开同一网址即可访问

## 🚀 使用方法

### 1. 部署（一次性）

本仓库已部署到 GitHub Pages，访问：

**https://qianzhu123.github.io/vocab-tts/**

如需重新部署：
- Settings → Pages → Source 选 `main` 分支根目录 → Save

### 2. 配置 Token（首次打开页面时）

1. 访问 https://github.com/settings/tokens/new 创建 Personal Access Token
2. **必须勾选 `repo` 权限**
3. 在页面顶部把 Token 填入，格式：`用户名/仓库名`（默认 `qianzhu123/vocab-tts`）
4. 保存后自动从云端拉取

> ⚠️ Token 只存在你浏览器本地，不会上传到任何地方。但**任何人拿到这个 Token 都能读写你的仓库**，请勿公开。

## 🛠 技术

- 纯 HTML + JS（无后端）
- Web Speech API（浏览器原生 TTS）
- GitHub Contents API（当 KV 用）

## 📁 文件结构

- `index.html` — 单文件应用，所有逻辑都在里面
