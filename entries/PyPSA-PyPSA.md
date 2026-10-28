# PyPSA/PyPSA

## 简介

Python for Power System Analysis：面向电力与多能源系统的建模和优化框架，做机组组合、经济调度、容量扩展规划（线性/混合整数优化），默认带 HiGHS 求解器。

## 适用场景

- 适合：讲解经济调度、新能源消纳、储能配置、长期容量规划；做「高比例可再生能源」类课程项目。
- 不适合：只想算一次交流潮流细节（用 pandapower 更直接），或需要秒级动态过程。

## 快速用法

对照上游 README（2026-10-28 版本）：

```bash
pip install pypsa
```

```python
import pypsa

n = pypsa.examples.ac_dc_meshed()   # 自带示例网络
n.optimize()                        # 线性最优潮流 / 调度
n.statistics.energy_balance()       # 能量平衡统计
```

## 推荐理由

学术界能源系统规划的常用开源工具（入库时约 2.2 千 Star，MIT），社区活跃、文档系统；PyPSA-Eur 等大模型都建在它上面，学生学会后可直接读相关论文的复现代码。

## 入库日期

2026-10-28

## 源链接

https://github.com/PyPSA/PyPSA

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
