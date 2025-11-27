# Audio Recorder & Preview Tool

一个基于 Web Audio API 的在线录音和文件预览工具，支持模拟 uniapp 录音功能和智能文件预览。

## 功能特性

- 🎤 **Web 录音功能**：支持麦克风录音，模拟 uniapp MP3 输出格式
- 🔍 **智能预览器**：自动识别音频/图片文件并预览
- ⚡ **实时倒计时**：录音时显示剩余时间，最后10秒高亮提醒
- 🎨 **科技感 UI**：现代化深色主题界面设计
- 📱 **响应式设计**：适配移动端和桌面端

## 技术特点

- 基于原生 Web Audio API，无需第三方库
- 支持多种音频格式：MP3, WAV, WebM, AAC, M4A, OGG
- 支持多种图片格式：JPG, PNG, GIF, WebP, BMP
- 智能解析 JSON 响应中的 fileUrl 字段
- 自动处理 COS 临时签名链接

## 使用说明

1. 点击"开始录音"按钮授权麦克风访问
2. 录音时显示60秒倒计时，最后10秒会有高亮提醒
3. 点击"保存文件"下载录音（模拟 MP3 格式）
4. 在预览器中粘贴文件 URL 或 JSON 响应进行预览

## 支持格式

### 输入格式
- 直接粘贴文件 URL（如：`https://xxx.mp3?sign=...`）
- 粘贴完整 JSON 响应（如：`{"code":200, "data": {"fileUrl": "..."}}`）

### 预览格式
- 音频：MP3, WAV, WebM, AAC, M4A, OGG
- 图片：JPG, JPEG, PNG, GIF, WebP, BMP

## 浏览器要求

- 支持 Web Audio API（现代浏览器均支持）
- HTTPS 或 localhost 环境（用于麦克风访问）

## 技术栈

- HTML5
- CSS3
- JavaScript (ES6+)
- Web Audio API
- MediaRecorder API

## 本地运行

直接打开 `index.html` 文件即可使用（需要在 HTTPS 或 localhost 环境下才能使用录音功能）。
<img width="1396" height="1069" alt="image" src="https://github.com/user-attachments/assets/272c2c8c-deaf-49e2-93f8-f5a0c2db0107" />

## 许可证

MIT
