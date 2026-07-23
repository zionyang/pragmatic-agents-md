# Installation Guide

This guide explains how to prepare and, only after explicit confirmation, place a copyable template in an Agent or project environment. It is not a one-click installer and does not establish a configuration path, file name, loading behavior, or command for any Agent product.

Use the [repository README](../README.md) to choose a language, the [template index](../templates/README.md) to choose a starting point, and the other guides linked below for tailoring and project facts. The templates remain the source of the rules themselves.

## Support Evidence

An Agent product is supported for a specific installation only when its actual configuration entry, existing configuration, or official documentation has been read and confirms the relevant behavior. Do not infer a path from a product name, another operating system, or a similar Agent.

For an unknown Agent, provide a candidate and explain what remains unverified. Do not claim that a file will be loaded automatically. A human may still copy reviewed text into an Agent entry they know is appropriate, but this guide does not make that choice on their behalf.

## Canonical Workflow

Every installation mode uses this sequence:

1. Read the repository guidance and the applicable template.
2. Discover the target environment and existing instructions read-only.
3. Select a mode and source template.
4. Generate a candidate using verified information only.
5. Show the target, rationale, diff, risks, verification method, and rollback method.
6. Wait for explicit confirmation for the proposed write or merge.
7. Write or merge only after that confirmation.
8. Read the result back and verify its content, scope, and any loading behavior that can actually be verified.

The candidate-only branch stops after step 5. It does not create a file, backup, installation, network request, commit, push, deployment, or publication.

## Read-Only Discovery

Before selecting a mode, inspect only the information needed to establish the target and its constraints:

- the user's requested scope: global, project root, a specified project subdirectory, or candidate only;
- the Agent's existing configuration and verified documentation, when a product-specific target is requested;
- existing global and project instruction files, including their visible hierarchy and scope;
- for a target project, its available instructions, README, contributor documentation, build configuration, CI, and Git status;
- whether the user already has compatible global rules.

Do not print or copy credentials, tokens, passwords, cookies, environment-variable values, private paths, machine metadata, or session material while inspecting these sources.

## Choose a Mode

| Mode | Use when | Candidate source | Boundary |
| --- | --- | --- | --- |
| Global | The user needs stable cross-project behavior and the actual global entry can be verified. | [Global template](../templates/global/README.md) in the user's language. | Compare with existing global rules; prefer a reviewable merge candidate. |
| Project overlay | Compatible global rules already apply to the project. | [English overlay](../templates/project/AGENTS.overlay.md) or [Simplified Chinese overlay](../templates/project/AGENTS.overlay.zh-CN.md). | Add verified project facts only; do not duplicate or weaken global safety boundaries. |
| Project standalone | No compatible global rules apply, or the project needs self-contained minimum safety boundaries. | [English standalone](../templates/project/AGENTS.standalone.md) or [Simplified Chinese standalone](../templates/project/AGENTS.standalone.zh-CN.md). | Preserve the standalone template's minimum safety boundaries. |
| Candidate only | The user wants a draft, review, or comparison, or has not authorized a write. | The applicable template and verified evidence. | Stop after presenting the candidate and diff. |
| Unknown Agent | The Agent's entry or loading behavior cannot be verified. | The applicable template as plain candidate text. | Do not guess a target or promise automatic installation. |

Use [PROJECT.md](PROJECT.md) before selecting an overlay or standalone project candidate. Use [CUSTOMIZE.md](CUSTOMIZE.md) when the candidate needs to distinguish stable safety boundaries from preferences or authorization policy.

## Prepare a Candidate

Use only verified project facts, existing applicable rules, and explicit user instructions. Preserve unknown information as blank or pending confirmation rather than guessing it. For an existing target, show a comparison with the current content. For a missing target, show the proposed new-file content and identify it as an addition.

Before asking for write confirmation, state all of the following:

- the exact discovered target, or that no target has been verified;
- the selected mode and source template;
- the relationship to existing global, parent, or child instructions;
- rules and facts retained, added, changed, or removed;
- the verification method and any limitation on verifying actual Agent loading;
- the rollback method and any limits on reliable rollback.

## Write and Merge Rules

Do not write, overwrite, merge, create a backup, install dependencies, use the network, commit, push, deploy, or publish before the user explicitly confirms that occurrence.

When a confirmed write is authorized, prefer merging with existing rules. Create a new target only when it does not exist. Replace an existing target only when the user explicitly chooses replacement. If a backup is needed, explain its location, sensitivity, and retention before creating it.

A successful build, test, preview, acceptance check, or diff review does not authorize a commit, push, deployment, publication, or any other separate external action.

## Read-Back Verification

After a confirmed write or merge:

1. Read the actual target file back.
2. Compare it with the confirmed candidate.
3. Confirm that no secrets, private paths, machine metadata, or session material entered the target.
4. For project files, check the visible parent and child instruction relationship and report unresolved conflicts.
5. Confirm loading only by a method that is actually supported for the Agent product. If that is not possible, state that the file was written but loading remains unverified.

## Related Guides

- [Customization Guide](CUSTOMIZE.md): decide what may be tailored and when to ask.
- [Project Adaptation Guide](PROJECT.md): discover project facts and select overlay or standalone mode.
- [Rule Guide](../GUIDE.md): understand the intent and boundary of every global rule.
- [Simplified Chinese installation guide](INSTALL.zh-CN.md).
