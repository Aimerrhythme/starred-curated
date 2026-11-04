# microsoft/TokenEconomizer

## 简介

微软与 UC Berkeley 的编程 Agent 降本插件：从同一仓库的历史会话中学习，用「微技能」记住仓库惯例、裁掉从不用的工具、在 Agent 陷入失败循环时介入，不改 Agent 本身。

## 适用场景

- 适合：在少数几个常用仓库里反复跑 Claude Code、Codex、Copilot CLI 等，想降低 token 花费。
- 不适合：每次都是全新仓库的一次性任务（可学的经验少）；不愿意让插件在本机 `~/.tokeneconomizer` 记录会话经验。

## 快速用法

对照上游 README（2026-11-04 版本），以 Claude Code 为例：

```bash
git clone https://github.com/microsoft/TokenEconomizer.git
claude plugin marketplace add "$PWD/TokenEconomizer"
claude plugin install tokeneconomizer@tokeneconomizer
```

启动 `claude` 后运行 `/tokeneconomizer:status` 检查状态。Cursor Agent 支持标为实验性，步骤见上游 README。

## 推荐理由

近期 Star 激增（10 月中旬创建，入库时约 4.7 千 Star，Apache-2.0），且附论文与可复跑实验：README 报告 SWE-Bench 上平均成本降低 18.4–30.9%（上游自测数据，未独立复现）。

## 入库日期

2026-11-04

## 源链接

https://github.com/microsoft/TokenEconomizer

## 是否已 Star

是（2026-11-04，每周策展自动化代为点亮）。
