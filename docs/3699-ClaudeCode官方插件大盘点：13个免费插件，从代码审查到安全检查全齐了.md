# Claude Code官方插件大盘点：13个免费插件，从代码审查到安全检查全齐了

> 原文链接：[https://www.laoshoucun.com/claudedt/3699](https://www.laoshoucun.com/claudedt/3699)

帮朋友配 Claude Code 环境，顺手翻了翻 anthropics/claude-code 这个仓库，翻出个多数人不知道的角落：CLI 本体之外，里面码着一个官方插件目录，13 个官方亲手维护的插件，零收费。朋友看了直呼白瞎，说裸用了俩月。这批插件还有个隐藏价值：它们本身就是插件系统的教科书示范，斜杠命令、专职 agent、钩子、MCP 服务器怎么咬合运转，翻一遍源码全明白。下面按值得装的程度过一遍。

第一梯队：审查和 Git 日常

code-review 值得单独说。一次审查派五个 Sonnet agent 并行：一个查 CLAUDE.md 合规，一个挖潜在 bug，一个补历史上下文，一个翻 PR 历史，一个读代码注释，各自的结果按置信度筛掉误报，最后汇成一份干净报告。小团队没人力看 PR 的，装它兜底。

commit-commands 管 Git 三件套的体力活，/commit 完成提交，/commit-push-pr 一步推送加建 PR，/clean_gone 清扫失效分支。pr-review-toolkit 思路跟 code-review 相反，不打综合分只走专项：评论质量、测试覆盖、静默失败、类型设计、代码简化六个专项 agent 各管一摊，哪块薄弱跑哪块。

趣味度最高的两个

ralph-wiggum，名字来自《辛普森一家》，本质是台自循环执行器。敲 /ralph-loop，Claude 对同一任务无限迭代直到彻底完成，中途想溜，Stop 钩子把它拦下来逼着继续。挂机跑长任务的邪道玩法，官方亲自示范。security-guidance 像个不知疲倦的安全哨兵，PreToolUse 钩子实时盯九类危险模式：命令注入、XSS、eval 滥用、危险 HTML、pickle 反序列化、os.system 调用都在名单上，编辑文件一旦触碰立即告警。想让 AI 写代码又怕它写出漏洞的，闭眼装。

剩下八个，一人一句

frontend-design 治"一眼 AI 审美"，检测到前端任务自动启用；feature-dev 是七阶段结构化开发流，探索、架构、审查三个 agent 随行；hookify 最省心，对话里说句"别再干 XX 了"钩子自动生成；plugin-dev 给你八阶段向导手把手造插件；agent-sdk-dev 帮 Agent SDK 项目搭脚手架；explanatory-output-style 往会话开头注入实现原理讲解；learning-output-style 走教学模式，关键决策点要求你亲手写 5 到 10 行代码；claude-opus-4-5-migration 管搬家，把代码从 Sonnet 4.x / Opus 4.1 平滑迁到 Opus 4.5。

安装两条路：Claude Code 里用 /plugin 命令装，或写进项目的 .claude/settings.json。另外每个插件的标准目录结构（.claude-plugin/plugin.json 加 commands/、agents/、skills/、hooks/ 四件套）就是现成的插件开发参考模板。想看系统性拆解，站内插件栏目持续更新中。

Claude Code会员中转站 微信:douhanq

---

原文链接：[https://www.laoshoucun.com/claudedt/3699](https://www.laoshoucun.com/claudedt/3699)
