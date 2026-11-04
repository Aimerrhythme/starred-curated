# PowerGridModel/power-grid-model

## 简介

LF Energy 旗下的配电网稳态分析库，C++ 内核、Python/C 接口，支持潮流、状态估计和短路计算，主打大批量场景下的速度。

## 适用场景

- 适合：配电网（含不平衡三相）潮流和状态估计；需要对成千上万个负荷/光伏场景批量算潮流，用来生成机器学习训练数据或做时序分析。
- 不适合：输电网经济调度、容量规划（换 PyPSA）；刚入门只想几行建一个小算例（pandapower 更顺手）。

## 快速用法

对照上游 README（2026-11-04 版本）：

```bash
pip install power-grid-model
```

建模与求解示例以官方 [power-grid-model-workshop](https://github.com/PowerGridModel/power-grid-model-workshop/tree/main/examples) 的潮流与状态估计 notebook 为准；本笔记不复写接口细节（未核实）。

## 推荐理由

和 pandapower 互补：同样开源（MPL-2.0），但面向配电网运营商的生产级批量计算，并配有 power-grid-model-io 格式转换和官方 AI agent skills 仓库，适合讲「电网计算如何为 AI 供数」。

## 入库日期

2026-11-04

## 源链接

https://github.com/PowerGridModel/power-grid-model

## 是否已 Star

是（2026-11-04，每周策展自动化代为点亮）。
