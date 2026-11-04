# Power-Agent/PowerMCP

## 简介

一组面向电力系统软件的 MCP 服务器（PowerWorld、OpenDSS、pandapower 等），让大模型直接调用仿真软件做 N-1 校核、负荷增长评估并生成报告。

## 适用场景

- 适合：演示或研究「LLM Agent + 电力仿真软件」；给 Claude Desktop 等 MCP 客户端接上 pandapower 做对话式潮流分析。
- 不适合：需要可审计、确定性结果的正式计算（Agent 结论须人工复核）；手头没有对应商业软件授权时，部分服务器用不了。

## 快速用法

对照上游 README（2026-11-04 版本）：

```bash
pip install powermcp
powermcp install   # 交互选择工具、填写本地软件路径，并写入 MCP 客户端配置
```

各服务器支持的软件版本与依赖以上游文档为准（未逐项核实）。

## 推荐理由

电力 + AI Agent 方向少见的成体系开源实现（入库时约 230 Star，MIT），有演示视频和教程，适合作为「智能电网 × 大模型」毕设或课堂拓展的起点。

## 入库日期

2026-11-04

## 源链接

https://github.com/Power-Agent/PowerMCP

## 是否已 Star

是（2026-11-04，每周策展自动化代为点亮）。
