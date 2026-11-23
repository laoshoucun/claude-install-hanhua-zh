# Claude克劳德 安装教程与使用指南官网下载

> **官方入口：[www.laoshoucun.com/anzhuang](https://www.laoshoucun.com/anzhuang)**
> 桌面版 / 命令行 / 网页版三种形态 · 按需选一个，不用都装

## 仓库介绍

本仓库内容整理自 [老手村](https://www.laoshoucun.com/)，已收录 17 篇，每篇都保留官网原文链接：可以在这里直接读，也可以 `git clone` 到本地检索。

Claude 是 Anthropic 推出的大模型，Claude Code 是它的命令行编程工具。国内用户卡住的地方通常不在模型本身，而在装这一步：npm 那条路官方已经弃用，照老教程装会装出问题；桌面版和命令行的能力边界也不一样。本仓库收录老手村 Claude Code 栏目里偏实操的文章，讲清楚怎么装、装完怎么用、插件和技能怎么接。


## 安装入口

Claude 分两种用法：网页版直接用，桌面客户端和命令行工具要装。

### ➡️ [点击进入 Claude 安装下载页（www.laoshoucun.com/anzhuang）](https://www.laoshoucun.com/anzhuang)

| 形态 | 适合谁 | 装法 |
| --- | --- | --- |
| 网页版 | 只想聊天、写东西 | 打开浏览器登录即可，不用装 |
| 桌面客户端 | 要发文件、长文写作 | 官网下载安装包，按系统选 |
| Claude Code（CLI） | 要它读项目、改代码 | 官方推荐的四种方式，npm 那条已弃用 |

⛔ 最常见的一个坑：照着旧教程用 npm 装 Claude Code，装出来的版本官方已经不再维护。仓库里《Claude Code安装教程2026最新版》那篇专门讲了这个，装之前先看它。

安装步骤、登录、以及装完之后怎么接插件和技能，仓库里 17 篇按时间倒序排好了。

## 主要特点

- 官方推荐的四种安装方式逐条讲，npm 弃用之后该走哪条路单独说明。
- 桌面版与命令行分开讲，多会话同时开怎么用单独一篇。
- 官方技能与插件：从官方仓库怎么装、SKILL.md 怎么写、发布要守哪几条规范。
- 团队场景单独交代：规则文件怎么写、多人协作怎么分工。
- 每篇保留官网原文链接，可在线阅读，也可 git clone 到本地检索。

## 常见问题

**npm 装 Claude Code 还能用吗？** 官方已不再推荐这条路，新版本别再照着老教程装。换成官方推荐的四种方式之一，《Claude Code安装教程2026最新版》那篇写全了。

**桌面版和命令行有什么区别？** 桌面版能开多个会话、适合长文和文档类活；命令行直接在你项目目录里干活，适合改代码。两个可以同时用。

**技能和插件是一回事吗？** 不是。技能（Skills）是给它一套做事的流程和规范，插件（Plugins）是接外部工具。装法不同，仓库里分两篇讲。

**装完登录不上怎么办？** 先确认网络能到官方服务，再检查账号地区限制。这部分不展开，按官方提示走。

## 文章目录（17 篇）

- 2026-11-21 · [想发布自己的Claude技能？官方仓库这3条规范先看清楚](https://www.laoshoucun.com/claudedt/3703) · [仓库内阅读](docs/3703-想发布自己的Claude技能？官方仓库这3条规范先看清楚.md)
- 2026-11-21 · [Claude Code官方技能怎么装：两步接入官方插件市场（实操教程）](https://www.laoshoucun.com/claudedt/3702) · [仓库内阅读](docs/3702-ClaudeCode官方技能怎么装：两步接入官方插件市场（实操教程）.md)
- 2026-11-21 · [Anthropic官方技能库全解：Word、PPT、Excel、PDF文档技能免费用](https://www.laoshoucun.com/claudedt/3701) · [仓库内阅读](docs/3701-Anthropic官方技能库全解：Word、PPT、Excel、PDF文档技能免.md)
- 2026-11-20 · [Claude自定义技能怎么做？一个SKILL.md文件就够了，官方模板直接抄](https://www.laoshoucun.com/claudedt/3700) · [仓库内阅读](docs/3700-Claude自定义技能怎么做？一个SKILL.md文件就够了，官方模板直接抄.md)
- 2026-11-20 · [Claude Code官方插件大盘点：13个免费插件，从代码审查到安全检查全齐了](https://www.laoshoucun.com/claudedt/3699) · [仓库内阅读](docs/3699-ClaudeCode官方插件大盘点：13个免费插件，从代码审查到安全检查全齐了.md)
- 2026-11-20 · [Claude Code安装教程2026最新版：npm已弃用，官方推荐这四种方式](https://www.laoshoucun.com/claudedt/3698) · [仓库内阅读](docs/3698-ClaudeCode安装教程2026最新版：npm已弃用，官方推荐这四种方式.md)
- 2026-11-04 · [Claude Code 额度不够用，让它当项目经理，活交给免费 Agent 干](https://www.sz003.com/codexdt/2752) · [仓库内阅读](docs/2752-ClaudeCode额度不够用，让它当项目经理，活交给免费Agent干.md)
- 2026-11-03 · [Grok Bot 怎么用：把 Claude Code 和 Codex 接进去，手机上派活](https://www.sz003.com/codexdt/2751) · [仓库内阅读](docs/2751-GrokBot怎么用：把ClaudeCode和Codex接进去，手机上派活.md)
- 2026-10-16 · [Claude Code 桌面版能同时开好几个会话，写代码开始像带队](https://www.laoshoucun.com/claudedt/3585) · [仓库内阅读](docs/3585-ClaudeCode桌面版能同时开好几个会话，写代码开始像带队.md)
- 2026-10-05 · [Claude Code 开放了改装权，程序员把编码工具玩成了乐高](https://www.laoshoucun.com/claudedt/3483) · [仓库内阅读](docs/3483-ClaudeCode开放了改装权，程序员把编码工具玩成了乐高.md)
- 2026-09-28 · [Anthropic 把工作台改名游乐场：不写代码也能跑通 Claude 接口](https://www.laoshoucun.com/claudedt/3396) · [仓库内阅读](docs/3396-Anthropic把工作台改名游乐场：不写代码也能跑通Claude接口.md)
- 2026-09-26 · [Opus 5.5 三个新玩法：搭乐高，改宜家说明书，复刻塞尔达](https://www.laoshoucun.com/claudedt/3360) · [仓库内阅读](docs/3360-Opus5.5三个新玩法：搭乐高，改宜家说明书，复刻塞尔达.md)
- 2026-09-26 · [实测 Opus 5.5：一句提示词出 100 个网页，动画和音乐也能一次写完](https://www.laoshoucun.com/claudedt/3351) · [仓库内阅读](docs/3351-实测Opus5.5：一句提示词出100个网页，动画和音乐也能一次写完.md)
- 2026-09-18 · [Claude Code 项目功能重构：说一个目标，云端一群智能体分头写码并提合并请求](https://www.laoshoucun.com/claudedt/3221) · [仓库内阅读](docs/3221-ClaudeCode项目功能重构：说一个目标，云端一群智能体分头写码并提合并请求.md)
- 2026-09-18 · [Claude 统一入口上线：Cowork 并入聊天框，文档和幻灯片都能在里面做完](https://www.laoshoucun.com/claudedt/3219) · [仓库内阅读](docs/3219-Claude统一入口上线：Cowork并入聊天框，文档和幻灯片都能在里面做完.md)
- 2026-09-18 · [Claude Code 团队怎么用 Claude Code：八成日常活交给 AI，工程师只下一个目标](https://www.laoshoucun.com/claudedt/3213) · [仓库内阅读](docs/3213-ClaudeCode团队怎么用ClaudeCode：八成日常活交给AI，工程师只.md)
- 2026-09-04 · [Claude Code 更新 v2.1.260：新增 /diff 全屏对比面板，/cost 会提示缓存未命中原因](https://www.laoshoucun.com/claudedt/3025) · [仓库内阅读](docs/3025-ClaudeCode更新v2.1.260：新增diff全屏对比面板，cost会提.md)

---

**官方入口：[Claude安装](https://www.laoshoucun.com/anzhuang)**

© [老手村](https://www.laoshoucun.com/) · 本仓库为官网内容镜像，文章版权归原作者所有。
