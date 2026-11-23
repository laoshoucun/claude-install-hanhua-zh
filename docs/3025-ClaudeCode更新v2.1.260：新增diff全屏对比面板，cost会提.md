# Claude Code 更新 v2.1.260：新增 /diff 全屏对比面板，/cost 会提示缓存未命中原因

> 原文链接：[https://www.laoshoucun.com/claudedt/3025](https://www.laoshoucun.com/claudedt/3025)

Claude Code 9月3日更新到了 v2.1.260。这一版没有新模型发布，但几处改动都是天天用的人会碰到的问题。

最直观的是看代码改动的方式。以前改动的 diff 要么切到别的窗口，要么挤在终端里一条条翻。现在对话旁边多了一个全屏 diff 面板，敲 /diff 就能切换。改动量大的时候，或者多人 review 的时候，全屏看比挤在终端里舒服，也更容易发现不该动的地方。

花钱的问题也有人管了。/cost 命令和状态行现在会显示缓存没命中的可能原因。跑长任务的人都知道，缓存命中率直接决定花费，同样的活费用忽高忽低，多半是缓存悄悄没命中。现在工具直接提示原因，可以对着调整会话习惯，把缓存用起来，不用再对着账单猜。

自动化场景同样有更新。headless 会话支持了 /reload-plugins 和基于文本的 /advisor，跑无人值守任务、把 Claude Code 接进 CI 和脚本的团队，加载新插件不用再重启整个会话。

另外这版还修了一批零碎问题，涉及权限规则、Bash 沙箱、Bedrock 和 AWS SSO 登录、模型切换、后台会话、界面显示，以及 VSCode 集成。整体看节奏没变，Claude Code 基本保持每周一更。

想省时间的可以先试 /diff 全屏面板，想省钱的跑一遍 /cost 看缓存提示。两个功能都在这一版里，更新后就能用。

---

原文链接：[https://www.laoshoucun.com/claudedt/3025](https://www.laoshoucun.com/claudedt/3025)
