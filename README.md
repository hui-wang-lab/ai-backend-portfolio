# AI Backend Portfolio

围绕企业级 AI 应用后端工程化的公开作品集，聚焦 RAG 知识服务、LLM Gateway、数字员工运行时、业务型 AI 应用和复杂业务链路治理。

这里收录可运行 Demo、脱敏 case study、架构图、工程文章和设计取舍说明。核心关注点包括服务边界、数据流、权限控制、日志审计、trace、评测、降级、可观测性和产品化补齐。

## 关注方向

- 企业知识接入与可信 RAG 链路
- 模型调用网关与 AI 平台服务边界
- 数字员工 / Agent 运行时建模
- 业务问答系统的评测与反馈闭环
- 状态机、幂等、超时补偿和复杂业务链路治理

## 作品主线

```text
文档解析与切片 -> 企业知识检索/RAG -> 业务型 AI 应用 -> AI 能力平台化
ChunkFlow      -> RecallForge        -> PeiLian      -> ai-platform
```

## 作品矩阵

| 作品 | 类型 | 工程侧重点 | 设计关注点 |
| --- | --- | --- | --- |
| [ai-platform](https://github.com/hui-wang-lab/ai-platform) | 可运行工程 / 平台骨架 | AI 平台服务边界、控制台、知识服务、数字员工、LLM Gateway | 企业级 AI 应用平台的能力组织与服务边界 |
| [RecallForge](https://github.com/hui-wang-lab/RecallForge) | RAG 服务 Demo | 文档接入、检索、引用、权限隔离、可追溯、可评测 | 可信 RAG 的链路设计、质量控制与评测闭环 |
| [ChunkFlow](https://github.com/hui-wang-lab/ChunkFlow) | 文档解析与切片服务 | 多解析器降级、文档类型识别、父子 chunk、质量诊断 | 文档解析、父子 chunk、切片质量与诊断链路 |
| [PeiLian](https://github.com/hui-wang-lab/PeiLian) | 业务型 AI 应用 Demo | persona、对话状态、规则评估、LLM-as-Judge、Web 报告 | 业务型 AI 应用的对话状态、评估与报告闭环 |
| [双录坐席调度 Case Study](case-studies/dual-recording-dispatch.md) | 脱敏复盘 | 状态机、幂等、超时补偿、Redis / SQL 优化、线上排查 | 复杂业务链路中的状态治理、补偿机制与性能优化 |
| [智能客服问答优化 Case Study](case-studies/customer-service-qa-optimization.md) | 脱敏复盘 | 问题归因、知识维护、命中分析、反馈闭环、RAG 迁移 | 问答系统的知识维护、问题归因与 RAG 经验迁移 |

## 能力地图

| 能力 | 对应材料 |
| --- | --- |
| RAG 工程化 | `ChunkFlow` 负责高质量切片，`RecallForge` 负责企业知识检索与 RAG 服务 |
| AI 应用后端架构 | `ai-platform` 以服务边界组织训练、知识、编排、数字员工和模型网关能力 |
| 数字员工 / Agent 建模 | `ai-platform` 与 `PeiLian` 展示 persona、run、state、event、trace 类后端建模思路 |
| 评测与可观测 | `PeiLian` 的规则评估 / LLM-as-Judge，`ChunkFlow` 的质量监控，`RecallForge` 的可评测性设计 |
| 真实业务系统经验 | 双录调度和智能客服 case study 展示状态流转、性能优化、问题归因和复盘 |
| 企业交付边界 | 所有公开内容均使用学习、重构、脱敏或合成数据，不暴露公司代码、客户数据和密钥 |

## 推荐阅读路径

快速浏览：

1. 看本页的关注方向和作品矩阵。
2. 打开 [ai-platform](https://github.com/hui-wang-lab/ai-platform)，理解整体平台边界。
3. 打开 [RecallForge](https://github.com/hui-wang-lab/RecallForge) 和 [ChunkFlow](https://github.com/hui-wang-lab/ChunkFlow)，看可信 RAG 链路。
4. 看 [双录坐席调度 Case Study](case-studies/dual-recording-dispatch.md)，确认真实业务系统经验。

技术深挖时：

- [AI 平台服务边界图](architecture/ai-platform-boundary.md)
- [RAG 工程链路](architecture/rag-engineering-chain.md)
- [阅读指南](guide/reading-guide.md)
- [工程文章](articles/README.md)

## 仓库结构

```text
ai-backend-portfolio
  README.md
  links.md
  architecture/
    ai-platform-boundary.md
    rag-engineering-chain.md
  case-studies/
    dual-recording-dispatch.md
    customer-service-qa-optimization.md
  guide/
    reading-guide.md
  articles/
    README.md
  assets/
    README.md
```

## 公开边界

本作品集只展示学习、重构或脱敏后的工程材料：

- 不包含公司私有代码。
- 不包含客户名称、客户数据、合同、真实接口地址或密钥。
- 不把 POC 包装成大规模生产系统。
- 重点展示工程建模、接口设计、数据流、日志、评测、降级和交付取舍。
