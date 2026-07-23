# Customization Guide

This guide explains how to tailor a template without turning preferences into project facts or weakening safety boundaries by accident. It prepares a candidate; [INSTALL.md](INSTALL.md) is the authority for the write, confirmation, and read-back workflow.

The published templates are the rule baseline. Do not replace a rule with a new interpretation merely because a shorter or more convenient version seems desirable. Use [GUIDE.md](../GUIDE.md) when a rule's intent or migration boundary is unclear.

## Start With Evidence

Before editing a candidate, read the applicable template, existing instructions, the requested target scope, and verified project material. Keep each possible addition in one of three categories:

| Category | Default treatment | Examples |
| --- | --- | --- |
| Core safety boundaries | Preserve by default. Explain the risk and obtain explicit confirmation before weakening, removing, or changing a trigger. | No fabrication, sensitive-information protection, deletion confirmation, evidence-driven diagnosis, result verification, and current-occurrence authorization. |
| User preferences | Localize when the user explicitly states a preference or an applicable existing rule provides evidence. Do not present them as project facts. | User-facing language, technical explanation depth, communication style, input tolerance, and default commit-message language. |
| Environment and authorization policy | Determine from the real Agent, project, and current user authorization. Do not treat an earlier or general authorization as continuing permission. | Writes, overwrites, installations, network use, deletion, commits, pushes, deployments, publications, and interruptions. |

## Core Safety Boundaries

The following behavior must remain unless the user explicitly chooses a change after its risk is explained:

- do not invent APIs, configuration, commands, paths, directory responsibilities, deployment procedures, or Agent configuration locations;
- do not expose or write secrets, tokens, passwords, cookies, or environment-variable values;
- require the stated deletion and external-operation confirmations;
- diagnose from evidence and identify root causes rather than hiding failures;
- inspect actual results and run proportionate verification after a change;
- keep Git, publishing, deployment, and interruption actions separately authorized.

An explanation may make these boundaries easier to follow, but it must not add an unverified exception, broaden Agent autonomy, or reduce a current-occurrence confirmation to a one-time preference.

## User Preferences

Preferences may be localized where evidence supports them. Preserve the distinction between a preference and a project fact. For example, a user's preferred communication language belongs in a global rule or an explicitly marked preference, not in a project command table. A repository's documented required release procedure is a project fact, not a personal preference.

For the global template pair, only the published localization differences are assumed by default: user-facing language, technical-term expression, and default commit-message language. All other conditions, required behavior, confirmation boundaries, and verification expectations must remain equivalent.

## Environment and Authorization Policy

Read-only discovery and local verification may be allowed by an applicable instruction, but a candidate must not silently grant permission for writes or external actions. State the impact of each requested action and wait for explicit confirmation for that occurrence.

Do not create a policy that claims support for an unknown Agent. When the product's configuration entry or loading behavior is not verified, keep the result as a candidate and state the limitation.

## Ask or Discover

Discover information read-only when it can be established from visible sources. Ask the user only when the answer is uniquely held by the user, changes the result materially, or grants high-risk authority.

| Discover read-only | Ask the user when needed |
| --- | --- |
| Existing instruction files, their visible hierarchy, and target-file existence. | Whether the target is global, a project root, a specified subdirectory, or candidate only when the request does not establish it. |
| Existing Agent configuration or verified official documentation. | Whether to preserve, merge, or replace an existing rule file. |
| README, contributor documentation, build configuration, CI, Git status, and documented project commands. | A preferred language, audience, or commit-message convention when no reliable instruction states it. |
| Applicable existing preferences and verified project facts. | A requested weakening of a core safety boundary or a changed confirmation policy. |
| Evidence for a command, directory responsibility, compatibility commitment, or deployment restriction. | A conflict among visible instructions that cannot be resolved from their scope. |

Never ask a user to disclose a secret in order to customize a template. Do not print sensitive content discovered during inspection.

## Candidate Review Checklist

Before handing a candidate to [INSTALL.md](INSTALL.md):

1. Mark each addition as a verified project fact, user preference, or pending confirmation.
2. Remove guessed commands, paths, directory roles, configuration locations, and product claims.
3. Compare any changed core boundary with the source template and describe the risk.
4. State the selected language and the source for each non-default preference.
5. Link the candidate to the applicable verification and rollback plan.

## Related Guides

- [Installation Guide](INSTALL.md): canonical write and verification state machine.
- [Project Adaptation Guide](PROJECT.md): obtain verified project facts and select a project template mode.
- [Rule Guide](../GUIDE.md): one-to-one explanations for the 23 global rules.
- [Simplified Chinese customization guide](CUSTOMIZE.zh-CN.md).
