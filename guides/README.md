# Guide Index

These operational guides help a person or Agent discover an environment, prepare a candidate, obtain confirmation, write only when authorized, and verify the actual result. They are not an automatic installer and do not establish configuration paths or loading behavior for an unknown Agent product.

| Guide family | English | Simplified Chinese | Use it for |
| --- | --- | --- | --- |
| Installation | [INSTALL.md](INSTALL.md) | [INSTALL.zh-CN.md](INSTALL.zh-CN.md) | Selecting a mode, discovering a verified target, presenting a candidate, confirming a write, and reading the result back. |
| Customization | [CUSTOMIZE.md](CUSTOMIZE.md) | [CUSTOMIZE.zh-CN.md](CUSTOMIZE.zh-CN.md) | Separating core safety boundaries, user preferences, and environment or authorization policy. |
| Project adaptation | [PROJECT.md](PROJECT.md) | [PROJECT.zh-CN.md](PROJECT.zh-CN.md) | Reading project facts and instruction hierarchy, then choosing overlay or standalone mode. |
| Rule explanation | [../GUIDE.md](../GUIDE.md) | [../GUIDE.zh-CN.md](../GUIDE.zh-CN.md) | Reviewing the intent, boundary, and migration concern for each of the 23 global rules. |

Start from the repository [README](../README.md) or [Simplified Chinese README](../README.zh-CN.md), then select a template through the [template index](../templates/README.md). Agents working in this repository must also follow the [bootstrap instructions](../AGENTS.md).

All operating guides share one boundary: read-only discovery and candidate generation may precede a write, but a write, overwrite, merge, backup, installation, network action, commit, push, deployment, or publication requires its own explicit confirmation. For an unknown Agent, provide a candidate and state what cannot be verified; do not guess a target or promise automatic loading.
