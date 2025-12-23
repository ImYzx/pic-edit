# ⚡ PicEdit - 在线图片处理工具箱

一个基于纯前端技术（Vue 2 + Tailwind CSS）构建的轻量级图片处理工具集合。无需上传服务器，所有处理均在本地浏览器完成，安全高效。

> 🌐 **在线体验**: [https://imyzx.github.io/pic-edit/](https://imyzx.github.io/pic-edit/)

## 🛠️ 功能模块

本项目包含四个核心工具：

### 1. 🎭 一键绿幕抠 (Green Screen Remover)
- **功能**: 自动识别并移除图片的绿色背景（或自定义颜色）。
- **特色**: 支持容差调节、边缘平滑、实时预览。
- **场景**: 直播截图处理、素材合成。

### 2. 🔪 一键雪碧切 (Sprite Cutter)
- **功能**: 将 Sprite Sheet (雪碧图) 自动切分为序列帧。
- **特色**: 
  - 支持自定义行列、边距。
  - **GIF 合成**: 自动将切分后的帧合成为 GIF 动图，支持倍速调整。
  - **序列帧管理**: 支持帧的删除、复制、排序。
  - **一键打包**: 支持导出所有帧为 ZIP 压缩包。

### 3. 🧼 一键水印除 (Watermark Remover)
- **功能**: 简单的图片修复与水印去除工具。
- **特色**: 提供涂抹修复画笔，基于像素扩散算法填补缺失区域。

### 4. 📉 一键图片压 (Image Compressor)
- **功能**: 图片压缩与格式转换。
- **特色**: 
  - 支持 JPG/PNG/WebP 格式互转。
  - 实时调整压缩质量与尺寸。
  - 直观的文件大小对比。

## 💻 技术栈

- **Core**: Vue.js 2
- **UI Framework**: Tailwind CSS
- **Libraries**:
  - `JSZip`: 文件打包
  - `FileSaver.js`: 文件下载
  - `gif.js`: GIF 生成
  - `gifuct-js`: GIF 解析

### 5. 🎞️ GIF 分分合 (GIF Splitter/Merger)
- **功能**: 
  - **GIF 拆分**: 上传 GIF 动图，一键提取所有帧，支持查看帧延迟，可打包下载。
  - **GIF 合成**: 将多张静态图片拼接为 GIF，自定义帧率与循环模式。
- **特色**: 纯前端解析与生成，解决 GIF 解析库冲突问题。

## 🚀 使用方法

无需安装 Node.js 环境，直接双击打开 `index.html` 即可使用。

或者使用任何静态文件服务器运行：

```bash
# 使用 Python
python -m http.server 8000

# 使用 NodeJS http-server
npx http-server .
```

## 🤝 贡献

欢迎提交 Issue 或 Pull Request！

Repo: [git@github.com:ImYzx/pic-edit.git](https://github.com/ImYzx/pic-edit)
