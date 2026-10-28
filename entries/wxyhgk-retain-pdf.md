# wxyhgk/retain-pdf

## 简介

翻译 PDF 时尽量保住原来的版面、公式和结构，可以对照阅读，也可以对这篇文档做 AI 问答。

## 适用场景

- 适合：读外文手册、论文，整理成课堂材料；需要边看原文边看译文。
- 不适合：只要抽出纯文字做检索。那种需求用普通 PDF 文本提取更轻。多用户、按页计费是另一套配置，见 Docker 说明里的「多用户模式」。

## 快速用法

桌面端从 Releases 安装：https://github.com/wxyhgk/retain-pdf/releases （Windows `Setup.exe`、macOS `.dmg`、Linux `.deb`）。

要在服务器上跑，对照 `ops/deployment/docker/delivery/README.md`（2026-10-28）：

```bash
git clone https://github.com/wxyhgk/retain-pdf.git
cd retain-pdf/ops/deployment/docker/delivery
docker compose up -d
```

上游写启动后访问 http://127.0.0.1:40001 。模型密钥等配置以该目录的说明为准。

## 推荐理由

MIT，入库时约 2.7 千 Star。技术 PDF 一翻译就散版、公式乱；这个把对照留在原版面上，备课时能对着原文改讲义。

## 入库日期

2026-10-28

## 源链接

https://github.com/wxyhgk/retain-pdf

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
