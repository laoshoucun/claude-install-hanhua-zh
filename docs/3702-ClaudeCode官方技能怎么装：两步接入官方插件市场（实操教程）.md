# Claude Code官方技能怎么装：两步接入官方插件市场（实操教程）

> 原文链接：[https://www.laoshoucun.com/claudedt/3702](https://www.laoshoucun.com/claudedt/3702)

想给Claude Code加官方技能，最快的路是官方技能仓库anthropics/skills。它把文档处理、编程辅助这些技能打包成插件，两步就能装好。这篇是实操向的安装教程。

第一步：把官方仓库注册成插件市场

在Claude Code里执行一行命令：/plugin marketplace add anthropics/skills。这会把Anthropic官方技能仓库注册成你的插件市场（marketplace）。之后Claude Code就知道从哪里拉取技能了。

第二步：装你要的技能包

官方仓库里有两个可直接安装的插件：document-skills（文档技能：Word/PPT/Excel/PDF等文档创建与编辑能力）和example-skills（示例技能合集，涵盖创意、设计、开发、企业沟通等方向的演示技能）。安装命令二选一：

/plugin install document-skills@anthropic-agent-skills

/plugin install example-skills@anthropic-agent-skills

也可以走菜单：/plugin marketplace add后选择"Browse and install plugins"，先选anthropic-agent-skills，再挑document-skills或example-skills，点Install now。

装完怎么用

装好后不用任何额外操作——直接在对话里提需求就行。比如装了document-skills，你可以说"用PDF技能提取这个文件的表单字段"，Claude Code会自动调用对应的技能来处理。技能的本质是一组指令加脚本：Claude需要时动态加载，专门干某一类活。

几个注意点

第一，example-skills里的技能偏演示和教育用途，官方明确说线上行为和示例可能有差异，重要场景先自己测一遍；第二，文档技能（docx/pdf/pptx/xlsx）是source-available（源码可用但非完全开源），拿它做参考学习可以，商用要看清条款；第三，想找灵感可以浏览仓库的skills目录，里面有从艺术、音乐到测试、MCP生成的几十个示例，照着SKILL.md的结构就能理解技能是怎么写出来的。

对还不熟技能概念的用户，简单理解：技能就是给Claude的一本"工种手册"，装好之后它遇到对应任务就知道按手册干活。官方技能仓库是目前质量最有保障的技能来源，建议第一个装。

Claude Code会员中转站 微信:douhanq

---

原文链接：[https://www.laoshoucun.com/claudedt/3702](https://www.laoshoucun.com/claudedt/3702)
