# 贡献指南

感谢你的宝贵时间。你的贡献将使这个项目变得更好！在提交贡献之前，请务必花点时间阅读下面的入门指南。

## 语义化版本

该项目遵循语义化版本。我们对重要的漏洞修复发布修订号，对新特性或不重要的变更发布次版本号，对重大且不兼容的变更发布主版本号。

每个重大更改都将记录在 `CHANGELOG.md` 中。

## 提交 Pull Request

1. Fork [此仓库](https://github.com/Tikas/Hexo-Theme-ApexFolio)，从 `main` 创建分支。新功能实现请发 pull request 到 `feature` 分支。其他更改发到 `main` 分支。
2. 使用 `npm install pnpm -g` 安装 `pnpm` 工具。
3. `vscode` 请安装 `Eslint` 插件。其它编辑器如 `webStorm` 默认启用了 `eslint` 功能则无需安装。
4. 根目录下执行 `pnpm bootstrap`。
5. 对代码库进行更改。请确保进行了相应的测试之后再提交。
6. 请在根目录下执行 `pnpm lint:fix` 进行代码格式检查。
7. 请在根目录下执行 `pnpm type-check` 进行类型检查。
8. 提交 git commit, 请同时遵守 [Commit 规范](#commit-指南)。
9. 提交 `pull request`， 如果有对应的 `issue`，请进行[关联](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword)。
10. 非 MD 文档或其他 **行尾空格没有语义** 的格式文档，请保持行尾没有空格。如果可以安装 [Trailing Spaces](https://marketplace.visualstudio.com/items?itemName=shardulm94.trailing-spaces) 插件来突出行尾的空格。

## Commit 指南

Commit messages 请遵循[conventional-changelog 标准](https://www.conventionalcommits.org/en/v1.0.0/)：

```bash
<类型>[可选 范围]: <描述>

[可选 正文]

[可选 脚注]
```

### Commit 类型

以下是 commit 类型列表:

- feat: 新特性或功能
- func: （function）小功能，增加小功能时使用这个提交，feat 是增加主要核心功能或特性时使用
- fix: 缺陷修复
- docs: 文档相关
- style: 代码风格或样式修改（不影响代码运行的变动）
- refactor: 代码重构（即不是新增功能，也不是修改bug的代码变动）包括编码过程中的代码结构调整，不是特指重构项目
- impr: （improvement）小的代码设计改进
- perf: 优化（提升性能、体验）
- test: 测试
- chore: 无关紧要的改动，例如删除用不到的注解、调整日志内容等
- revert: 回滚
- merge: 代码合并
- sync: 同步主线或分支的 Bug
- pom: 仅依赖和版本变化
- conf: 仅配置变化，Config 配置、Properties 文件
- typo: 修复小的拼写错误
- wip: （work in progress）少用，用于开发中的不完整提交，新工程开始时偶尔使用

## License

[LGPL-2.1](./LICENSE)
