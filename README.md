<p style="color:red;font-weight:bold;font-size:0.95rem;line-height:1.6;padding:0.75rem 1rem;border:1px solid rgba(255,0,0,0.3);border-radius:8px;background:rgba(255,0,0,0.05);">
⚠️ 免责声明：本项目部分代码由 AI 辅助生成，仅供学习和参考使用。使用者应自行审查代码安全性，作者不对因使用本项目造成的任何直接或间接损失承担责任。
</p >

# ham-web-page

业余无线电个人导航页，部署在 Cloudflare Workers 或任意静态托管平台。

## 功能

- 个人信息展示 — 呼号、位置、头像、CQ 标语
- 快捷链接 — 博客、日志、邮箱、GitHub、QRZ
- 邮箱一键复制 — 点击自动复制到剪贴板
- 深色/浅色主题切换 — 带 View Transition 动画
- 响应式设计 — 手机 / 桌面自适应
- 跟随系统主题 — 未手动设置时自动匹配系统偏好

## 技术栈

| 层 | 技术 |
| --- | --- |
| 语言 | HTML + CSS + JavaScript |
| 样式 | CSS 变量（CSS Custom Properties） |
| 动画 | CSS View Transition API |
| 图标 | 内联 SVG |
| 托管 | Cloudflare Workers / Pages / 任意静态托管 |

## 目录结构

```
├── index.html          # 导航页源码
├── Avatar.png          # 头像图片
└── README.md
```

## 自定义

### 修改个人信息

打开 `index.html`，搜索以下内容替换：

```
BH2XOL        → 你的呼号
大连 · 辽宁   → 你的位置
bh2xol@bh2xol.com → 你的邮箱
Avatar.png    → 你的头像图片
```

### 修改链接

找到 `<div class="links">` 部分，增删或修改 `<a>` 标签即可。

### 修改 CQ 标语

找到 `<div class="cq">` 那行，替换文字。

## 部署

将 `index.html` 和 `Avatar.png` 上传到 Cloudflare Workers 或 Pages，或者直接用 GitHub Pages。

## 授权

MIT
