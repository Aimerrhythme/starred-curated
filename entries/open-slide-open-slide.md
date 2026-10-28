# open-slide/open-slide

## 简介

给 AI agent 用的幻灯片框架：每一页是代码，整套课件可以进 git，由 agent 改，而不是锁在二进制 pptx 里。

## 适用场景

- 适合：用 AI 批量改、拆、重排课件，并且希望 diff 能看出改了哪一页。
- 不适合：交给没有 Node 环境的人当场改一页。那种场合仍用办公软件。

## 快速用法

对照上游 README 的 Get started（2026-10-28），本机需要能跑 `pnpm`：

```bash
npx @open-slide/cli init my-slide
cd my-slide
pnpm dev
```

脚手架带了给 Claude Code 用的 agent skills。页面在 `slides/<id>/index.tsx`，也可以手改。约定见仓库 `CLAUDE.md`。

## 推荐理由

MIT，入库时约 9.4 千 Star。课件要反复交给 agent 改时，二进制幻灯片几乎没法审阅；页做成代码之后，可以按 git 历史维护讲义。

## 入库日期

2026-10-28

## 源链接

https://github.com/open-slide/open-slide

## 是否已 Star

是（2026-10-28，每周策展自动化代为点亮）。
