# ai-governance-audit-chain · AI Governance Audit Chain

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
![Skill](https://img.shields.io/badge/type-Agent%20Skill-blue.svg)
![Standard](https://img.shields.io/badge/standard-ISO%20IEC%2042001%20%7C%20NIST%20AI%20RMF-4f8cff.svg)

> Chinese version: [README.md](README.md)

This Agent Skill generates an **auditable evidence chain aligned with ISO/IEC 42001 (AI Management System, AIMS) and NIST AI RMF** for any AI system or agent. It ships six evidence-artifact templates (decision log, risk register, model card, change record, human-oversight proof, incident ledger), a clause-mapping table, and a forensics self-check list — turning the "AI passport / XCGS governance" stance into an auditable, certifiable, externally defensible evidence base.

## Features

- Six evidence-artifact templates, ready to copy into spreadsheets.
- Clause mapping to ISO/IEC 42001 clauses and NIST AI RMF four functions.
- Pre-release / pre-certification self-check list.
- Every artifact rooted at the agent identity code (GB/Z 185) for chain-of-custody traceability.

## Quick Start

```bash
git clone --depth 1 https://github.com/SynomosAI/ai-governance-audit-chain.git
cd ai-governance-audit-chain
# cp -r . ~/.workbuddy/skills/ai-governance-audit-chain/
```

```text
Trigger phrases: AI audit evidence, auditable evidence chain, ISO 42001 evidence,
AI governance forensics, compliance evidence, audit working papers, AI management system.
```

## Six artifacts at a glance

| Artifact | Purpose |
|---|---|
| Decision Log | record every AI decision |
| Risk Register | log and track risks |
| Model Card | model/version release basis |
| Change Record | model/process change traceability |
| Human Oversight Proof | prove high-risk actions were human-reviewed |
| Incident Ledger | incident closure with CAPA |

Full field tables are in [`SKILL.md`](SKILL.md).

## License

MIT; see [`LICENSE.md`](LICENSE.md). The rights notice in SKILL.md (© 2026 注册老炮@MedXpert, MIT) is preserved verbatim.

## Security

Report issues privately per [`SECURITY.md`](SECURITY.md).

## Disclaimer

This is theoretical stance and tooling exploration, not a claim of certification, commercial delivery, or service to any customer. External standards (ISO/IEC 42001, NIST AI RMF, GB/Z 185) are paraphrases of public material — verify independently before formal citation.
