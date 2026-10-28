# gridfm/gridfm-datakit

## 简介

为电网机器学习 / 基础模型（Grid Foundation Model）批量生成潮流数据的工具包：在标准算例上扰动负荷与拓扑，调用 PowerModels.jl 求解，并校验数据的物理一致性。

## 适用场景

- 适合：训练图神经网络做潮流近似、搭建「电网 + AI」课程的数据集、需要大量带标签潮流样本的研究。
- 不适合：只想跑几次潮流（直接用 pandapower）；环境依赖 Julia，Windows 上不支持 Python 3.12。

## 快速用法

对照上游 README（2026-10-28 版本），Python 3.10–3.12：

```bash
pip install gridfm-datakit
gridfm_datakit setup_pm                       # 安装 Julia + PowerModels + Ipopt
gridfm_datakit generate path/to/config.yaml   # 按配置生成数据；示例配置在 scripts/config/
```

也可以在 Jupyter 里用 `from gridfm_datakit.interactive import interactive_interface` 交互式配置。

## 推荐理由

「电力 + 机器学习」方向较新的项目（2025 年创建，入库时约 170 Star，Apache-2.0，近期仍在更新），解决了电网 AI 研究最缺的一环——规模化、可校验的训练数据；适合作为教辅仓 `ee-open-data-samples` 的进阶参考。

## 入库日期

2026-10-28

## 源链接

https://github.com/gridfm/gridfm-datakit

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
