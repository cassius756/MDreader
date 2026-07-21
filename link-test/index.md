# 链接跳转测试首页 / Link Test Index

这是测试首页。请用「打开文件夹」选择整个 `link-test` 目录,然后从这里点击下面的各种链接验证功能。

## 1. 内部文件链接(同目录)

跳到 [readme.md](readme.md) —— 同目录、无 `./` 前缀。

跳到 [readme 带点斜杠](./readme.md) —— 同目录、带 `./` 前缀。

## 2. 内部文件链接(子目录)

跳到 [子目录笔记](sub/notes.md) —— 进入子文件夹。

跳到 [子目录笔记带点斜杠](./sub/notes.md) —— 同上,带 `./`。

## 3. 内部文件链接(带锚点)

跳到 [readme 的某节](readme.md#section-2) —— 会跳到文件,但锚点滚动需 marked 扩展支持(本版本仅跳文件)。

## 4. 外部网页链接(新窗口打开)

- [Google](https://www.google.com)
- [GitHub](https://github.com)
- [项目 marked.js](https://marked.js.org/)
- [KaTeX 官网](https://katex.org/)

外部链接后应有 `↗` 视觉标识。

## 5. 找不到的文件(应弹 toast)

点击 [不存在的文件](missing-file.md) —— 应看到 "找不到文件:missing-file.md" 提示。

## 6. 文档内锚点(浏览器默认滚动)

跳到 [本页底部](#bottom-anchor) —— 应滚动到本页底部(由 marked 是否生成 id 决定)。

---

<div id="bottom-anchor"></div>

## 本页底部

你已滚动到本页底部。回 [顶部](#链接跳转测试首页--link-test-index)?
