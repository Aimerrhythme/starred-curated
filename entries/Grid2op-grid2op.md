# Grid2op/grid2op

## 简介

把电网运行建模成序贯决策问题的测试平台：Agent 观察电网状态、执行拓扑调整/再调度等动作，用于强化学习等方法的训练与评测，是 L2RPN 竞赛的底座（最初由 RTE 开发）。

## 适用场景

- 适合：「AI + 电网调度」课程、强化学习在电力系统中的入门实验、复现 L2RPN 论文。
- 不适合：需要精确物理仿真或规划优化的研究；它关注的是运行决策接口。

## 快速用法

```bash
pip install grid2op
```

```python
import grid2op

env = grid2op.make("rte_case5_example", test=True)   # 小算例，test=True 不下载完整数据
obs = env.reset()
obs, reward, done, info = env.step(env.action_space({}))  # 空动作走一步
```

环境名和 `step` 返回值随版本可能变化（新版可能返回 5 元组，未核实），以 `getting_started/` 里的 notebook 为准，可直接在 Colab 打开。

## 推荐理由

电力系统 + 强化学习方向少有的长期维护（2019 至今）、有竞赛和论文生态的开源平台，MPL-2.0；notebook 教程从电力基础讲起，适合给 AI 背景的学生入门电网。

## 入库日期

2026-10-28

## 源链接

https://github.com/Grid2op/grid2op

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
