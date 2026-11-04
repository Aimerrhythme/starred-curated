# pvlib/pvlib-python

## 简介

社区维护的光伏系统性能仿真工具箱：太阳位置、辐照度分解与转置、组件温度、直流/交流出力等模型都有基准实现，常被当作光伏建模的「参考答案」。

## 适用场景

- 适合：光伏出力估算、辐照数据预处理、给 LSTM / 机器学习光伏预测课题生成物理特征或物理基线；课堂演示「从气象数据到逆变器出力」的完整链路。
- 不适合：电站级电气拓扑、并网潮流（换 pandapower）；只想要一个现成的黑箱预测模型。

## 快速用法

对照上游 README 与文档（2026-11-04 版本）：

```bash
pip install pvlib
```

```python
import pandas as pd
from pvlib.location import Location

site = Location(latitude=31.2, longitude=121.5, tz="Asia/Shanghai")
times = pd.date_range("2026-06-21", periods=24, freq="1h", tz=site.tz)
clearsky = site.get_clearsky(times)   # 晴空 GHI / DNI / DHI
print(clearsky.head())
```

更完整的 `ModelChain` 出力流程见官方文档 User Guide（参数细节未逐项核实）。

## 推荐理由

入库时约 1.7 千 Star、BSD-3-Clause，十年持续维护并有 JOSS 论文可引用；学生做光伏预测时可用它补上物理模型基线，避免只拿数据硬套网络。

## 入库日期

2026-11-04

## 源链接

https://github.com/pvlib/pvlib-python

## 是否已 Star

是（2026-11-04，每周策展自动化代为点亮）。
