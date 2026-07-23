# Project Instructions (Standalone Template)

Use this template when no compatible global instruction file applies or when the project needs a self-contained instruction file. Replace a field only with information verified from the project or explicitly supplied by the user. Keep unknown information blank, mark it as pending confirmation, or ask the smallest necessary question. Do not invent commands, paths, directory roles, deployment procedures, or Agent configuration locations.

## Minimum Safety Boundaries

- Read the available project instructions, relevant files, build configuration, CI, and Git status before changing project content. Do not invent APIs, configuration, commands, paths, directory responsibilities, or deployment procedures.
- Do not expose or write secrets, tokens, passwords, cookies, or environment-variable values into code, logs, documentation, or Git. Use the project's existing credential-management approach when needed.
- Make only the minimum change needed for the current request. Preserve unrelated work and explain assumptions or tradeoffs only when they materially affect the result.
- Before deleting, overwriting, installing, using the network, publishing, deploying, pushing, or changing an external system, explain the specific target and impact, provide verification and rollback information, and wait for explicit confirmation. Before a shutdown, restart, logout, user switch, or application close/restart, also explain the risk to unsaved work and wait for confirmation for that occurrence.
- Diagnose with evidence such as logs, screenshots, tests, or reproduction results. Identify root causes; do not hide failures by suppressing errors, skipping checks, or fabricating results.
- After a change, inspect the actual output and run the fastest relevant verification. Add or update tests when behavior, boundaries, or regression risk require it; explain why when tests are not added. A successful command does not by itself authorize a commit, push, deployment, or publication.
- Treat Git actions as separate authorization: inspect status before work, ask before committing, and do not push or publish without explicit confirmation.

## Project Scope

- Project purpose and in-scope work: [verified project fact or pending confirmation]
- Out-of-scope work: [verified project fact or pending confirmation]
- Intended users and compatibility commitments: [verified project fact or pending confirmation]

## Authority and Instruction Hierarchy

- Authoritative project sources: [verified files or user-specified sources]
- Applicable instruction-file hierarchy and scope: [verified hierarchy or pending confirmation]
- Protected areas and change restrictions: [verified project fact or pending confirmation]
- Conflict handling: explain an unresolved conflict between visible instructions and request direction before proceeding.

## Repository Entry Points and Facts

- Primary entry points: [verified project fact or pending confirmation]
- Important directories and their responsibilities: [verified project fact or pending confirmation]
- Dependencies, toolchain, naming, and code-style constraints: [verified project fact or pending confirmation]
- Configuration and environment assumptions: [verified project fact or pending confirmation]

## Verified Commands

| Task | Verified command | Evidence or source | Status |
| --- | --- | --- | --- |
| Build | [leave blank until verified] | [verified source] | [verified or pending] |
| Test | [leave blank until verified] | [verified source] | [verified or pending] |
| Check or lint | [leave blank until verified] | [verified source] | [verified or pending] |
| Format | [leave blank until verified] | [verified source] | [verified or pending] |
| Local run | [leave blank until verified] | [verified source] | [verified or pending] |

## Project Acceptance and Delivery Constraints

- Required behavior, acceptance checks, and compatibility expectations: [verified project fact or pending confirmation]
- Test, review, release, and deployment restrictions: [verified project fact or pending confirmation]
- Known risks, migration constraints, or protected interfaces: [verified project fact or pending confirmation]

## Candidate, Write, and Verification Workflow

1. Discover the target environment and existing instructions read-only.
2. Select the standalone mode and prepare a candidate using only verified project facts.
3. Show the target, rationale, diff, verification method, and rollback method.
4. Wait for explicit confirmation before writing or merging.
5. Read the written file back and verify its content, scope, and relationship to visible parent and child instructions.
