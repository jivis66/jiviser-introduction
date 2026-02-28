# jiviser-introduction

个人日常咨询指南仓库，用于配置 AI 助手每日推送精选内容。

## 目录

| 指南 | 内容 | 推送时间 | 文件 |
|-----|------|---------|------|
| Reddit Daily | AI 相关 Subreddit 监控 | 17:00 | [docs/reddit-dailly.md](docs/reddit-dailly.md) |
| Food Daily | 美食食谱推荐（时令结合） | 13:00 | [docs/food-daily.md](docs/food-daily.md) |
| Fitness Daily | 运动健康咨询（跑步/公路车） | 07:00 / 20:00 | [docs/fitness-daily.md](docs/fitness-daily.md) |
| AI Apps Daily | AI 工具与应用资讯 | 08:00 / 21:00 | [docs/ai-apps-daily.md](docs/ai-apps-daily.md) |
| Blogs Daily | 博客文章精选（技术/设计/人文） | 08:30 / 22:00 | [docs/blogs-daily.md](docs/blogs-daily.md) |

## 结构

```
docs/
├── reddit-dailly.md    # Reddit AI 社区监控
├── food-daily.md       # 美食推荐
├── fitness-daily.md    # 运动健康
├── ai-apps-daily.md    # AI 应用资讯
└── blogs-daily.md      # 博客文章精选
```

## 格式

所有指南采用统一结构：
- YAML 元数据配置（时间、轮换策略、偏好设置）
- 分类信息源表格（国际 + 中文来源）
- 每周轮换计划
- 输出模板（推送格式）
- 用户偏好配置

## 推送渠道

- Telegram

---

*使用 Claude Code 维护*
