# 小林面试笔记 AI 知识点速记

- 基于页面：`https://xiaolinnote.com/ai`
- 用途：快速回忆该页面覆盖的 AI 面试知识点
- 说明：这份笔记按网站目录页的专题结构整理，尽量贴近原页面，不额外扩写成通用教程

## 1. 页面主线

这页是 AI 面试题导航页，核心围绕 3 个已更新专题：

- `Agent 面试题`
- `RAG 面试题`
- `LLM 工具调用面试题`

页面表达出的重点是：

- AI 面试越来越偏系统化
- 不只问概念，还会追问原理、架构、选型、落地
- 真正高频的方向集中在 `Agent`、`RAG`、`工具调用`

---

## 2. Agent 面试题速记

### 2.1 页面重点

网站这一部分主要在讲：

- 什么是 `Agent`
- `Agent` 和大模型的区别
- `Agent` 的基本架构
- `Workflow / Agent / Tools` 的区别
- 常见设计范式
- 复杂任务拆解
- 记忆系统
- 多 Agent 协作

### 2.2 高频知识点

- `Agent` 是什么
- `Agent` 与传统 LLM 调用的差异
- `Agent` 的核心组件有哪些
- `ReAct`
- `Plan-and-Execute`
- `Reflection`
- 任务规划
- 长短期记忆
- 手搓 Agent
- `Multi-Agent`

### 2.3 记忆锚点

- `Agent`：不是只回答，而是会决策、会调用、会执行
- `Workflow`：流程更固定
- `Agent`：流程更动态
- `Tools`：外部能力接口
- `ReAct`：边想边做
- `Plan-and-Execute`：先规划再执行
- `Reflection`：做完再反思修正

### 2.4 面试常问词

- 什么是 Agent？
- Agent 基本架构是什么？
- Workflow、Agent、Tools 有什么区别？
- ReAct、Plan-and-Execute、Reflection 怎么理解？
- 复杂任务如何拆解？
- Agent 记忆系统怎么做？
- 为什么手搓 Agent？
- 什么是 Multi-Agent？

---

## 3. RAG 面试题速记

### 3.1 页面重点

网站这一部分主要覆盖：

- 什么是 `RAG`
- `RAG` 的完整工作流程
- `RAG` 解决什么问题
- `RAG` 与微调的区别
- 文档切割
- `Embedding`
- 向量数据库
- 检索优化
- `Query Rewrite`
- 高级 RAG
- 幻觉问题
- 效果评估
- 知识库动态更新

### 3.2 高频知识点

- `RAG` 基本流程
- `RAG` 的价值
- `Fine-tuning vs RAG`
- `Chunking`
- `Embedding`
- Vector Database
- Query 进入 RAG 后的处理链路
- Query Rewrite
- 检索优化
- `Self-RAG`
- `Corrective RAG`
- 图数据库
- 幻觉治理
- 效果评估

### 3.3 记忆锚点

- `RAG`：检索外部知识，再辅助生成
- 关键链路：`切块 -> 向量化 -> 建库 -> 检索 -> 生成`
- `微调`：偏能力塑造
- `RAG`：偏知识补充
- 好的 RAG 不只在“能查到”，还在“查得准、排得好、能更新”

### 3.4 面试常问词

- 什么是 RAG？
- RAG 的工作流程是什么？
- RAG 解决什么问题？
- RAG 和微调有什么区别？
- 文档切割怎么做？
- Embedding 是什么？
- 向量数据库如何选？
- Query Rewrite 是什么？
- 如何做检索优化？
- 什么是 Self-RAG / Corrective RAG？
- 如何减少幻觉？
- 如何评估 RAG 效果？
- 如何动态更新知识库？

---

## 4. LLM 工具调用面试题速记

### 4.1 页面重点

网站这一部分主要讲：

- `Function Calling`
- `MCP`
- `Skill`
- `A2A`
- 通信协议
- `LLM 网关`

### 4.2 高频知识点

- 什么是 `Function Calling`
- LLM 如何学会调用工具
- `Function Calling` 能力如何训练
- 什么是 `MCP`
- `MCP` 的核心内容与组成
- `MCP vs Function Calling`
- 为什么某些推理模型不支持 `MCP`
- 什么是 `Skill`
- `Skill vs MCP`
- `Function Calling / Skill / MCP` 的区别
- 什么是 `A2A`
- `A2A vs MCP`
- `MCP` 通信协议
- `SSE / WebSocket / WebRTC`
- 什么是 `LLM 网关`

### 4.3 记忆锚点

- `Function Calling`：让模型能调函数/工具
- `MCP`：工具与上下文接入的协议化方向
- `Skill`：能力封装
- `A2A`：Agent 与 Agent 协作
- 通信协议：重点看场景差异
- `LLM 网关`：偏平台层、治理层能力

### 4.4 面试常问词

- 什么是 Function Calling？
- LLM 怎么学会调用工具？
- Function Calling 如何训练？
- 什么是 MCP？
- MCP 核心内容是什么？
- MCP 和 Function Calling 有什么区别？
- 为什么有些模型不支持 MCP？
- 什么是 Skill？
- Skill 和 MCP 有什么区别？
- 什么是 A2A？
- A2A 和 MCP 有什么区别？
- SSE、WebSocket、WebRTC 如何区分？
- 什么是 LLM 网关？

---

## 5. 页面隐含的答题重点

从这个页面能提炼出 4 个统一答题方向：

- **概念**：先说清定义
- **架构**：再说组件和链路
- **区别**：再讲边界和选型
- **落地**：最后讲工程问题

也就是答题时尽量按：

`是什么 -> 为什么需要 -> 怎么做 -> 和谁不同 -> 项目里怎么落地`

---

## 6. 面试前最后速扫

如果临近面试，只扫这一页的关键词，优先记住：

- `Agent`
- `Workflow`
- `Tools`
- `ReAct`
- `Plan-and-Execute`
- `Reflection`
- `Memory`
- `Multi-Agent`
- `RAG`
- `Chunking`
- `Embedding`
- `Vector DB`
- `Query Rewrite`
- `Self-RAG`
- `Corrective RAG`
- `Function Calling`
- `MCP`
- `Skill`
- `A2A`
- `SSE`
- `WebSocket`
- `WebRTC`
- `LLM 网关`

---

## 7. 一句话总结

这页本质上是一张 AI 面试题地图，要求你围绕 `Agent`、`RAG`、`LLM 工具调用` 这三条主线，快速建立：

- 概念认知
- 关键区别
- 典型问题
- 面试问法
