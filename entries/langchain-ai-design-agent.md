# langchain-ai/design-agent

## 简介

LangChain 内部在用的设计 Agent「Content Studio」开源版：基于 Deep Agents，在 Slack 里接需求，产出按品牌规范做好的图片、幻灯片、图表和动态视频（课件、海报、短片都按「代码 → 渲染 → 检查」流程生成）。

## 适用场景

- 适合：研究「Agent + Skills + 沙箱」怎么落地成一个真实生产工具；想给课程/团队做一个按统一风格批量出图、出课件封面、出短视频的助手。
- 不适合：只想点几下出一张图（直接用图像模型更快）；没有 Docker、或不打算部署到 Slack / LangSmith 托管环境的场景，完整版依赖较重。

## 快速用法

对照上游 README「Try it locally」（2026-11-11 版本）。需要 Docker，演示用脚本化模型，不需要 API Key：

```bash
git clone https://github.com/langchain-ai/design-agent.git
cd design-agent
uv run design-agent sandbox build
uv run design-agent demo        # 输出在 workspace/out/demo/
```

在 `.env` 里配好模型 Key 后可直接提需求：

```bash
uv run design-agent ask "A LinkedIn card announcing our design review service, 1200x627."
```

## 推荐理由

和上周收录的 `langchain-ai/deepagents` 正好配套：那边是框架，这里是一个跑在框架上的完整应用，路由 Skill、35 个工作流、设计 wiki、子 Agent 与记忆分层都能直接读代码。2026-10 新开源，入库时约 600 Star，Apache-2.0，属于近期快速上涨的一类。

## 入库日期

2026-11-11

## 源链接

https://github.com/langchain-ai/design-agent

## 是否已 Star

是（2026-11-11，每周策展自动化代为点亮）。
