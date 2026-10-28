# davidmonterocrespo24/velxio

## 简介

在浏览器里仿真 Arduino、树莓派 Pico 和 ESP32：写代码、编译、看引脚和串口，不用先发板子。

## 适用场景

- 适合：单片机课预习，实验前把 Blink、串口这类程序跑通。在线编辑器不用安装。
- 不适合：自托管镜像里没有的板。STM32、树莓派 Linux、ESP32-C6 等只在 https://velxio.dev （部分要付费方案）或桌面版，Docker 镜像不含这些。

## 快速用法

在线直接打开 https://velxio.dev 。

自托管对照上游 README 的 Self-Hosting（2026-10-28）：

```bash
docker run -d --name velxio -p 3080:80 \
  ghcr.io/davidmonterocrespo24/velxio:master
```

浏览器打开 http://localhost:3080 。镜像里能跑 Arduino、Pico 和 ESP32 系列。README 还挂了几块命名卷，用来保住编译缓存；要反复编译再补上。板型以 README 的 Supported Boards 为准。

## 推荐理由

AGPL-3.0，另有商业许可（`COMMERCIAL_LICENSE.md`），入库时约 3.5 千 Star。课前预习不发板就能看到引脚和串口；自用看代码够用，改完再对外提供网络服务前先读 LICENSE。

## 入库日期

2026-10-28

## 源链接

https://github.com/davidmonterocrespo24/velxio

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
