# Project Templates

Choose an overlay template when compatible global rules already apply:

- [English overlay](AGENTS.overlay.md)
- [Simplified Chinese overlay](AGENTS.overlay.zh-CN.md)

Choose a standalone template when no compatible global rules apply or the project needs self-contained minimum safety boundaries:

- [English standalone](AGENTS.standalone.md)
- [Simplified Chinese standalone](AGENTS.standalone.zh-CN.md)

All four templates leave project facts unfilled. Populate commands, paths, directory responsibilities, toolchain facts, configuration assumptions, acceptance checks, release constraints, and deployment details only from verified project evidence or explicit user instruction. Unknown information must remain blank, be marked for confirmation, or lead to a necessary question.

Overlay templates supplement global rules and must not duplicate or weaken global safety, credential, deletion, explicit-confirmation, or external-operation boundaries. Standalone templates include the required minimum safety boundaries without depending on global rules. See the [project adaptation guide](../../guides/PROJECT.md) for fact discovery and mode selection, the [installation guide](../../guides/INSTALL.md) for confirmation and verification, and the [template index](../README.md) for broader selection.
