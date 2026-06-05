# Articles

这个目录用于沉淀与作品集主线相关的工程文章。文章优先保持长期有效，围绕系统设计、工程取舍、业务复盘和 AI 应用后端能力展开。

## 选题规划

| 文章 | 主题 | 对应材料 | 状态 |
| --- | --- | --- | --- |
| 企业级 RAG 为什么不能只做向量检索 | RAG 链路、引用、拒答、评测 | [RAG 工程链路](../architecture/rag-engineering-chain.md)、[RecallForge](https://github.com/hui-wang-lab/RecallForge) | Planned |
| LLM Gateway 的服务边界 | 参数白名单、超时、fallback、request_id、日志 | [AI 平台服务边界图](../architecture/ai-platform-boundary.md)、[ai-platform](https://github.com/hui-wang-lab/ai-platform) | Planned |
| 从 FAQ 优化到 RAG query log 与评测集 | 问答系统经验迁移、badcase 归因、评测闭环 | [智能客服问答优化 Case Study](../case-studies/customer-service-qa-optimization.md) | Planned |
| 状态机、幂等与超时补偿 | 复杂业务链路治理、性能优化、可观测 | [双录坐席调度链路优化 Case Study](../case-studies/dual-recording-dispatch.md) | Planned |

## 写作原则

- 聚焦工程问题，不写泛泛的技术趋势。
- 每篇文章尽量连接一个公开项目、架构图或 case study。
- 只使用公开、重构、脱敏或合成数据材料。
- 保留设计取舍、限制条件和后续演进方向。
- 不包含公司私有代码、客户数据、合同、真实接口地址或密钥。

## 文章模板

```text
# 标题

## 背景

这篇文章讨论的业务场景和工程问题。

## 问题

系统设计中遇到的边界、风险或复杂度。

## 方案

模块划分、数据流、接口边界和关键取舍。

## 结果

能改善什么，仍有哪些限制。

## 后续演进

如果继续产品化，还需要补齐什么。
```
