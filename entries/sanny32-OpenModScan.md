# sanny32/OpenModScan

## 简介

开源 Modbus 主站（客户端）调试工具，支持 Modbus TCP 和 RTU，用来读写寄存器、扫地址，替代商业软件 ModScan。

## 适用场景

- 适合：当上位机去连 ProtoForge 或其他 Modbus 从站，核对功能码、地址和字节序。
- 不适合：要嵌进自己程序的协议库。它是桌面调试器，不是客户端 SDK。

## 快速用法

从 Releases 装现成包，不必先编译：https://github.com/sanny32/OpenModScan/releases

入库时最新标签 `1.16.1` 有 Windows 安装包（`.exe`）和 Linux 包（`.deb`、`.rpm`、Flatpak）。从源码编译需要 Qt 5.15 及以上，步骤在 README。

连 ProtoForge 时，从站地址和端口以仿真器里该设备的配置为准。

## 推荐理由

MIT，入库时约 730 Star。实验里常用 ModScan 这类主站，商业版不方便发给学生；这里有现成的 Win/Linux 包，和 ProtoForge 拼起来就是主站加从站。

## 入库日期

2026-10-28

## 源链接

https://github.com/sanny32/OpenModScan

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
