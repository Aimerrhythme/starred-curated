# e2nIEE/pandapower

## 简介

基于 pandas 的电力系统建模与分析库，兼容 MATPOWER / PYPOWER 算例格式，支持潮流、短路、状态估计、最优潮流等，由 Kassel 大学与 Fraunhofer IEE 维护。

## 适用场景

- 适合：配电网/输电网潮流计算教学、课程设计、用 IEEE 标准算例做实验；结果直接是 DataFrame，便于接机器学习。
- 不适合：电磁暂态（EMT）仿真，或需要商用软件认证结果的工程报批。

## 快速用法

```bash
pip install pandapower
```

```python
import pandapower as pp
import pandapower.networks as pn

net = pn.case9()      # IEEE 9 节点算例
pp.runpp(net)         # 牛顿-拉夫逊潮流
print(net.res_bus)    # 各母线电压幅值/相角
```

接口以官方 Minimal Example（https://www.pandapower.org/start/）为准；Binder 上有交互教程。

## 推荐理由

持续维护近十年（入库当天仍有提交），BSD-3 许可，文档和教程完整，是 Python 生态里讲潮流计算最顺手的工具；配套的 SimBench 数据可直接做场景实验。

## 入库日期

2026-10-28

## 源链接

https://github.com/e2nIEE/pandapower

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
