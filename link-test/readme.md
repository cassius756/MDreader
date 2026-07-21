# README —— 链接测试

这是 `link-test` 文件夹的 readme.md,与 index.md 同级。

## Section 2

这是 readme.md 中的第二节,用于测试带锚点的链接能否(至少)跳到本文件。

## 返回

- [回 index](index.md) —— 回到同级首页
- [去子目录](sub/notes.md) —— 进入子目录

## 外部链接

- [MDN Web Docs](https://developer.mozilla.org/) 应在新窗口打开
- [邮件链接](mailto:nobody@example.com) 应由系统邮件客户端接管

## 上级链接测试

从 readme.md 用 `[../index.md]` 写法不应工作(因为 readme 已在根目录,`..` 会越界),
但 `[index.md]` 平级写法可以。点击 [平级 index](index.md) 验证。
