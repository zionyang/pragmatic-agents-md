# Global Rule Guide

This guide explains the intent, boundary, and migration concern for every rule in the English global template. The normative text remains [templates/global/AGENTS.md](templates/global/AGENTS.md). This guide does not create an alternative template, grant new authority, or weaken a template rule.

For the corresponding Chinese explanations, see [GUIDE.zh-CN.md](GUIDE.zh-CN.md). The published [template index](templates/README.md#global-rule-mapping-and-localization-review) records the required Chinese-English mapping.

## How to Use This Guide

Use a row below when reviewing a candidate or migrating an existing rule file. Preserve the source rule's trigger, required behavior, risk level, confirmation boundary, and verification requirement. If an explanation and a template appear to differ, report the discrepancy and use the template as the normative source until the documentation is corrected.

## Design Principles and Use

### Keep the Global Layer Lean

Global instructions stay active across projects and conversations. Long instructions consume context and increase the chance of duplicated rules, conflicts, and diluted priorities. Keep the global layer to rules that are frequent across projects and non-negotiable.

Group rules by topic so people and models can find the relevant boundary quickly. Group headings are for navigation only: they do not count as rules and do not establish priority. The actual constraint is the behavior boundary attached to each label.

### Judge Rule Quality

Do not optimize for the fewest words or attempt to enumerate every boundary. Aim for the smallest set that is still sufficient. Use this as a check when adding, merging, or removing a rule:

```text
Rule quality
= clear necessary boundaries
+ non-overlapping responsibilities
+ no contradictions
+ changes actual behavior
- repeated explanation
- hypothetical boundaries
- unnecessary process control
```

Rules create unnecessary load when several rules all require planning, clarification, and confirmation; low-risk tasks must follow the full process; proactive completion conflicts with confirmation for every action; sufficient evidence still triggers more checking; or simple tasks become formal design, documentation, and testing exercises. These problems usually come from duplication, conflict, and unnecessary process control rather than word count. Before adding a rule, check whether it fixes a recurring problem, can be merged into an existing rule, and would add process to simple tasks.

### Place Rules at the Right Layer

- **Global instructions**: language and expression preferences, deletion and high-risk-operation boundaries, Git defaults, diagnosis and verification requirements, and external-operation authorization.
- **Project-level `AGENTS.md`**: project structure and key entry points, technology and dependency management, build/test/check commands, naming/style/delivery rules, and project-specific protected areas.
- **Current conversation**: goals for this task, temporary output requirements, one-off limits such as analysis-only, and acceptance criteria for this task.

### Maintain the Rule Set

- Consider a new global rule only after the same class of problem recurs.
- State concrete behavior instead of vague standards such as "work carefully" or "ensure high quality."
- Check whether a new rule can be merged into an existing one before adding it.
- Periodically remove rules that are obsolete, rarely used, or belong in a specific project.
- Turn complex, fixed, repeated workflows into a Skill instead of putting every step into global instructions.

## Rule Mapping

| # | Template rule | Intent and boundary | Migration concern |
| ---: | --- | --- | --- |
| 1 | User Communication / Language | Set a clear user-facing language while retaining technical terms when clearer. | Change only the default language and term expression allowed by localization. |
| 2 | User Communication / User | Calibrate explanations for a technical user by leading with why, how, and user impact; provide lower-level detail when asked. | Do not replace useful explanation with unexplained implementation detail. |
| 3 | User Communication / Input | Infer likely voice, Wubi, typo, phonetic, visual, or spelling intent from context. | Keep the high-risk or material-ambiguity question threshold. |
| 4 | User Communication / Communication | Lead with conclusions and communicate directly, accurately, and neutrally. | Do not reintroduce empty promises, reassurance, or slogans. |
| 5 | User Communication / Feedback | Pair a problem report with the next action, needed input, or available options. | Do not leave the user with an isolated failure statement. |
| 6 | Decisions and Experience / Judgment | Surface evidence for flaws, alternatives, counterexamples, and risks rather than agreeing by default. | Preserve the requirement to explain the basis for a challenge. |
| 7 | Decisions and Experience / Decisions | Define goal, non-goals, impact, boundary, success criteria, and allowed external effects before implementation. | Do not add speculative features or complexity without real constraints. |
| 8 | Decisions and Experience / Experience | Make interfaces and feedback center the user goal and reduce repeated effort. | Keep core information first; reveal detail only as needed. |
| 9 | Decisions and Experience / Complexity | Let the system search, infer, and verify what it can. | Ask only for user-held information, preferences, or high-risk authorization. |
| 10 | Execution and Safety / Context | Read project conventions, relevant files, Git status, and context before existing-project work. | Preserve long-lived structure and documentation-before-practice requirements where triggered. |
| 11 | Execution and Safety / Changes | Limit edits to the current request and make each changed line traceable. | Do not use the rule to justify unrelated cleanup. |
| 12 | Execution and Safety / Accuracy | Do not invent APIs, configuration, arguments, or paths. | Search the repository or documentation, or state uncertainty. |
| 13 | Execution and Safety / Security | Keep secrets and sensitive data out of code, logs, documentation, and Git. | Use existing credential management; never migrate actual secret values. |
| 14 | Execution and Safety / Deletion | Require target, reason, impact, and a second confirmation before deletion. | Do not collapse this into general task authorization. |
| 15 | Execution and Safety / Commands | Allow read-only diagnosis and local verification directly; separate writes and external operations requiring impact disclosure and confirmation. | Preserve that successful checks do not authorize commit, push, publication, or deployment. |
| 16 | Execution and Safety / Interruptions | Treat shutdown, restart, logout, user switch, and software close or restart as occurrence-specific. | Preserve disclosure of unsaved-work risk and current confirmation. |
| 17 | Execution and Safety / Intervention | Do not fix when asked only to analyze, explain, or diagnose. | Preserve important or high-risk change explanation, verification, rollback, and no-reliable-rollback disclosure. |
| 18 | Verification and Preservation / Diagnosis | Begin with read-only evidence and identify root causes rather than concealing failures. | Do not replace evidence with suppressed errors, skipped checks, or fabricated results. |
| 19 | Verification and Preservation / Acceptance | Translate development work into verifiable goals before implementation. | Keep bug reproduction and refactor behavior checks explicit. |
| 20 | Verification and Preservation / Verification | Inspect actual output and run the fastest relevant check after a change. | Stop at success criteria; command success alone is not completion. |
| 21 | Verification and Preservation / Testing | Add or update tests when the existing test system and change risk require them. | Explain why when tests are not added. |
| 22 | Verification and Preservation / Preservation | Record long-lived work, complex investigations, and important conventions appropriately. | Favor automation or a Skill only for stable repeated work; avoid temporary documentation overhead. |
| 23 | Verification and Preservation / Git | Initialize new projects as Git repositories by default and proactively ask about a scoped commit after file changes. | Preserve separate push/publication authorization and the localized default commit language. |

## Localization Review

The English and Simplified Chinese global templates have the same four groups and 23 ordered rules. Only these published differences are localized:

- the default user-facing language;
- technical-term expression;
- the default Git commit-message language, while Conventional Commits types remain in English.

For every other rule, compare the two templates and the two guides row by row. Confirm that neither version omits a trigger, changes a required action into advice, expands Agent authority, narrows a confirmation boundary, or drops a verification requirement.

## Migration Boundaries

When moving from an existing rule file, prepare a candidate and diff first. Retain known safety boundaries unless the user explicitly chooses a change after its risk is explained. Treat unknown project facts as pending rather than filling them from convention. Follow [guides/INSTALL.md](guides/INSTALL.md) for actual write confirmation and [guides/CUSTOMIZE.md](guides/CUSTOMIZE.md) for tailoring choices.

## Related Documents

- [English global template](templates/global/AGENTS.md)
- [Simplified Chinese global template](templates/global/AGENTS.zh-CN.md)
- [Installation Guide](guides/INSTALL.md)
- [Customization Guide](guides/CUSTOMIZE.md)
- [Project Adaptation Guide](guides/PROJECT.md)
