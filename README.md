# ai-governance-audit-chain · AI 治理合规审计链

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
![Skill](https://img.shields.io/badge/type-Agent%20Skill-blue.svg)
![Standard](https://img.shields.io/badge/standard-ISO%20IEC%2042001%20%7C%20NIST%20AI%20RMF-4f8cff.svg)
![Version](https://img.shields.io/badge/version-1.0.0-informational.svg)
![Evidence Artifacts](https://img.shields.io/badge/artifacts-6%20templates-3ddc97.svg)

> English version: [README.en.md](README.en.md)

SynomosAI 四支柱体系：**身份（Identity）· 溯源（Traceability）· 治理（Governance）· 共生（Symbiosis）**——当 AI 进入商业，可信是唯一的硬通货。

> 本仓库属于 [SynomosAI](https://github.com/SynomosAI) 生态技能包的一员。生态全景见 [`synomosai-skills`](https://github.com/SynomosAI/synomosal-skills)，理论站位见 [`traceability-audit`](https://github.com/SynomosAI/traceability-audit)。

本技能为任何 AI 系统 / 智能体生成**对齐 ISO/IEC 42001（AI 管理体系 AIMS）与 NIST AI RMF** 的可审计证据链模板：六类证据工件（决策日志、风险登记册、模型卡、变更记录、人类监督证明、事件处置台账）+ 条款映射 + 取证自检清单。它把「AI 护照机制 / XCGS 治理系统」从理念落地为**可审计、可认证、可对外举证**的证据底座。

---

## ✨ 特性 / Features

- **六类证据工件模板**：每次 AI 动作按情形产出对应台账字段，可直接复制为表格。
- **条款映射表**：把工件映射到 ISO/IEC 42001 条款与 NIST AI RMF 四职能，确保证据被标准采信。
- **取证自检清单**：发布 / 认证前逐项打勾，未过不发。
- **以身份码为根**：所有工件的 `actor_agent` 关联智能体身份码（GB/Z 185），链式可溯源。
- **跨平台**：Windows / macOS / Linux。

---

## 🚀 快速开始 / Quick Start

> 前置：本技能是**模板与方法包**，无需安装运行时；把技能目录放进你的 Agent 技能目录即可触发。

```bash
# 1. 取得技能包
git clone --depth 1 https://github.com/SynomosAI/ai-governance-audit-chain.git
cd ai-governance-audit-chain

# 2. 放进 Agent 技能目录（示例：WorkBuddy）
#    cp -r . ~/.workbuddy/skills/ai-governance-audit-chain/
```

跑通后用自然语言触发，例如：「**帮我为这个 AI 决策建一条审计证据**」「**ISO 42001 需要哪些证据工件？**」「**NIST AI RMF 的 MEASURE 职能对应什么台账？**」。

---

## 📋 六类证据工件速查 / Six evidence artifacts

| 工件 | 用途 | 关键字段 |
|---|---|---|
| 1 决策日志 Decision Log | 记录每次 AI 决策 | decision_id, actor_agent, chosen, oversight, evidence_ref |
| 2 风险登记册 Risk Register | 登记与跟踪风险 | risk_id, likelihood/impact, treatment, residual |
| 3 模型卡 Model Card | 模型/版本放行依据 | model_id, intended_use, data_provenance, limitations |
| 4 变更记录 Change Record | 模型/流程变更留痕 | change_id, before/after, rollback, approver |
| 5 人类监督证明 Oversight Proof | 证明高风险动作被人审 | action_id, oversight_type, gate_result |
| 6 事件处置台账 Incident Ledger | 事件闭环 CAPA | incident_id, severity, root_cause, corrective |

字段完整说明见 [`SKILL.md`](SKILL.md) 第二节。

```text
触发词示例：
  AI 审计证据 / 可审计证据链 / ISO 42001 证据 / AI 治理取证
  合规取证 / 审计底稿 / AI 管理体系 / NIST AI RMF 证据
```

---

## 🧩 仓库结构 / Repository layout

```text
ai-governance-audit-chain/
├── README.md          # 本文件（中文主说明）
├── README.en.md       # 英文版说明
├── SKILL.md           # 技能主文件（YAML frontmatter + 全量方法与模板）
├── LICENSE.md         # MIT 许可证全文
├── CODEOWNERS         # 内容 owners
├── llms.txt           # 给 AI 的最小索引
├── llms-full.txt      # 给 AI 的完整说明
├── AGENTS.md          # 给 AI Agent 的工作指引
├── SECURITY.md        # 安全策略
└── .github/workflows/ # CI 门禁
```

---

## 仓库内容

AI 治理合规审计链（ISO 42001 / NIST AI RMF 证据模板）

## 元信息

- **技能名**：`ai-governance-audit-chain`
- **版本**：1.0.0
- **署名**：SynomosAI
- **许可**：MIT（详见仓库 LICENSE）

## 使用方式

1. 克隆本仓库或将该技能目录放入你的 Agent 技能目录（如 `~/.workbuddy/skills/`）；
2. 在 Agent 中按 `SKILL.md` 的描述触发对应能力；
3. 需要审计/合规证据的场景，参考 `SKILL.md` 内模板产出工件。

---

## License / 许可

本仓库以 **MIT** 许可证发布，全文见根目录 [`LICENSE.md`](LICENSE.md)。SKILL.md 中的权属声明（© 2026 注册老炮@MedXpert，MIT）逐字保留，未作改动。

---

## 🔒 安全 / Security

如发现安全问题，请按 [`SECURITY.md`](SECURITY.md) 私下报告，不要在公开 issue 中披露。

## 🤝 贡献 / Contributing

欢迎按 PR 流程提交改进；修改六类工件字段时请同步更新 `SKILL.md` 第二节与本 README 速查表。

---

## 免责声明

本仓库内容为 SynomosAI 的**理论站位与工具化探索**，不代表任何已获认证、已商业化交付或已服务特定客户的声明；文中涉及的 ISO/IEC 42001、NIST AI RMF、GB/Z 185 等外部标准与条款信息为公开资料转述，正式引用前请**独立核实**。API、授权码与形象大使等为路线图（roadmap）事项，尚未上线。
