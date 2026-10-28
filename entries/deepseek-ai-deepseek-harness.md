# deepseek-ai/deepseek-harness

## 简介

DeepSeek 官方开源的 Agent 运行框架（命令名 `dsh`），核心理念是「一切皆插件」：模型接入、工具、界面都以插件形式组合，基于 Cordis 框架。目前是开发者预览版。

## 适用场景

- 适合：想看一套完整的 Agent harness 如何拆成插件、想在本地用 Web UI 跑编程/工具调用 Agent，或给它写插件。
- 不适合：要求接口稳定的生产环境——上游明确写了会有破坏兼容的改动；也不建议随手装来源不明的第三方 `dsh` 插件。

## 快速用法

对照上游 README（2026-10-28 版本）：

```sh
# 需要 Node.js
npx @deepseek-ai/dsh web
# 默认在 http://127.0.0.1:3080 打开 Web UI；加 --no-open 不自动开浏览器
```

运行前先读仓库里的 `SAFETY.md`。插件开发从 `docs/architecture.md` 和 `docs/development.md` 开始。

## 推荐理由

2026-08 发布后 Star 激增（入库时约 26 万），是本季最受关注的 Agent 框架之一；官方出品、MIT 许可，插件化架构适合拿来讲解「Agent = 模型 + 工具 + 运行时」的分层。

## 入库日期

2026-10-28

## 源链接

https://github.com/deepseek-ai/deepseek-harness

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
