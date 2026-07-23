# 模板索引

本目录提供可复制的模板起点。模板不是自动安装器：先发现用户实际使用的 Agent 配置和既有指令，准备候选，展示目标、diff、验证与回滚方式，并在写入前等待明确确认。

| 模板类别 | 文件 | 适用情况 |
| --- | --- | --- |
| 全局 | [English](global/AGENTS.md)、[简体中文](global/AGENTS.zh-CN.md) | 用户需要跨项目稳定的协作偏好和安全边界。 |
| 项目 overlay | [English](project/AGENTS.overlay.md)、[简体中文](project/AGENTS.overlay.zh-CN.md) | 用户已具有兼容的全局规则，只需要补充已验证的项目级信息。 |
| 项目 standalone | [English](project/AGENTS.standalone.md)、[简体中文](project/AGENTS.standalone.zh-CN.md) | 没有兼容的全局规则，或项目需要自身具备最低安全边界。 |

不要将本索引或任一目录 README 复制为 `AGENTS.md` 配置。关于带确认门的流程，参阅[指南索引](../guides/README.zh-CN.md)、[安装指南](../guides/INSTALL.zh-CN.md)、[裁剪指南](../guides/CUSTOMIZE.zh-CN.md)、[项目适配指南](../guides/PROJECT.zh-CN.md)和[规则说明](../GUIDE.zh-CN.md)。这些指南不为未知 Agent 确定配置路径，也不承诺自动加载。

<a id="global-rule-mapping-and-localization-review"></a>

## 全局规则映射与本地化审校

中文全局模板有四个导航分组和 23 条有序规则。英文全局模板也有相同的四个分组和 23 条有序规则。下表是必须保留的语义审校记录；分组标题不计入规则数。

| # | 中文规则 | 英文对应项 | 审校处理 |
| ---: | --- | --- | --- |
| 1 | 用户与沟通 / 语言 | User Communication / Language | 将默认用户可见语言本地化为英文。 |
| 2 | 用户与沟通 / 用户 | User Communication / User | 语义等同。 |
| 3 | 用户与沟通 / 输入 | User Communication / Input | 语义等同，包括对语音和五笔输入的容错。 |
| 4 | 用户与沟通 / 沟通 | User Communication / Communication | 语义等同。 |
| 5 | 用户与沟通 / 反馈 | User Communication / Feedback | 语义等同。 |
| 6 | 决策与体验 / 判断 | Decisions and Experience / Judgment | 语义等同。 |
| 7 | 决策与体验 / 决策 | Decisions and Experience / Decisions | 语义等同。 |
| 8 | 决策与体验 / 体验 | Decisions and Experience / Experience | 语义等同。 |
| 9 | 决策与体验 / 复杂性 | Decisions and Experience / Complexity | 语义等同。 |
| 10 | 执行与安全 / 上下文 | Execution and Safety / Context | 语义等同。 |
| 11 | 执行与安全 / 改动 | Execution and Safety / Changes | 语义等同。 |
| 12 | 执行与安全 / 真实 | Execution and Safety / Accuracy | 语义等同。 |
| 13 | 执行与安全 / 安全 | Execution and Safety / Security | 语义等同。 |
| 14 | 执行与安全 / 删除 | Execution and Safety / Deletion | 语义等同。 |
| 15 | 执行与安全 / 命令 | Execution and Safety / Commands | 语义等同。 |
| 16 | 执行与安全 / 中断 | Execution and Safety / Interruptions | 语义等同。 |
| 17 | 执行与安全 / 介入 | Execution and Safety / Intervention | 语义等同。 |
| 18 | 验证与沉淀 / 排查 | Verification and Preservation / Diagnosis | 语义等同。 |
| 19 | 验证与沉淀 / 验收 | Verification and Preservation / Acceptance | 语义等同。 |
| 20 | 验证与沉淀 / 验证 | Verification and Preservation / Verification | 语义等同。 |
| 21 | 验证与沉淀 / 测试 | Verification and Preservation / Testing | 语义等同。 |
| 22 | 验证与沉淀 / 沉淀 | Verification and Preservation / Preservation | 语义等同。 |
| 23 | 验证与沉淀 / Git | Verification and Preservation / Git | 将默认 Git 提交信息语言本地化为英文；Conventional Commits 类型保持英文。 |

除默认用户可见语言、技术术语表达和默认 Git 提交信息语言外，译文必须保留中文模板的条件、必需行为、风险级别、确认边界和验证要求。
