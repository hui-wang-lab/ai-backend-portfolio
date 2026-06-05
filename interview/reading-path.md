# 面试阅读路径

## 给 HR / 猎头的 30 秒版本

我主要展示的是 AI 应用后端工程化能力，不是算法论文或纯前端展示页。作品集中有可运行工程、RAG 链路、业务型 AI 应用和脱敏业务系统复盘，适合 AI 应用后端负责人、Java 技术经理、RAG 应用架构方向。

建议只看：

1. [README 作品矩阵](../README.md#作品矩阵)
2. [GitHub Profile](https://github.com/hui-wang-lab)
3. [ai-platform](https://github.com/hui-wang-lab/ai-platform)

## 给技术面试官的 3 分钟版本

建议阅读顺序：

1. [AI 平台服务边界图](../architecture/ai-platform-boundary.md)
2. [RAG 工程链路](../architecture/rag-engineering-chain.md)
3. [RecallForge](https://github.com/hui-wang-lab/RecallForge)
4. [ChunkFlow](https://github.com/hui-wang-lab/ChunkFlow)
5. [双录坐席调度 Case Study](../case-studies/dual-recording-dispatch.md)

看完后能判断：

- 我是否理解企业 AI 平台的服务边界。
- 我是否理解可信 RAG，而不是只会向量库查询。
- 我是否有真实业务系统的状态、幂等、补偿和性能优化经验。

## 面试时如何引出作品

开场不要直接甩链接，可以这样说：

> 我这次准备了一份作品索引，里面把 AI 平台、RAG 知识服务、文档切片服务和双录调度链路做了整理。如果后面聊到具体技术点，我可以结合里面的架构图、接口设计和脱敏 case study 展开。

被问 RAG 时：

> 我在作品里的 RAG 链路不是只做向量查询，而是从文档解析、父子 chunk、ingest、召回、rerank、拒答、引用和 query log 形成一条工程链路。ChunkFlow 负责文档理解和切片，RecallForge 承接知识服务边界。

被问是否真实项目时：

> 公司项目代码和客户数据不能公开，所以我把真实经验拆成两类公开材料：一类是脱敏 case study，讲问题、方案和结果；另一类是用合成数据重构的 Demo，展示我对技术链路的理解和落地能力。

被问从 Demo 到生产差什么：

> 我不会把 Demo 包装成生产系统。我的文档会专门写权限、审计、日志、评测、降级、容量评估和产品化补齐项，因为这些才是企业 AI 应用真正难交付的地方。
