# frangoteam/FUXA

## 简介

浏览器里的 SCADA / HMI：画监控画面，用 Modbus、OPC UA、MQTT、西门子 S7 等去连设备或仿真器。

## 适用场景

- 适合：做一张简单过程画面，接 ProtoForge 里的虚拟从站，把「通信 + 画面」串成一次课。
- 不适合：直接当生产 SCADA。入库时开放 issue 约三百条，协议连接和界面问题要自己核对后再用。

## 快速用法

对照上游 README（2026-10-28 版本）：

```bash
docker run -d -p 1881:1881 frangoteam/fuxa:latest
```

浏览器打开 http://localhost:1881 。这条命令不保留工程；要保住画面和配置，用 README 里带 `_appdata`、`_db` 等 volume 的写法。

## 推荐理由

MIT，入库时约 5.2 千 Star。协议和 ProtoForge 重叠，课堂里可以一边仿真从站、一边画画面。留下它是因为这条链路能跑通；开放 issue 多，接入前先扫未关闭的连接类问题。

## 入库日期

2026-10-28

## 源链接

https://github.com/frangoteam/FUXA

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
