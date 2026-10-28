# bojieli/ai-infra-book

## 简介

李博杰的开源中文书稿《深入理解 AI Infra：量化分析与系统设计》：从硬件约束和模型架构出发，用数量级估算推导 LLM 推理与训练系统设计，附可复算书中数字的 Python 计算工具。

## 适用场景

- 适合：给学生或自己补「显存、带宽、KV 缓存、卡间通信」这类量化直觉；备课时直接引用章节和计算脚本。
- 不适合：找某个推理框架的部署手册——这是原理书，且仍是初稿，数字以最新修订为准。

## 快速用法

在线阅读：https://bojieli.github.io/ai-infra-book/ （PDF / EPUB 在 Releases）。

复算书中数字（只需 Python 3.10+ 标准库，不要 GPU）：

```bash
git clone https://github.com/bojieli/ai-infra-book.git
cd ai-infra-book
python3 calculations/calc.py models
python3 calculations/calc.py reproduce
```

## 推荐理由

中文原创、Apache-2.0、带可复现计算，入库时约 7 千 Star 且有繁中/英/俄社区译本；「搬什么、搬多少、搬几次」的分析框架很适合电气背景的学生理解 AI 算力系统，和教辅仓 `ee-ai-teaching-briefs` 能互相引用。

## 入库日期

2026-10-28

## 源链接

https://github.com/bojieli/ai-infra-book

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
