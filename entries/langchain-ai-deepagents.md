# langchain-ai/deepagents

## 简介

LangChain 出品的开箱即用 Agent 框架，基于 LangGraph，内置子 Agent、文件系统、上下文压缩、Shell、持久记忆、人工审批和 Skills，模型无关。

## 适用场景

- 适合：自己搭一个能做长链路多步任务的 Agent（调研、写报告、跑脚本），又不想从零写规划和上下文管理。
- 不适合：只需要单次问答或简单工具调用（直接调模型 API 更轻）；不想引入 LangChain 生态依赖。

## 快速用法

对照上游 README（2026-11-04 版本）：

```bash
uv add deepagents
```

```python
from deepagents import create_deep_agent

agent = create_deep_agent(
    model="openai:gpt-6-astra",   # 换成你可用的模型标识
    system_prompt="You are a research assistant.",
)
result = agent.invoke({"messages": "Research LangGraph and write a summary"})
```

## 推荐理由

长期维护、口碑稳定（入库时约 3.1 万 Star，MIT），文档完整并有 JS 版本；和已收录的 deepseek-harness 相比，它是可嵌入自己代码的库，而不是独立应用。

## 入库日期

2026-11-04

## 源链接

https://github.com/langchain-ai/deepagents

## 是否已 Star

是（2026-11-04，每周策展自动化代为点亮）。
