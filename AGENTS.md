# Repository Bootstrap

## Purpose and Scope

This repository distributes portable `AGENTS.md` templates and supporting Markdown guidance. It is not an installer, a private configuration archive, or authorization to modify a user's environment.

This root `AGENTS.md` is the instruction file for an Agent working **on this repository**. It is not a template for a user to install. Final user-facing templates belong only under `templates/` once they are published.

Humans may copy a completed template directly. The Agent-guided workflow is an optional safety aid, not a prerequisite for using a template.

## Language Routing

Use the language of the current user. Start with [README.md](README.md) for English or [README.zh-CN.md](README.zh-CN.md) for Simplified Chinese. Preserve precise technical terms where that makes the instruction clearer.

## Read Before Acting

Before proposing a change or an installation workflow, read the relevant repository material in this order:

1. This file.
2. The README selected by the user's language.
3. Use the index matching the user's language: [English template index](templates/README.md) or [Simplified Chinese template index](templates/README.zh-CN.md); then read the relevant global or project template and, when the request concerns templates or guides, the matching [English guide index](guides/README.md) or [Simplified Chinese guide index](guides/README.zh-CN.md).
4. For a user's target project, only the target path and its available instructions, README, contributor documentation, build configuration, CI, and Git status.

Do not treat `templates/**/AGENTS*.md` as instructions for maintaining this repository. Those files are distribution artifacts once they exist.

## Supported Request Modes

Classify a request before taking action:

| Mode | Use when | Required behavior |
| --- | --- | --- |
| Global | The user wants stable cross-project behavior. | Discover the actual Agent product and existing global rules before proposing a template. |
| Project overlay | The user already has global rules. | Add verified project facts without duplicating or weakening global safety boundaries. |
| Project standalone | The user has no global rules or requests a self-contained project file. | Include the required project facts and minimum safety boundaries. |
| Candidate only | The user wants review, comparison, or a draft. | Produce a candidate and do not write to the target environment. |

For an unknown Agent product, inspect its existing configuration or verified documentation first. Never invent an installation path, loading behavior, command, or compatibility claim.

## Safe Workflow

For any request that could affect a user environment, follow this sequence:

```text
Read repository guidance
  -> Read-only discovery
  -> Choose mode and source template
  -> Generate a candidate
  -> Show target, rationale, diff, verification, and rollback
  -> Wait for explicit confirmation
  -> Write or merge
  -> Read back and verify
```

Read-only discovery may inspect visible instructions, target-project facts, the existence and hierarchy of target files, and Git status. Do not print credentials or other sensitive content.

Before each write, overwrite, installation, network request, commit, push, deployment, publication, or other external change, explain the specific impact and wait for explicit confirmation for that action. A successful build, test, preview, or diff does not authorize any of those actions.

After a confirmed write, read the actual target file back and verify its content, scope, relationship to visible parent and child instructions, and any supported loading behavior. If loading cannot be verified, say so plainly.

## Content Boundaries

- Use verified project facts only. Omit, mark for confirmation, or ask about unknown information; never guess commands, paths, directory responsibilities, deployment processes, or configuration locations.
- Preserve core safety boundaries unless the user explicitly chooses to change them after an explanation of the risk: no fabrication, sensitive-information protection, deletion confirmation, evidence-driven diagnosis, and result verification.
- Keep modifications minimal, reviewable, and attributable to the current request.
- Do not expose or copy credentials, tokens, passwords, cookies, environment-variable values, private absolute paths, usernames, machine metadata, session material, private Git history, or local Agent metadata.
- Do not use this repository to bypass existing project instructions, user confirmation, platform permissions, or external-operation controls.

## Repository Boundaries

The global templates and project overlay and standalone templates under `templates/` remain copyable starting points; they still require discovery and confirmation before being written into a user's environment. Read the relevant guide in `guides/` for operational workflow and the root-level `GUIDE*.md` files for rule intent and migration boundaries.

Do not initialize Git, create a remote repository, commit, push, publish, or add automation unless the current user explicitly authorizes that specific action.

## Completion Checks for Repository Changes

When changing this repository, read every changed or added file back, verify relative links and file roles, inspect the actual directory structure, and report a scoped diff summary. Do not claim that unavailable templates, guides, or installation flows have been implemented or validated.
