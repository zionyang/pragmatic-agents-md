# Project Instructions (Overlay Template)

Use this template only when a compatible global instruction file already applies. It adds verified project facts and project-specific constraints; it does not replace or weaken global safety, sensitive-information, deletion, or confirmation boundaries.

Replace a field only with information verified from the project or explicitly supplied by the user. Keep unknown information blank, mark it as pending confirmation, or ask the smallest necessary question. Do not infer commands, paths, directory roles, deployment procedures, or Agent configuration locations.

## Project Scope

- Project purpose and in-scope work: [verified project fact or pending confirmation]
- Out-of-scope work: [verified project fact or pending confirmation]
- Intended users and compatibility commitments: [verified project fact or pending confirmation]

## Authority and Instruction Hierarchy

- Authoritative project sources: [verified files or user-specified sources]
- Applicable instruction-file hierarchy and scope: [verified hierarchy or pending confirmation]
- Protected areas and change restrictions: [verified project fact or pending confirmation]
- Conflict handling: preserve global safety boundaries; explain any unresolved project-level conflict and ask for direction before proceeding.

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

## Working Relationship with Global Rules

- Treat this file as a project-specific supplement to the existing global rules.
- Keep user preferences as preferences; do not present them as project facts.
- Do not silently override global safety, credential protection, deletion, explicit-confirmation, or external-operation boundaries.
- Before writing a project instruction file, explain the target, selected mode, relationship to existing instructions, retained/changed/removed rules, verification method, and rollback method; then wait for explicit confirmation.
