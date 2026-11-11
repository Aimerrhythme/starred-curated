# davidusb-geek/emhass

## 简介

面向家庭的能量管理优化工具（Energy Management for Home Assistant）：用线性规划结合电价、光伏出力和储能，给可延迟负荷与电池排出最优日前/滚动（MPC）计划；内置基于 skforecast + scikit-learn 的负荷预测器。

## 适用场景

- 适合：讲「预测 + 优化」完整链条的用户侧能量管理案例；光伏 + 储能 + 可调负荷的课程设计；带学生对比不同负荷预测模型对调度结果的影响。
- 不适合：电网侧大规模调度（用 PyPSA 等）；没有任何实测数据、又不想接 Home Assistant 的纯理论推导。

## 快速用法

对照上游 docs/quick_start.md 与 installation_methods.md（2026-11-11 版本）：

```bash
python3 -m pip install emhass
# 或 Docker：
docker run --rm -it -p 5000:5000 --name emhass-container \
  -v /emhass/share:/share -v /emhass/secrets_emhass.yaml:/app/secrets_emhass.yaml \
  ghcr.io/davidusb-geek/emhass:latest
```

服务起来后可在 `http://localhost:5000` 网页里点优化，或：

```bash
curl -i -H 'Content-Type:application/json' -X POST -d '{}' http://localhost:5000/action/dayahead-optim
```

默认配置自带 2 个可延迟负荷、无光伏无电池，可不连 Home Assistant 先跑通；ML 预测走 `forecast-model-fit / predict / tune` 接口（见 docs/mlforecaster.md）。

## 推荐理由

2021 年起持续维护，入库时约 740 Star，MIT；把线性规划、MPC 和机器学习负荷预测放在同一个能实际落地的小系统里，比纯论文代码更接近现场，正好补上收集仓里「用户侧能量管理」这一块。

## 入库日期

2026-11-11

## 源链接

https://github.com/davidusb-geek/emhass

## 是否已 Star

是（2026-11-11，每周策展自动化代为点亮）。
