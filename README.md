# InkCraft 写作方法库

这是一套长篇网文的体裁写作方法：结构、开篇、场景写法和成文节奏。
它不是 InkCraft 软件，也不包含小说原文。

内容采用 [CC BY 4.0](./LICENSE)。署名 InkCraft 后可以修改和商业使用。
InkCraft 名称、Logo 和视觉资产不在许可范围内。桌面端与 Agent 仍是闭源商业产品。

## 体裁速查

从手册页进入，不要只扫 Skill 名。体裁不明时，先用调度 Skill `write-genre`（[`genres/SKILL.md`](./genres/SKILL.md)）。

| 体裁 | Skill | 适用 | 手册 |
|---|---|---|---|
| 玄幻 | `write-xuanhuan` | 玄幻、东方玄幻、异界、高武 | [结构](./genres/xuanhuan/01-structure.md) |
| 仙侠 | `write-xianxia` | 仙侠、修真、修仙、宗门 | [结构](./genres/xianxia/01-structure.md) |
| 洪荒 | `write-honghuang` | 洪荒、封神、神话流 | [结构](./genres/honghuang/01-structure.md) |
| 都市超凡 | `write-urban-supernatural` | 都市超凡、都市异能、都市高武 | [结构](./genres/urban-supernatural/01-structure.md) |
| 末世 | `write-apocalypse` | 末世、灾变、废土、生存 | [结构](./genres/apocalypse/01-structure.md) |
| 无限流 | `write-infinite-flow` | 无限流、诸天流、副本、轮回 | [结构](./genres/infinite-flow/01-structure.md) |
| 历史权谋 | `write-historical-strategy` | 历史权谋、架空历史、争霸 | [结构](./genres/historical-strategy/01-structure.md) |
| 悬疑惊悚 | `write-mystery-horror` | 悬疑、惊悚、灵异、克苏鲁 | [结构](./genres/mystery-horror/01-structure.md) |
| 科幻 | `write-science-fiction` | 科幻、赛博、星际、太空 | [结构](./genres/science-fiction/01-structure.md) |
| 游戏轻喜剧 | `write-game-light-comedy` | 游戏、轻小说、沙雕、搞笑 | [结构](./genres/game-light-comedy/01-structure.md) |
| 都市言情 | `write-urban-romance` | 都市言情、言情、都市爱情 | [结构](./genres/urban-romance/01-structure.md) |
| 古言 | `write-ancient-romance` | 古言、宅斗、穿书、宫斗 | [结构](./genres/ancient-romance/01-structure.md) |
| 现实职场 | `write-realistic-career` | 现实、职业文、职场、年代文 | [结构](./genres/realistic-career/01-structure.md) |

完整分组见 [`genres/README.md`](./genres/README.md)。每个体裁目录里：`01` 结构，`02` 开篇，`03` 场景写法，`04` 成文，`05` 自检。

## 给 Agent 用

通用规则：拷贝该体裁的 `SKILL.md`，放到 Agent 的 skill 目录里，**子目录名必须等于** frontmatter 里的 `name`（例如 `write-xuanhuan`）。只拷 `SKILL.md` 即可工作；同目录 `01`–`05` 是展开，不是前提。

下面只说明目录放哪。不要把这些产品当成这套方法的说明书。

### Claude Code

放到项目或用户的技能目录（常见为 `.claude/skills`），再建与 `name` 同名的子目录，放入 `SKILL.md`。需要手册时，把 `01`–`05` 放在同一子目录。

### Cursor / Windsurf / Antigravity

放到该产品的技能或规则目录，同样用与 `name` 同名的子目录承载 `SKILL.md`。

- Cursor：常见为项目下的技能目录
- Windsurf：常见为规则或技能目录
- Antigravity：常见为 `.gemini/skills`

### Dify / LangChain / 自建 Agent

把对应体裁的 `01`–`05` 当作知识文档导入；或把 `SKILL.md` 里的触发条件、执行步骤、成功标准、硬约束拼进系统提示。这是写作方法，不是自动写书接口。

InkCraft 桌面端：在 `.inkcraft/skills` 下建立与 `name` 同名的子目录。

## 套用前后

同一场「展示能力」的虚构片段。左边是常见空转，右边按玄幻「力量体系边界设计」写：先看见反馈，再看见为什么不能一直用。

**未约束**

> 他眼中闪过精光，体内力量如潮水般涌动。一拳轰出，天地变色，那股毁天灭地的威压让所有人震撼不已。他知道，自己已经今非昔比。

**套用后**

> 她咬破指尖催动骨纹，掌心渗出白霜爬上黑铁锁梁，精铁脆裂成渣。再次催动时，小臂经脉如针扎，骨纹暗淡半寸，指节握不拢——今日不能动第三次。

差别：有触发、有可见后果、有边界。读者能回答「什么时候有用」和「为什么不能一直用」。其他体裁同样先看 `03-methods.md` 里「纸上必须看见」那一行。

## 不保证

- 不是某部网文的仿写指南
- 成文区间是软参考，不是合格线
- 不提供自动写作软件
