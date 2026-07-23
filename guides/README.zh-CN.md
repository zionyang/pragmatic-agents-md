# 指南索引

这些操作指南帮助人类用户或 Agent 发现环境、准备候选、取得确认，只在获得授权后写入，并验证实际结果。它们不是自动安装器，也不为未知 Agent 产品确定配置路径或加载行为。

| 指南类别 | 英文 | 简体中文 | 用途 |
| --- | --- | --- | --- |
| 安装 | [INSTALL.md](INSTALL.md) | [INSTALL.zh-CN.md](INSTALL.zh-CN.md) | 选择模式、发现已验证目标、展示候选、确认写入并回读实际结果。 |
| 裁剪 | [CUSTOMIZE.md](CUSTOMIZE.md) | [CUSTOMIZE.zh-CN.md](CUSTOMIZE.zh-CN.md) | 区分核心安全边界、用户偏好以及环境或授权策略。 |
| 项目适配 | [PROJECT.md](PROJECT.md) | [PROJECT.zh-CN.md](PROJECT.zh-CN.md) | 读取项目事实和指令层级，再选择 overlay 或 standalone 模式。 |
| 规则说明 | [../GUIDE.md](../GUIDE.md) | [../GUIDE.zh-CN.md](../GUIDE.zh-CN.md) | 审阅 23 条全局规则各自的意图、边界和迁移关注点。 |

从仓库[英文 README](../README.md)或[简体中文 README](../README.zh-CN.md)开始，再通过[简体中文模板索引](../templates/README.zh-CN.md)选择模板。维护本仓库的 Agent 还必须遵循[bootstrap 指令](../AGENTS.md)。

所有操作指南共用一个边界：只读发现和候选生成可以先于写入；但写入、覆盖、合并、备份、安装、联网、提交、推送、部署或发布都需要各自的明确确认。对于未知 Agent，提供候选并说明无法验证的部分；不得猜测目标，也不得承诺自动加载。
