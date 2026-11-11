# SanPen/VeraGrid

## 简介

Python 写的电力系统规划与仿真软件（原名 GridCal），带图形界面也能当库用：潮流、最优潮流、短路、RMS/EMT 动态、小信号稳定、随机潮流、连锁故障等，支持读 MATPOWER、PSS/E、PowerFactory、CIM/CGMES 等格式。

## 适用场景

- 适合：课堂演示时既要有 GUI 画单线图、又要能用脚本批量算；需要 CGMES/CIM 模型互通；做随机潮流、蒙特卡洛等可用于生成 ML 训练数据的分析。
- 不适合：只需要轻量的稳态潮流脚本（pandapower 上手更快）；需要严格商业认证结果的工程计算。

## 快速用法

对照上游 README「Installation」「API」（2026-11-11 版本）：

```bash
pip install VeraGrid
veragrid            # 打开图形界面
```

```python
import VeraGridEngine as vg

grid = vg.open_file("case14.m")   # 也可读 .raw / .dgs / CGMES zip 等
res = vg.power_flow(grid)         # 默认选项运行潮流
```

结果对象的字段名未逐一核实，以官方文档 https://veragrid.readthedocs.io 为准。

## 推荐理由

2015 年起持续维护，入库时约 640 Star，MPL-2.0，进入 LF Energy Landscape；和已收录的 pandapower / PyPSA 相比，它多了完整 GUI 和动态、稳定类计算，适合给专科、专升本学生做「先看图、再写脚本」的过渡。

## 入库日期

2026-11-11

## 源链接

https://github.com/SanPen/VeraGrid

## 是否已 Star

是（2026-11-11，每周策展自动化代为点亮）。
