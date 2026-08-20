# 有些急性子 · Joe-rq

**AI 解决方案工程师 / FDE** —— 深入业务现场，把模糊需求交付成可验证的 AI 系统。

![Role](https://img.shields.io/badge/Role-AI%20解决方案%20%2F%20FDE-blue)
![Field](https://img.shields.io/badge/Field-ToB%20AI%20落地-green)
![Focus](https://img.shields.io/badge/Focus-Agent%20·%20RAG%20·%20评测-orange)

---

## 我是谁

ToB 交付出身，行业纵深目前在医疗信息化（3 年多 HIS / LIS / PACS / 医保一线交付），从「交付项目」走到「推动全公司 AI 落地」——这套「诊断真实工作流 → 收敛可验证方案 → 交付并推动采用」的方法不绑定行业：

- **AI 赋能**：922 份员工需求调研 → 4 次公司级培训（累计上千人次）→ 10+ 个可复用 Skill 被同事日常使用并二次迭代；另有 4 场外部企业培训与技术分享
- **产品闭环**：独立完成过「需求调研 → 方案与原型 → 开发部署 → 真实用户使用 → 知识转移」的完整产品周期（见 MediAppHub）；习惯用数据反馈驱动迭代（个人内容工作流接入 33 条历史笔记数据指导选题与回退策略）
- **业务诊断**：独立完成 59 家厂商、24 万行数据的医院机器人应用场景调研（约 7 万字报告，直接向总裁汇报）
- **工程杠杆**：系统学习过大模型研发全链路（数据 / 预训练 / SFT / 评测），日常用 Claude Code / Codex 独立完成原型、评测与交付

观猹 FDE 实战共学营优秀学员（结课项目：差旅报销预审 PoC，300 单合成数据 0 error，15/15 验收用例通过）。

---

## 主要项目（AI 落地与交付）

### [harness-lab](https://github.com/Joe-rq/harness-lab) — 开源 AI 交付治理框架

- **情境**：AI Coding 让开发变快，但需求漂移、验收无据、经验不回流——快而没有治理等于失控。
- **行动**：独立设计 41 个零依赖治理脚本 + 6 个 Agent Skill，封装需求生命周期、Review/QA/Ship 证据链、范围门禁与回滚要求；PreToolUse 硬阻断 hook 防止越界写入。
- **结果**：框架自身 97 条 REQ 全程由其管理，并已用于 MediAppHub 等真实项目；17 Stars（2026-08）。

### [fde-delivery-os](https://github.com/Joe-rq/fde-delivery-os) × [ai-native-delivery-workbench](https://github.com/Joe-rq/ai-native-delivery-workbench) — FDE 交付操作系统

- **情境**：FDE 交付从机会诊断到资产复用涉及大量判断与证据，散落在文档和记忆里就无法复用。
- **行动**：把机会诊断 → SOW/Spec → 原型 → Eval → 生产化 → 复用串成可执行体系，沉淀 6 篇方法、4 套 Playbook、7 个模板与可调用 Skill，用版本化案例记录管理事实、假设与验收。
- **结果**：覆盖 7 类交付风险，10/10 项确定性测试通过（合成数据环境）。

### [MediAppHub](https://github.com/Joe-rq/MediAppHub) — 独立开发的医疗产品

- **情境**：一家客户医院信息科有真实的产品需求，等不到厂商排期。
- **行动**：独立设计并开发（19 张表 / 17 个 API / 12 个服务 / 50+ 项测试，累计交付 57 条需求），协助完成医院内网 Docker 部署。
- **结果**：2 名用户持续使用至今，基本功能反馈满意；完成知识转移，信息科可用 AI 自主优化迭代，无需本人维护。

### [travel-reimbursement-agent](https://github.com/Joe-rq/travel-reimbursement-agent) — 差旅发票智能管家

- **情境**：本人频繁差旅，发票整理与报销填报是真实痛点；企业系统闭源无 API，无法自动提交。
- **行动**：明确定位为「填报准备副驾驶」——OCR / AI Vision 识别 + 票面与口述时间线校准 + 15 条确定性规则 + 6 个 Agent Tool，CLI / Web 双入口，最终提交保留人工边界。
- **结果**：6 个核心模块 55 个测试用例，一键生成填报卡及 PDF / Excel 附件包。

### [iris-eval](https://github.com/Joe-rq/iris-eval) — 领域数据、LoRA 与评测

- **情境**：领域微调到底值不值得做？需要一个有数据的回答，而不是信仰。
- **行动**：从 196 份资料筛选 4 份官方 Guide（978 页）构建 3,100 条中文 SFT 数据（94% 领域相关）；完成 LoRA r=16 / r=32 对照实验与 lm-eval-harness 标准评测。
- **结果**：参数翻倍仅改善约 2% loss 且出现关键事实错误——不能只看 loss 判断业务可用性；发现答案抽取规则不同造成 34 个百分点的评测差异。

## 更多项目

- [**agent-flow-lite**](https://github.com/Joe-rq/agent-flow-lite) — 轻量级全栈 AI 编排平台，多模型可切换
- [**lesson-design-agent**](https://github.com/Joe-rq/lesson-design-agent) — 从一句话需求生成完整可试讲教案 + PPT
- [**academic-paper-workflow**](https://github.com/Joe-rq/academic-paper-workflow) — AI 辅助学术论文写作工作流

---

## 现在关注

FDE 交付方法论 · Agent 评测 · 企业 AI 赋能与组织采用 · AI 产品化（从 PoC 到真实用户使用）

## 联系方式

- GitHub: [@Joe-rq](https://github.com/Joe-rq)
- Email: [qrq-hit@foxmail.com](mailto:qrq-hit@foxmail.com)

---

> 不只是「会 AI 的 PM」——是能把 AI 产品从需求做到真实用户、并对业务结果负责的人。
