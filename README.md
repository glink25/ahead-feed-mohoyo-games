# ahead-feed-mohoyo-games

面向 Ahead / Open Event Feed 的米哈游游戏事件源集合。每款游戏使用独立 manifest，玩家可以只订阅自己关心的游戏。

## Feeds

| 游戏 | Manifest | 内容 |
| --- | --- | --- |
| 原神 | `feeds/genshin-impact.yaml` | 版本更新、版本前瞻、深境螺旋与幻想真境剧诗刷新 |
| 崩坏：星穹铁道 | `feeds/honkai-star-rail.yaml` | 版本更新、版本前瞻、混沌回忆/虚构叙事/末日幻影轮换 |
| 绝区零 | `feeds/zenless-zone-zero.yaml` | 版本更新、版本前瞻、危局强袭战等高难轮换 |
| 源初之结 | `feeds/nodusfall.yaml` | 官宣、展会展示、测试与上线进度 |

## 维护原则

- 重点记录玩家真正需要提前知道的“大事件”，不收录日常签到、普通卡池和零碎网页活动。
- 历史事件默认覆盖最近一年，并保留重要产品节点。
- 日期优先采用 HoYoLAB、游戏官网、官方直播等一手来源。
- 尚未公布确切日期的测试或版本使用 `unknown`，不按惯常周期伪造日期。
- `confidence` 使用 `confirmed` / `likely` / `rumored` 表达信息强度。
- 中国大陆玩家常用时间统一按 UTC+8 表述；仅有日期而无必要时刻时使用 `exact`。

数据人工梳理，发现官方改期或遗漏欢迎提交 Issue。