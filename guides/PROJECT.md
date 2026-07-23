# Project Adaptation Guide

This guide prepares project-level instruction candidates. It does not invent repository facts and does not authorize a write. Use [INSTALL.md](INSTALL.md) for the canonical confirmation, write, read-back, and verification workflow.

## Scope and Sources

Confirm the target project and requested scope before collecting facts. Read only the target path and the material needed to establish its constraints:

- applicable `AGENTS.md` files and their visible parent and child hierarchy;
- repository README and contributor documentation;
- build configuration, CI, package or dependency manifests, and documented commands;
- relevant source directories and protected areas;
- Git status and any project documentation that defines acceptance, compatibility, release, or deployment constraints.

Do not treat a visible instruction hierarchy as proof of an Agent product's loading order unless that product behavior is actually verified. Record the files' apparent scope and escalate unresolved conflicts instead of guessing precedence.

## Classify What You Learn

| Category | Permitted candidate treatment |
| --- | --- |
| Verified project fact | Include it with its evidence or source. Examples include documented commands, directory responsibilities, toolchain constraints, and stated compatibility commitments. |
| User preference | Keep it explicitly labeled as a preference or leave it to applicable global rules. Do not present it as a repository requirement. |
| Unknown information | Leave it blank, mark it pending confirmation, or ask the smallest necessary question. Do not infer it from convention. |

Never invent commands, paths, directory responsibilities, deployment procedures, configuration locations, APIs, or Agent configuration locations. Do not copy private paths, credentials, session material, or machine metadata into a project candidate.

## Select Overlay or Standalone

Choose an overlay candidate only when compatible global rules are known to apply. An overlay adds verified project facts and project constraints; it must not duplicate, replace, or weaken global safety, sensitive-information, deletion, explicit-confirmation, or external-operation boundaries.

Choose a standalone candidate when no compatible global rules apply, their applicability cannot be established, or the project needs self-contained minimum safety boundaries. The standalone template includes those required boundaries and must retain them.

| Decision | Template |
| --- | --- |
| Compatible global rules apply | [English overlay](../templates/project/AGENTS.overlay.md) or [Simplified Chinese overlay](../templates/project/AGENTS.overlay.zh-CN.md) |
| No compatible global rules apply, or self-contained rules are required | [English standalone](../templates/project/AGENTS.standalone.md) or [Simplified Chinese standalone](../templates/project/AGENTS.standalone.zh-CN.md) |
| Applicability remains unknown | Keep a candidate only and ask the smallest necessary question before selecting a write target. |

Use [CUSTOMIZE.md](CUSTOMIZE.md) if a current user preference or authorization policy affects the candidate.

## Prepare the Candidate and Diff

The candidate must identify:

- the target file and its discovered instruction relationship;
- the selected overlay or standalone mode and the reason for it;
- authoritative project sources and evidence for each project fact;
- retained, added, changed, and removed material;
- blank or pending fields that were not verified;
- acceptance checks, verification method, and rollback method.

For an existing target, present a reviewable diff. For a missing target, present the full proposed content as a new-file candidate. Do not write, merge, replace, create a backup, or modify a project while preparing this material.

## Handle Conflicts

When visible instructions conflict, describe the affected scope, the conflicting requirements, and the practical impact. Preserve global safety boundaries in overlay mode. Request direction before proceeding when the conflict cannot be resolved from the available instructions and verified product behavior.

## Continue Through Installation

After the user has reviewed the candidate, follow [INSTALL.md](INSTALL.md): show the complete write impact, wait for explicit confirmation, then write or merge and read the actual result back. A verified project build or test does not authorize a commit, push, deployment, or publication.

## Related Guides

- [Installation Guide](INSTALL.md): write and verification workflow.
- [Customization Guide](CUSTOMIZE.md): safety-boundary, preference, and authorization classification.
- [Rule Guide](../GUIDE.md): intent and migration boundaries for global rules.
- [Simplified Chinese project adaptation guide](PROJECT.zh-CN.md).
