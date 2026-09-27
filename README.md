# 有些急性子 · Joe-rq

**AI-native FDE / AI Systems Builder** —— 从真实业务现场出发，把 AI 做成**可训练、可约束、可评测、可交付**的系统。

3 年+ 医疗信息化一线交付（HIS / LIS / PACS / 医保），习惯先问：真实问题是什么、系统边界在哪里、如何验收、出问题如何回退——现在把这套交付方法延伸到模型、Agent、Harness 与 Eval。

## 我在构建什么

一条逐渐收敛的 AI Systems Engineering 路径：

| 层级 | 关注的问题 | 代表项目 |
|---|---|---|
| **模型** | 决策模型、后训练、模型行为 | [ReJev](https://github.com/Joe-rq/ReJev) |
| **Agent** | Tools、Router、确定性与生成式协同 | [EduAssistant](https://github.com/Joe-rq/EduAssistant) |
| **Harness** | Spec、边界、Review、QA、交付治理 | [harness-lab](https://github.com/Joe-rq/harness-lab) |
| **Eval** | 受控评测、证据链、可复现 | [MedMirror](https://github.com/Joe-rq/MedMirror) |
| **Delivery** | 从需求发现到部署、采用与复用 | [MediAppHub](https://github.com/Joe-rq/MediAppHub) / [ai-native-delivery-workbench](https://github.com/Joe-rq/ai-native-delivery-workbench) |

## 代表项目

### [ReJev](https://github.com/Joe-rq/ReJev) — 轻量决策模型后训练

基于 MiniCPM5-2B，独立复现 Jev 风格选项决策模型的训练与评测流程。重点不是「复刻 Jev」，而是通过完整受控实验，理解决策模型如何训练、模型能力结论如何被可靠证明。

**51.11% → 80.50%（+29.39pp）· 1,892 题封存留出集 · 0% 无效输出 · 训练成本 $5.31**

### [MedMirror](https://github.com/Joe-rq/MedMirror) — 可复核的医疗大模型 Eval 工作流

面向大模型呈现差异研究：受控协议、有界追问、来源查证、Evidence Package。重点不是让模型「回答一次」，而是让整个评测过程可以复现、追溯、审计。

**30 条真实模型试次 · 284 项离线测试 · 预算硬闸 + CI 四闸**

### [harness-lab](https://github.com/Joe-rq/harness-lab) — AI Coding 交付治理 Harness

AI Coding 让开发变快，也带来需求漂移、Agent 越界、Review 无据、QA 缺证据。harness-lab 把需求生命周期、范围门禁、Review/QA/Ship 证据链固化为脚本与 Skill——当 AI 成为软件生产主体之一，工程体系必须跟上。

**41 个零依赖治理脚本 · 6 个 Agent Skill · 97 条 REQ 自举验证**

## 从实验到真实交付

### [MediAppHub](https://github.com/Joe-rq/MediAppHub) — 独立交付的医疗产品

一家客户医院信息科的真实需求，等不到厂商排期。我独立完成需求沟通、产品设计、开发测试与院内 Docker 部署，并完成知识转移——信息科可以脱离我自主迭代。

**19 张表 · 17 个 API · 50+ 项测试 · 2 名真实用户持续使用至今**

它要回答的问题只有一个：系统最后能不能真正被部署、被使用、被接手。

## 我的工程原则

**1. 能确定性解决的，不默认交给 LLM。**
EduAssistant 用「规则 → 工具 → 生成」三层路由，把确定性问题从 LLM 路径上剥离：11 个工具、23 项测试、40 case × 4 领域 Benchmark。

**2. 没有 Eval，就不要轻易相信 Demo。**
封存留出集与统计检验（ReJev）、Run Archive 与来源查证（MedMirror）、34 个百分点的评测口径教训（iris-eval）——结论必须附带证据链。

**3. 最终交付的是系统，不是 Prompt。**
Spec、Harness、Eval、部署、知识转移——目标是下一位接手者（人或 Agent）能继续运行、测试和迭代。

## 更多项目

[iris-eval](https://github.com/Joe-rq/iris-eval) · [fde-delivery-os](https://github.com/Joe-rq/fde-delivery-os) · [ai-native-delivery-workbench](https://github.com/Joe-rq/ai-native-delivery-workbench) · [travel-reimbursement-agent](https://github.com/Joe-rq/travel-reimbursement-agent) · [lesson-design-agent](https://github.com/Joe-rq/lesson-design-agent)

## 现在关注

决策模型与后训练 · Agent Harness · Eval-driven Development · FDE 与企业 AI 交付

## 联系方式

- GitHub: [@Joe-rq](https://github.com/Joe-rq)
- Email: [qrq-hit@foxmail.com](mailto:qrq-hit@foxmail.com)

> 我不只对「做出 Demo」负责，更对问题判断、交付边界和真实采用负责。
