# riclolsen/json-scada

## 简介

以 MongoDB 为实时核心库的开源 SCADA / IIoT 平台与协议网关，驱动覆盖 IEC 61850、IEC 60870-5-101/103/104、DNP3、ICCP/TASE.2、Modbus、OPC UA、MQTT（Sparkplug B），带 Web HMI、SVG 画面编辑器和 PostgreSQL/TimescaleDB + Grafana 历史库。

## 适用场景

- 适合：变电站自动化、配网主站通信规约的教学演示；用 Docker 一条命令起一个带 104/61850 端口的「迷你主站」，配合仿真从站做实训；把 SCADA 历史数据导出给 ML 做分析。
- 不适合：只需要 Modbus 小实验（FUXA、OpenModScan 更轻）；未经安全评估直接接入生产网络。

## 快速用法

对照上游 README「Running Via Docker」（2026-11-11 版本）：

```bash
sudo docker run -p 80:80 -p 9000:9000 -p 4840:4840 -p 2404:2404 -p 20000:20000 \
  -d --name=json_scada ricardolo/json-scada:latest
```

浏览器打开 `http://127.0.0.1`，默认账号见上游 README（演示用，部署时务必改密码）。2404 为 IEC 104 端口，4840 为 OPC UA。

## 推荐理由

上游说明其已在两个大型调度中心（80+ 变电站、约 9 万测点）和约 40 座 230 kV 以下变电站当地运行 5 年以上；电力专用规约覆盖面在开源项目里少见，是已收录 FUXA（通用工控 HMI）的电力侧补充。2020 年起持续维护，入库时约 500 Star，GPL-3.0。

## 入库日期

2026-11-11

## 源链接

https://github.com/riclolsen/json-scada

## 是否已 Star

是（2026-11-11，每周策展自动化代为点亮）。
