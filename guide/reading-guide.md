# 阅读指南

这份指南用于帮助读者快速理解作品集的组织方式。内容按“概览、技术链路、业务复盘、公开边界”排列，既可以快速浏览，也可以沿着具体主题深入阅读。

## 快速浏览

适合先建立整体印象：

1. [作品矩阵](../README.md#作品矩阵)：了解每个公开仓库和 case study 的定位。
2. [能力地图](../README.md#能力地图)：查看 RAG、AI 平台、数字员工、评测和业务系统经验对应到哪些材料。
3. [GitHub Profile](https://github.com/hui-wang-lab)：查看公开项目入口和整体工程主线。

## 技术链路

适合关注系统设计、服务边界和 RAG 工程化细节的读者：

1. [AI 平台服务边界图](../architecture/ai-platform-boundary.md)
2. [RAG 工程链路](../architecture/rag-engineering-chain.md)
3. [ai-platform](https://github.com/hui-wang-lab/ai-platform)
4. [RecallForge](https://github.com/hui-wang-lab/RecallForge)
5. [ChunkFlow](https://github.com/hui-wang-lab/ChunkFlow)

## 业务复盘

适合关注真实业务系统治理经验的读者：

1. [双录坐席调度链路优化 Case Study](../case-studies/dual-recording-dispatch.md)
2. [智能客服问答优化 Case Study](../case-studies/customer-service-qa-optimization.md)

这两份材料重点呈现状态流转、幂等、超时补偿、性能优化、知识维护、问题归因和反馈闭环。

## 主题索引

| 主题 | 推荐材料 |
| --- | --- |
| 企业 AI 平台边界 | [AI 平台服务边界图](../architecture/ai-platform-boundary.md)、[ai-platform](https://github.com/hui-wang-lab/ai-platform) |
| 可信 RAG 链路 | [RAG 工程链路](../architecture/rag-engineering-chain.md)、[RecallForge](https://github.com/hui-wang-lab/RecallForge) |
| 文档解析与切片 | [ChunkFlow](https://github.com/hui-wang-lab/ChunkFlow) |
| 业务型 AI 应用 | [PeiLian](https://github.com/hui-wang-lab/PeiLian) |
| 复杂业务链路治理 | [双录坐席调度链路优化 Case Study](../case-studies/dual-recording-dispatch.md) |
| 问答系统优化经验 | [智能客服问答优化 Case Study](../case-studies/customer-service-qa-optimization.md) |

## 公开边界

本作品集只使用公开、重构、脱敏或合成数据材料：

- 不包含公司私有代码。
- 不包含客户名称、客户数据、合同、真实接口地址或密钥。
- Demo 不等同于生产系统，文档会明确标注工程边界和后续产品化补齐项。
- Case study 聚焦问题建模、方案设计、结果复盘和可迁移的工程经验。
