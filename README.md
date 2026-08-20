# InkCraft 写作方法库

面向长篇网文的体裁写作方法与 Agent AI Skill 库。将长篇小说创作拆解为结构设计、前三章开篇、具体场景推进、成文四轴规范与自检清单。

内容不包含小说原文，也不包含写作软件本身。

---

## 目录结构

全库包含 **13 种主流体裁**，每个体裁目录下结构保持一致：

```
genres/
├── axes.md                  # 全体裁共用的四条成文轴（节奏、叙述距离、对白、比喻）
├── SKILL.md                 # 统一体裁调度器（write-genre）
└── <genre-id>/
    ├── SKILL.md             # Agent 技能配置（定义、执行步骤与硬约束）
    ├── 01-structure.md      # 结构：读者承诺、每场状态变化、开书先定、卡住自查
    ├── 02-opening.md        # 开篇：前三章承诺链与顺序变化
    ├── 03-methods.md        # 场景写法：6 大核心场景写法与教学示例
    ├── 04-prose.md          # 成文：粗区间与四轴落地规则
    └── 05-checklist.md      # 自检：完成后的核对清单与回退方案
```

---

## 支持体裁

| 分类 | 体裁 | Skill ID | 目录 |
| :--- | :--- | :--- | :--- |
| **幻想修真** | 玄幻 | `write-xuanhuan` | [`genres/xuanhuan/`](./genres/xuanhuan/01-structure.md) |
| | 仙侠 | `write-xianxia` | [`genres/xianxia/`](./genres/xianxia/01-structure.md) |
| | 洪荒 | `write-honghuang` | [`genres/honghuang/`](./genres/honghuang/01-structure.md) |
| | 都市超凡 | `write-urban-supernatural` | [`genres/urban-supernatural/`](./genres/urban-supernatural/01-structure.md) |
| **悬疑科幻** | 末世 | `write-apocalypse` | [`genres/apocalypse/`](./genres/apocalypse/01-structure.md) |
| | 无限流 | `write-infinite-flow` | [`genres/infinite-flow/`](./genres/infinite-flow/01-structure.md) |
| | 悬疑惊悚 | `write-mystery-horror` | [`genres/mystery-horror/`](./genres/mystery-horror/01-structure.md) |
| | 科幻 | `write-science-fiction` | [`genres/science-fiction/`](./genres/science-fiction/01-structure.md) |
| **权谋职场** | 历史权谋 | `write-historical-strategy` | [`genres/historical-strategy/`](./genres/historical-strategy/01-structure.md) |
| | 现实职场 | `write-realistic-career` | [`genres/realistic-career/`](./genres/realistic-career/01-structure.md) |
| **言情喜剧** | 都市言情 | `write-urban-romance` | [`genres/urban-romance/`](./genres/urban-romance/01-structure.md) |
| | 古言 | `write-ancient-romance` | [`genres/ancient-romance/`](./genres/ancient-romance/01-structure.md) |
| | 游戏轻喜剧 | `write-game-light-comedy` | [`genres/game-light-comedy/`](./genres/game-light-comedy/01-structure.md) |

---

## 使用方式

### 给 Agent 用

- **指定体裁**：将对应体裁目录下的 `SKILL.md` 放入 Agent 的 skills 目录（目录名同 `name`，如 `write-xuanhuan`），只拷 `SKILL.md` 即可工作。
- **自动分流**：使用 `genres/SKILL.md`（`write-genre`），根据任务描述自动路由到具体体裁。
- **场景生成**：Agent 在写具体某场戏时，按需打开对应体裁的 `03-methods.md` 查阅具体执行步骤。

### 自己读

从 [体裁目录](./genres/README.md) 打开对应体裁：
- 定整本书与细纲看 `01-structure.md`
- 写前三章看 `02-opening.md`
- 写具体单场戏看 `03-methods.md`
- 修句子看 `04-prose.md`
- 写完核对看 `05-checklist.md`

---

## 开源协议

- 写作方法与 Skill 正文采用 [CC BY 4.0](./LICENSE) 许可，署名 InkCraft 后可修改和商业使用。
- InkCraft 名称商标、Logo 视觉资产及 InkCraft 软件产品仍为闭源商业资产，不在许可范围内。
