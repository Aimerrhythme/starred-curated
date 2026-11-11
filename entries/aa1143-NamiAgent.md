# aa1143/NamiAgent

## 简介

零基础中文 AI Agent 教程 + 可在本地运行的小型 Agent：从 100 行的 while 循环起步，每课加一项能力（工具、权限、上下文管理、Skills、MCP、子 Agent、计划、记忆），最后拆解 Claude Code、Codex 等主流 Agent 的做法。

## 适用场景

- 适合：自己或学生想从原理上弄懂「Agent 到底是什么」；给课程做一次「手写 Agent」实验，每课目录都是可运行快照，可以对比相邻两课的差异。
- 不适合：要现成的生产级 Agent 框架（选 deepagents 等）；只想用、不想看实现的场景。

## 快速用法

对照上游 README「快速开始」（2026-11-11 版本），需要 Python 3.10+：

```bash
git clone https://github.com/aa1143/NamiAgent.git
cd NamiAgent
pip install -r requirements.txt
export API_KEY=你的模型密钥          # 默认 DeepSeek，可用 BASE_URL / MODEL 换成其他 OpenAI 兼容接口
export NAMI_WORKSPACE=~/agent-workspace
mkdir -p $NAMI_WORKSPACE
cd lessons/lesson-05 && python agent.py
```

不花钱跑测试（假模型，无需 Key）：`cd lessons/lesson-11 && pytest -q`。

## 推荐理由

只依赖 `openai` 一个包、不套任何框架，每一步都能在自带网页端里看到上下文怎么变长、调了什么工具；中文讲义 + 分课代码 + 测试齐全，拿来当教学材料的成本很低。2026-10-30 新建，入库时约 500 Star，MIT。

## 入库日期

2026-11-11

## 源链接

https://github.com/aa1143/NamiAgent

## 是否已 Star

是（2026-11-11，每周策展自动化代为点亮）。
