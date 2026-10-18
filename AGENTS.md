# AGENTS.md — 给 AI Agent 的工作指引

本文件面向自动化 AI Agent（编码助手、技能加载器、知识库机器人）。人类读者请看 [README.md](README.md)。

## 这个仓库是什么

`ai-governance-audit-chain` 是一个 **Agent Skill 发布包**，不是可运行的 SDK。核心资产是 [`SKILL.md`](SKILL.md)（遵循 Agent Skills 规范，带 YAML frontmatter）。它提供对齐 ISO/IEC 42001 与 NIST AI RMF 的六类证据工件模板、条款映射与取证自检清单。

## 可用的工作命令

```bash
# 查看技能元数据（名称 / 版本 / 许可 / 作者）
head -20 SKILL.md

# 查看六类工件字段表与条款映射
grep -n "工件\|条款映射" SKILL.md
```

前置依赖：无运行时依赖；本仓为模板/方法包。

## 约定（Do）

- 修改前先读 `SKILL.md` 的 YAML frontmatter，**保持字段兼容**（`name` / `version` / `author` / `license` 等）。
- 修改六类工件字段时，同步更新 README 速查表与本文件的「六类工件」描述。
- 新增工件类型时，在 `SKILL.md` 第二、三节补字段表与条款映射行。

## 禁止（Don't）

- 不要改动 `SKILL.md` 的 `author` / `license` 字段与 `LICENSE.md` 的版权主体（© 2026 注册老炮@MedXpert）——**权属字段只由维护者变更**。
- 不要在仓库内提交任何密钥、令牌或真实客户数据。
- 不要声称本仓「已认证 / 已商用交付 / 已服务特定客户」。
- 不要把模板字段示例值当作真实证据对外举证。

## 边界

本仓专注**AI 治理审计证据模板**；不覆盖具体行业（医疗器械、金融等）的专项检查，也不替代真实认证审核。
