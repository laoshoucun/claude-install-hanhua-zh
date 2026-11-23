# Anthropic官方技能库全解：Word、PPT、Excel、PDF文档技能免费用

> 原文链接：[https://www.laoshoucun.com/claudedt/3701](https://www.laoshoucun.com/claudedt/3701)

上周让 Claude 改一份 Word 的格式，改得又快又对。好奇背后谁在干活，翻了 Anthropic 的官方 skills 仓库，答案敞在那：支撑文档能力的四个技能，docx、pdf、pptx、xlsx，源码全部公开，四个文件夹随便读。授权严格说是 source-available 不是完全开源，但作为一套在生产环境真实跑着的实现，参考价值甩市面上多数教程几条街。你在 Claude.ai 里说"帮我做份 PPT""把这份 Word 改一下"，真正动手的就是这四位。

仓库三块，各管各的

布局清爽。skills 目录是核心，按用途分四类：创意与设计方向收绘画、音乐等技能；开发与技术方向有 Web 应用测试、MCP 服务器生成等；企业与沟通方向放品牌规范、沟通模板；文档四件套压轴。spec 目录存 Agent Skills 规范，template 目录放技能模板，想自己写技能的从 template 起步最顺。

四件套，两类人各有看头

这四个技能是 Claude 文档能力的发动机：新建文档、调整格式、抽取内容、处理表单字段，点"创建文件"时忙活的就是它们。普通用户的意义直接：付费版 Claude.ai 里这些能力全部就位，开箱即用。开发者看的是另一层，官方怎么把"操作 Office 文档"这种复杂任务一步步拆成技能指令，这套拆解思路是做企业自动化技能时最好的照抄对象。

接进 Claude Code：两步

先注册官方市场：/plugin marketplace add anthropics/skills；再一条命令装包：

/plugin install document-skills@anthropic-agent-skills（文档四件套）

/plugin install example-skills@anthropic-agent-skills（示例技能集）

装完即用，自然语言触发，比如"用 PDF 技能把这份文件的表单字段提出来"。桌面端用户不用碰命令行，设置界面的插件市场里搜着装。API 用户走另一扇门，Skills 接口支持上传自定义技能、调用官方预置技能，做产品集成的选这条。

一个务实提醒别省：官方在仓库里白纸黑字写了，这批技能定位演示和教学，实际行为可能与 Claude 产品内的表现有差异，进关键业务流程前先在自己环境完整测一轮。生态里还有 Notion 等合作伙伴的官方技能在路上，站内插件栏目后续持续跟进。

Claude Code会员中转站 微信:douhanq

---

原文链接：[https://www.laoshoucun.com/claudedt/3701](https://www.laoshoucun.com/claudedt/3701)
