# suoten/ProtoForge

## 简介

中文 Web 的工业协议仿真器：在一台电脑上模拟 Modbus TCP、西门子 S7、OPC UA、BACnet 等从站，用来测上位机、SCADA 和网关，不必先有实物 PLC。

## 适用场景

- 适合：通信实训、课程设计联调；实验室没有 PLC 时，先把协议跑通。可与本页的 FUXA、OpenModScan 对打。
- 不适合：要拿去替代现场 PLC 做联锁或报批。它仿真的是通信对象，不是控制器本体。

## 快速用法

对照上游 README（2026-10-28 版本）：

```bash
docker run -d --name protoforge -p 8000:8000 \
  -e PROTOFORGE_ADMIN_PASSWORD=admin \
  -v protoforge-data:/app/data \
  suoten/protoforge:latest
```

浏览器打开 http://localhost:8000 ，用 `admin` / `admin` 登录。官方仓库是 `suoten/ProtoForge`，Docker 镜像为 `suoten/protoforge`；同名搬运仓不要当最新版。

## 推荐理由

MIT，入库时约 280 Star。一条命令就能起多种工业从站，中文界面，正好填「有上位机、没有 PLC」的课。和 FUXA（画面）、OpenModScan（主站）可以拼成一套通信实验。

## 入库日期

2026-10-28

## 源链接

https://github.com/suoten/ProtoForge

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
