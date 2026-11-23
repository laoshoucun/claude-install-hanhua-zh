# Claude自定义技能怎么做？一个SKILL.md文件就够了，官方模板直接抄

> 原文链接：[https://www.laoshoucun.com/claudedt/3700](https://www.laoshoucun.com/claudedt/3700)

同事每周给 Claude 交代一遍周报格式，交代到第三周开始烦了。我告诉他这活十分钟就能一劳永逸：写个自定义技能。剥开营销话术，Claude 的技能（Skills）系统本体朴素得吓人，一个文件夹，里面一份 SKILL.md，按需配几个脚本和资源文件，就这些。加载之后 Claude 就掌握了按你的规矩处理某类任务的能力，照公司品牌规范产文档、按团队流程跑数据分析，写一次，永久复用。这篇从零开始手把手拆解，素材全部取自 Anthropic 官方 skills 仓库的说明文档，结构照抄就行。

SKILL.md 的最小可用结构

跑起来只需要 frontmatter 两个字段加正文指令：

---
name: my-skill-name
description: 说清这个技能干什么、什么时候该用它
---

# 技能名称
[这里写 Claude 要遵循的指令]
## 示例
- 用法示例1
## 约束
- 规则1

几个坑别踩。name 必须全小写、连字符分词，且不得含"claude""anthropic"等保留词，官方仓库前阵子刚因此给自家 academy-guide 技能改了名，前车之鉴。description 的写法讲究"做什么+何时用"二合一：Claude 就是靠这段文字判断何时自动启用技能，写得含糊，技能就沦为一辈子不触发的摆设。正文承载完整指令，步骤、示例、边界情况的处理方式，颗粒度越细，触发后的表现越稳。

起步姿势：拿模板当骨架

别对着空白文档硬写。官方仓库 template 目录里备好了技能模板，fork 过来改，效率远高于从零起步。写完自己的想对标成熟案例？仓库里几十个官方示例敞开供应，创意设计到企业工作流都有，它们就是"指令该怎么组织"的现成教材。

安装路径：三端各走各的门

Claude Code 用户最方便，一条命令挂上官方市场：/plugin marketplace add anthropics/skills，随后用 /plugin 装技能包。自研技能更简单，丢进项目的 .claude 目录就自动被识别。Claude.ai 网页版的付费用户支持直接上传自定义技能；API 调用方走 Skills 接口。

顺带一个值得知道的信息：Agent Skills 已有独立开放标准（agentskills.io），Claude 的实现只是其中之一。这意味着你写的技能文件结构有机会在其他 agent 工具里直接通用，这份数字资产的保值性比想象中好。

最后一条实操建议：第一个技能切忌贪大。选一件每周都要重复交代的琐事，典型如"按我们的格式写周报"，控制在五十行以内写完，投用一周，再根据 Claude 的实际表现迭代三个版本。走完这个循环，整套玩法你就吃透了。想直接用现成技能的，站内插件栏目有持续整理。

Claude Code会员中转站 微信:douhanq

---

原文链接：[https://www.laoshoucun.com/claudedt/3700](https://www.laoshoucun.com/claudedt/3700)
