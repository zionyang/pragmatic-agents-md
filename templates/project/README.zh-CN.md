# 项目模板

兼容的全局指令文件已经生效时，选择 overlay 模板：

- [英文 overlay](AGENTS.overlay.md)
- [简体中文 overlay](AGENTS.overlay.zh-CN.md)

没有兼容的全局指令文件，或项目需要自包含的最低安全边界时，选择 standalone 模板：

- [英文 standalone](AGENTS.standalone.md)
- [简体中文 standalone](AGENTS.standalone.zh-CN.md)

四份模板都将项目事实留空。只有来自已验证项目证据或用户明确指示的信息，才能填入命令、路径、目录职责、工具链事实、配置假设、验收检查、发布约束和部署细节。未知信息必须保持为空、标记为待确认，或引出必要的问题。

overlay 模板补充全局规则，不得重复或削弱全局安全、凭据、删除、明确确认或外部操作边界。standalone 模板不依赖全局规则，并包含所需的最低安全边界。项目事实发现和模式选择见[项目适配指南](../../guides/PROJECT.zh-CN.md)，确认与验证见[安装指南](../../guides/INSTALL.zh-CN.md)，更广泛的选择见[模板索引](../README.zh-CN.md)。
