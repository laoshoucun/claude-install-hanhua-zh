# Claude Code安装教程2026最新版：npm已弃用，官方推荐这四种方式

> 原文链接：[https://www.laoshoucun.com/claudedt/3698](https://www.laoshoucun.com/claudedt/3698)

朋友发来一篇 Claude Code 安装教程让我看看靠不靠谱，打开一看，开头就是 npm install -g @anthropic-ai/claude-code。这条路过时了。官方 2026 年 1 月更新了安装文档，npm 方式明确标记弃用，改推四种官方渠道。这类文章搜索引擎里一抓一大把，照着装能用，但后续版本不保证兼容。这篇按最新 README 把安装一次说清。

四种官方方式，按平台挑

MacOS 和 Linux 首选安装脚本：

curl -fsSL https://claude.ai/install.sh | bash

同一平台也可以 Homebrew：brew install --cask claude-code。

Windows 用户推荐 PowerShell：

irm https://claude.ai/install.ps1 | iex

机器上有 WinGet 的话，winget install Anthropic.ClaudeCode 走微软包管理器，后续更新更省心。npm 那条路现在还能走，但官方已标 Deprecated，新装用户没必要再从这儿进。

装完第一步：cd 进项目跑起来

装完 cd 到项目目录，敲 claude 回车进交互界面。它的定位是"住在你终端里的编程智能体"：理解整个代码库结构、执行例行任务、解释复杂代码、处理 git 工作流，全用自然语言指挥。

终端之外，同一套能力还有两个入口：IDE 扩展（VS Code 等编辑器可用），以及 GitHub 上的 @claude，在 PR 或 issue 里 @它，代码审查、修 bug 都能远程干。

新手常见问题，先备好答案

报 bug 不用翻论坛，CLI 里直接输 /bug，问题描述和上下文一起带过去，比手写 issue 高效。使用问题进官方 Claude Developers Discord，维护者和重度用户都在里面。

隐私方面官方说法明确：收集的数据包括代码接受率、会话对话和用户反馈，承诺不把用户反馈用于模型训练，会话数据访问有严格限制。

安装卡住先查两件事，系统版本是否达标，以及是否挂了代理：安装脚本要从 claude.ai 拉文件，网络不通一切白搭。跑通之后，进阶玩法（自定义命令、技能、插件）站内教程区会陆续更新，先把Claude 本身用顺手再说。

Claude Code会员中转站 微信:douhanq

---

原文链接：[https://www.laoshoucun.com/claudedt/3698](https://www.laoshoucun.com/claudedt/3698)
