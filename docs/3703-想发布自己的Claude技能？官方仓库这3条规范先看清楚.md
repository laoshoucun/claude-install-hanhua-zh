# 想发布自己的Claude技能？官方仓库这3条规范先看清楚

> 原文链接：[https://www.laoshoucun.com/claudedt/3703](https://www.laoshoucun.com/claudedt/3703)

Anthropic官方技能仓库anthropics/skills最近动作不少：前端设计技能更新、部分技能改名、技能规范文档持续完善。如果你打算把自己写的技能分享出去，或准备把技能打包成可上传的自定义技能，官方仓库这几条规则先看清楚。

<img src=&quot;https://cdn.laoshoucun.com/web/claude/2026/09/20260904191121_058649.png&quot; alt=&quot;Claude技能规范" style="max-width:100%;height:auto;border-radius:8px;margin:16px 0;" />

技能名有"保留字"限制

官方仓库近期把一个叫claude-academy-guide的技能改名为academy-guide，原因写得很直白：技能名不能包含"claude"或"anthropic"这类保留词。这是为了技能可作为自定义技能上传而做的合规调整——你自己的技能命名时也注意避开品牌保留词，否则打包上传时会过不了校验。

描述有1024字符上限

同一个commit里，官方还把该技能的description从1176字符压缩到992字符——因为技能上传校验对SKILL.md frontmatter里的description有1024字符上限。这提醒我们：技能描述要精炼。写技能时description是"什么时候该调用这个技能"的判据，AI靠它决定要不要加载，太长反而稀释匹配度，一般一两句话说清用途和触发场景最好。

跟着规范走：agentskills.io

仓库README明确指向了agentskills.io——Agent Skills开放标准站点。技能不是Anthropic一家的私货，而是有公开规范的：一个技能=一个文件夹+SKILL.md（YAML frontmatter写明name和description，正文写操作指引）。官方仓库的template目录就是标准模板，照着它新建技能不会错。

结构参考：官方仓库怎么组织

想借鉴官方做法的，仓库结构值得看：skills目录放示例技能（按Creative & Design、Development & Technical、Enterprise & Communication、Document Skills分类），spec目录放Agent Skills规范，template目录放模板，.claude-plugin目录支撑Claude Code插件市场。其中docx、pdf、pptx、xlsx四个文档技能是Claude文档能力的底层实现，源码可用但非完全开源——做深度参考价值很大，商用要留意授权。

一句话：技能想发布出去，命名避开保留词、描述压到1024字符内、按agentskills.io规范组织，这三件事做到位就基本能过审。剩下的，就是你的技能本身有没有真本事了。

Claude Code会员中转站 微信:douhanq

---

原文链接：[https://www.laoshoucun.com/claudedt/3703](https://www.laoshoucun.com/claudedt/3703)
