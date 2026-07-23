# Template Index

This directory contains copyable template starting points. A template is not an automatic installer: discover the user's actual Agent configuration and existing instructions, prepare a candidate, show its target, diff, verification, and rollback, and wait for explicit confirmation before writing.

| Template family | Files | Use when |
| --- | --- | --- |
| [Global](global/README.md) | [English](global/AGENTS.md), [Simplified Chinese](global/AGENTS.zh-CN.md) | The user needs stable cross-project collaboration preferences and safety boundaries. |
| [Project overlay](project/AGENTS.overlay.md) / [中文](project/AGENTS.overlay.zh-CN.md) | The user already has compatible global rules and needs only verified project-specific additions. |
| [Project standalone](project/AGENTS.standalone.md) / [中文](project/AGENTS.standalone.zh-CN.md) | No compatible global rules apply, or the project needs its own minimum safety boundaries. |

Do not copy this index or either directory README as an `AGENTS.md` configuration. The stage 4 installation, customization, project-adaptation, and rule-explanation guides are not available yet; see [guides/README.md](../guides/README.md) for that boundary.

## Global Rule Mapping and Localization Review

The Chinese global template has four navigation groups and 23 ordered rules. The English global template has the same four groups and 23 ordered rules. The following map is the required semantic review record; group headings do not count as rules.

| # | Chinese rule | English counterpart | Review treatment |
| ---: | --- | --- | --- |
| 1 | 用户与沟通 / 语言 | User Communication / Language | Localize the default user-facing language to English. |
| 2 | 用户与沟通 / 用户 | User Communication / User | Semantic equivalent. |
| 3 | 用户与沟通 / 输入 | User Communication / Input | Semantic equivalent, including voice and Wubi input tolerance. |
| 4 | 用户与沟通 / 沟通 | User Communication / Communication | Semantic equivalent. |
| 5 | 用户与沟通 / 反馈 | User Communication / Feedback | Semantic equivalent. |
| 6 | 决策与体验 / 判断 | Decisions and Experience / Judgment | Semantic equivalent. |
| 7 | 决策与体验 / 决策 | Decisions and Experience / Decisions | Semantic equivalent. |
| 8 | 决策与体验 / 体验 | Decisions and Experience / Experience | Semantic equivalent. |
| 9 | 决策与体验 / 复杂性 | Decisions and Experience / Complexity | Semantic equivalent. |
| 10 | 执行与安全 / 上下文 | Execution and Safety / Context | Semantic equivalent. |
| 11 | 执行与安全 / 改动 | Execution and Safety / Changes | Semantic equivalent. |
| 12 | 执行与安全 / 真实 | Execution and Safety / Accuracy | Semantic equivalent. |
| 13 | 执行与安全 / 安全 | Execution and Safety / Security | Semantic equivalent. |
| 14 | 执行与安全 / 删除 | Execution and Safety / Deletion | Semantic equivalent. |
| 15 | 执行与安全 / 命令 | Execution and Safety / Commands | Semantic equivalent. |
| 16 | 执行与安全 / 中断 | Execution and Safety / Interruptions | Semantic equivalent. |
| 17 | 执行与安全 / 介入 | Execution and Safety / Intervention | Semantic equivalent. |
| 18 | 验证与沉淀 / 排查 | Verification and Preservation / Diagnosis | Semantic equivalent. |
| 19 | 验证与沉淀 / 验收 | Verification and Preservation / Acceptance | Semantic equivalent. |
| 20 | 验证与沉淀 / 验证 | Verification and Preservation / Verification | Semantic equivalent. |
| 21 | 验证与沉淀 / 测试 | Verification and Preservation / Testing | Semantic equivalent. |
| 22 | 验证与沉淀 / 沉淀 | Verification and Preservation / Preservation | Semantic equivalent. |
| 23 | 验证与沉淀 / Git | Verification and Preservation / Git | Localize the default commit-message language to English; keep Conventional Commits types in English. |

Aside from the default user-facing language, technical-term expression, and default Git commit-message language, a translation must preserve the Chinese template's conditions, required behavior, risk level, confirmation boundary, and verification requirement.
