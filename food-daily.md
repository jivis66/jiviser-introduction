# 美食Daily 推荐清单

> **用途**: 本文件用于配置AI助手每日推荐一道精选美食食谱
> **推送时间**: 每日 13:00
> **推送渠道**: Telegram
> **输出语言**: 中文（非中文内容需翻译）
> **推荐数量**: 每日1道精选菜肴

---

## 元数据配置

```yaml
schedule: "13:00"  # 每天推送时间
timezone: "local"
output_format: "single-recipe"
recipe_selection:
  strategy: "seasonal-rotation"  # 时令轮换
  daily_limit: 1
  content_structure:
    - 菜品名称（中文翻译）
    - 特色简介（3-5句话）
    - 核心制作步骤（简化版，5-8步）
    - 时令搭配说明
    - 来源链接
translation:
  enabled: true
  target_language: "zh-CN"
  source_languages: ["en", "ja", "ko"]
seasonal_rules:
  spring: ["春笋", "韭菜", "荠菜", "豌豆", "草莓"]
  summer: ["黄瓜", "番茄", "茄子", "西瓜", "荔枝", "凉拌菜"]
  autumn: ["南瓜", "板栗", "螃蟹", "柿子", "莲藕", "百合"]
  winter: ["白萝卜", "羊肉", "火锅", "炖菜", "柑橘"]
preferences:
  exclude: ["过于复杂", "特殊器具", "难买食材"]
  prioritize: ["时令食材", "快手菜", "家庭友好", "有特色"]
delivery:
  channel: "telegram"
  format: "markdown"
  include_image: true  # 如果有图片链接
```

---

## 信息源列表

### 🍳 国际知名美食网站（英文）

<!-- category: international-western -->
<!-- priority: high -->
<!-- content_types: [recipes, techniques, baking] -->

| 网站名称 | RSS订阅地址 | 特色内容 | 适合场景 |
|---------|------------|---------|---------|
| Serious Eats | feeds.feedburner.com/seriouseats | 硬核美食科学、权威食谱、烹饪技术解析 | 想深入理解烹饪原理 |
| The Kitchn | thekitchn.com/main.rss | 每日家居烹饪杂志，厨房设计、烹饪课程 | 日常烹饪灵感 |
| Cookie and Kate | feeds.feedburner.com/CookieAndKate | 健康全食、素食食谱，强调时令食材 | 健康饮食、素食者 |
| Gimme Some Oven | gimmesomeoven.com/feed | 1500+ 快手食谱，适合忙碌家庭 | 快速备餐 |
| Damn Delicious | damndelicious.net/feed | 快手简易餐，适合日常家庭烹饪 | 新手友好 |
| Once Upon A Chef | onceuponachef.com/feed | 专业厨师出品，步骤详尽，中高端烹饪 | 周末精心烹饪 |
| Sally's Baking Addiction | feeds.feedburner.com/SallysBakingAddiction | 烘焙专长，甜点、面包食谱 | 烘焙爱好者 |
| Minimalist Baker | minimalistbaker.com/feed | 简单素食，10种食材以内、30分钟完成 | 极简烹饪 |
| Pinch of Yum | pinchofyum.com/feed | 轻松有趣的美食摄影与食谱 | 视觉享受 |
| Budget Bytes | budgetbytes.com/feed | 预算友好型食谱，适合精打细算 | 经济实惠 |

---

### 🥢 专注中餐与亚洲料理（英文）

<!-- category: asian-chinese -->
<!-- priority: high -->
<!-- content_types: [authentic-recipes, cultural-background, step-by-step] -->

| 网站名称 | RSS订阅地址 | 特色 | 适合场景 |
|---------|------------|------|---------|
| The Woks of Life | thewoksoflife.com/feed | 一家四口经营，英文世界最权威中餐博客，川粤家常菜 | 地道中餐 |
| China Sichuan Food | chinasichuanfood.com/feed | 正宗川菜食谱，详细步骤图解 | 川菜爱好者 |
| Omnivore's Cookbook | omnivorescookbook.com/feed | 北京移民博主，现代中餐做法，简化传统工序 | 简化中餐 |
| Red House Spice | redhousespice.com/feed | 中英双语博主，正宗中餐与亚洲风味 | 双语对照 |
| Just One Cookbook | justonecookbook.com/feed | 日本家庭料理，1000+ 正宗日式食谱 | 日料爱好者 |
| Lady and Pups | ladyandpups.com/feed | 创意中餐与亚洲融合菜，风格独特 | 创意料理 |
| Madame Huang's Kitchen | feeds.feedburner.com/blogspot/madamehuang | 深入介绍中国饮食文化与历史背景 | 文化探索 |

---

### 🇨🇳 国内中文美食源（通过RSSHub）

<!-- category: domestic-chinese -->
<!-- priority: medium -->
<!-- content_types: [user-generated, trending, authentic-local] -->

| 来源 | RSSHub地址 | 说明 | 适合场景 |
|-----|-----------|------|---------|
| 下厨房-热门作品 | https://rsshub.app/xiachufang/popular | 下厨房用户热门作品动态 | 流行趋势 |
| 下厨房-用户作品 | https://rsshub.app/xiachufang/user/{用户ID} | 订阅特定博主的最新作品 | 关注特定博主 |
| 下厨房-用户菜谱 | https://rsshub.app/xiachufang/user/{用户ID}/catalog | 订阅特定博主的菜谱合集 | 系统学习 |
| 豆果美食-热门 | https://rsshub.app/douguo/popular | 豆果热门食谱 | 大众口味 |
| 美食杰-最新 | https://rsshub.app/meishijie/latest | 美食杰最新食谱 | 家常菜 |

**推荐订阅的下厨房博主ID示例**:
- 下厨房官方: `101527771`
- 可根据喜好搜索并替换 `{用户ID}`

---

## 时令食材对照表

<!-- category: seasonal-reference -->
<!-- priority: reference -->

| 季节 | 时令蔬菜 | 时令水果 | 时令肉类/海鲜 | 推荐菜系 |
|-----|---------|---------|--------------|---------|
| 春季 (3-5月) | 春笋、韭菜、荠菜、豌豆苗、香椿、菠菜 | 草莓、樱桃、枇杷、桑葚 | 鲈鱼、鲥鱼、螺蛳 | 清淡、鲜嫩 |
| 夏季 (6-8月) | 黄瓜、番茄、茄子、苦瓜、丝瓜、空心菜 | 西瓜、荔枝、龙眼、桃子、李子 | 小龙虾、花蛤、扇贝 | 凉拌、清蒸 |
| 秋季 (9-11月) | 南瓜、板栗、莲藕、山药、芋头、百合 | 柿子、梨、苹果、石榴、柚子 | 大闸蟹、鲈鱼、羊肉 | 炖汤、红烧 |
| 冬季 (12-2月) | 白萝卜、白菜、芥菜、冬笋、胡萝卜 | 柑橘、橙子、柚子、冬枣 | 羊肉、牛肉、腊肉 | 火锅、炖煮 |

---

## 输出格式规范

### 每日推荐模板

```markdown
🍽️ **今日推荐** | [菜品名称]

📍 **来源**: [网站名称] ([来源链接])

🌟 **特色简介**:
[3-5句话介绍这道菜的特点、风味、适合场合]
[突出使用的时令食材和健康亮点]

⏱️ **制作时间**: [准备时间] + [烹饪时间]
👥 **份量**: [几人份]
💰 **预算**: [成本估算]

📝 **核心制作步骤**:

1. **[步骤标题]**
   [具体操作内容]

2. **[步骤标题]**
   [具体操作内容]

...(5-8个核心步骤)

🥬 **时令说明**:
[解释为什么这道菜适合当前季节，使用的时令食材有哪些]

💡 **小贴士**:
[1-2个关键技巧或替代建议]

---
*明天13:00见！*
```

---

## 轮换策略

<!-- category: rotation-strategy -->

### 每周主题安排

| 星期 | 主题 | 偏好来源 | 菜系重点 |
|-----|------|---------|---------|
| 周一 | 快手工作日晚餐 | Damn Delicious, Gimme Some Oven | 简单快捷 |
| 周二 | 亚洲风味 | The Woks of Life, Just One Cookbook | 中日料理 |
| 周三 | 健康轻食 | Cookie and Kate, Minimalist Baker | 低脂健康 |
| 周四 | 中式家常菜 | 下厨房热门, China Sichuan Food | 地道中餐 |
| 周五 | 周末预备餐 | Once Upon A Chef, Serious Eats | 适合周末尝试 |
| 周六 | 烘焙甜点 | Sally's Baking Addiction, Pinch of Yum | 甜品烘焙 |
| 周日 | 大餐/聚会菜 | Budget Bytes, The Kitchn | 适合多人分享 |

### 内容过滤规则

- ❌ **排除**:
  - 需要特殊器具（如sous vide、专业烤箱）
  - 食材难以购买（需在一线城市进口超市才有）
  - 制作时间超过2小时（周末主题除外）

- ✅ **优先**:
  - 使用当前时令食材
  - 制作步骤清晰的食谱
  - 家庭常见食材为主
  - 有详细图片或视频辅助

- 🔄 **翻译要求**:
  - 菜名使用中文（英文原名可选附注）
  - 食材使用中文常用名称
  - 度量单位转换为中文常用单位（克、毫升、勺等）

---

## 用户偏好学习

> **注意**: 以下部分由AI助手根据用户反馈动态更新

```yaml
user_preferences:
  liked_cuisines: []      # 记录用户喜欢的菜系
  disliked_ingredients: [] # 记录用户不喜欢的食材
  dietary_restrictions: [] # 饮食限制（素食、清真、过敏等）
  cooking_skill: ""        # 烹饪水平偏好
  preferred_difficulty: "" # 难度偏好
  saved_recipes: []        # 用户收藏的食谱
  feedback_history: []     # 历史反馈记录
```

**每日确认问题模板**:
> 这道菜符合您的口味吗？您希望明天看到什么类型的菜肴？（川菜/日料/快手菜/其他）

---

## RSS阅读器推荐

| 工具 | 平台 | 特点 | 适用人群 |
|-----|------|------|---------|
| Feedly | Web/iOS/Android | 界面美观，支持分类管理，免费版100个源 | 普通用户 |
| Inoreader | Web/iOS/Android | 功能全面，支持全文抓取与规则过滤 | 高级用户 |
| Reeder | iOS/macOS | 苹果生态最佳体验，iCloud同步 | 苹果用户 |
| NetNewsWire | iOS/macOS | 开源免费，原生应用，极速流畅 | 苹果用户 |
| FreshRSS | 自托管 | 适合技术用户自建服务器 | 技术用户 |

---

## 外部资源补充

**视频平台**（可配合食谱观看）:
- YouTube: The Woks of Life, Just One Cookbook 等均有视频频道
- Bilibili: 搜索对应中文菜名通常有视频教程

**小红书/B站**（通过RSSHub订阅）:
- 小红书用户: `https://rsshub.app/xiaohongshu/user/{用户ID}`
- B站UP主: `https://rsshub.app/bilibili/user/video/{UID}`

---

*最后更新: 2026-02-28*
*版本: 1.0*
