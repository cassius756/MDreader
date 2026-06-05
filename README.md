<div align="center">

# MD 阅读器 / MD Reader

📖 一个轻量、简洁的 Markdown 与纯文本文件阅读器，基于浏览器运行。

A lightweight, clean Markdown & plain text file reader that runs entirely in the browser.

</div>

---

## 功能特性 / Features

- **Markdown 渲染** — 支持 GFM 标准，含代码高亮、表格、引用等
- **纯文本查看** — 以等宽字体展示 `.txt` 文件
- **Mermaid 图表** — 在 Markdown 中渲染流程图、时序图等（需联网加载库）
- **文件夹浏览** — 打开整个文件夹，侧栏树状浏览，支持键盘上下键切换
- **拖拽支持** — 直接拖入文件或文件夹即可打开
- **离线友好** — marked 和 mermaid 优先使用本地文件，失败后回退至 CDN

---

- **Markdown Rendering** — GFM-compliant with code blocks, tables, blockquotes, etc.
- **Plain Text Viewer** — `.txt` files displayed in monospace font
- **Mermaid Diagrams** — Render flowcharts, sequence diagrams, etc. in Markdown (requires network for library)
- **Folder Browsing** — Open an entire folder with a sidebar file tree; navigate with arrow keys
- **Drag & Drop** — Drag files or folders directly into the window
- **Offline-Friendly** — Falls back to CDN only when local library files are unavailable

---

## 快速开始 / Quick Start

### 方式一：直接打开 / Open Directly

用浏览器打开 `code.html` 即可。

> **Windows 用户提示**：如果 `start.vbs` 存在，双击它会以 Edge 无边框模式启动应用。
> 首次发布前请检查 `start.vbs` 中的路径是否为相对路径，避免泄露本地目录结构。

---

### 方式二：本地服务器 / Local Server（推荐）

```bash
# 使用 Python
python -m http.server 8080

# 或使用 Node.js
npx serve .
```

然后在浏览器中访问 `http://localhost:8080/code.html`。

---

## 项目文件 / Project Files

| 文件 | 说明 |
|------|------|
| `code.html` | 主程序 —— 一个自包含的 HTML 文件，包含全部样式与逻辑 |
| `start.vbs` | （可选）Windows 快捷启动脚本，以 Edge 无边框模式运行 |
| `README.md` | 本说明文档 |

---

## 技术栈 / Tech Stack

- **Vanilla HTML/CSS/JS** — 无框架依赖，单文件自包含
- **[marked](https://marked.js.org/)** — Markdown 解析渲染
- **[Mermaid](https://mermaid.js.org/)** — 图表渲染

> marked 和 mermaid 优先加载本地 `marked.min.js` / `mermaid.min.js`，若不存在则自动从 CDN 获取。

---

## 兼容性 / Browser Support

- Chrome / Edge (推荐 / Recommended)
- Firefox
- Safari
- 基于 Chromium 的其他浏览器

---

## 许可 / License

[MIT](LICENSE)
