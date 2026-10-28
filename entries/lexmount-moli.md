# lexmount/moli

## 简介

用 Rust 写的、面向 AI Agent 的无头浏览器：默认只做 DOM/结构，需要时再开启布局与渲染，资源占用比完整 Chromium 小。可通过 CLI、CDP、WebDriver Classic / BiDi 调用。

## 适用场景

- 适合：给 Agent 做网页抓取、转 Markdown/语义树、轻量浏览器自动化；已有 Playwright 脚本想换一个更省资源的后端。
- 不适合：对页面像素级兼容性要求很高、或依赖完整 Chrome 扩展生态的场景，仍用真实浏览器更稳。

## 快速用法

对照上游 README（2026-10-28 版本），Linux / macOS：

```sh
curl --proto '=https' --tlsv1.2 -fsSL \
  https://github.com/lexmount/moli/releases/latest/download/moli-installer.sh | sh

# 把网页抓成 Markdown
moli fetch --dump markdown --wait-until done https://example.com

# 起自动化服务（CDP / WebDriver 同一端口），Playwright 可用 connectOverCDP 连 127.0.0.1:9222
moli serve --layout
```

## 推荐理由

2026-08 发布，两个多月涨到约 2.1 万 Star，上过 Trendshift 日/周榜；它把「Agent 读网页」这件事做成了结构优先、按需渲染，正好补上 Agent 工具链里取网页这一环，Apache-2.0 许可。

## 入库日期

2026-10-28

## 源链接

https://github.com/lexmount/moli

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
