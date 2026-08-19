---
name: write-genre
id: write-genre
description: 按项目或用户指定的体裁，选择对应的 write-<id> Skill。当用户要求按某个体裁写、或项目体裁尚未对应到具体 Skill 时使用。
version: "1"
---

# 体裁写作调度

## 触发条件

用户要求按某个体裁写、改或审长篇，但尚未加载具体 `write-<id>`。

## 执行步骤

1. 从用户说明和项目设定中识别体裁。对照下表 aliases。
2. 命中则加载对应 Skill，并按其执行步骤工作。本 Skill 不重复展开写法。
3. 无法判断时，先问作者是哪一类，给出下表中文名供选择。不要猜。

| 触发词 | Skill |
|---|---|
| 玄幻、东方玄幻、异界、高武 | write-xuanhuan |
| 仙侠、修真、修仙、宗门 | write-xianxia |
| 洪荒、封神、神话流 | write-honghuang |
| 都市超凡、都市异能、都市高武 | write-urban-supernatural |
| 末世、灾变、废土、生存 | write-apocalypse |
| 无限流、诸天流、副本、轮回 | write-infinite-flow |
| 历史权谋、架空历史、争霸 | write-historical-strategy |
| 悬疑、惊悚、灵异、克苏鲁 | write-mystery-horror |
| 科幻、赛博、星际、太空 | write-science-fiction |
| 游戏、轻小说、沙雕、搞笑 | write-game-light-comedy |
| 都市言情、言情、都市爱情 | write-urban-romance |
| 古言、宅斗、穿书、宫斗 | write-ancient-romance |
| 现实、职业文、职场、年代文 | write-realistic-career |

## 成功标准

- 已选中且只执行一个 `write-<id>`
- 体裁不明时已经向作者提问，而不是擅自开写

## 硬约束

- 不要同时套用多个体裁的成文区间
- 不要把本表写成某部作品的分类
