# pragmatic-agents-md

`AGENTS.md` templates and guides for people and AI coding Agents.

[阅读简体中文文档](README.zh-CN.md).

## How to Use It

- Copy a template and adapt it to your environment.
- Or let your Agent read this repository, check your existing rules and target project, and prepare a reviewable update for you.
- The Agent does not change your configuration until you approve it.

## Template Types

- **Global templates**: For preferences that should apply across projects, such as the user's language, Wubi or Pinyin input, response style, and confirmation boundaries for file changes, network access, and Git operations.
- **Project overlay templates**: For projects where compatible global rules already apply and you only need to add project-specific information, such as directory responsibilities, build and test commands, release restrictions, or areas that must not be changed.
- **Project standalone templates**: For projects where no suitable global rules are available or where the project needs its own minimum safety boundaries.

## What This Repository Provides

- English and Simplified Chinese templates for global `AGENTS.md` behavior.
- Project-level overlay and standalone templates.
- Guidance for discovering an Agent's real configuration, tailoring a candidate, obtaining confirmation, writing it, and verifying the result.
- Explanations of rule intent, boundaries, and migration choices.

It is not a one-click installer, a private configuration backup, or permission to change an existing project or Agent configuration without explicit confirmation.

## Available Materials

- [AGENTS.md](AGENTS.md) is the bootstrap instruction file for an Agent working on this repository.
- [Global templates](templates/global/README.md) are available in English and Simplified Chinese.
- [Project templates](templates/project/README.md) are available as English and Simplified Chinese overlay and standalone variants.
- [Guides](guides/README.md) are available in English and Simplified Chinese for installation, customization, and project adaptation.
- [Rule guides](GUIDE.md) and [Simplified Chinese rule guides](GUIDE.zh-CN.md) explain the 23 global rules and their migration boundaries.

The template files are copyable starting points. Do not copy a directory README as an `AGENTS.md` configuration. The guides describe a confirmation-gated workflow; they do not authorize any environment change by themselves.

## Agent Starter Prompt

Use this prompt after cloning or opening this repository with an Agent:

> Read the repository root `AGENTS.md`, then read the README in my language. Explain the available template or guide status, inspect any target environment read-only, and prepare a candidate only if the required source material exists. Before any write, overwrite, installation, network action, commit, push, deployment, or publication, show the target, rationale, diff, verification, and rollback, then wait for my explicit confirmation.

For an unknown Agent product, the Agent must discover its documented or existing configuration rather than guess a path or claim automatic loading.

## Repository Map

| Location | Role now | Planned role |
| --- | --- | --- |
| [AGENTS.md](AGENTS.md) | Active repository bootstrap instructions. | Remains the instruction file for Agents maintaining or using this repository. |
| [templates/](templates/README.md) | Active index for global, project overlay, and project standalone templates in English and Simplified Chinese. | Receives future mapping and localization updates. |
| [guides/](guides/README.md) | Active index for installation, customization, and project-adaptation guides. | Continues to route readers to the applicable operational guide. |

## Safety and Support Boundaries

Agents should use this workflow:

```text
Read repository guidance
  -> Read-only discovery
  -> Choose mode and template
  -> Generate a candidate
  -> Show diff, risk, verification, and rollback
  -> Wait for explicit confirmation
  -> Write or merge
  -> Read back and verify
```

The workflow does not authorize writes, overwrites, installation, network access, commits, pushes, deployment, publication, or any other external change. It also does not promise a fixed configuration path or automatic loading for an unknown Agent product.

## License

Documentation and templates in this repository are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Redistribution or public adaptations must provide attribution, link the license, and indicate changes. See [LICENSE](LICENSE) for the complete license text.
