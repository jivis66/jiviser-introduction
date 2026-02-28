# 博客Daily 收集指南

> **用途**: 本文件用于配置AI助手收集和推荐优质博客文章，涵盖技术、设计、产品、人文等领域
> **推送时间**: 每日 08:30 (晨间阅读) 或 22:00 (晚间深度阅读)
> **推送渠道**: Telegram
> **输出语言**: 中文（外文内容提供摘要翻译）
> **内容形式**: 每日3-5篇精选文章 + 1篇深度推荐 + 金句摘录

---

## 元数据配置

```yaml
schedule:
  - "08:30"  # 晨间阅读：技术资讯、行业动态
  - "22:00"  # 晚间阅读：深度长文、人文思考
timezone: "local"
output_format: "blog-curation"
content_mix:
  morning:
    - 技术头条（1-2条）
    - 产品/设计新思维（1-2条）
    - 工具推荐（1个）
  evening:
    - 深度长文（1篇，技术或人文）
    - 独立博客精选（1篇）
    - 金句摘录（3-5条）
rotation:
  monday: "技术架构与工程"
  tuesday: "产品思维与设计"
  wednesday: "独立博客与人文"
  thursday: "创业与商业观察"
  friday: "工具与效率"
  saturday: "本周博客精华回顾"
  sunday: "下周值得关注"
preferences:
  exclude: ["低质量转载", "过度SEO内容", "付费墙强限制"]
  prioritize: ["原创深度", "实战经验", "独立思考", "长期更新"]
focus_areas:
  - tech_engineering    # 技术工程
  - product_design      # 产品设计
  - indie_hacker        # 独立开发者
  - business_startup    # 创业商业
  - humanities_thought  # 人文思考
delivery:
  channel: "telegram"
  format: "markdown"
  include_excerpt: true  # 文章摘录
```

---

## 信息源列表

### 💻 技术工程博客

<!-- category: tech-engineering -->
<!-- priority: high -->
<!-- content_types: [architecture, tutorials, best-practices, case-studies] -->

| 博客名称 | 作者/机构 | 网址/RSS | 特色内容 | 语言 |
|---------|----------|---------|---------|------|
| High Scalability | 社区 | highscalability.com | 大型系统架构案例 | 英文 |
| Martin Fowler | Martin Fowler | martinfowler.com | 软件架构、重构、敏捷 | 英文 |
| Joel on Software | Joel Spolsky | joelonsoftware.com | 软件商业、管理思考 | 英文 |
| Paul Graham | Paul Graham | paulgraham.com/articles.html | 创业、编程、思考 | 英文 |
| Dan Luu | Dan Luu | danluu.com | 深入技术细节、性能分析 | 英文 |
| Julia Evans | Julia Evans | jvns.ca | 图解技术、友好解释 | 英文 |
| Armin Ronacher | Armin Ronacher | lucumr.pocoo.org | Flask作者、Python/ Rust | 英文 |
| Basecamp Blog | Basecamp | basecamp.com | 远程工作、产品哲学 | 英文 |
| Stack Overflow Blog | Stack Overflow | stackoverflow.blog | 开发者生态、技术趋势 | 英文 |
| GitHub Blog | GitHub | github.blog | 开源、开发者工具 | 英文 |
| Cloudflare Blog | Cloudflare | blog.cloudflare.com | 网络、安全、性能 | 英文 |
| Netflix Tech Blog | Netflix | netflixtechblog.com | 大规模系统实践 | 英文 |
| Uber Engineering | Uber | uber.com/blog/engineering | 工程实践、开源项目 | 英文 |
| 美团技术团队 | 美团 | tech.meituan.com | 中文大厂技术实践 | 中文 |
| 阿里技术 | 阿里巴巴 | developer.aliyun.com | 阿里云技术文章 | 中文 |
| 字节跳动技术博客 | 字节 | bytebytego.com | 系统设计、架构 | 中文 |
| 阮一峰的网络日志 | 阮一峰 | ruanyifeng.com/blog | 科技周刊、入门教程 | 中文 |
| 酷壳 | 陈皓 | coolshell.cn | 技术思考、职场建议 | 中文 |
| 透明思考 | 张逸 | thinkinginobjects.com | 架构设计、DDD | 中文 |
| 程序员的喵 | 喵叔 | catcoding.me | 独立开发者、技术成长 | 中文 |
| 扯淡大叔 | 大叔 | chegva.com | 架构、技术管理 | 中文 |
| 面向信仰编程 | Draven | draveness.me | 源码分析、分布式 | 中文 |
| 煎鱼 | 煎鱼 |eddycjy.com | Go语言、后端技术 | 中文 |
| 极客时间专栏 | 多位作者 | time.geekbang.org | 体系化技术内容 | 中文 |

---

### 🎨 产品设计与UX

<!-- category: product-design -->
<!-- priority: high -->
<!-- content_types: [design-systems, ux-research, product-thinking, case-studies] -->

| 博客名称 | 作者/机构 | 网址/RSS | 特色内容 | 语言 |
|---------|----------|---------|---------|------|
| Intercom Blog | Intercom | intercom.com/blog | 产品管理、客户成功 | 英文 |
| First Round Review | First Round | firstround.com/review | 创业、产品、管理 | 英文 |
| Lenny's Newsletter | Lenny Rachitsky | lennyrachitsky.com | 产品管理、增长 | 英文 |
| Julie Zhuo | Julie Zhuo | juliezhuo.com | 产品设计、团队管理 | 英文 |
| Design Better | InVision | designbetter.co | 设计系统、设计思维 | 英文 |
| Nielsen Norman Group | NN/g | nngroup.com/articles | UX研究、可用性 | 英文 |
| Smashing Magazine | Smashing | smashingmagazine.com | 前端、设计、UX | 英文 |
| Refactoring UI | Adam Wathan | refactoringui.com | 界面设计实用技巧 | 英文 |
| Growth.design | Dan Benoni | growth.design | 产品心理学案例 | 英文 |
| 产品犬舍 | 多个作者 | pmthinking.com | 中文产品思考 | 中文 |
| 即刻产品笔记 | 即刻团队 | 即刻 | 产品迭代思考 | 中文 |
| 刘言飞语 | 刘飞 | liufei.design | 产品设计、播客 | 中文 |
| 幕后产品 | 各种产品人 | - | 产品设计实践 | 中文 |
| 体验设计笔记 | 设计师 | uxnote.net | UX设计方法 | 中文 |
| 设计潜台词 | 设计团队 | - | 设计思考与案例 | 中文 |

---

### 🚀 独立开发者与Indie Hacker

<!-- category: indie-hacker -->
<!-- priority: high -->
<!-- content_types: [bootstrapping, saas, marketing, personal-stories] -->

| 博客名称 | 作者 | 网址/RSS | 特色内容 | 语言 |
|---------|------|---------|---------|------|
| Indie Hackers | 社区 | indiehackers.com | 独立开发者社区 | 英文 |
| Pieter Levels | Pieter Levels | levels.io | 独立开发、数字游民 | 英文 |
| Starter Story | Pat Walls | starterstory.com | 创业故事采访 | 英文 |
| Microconf | Microconf | microconf.com/blog | 微创业、SaaS | 英文 |
| TinySeed Blog | TinySeed | tinyseed.com | 加速器、 bootstrap | 英文 |
| Courtland Allen | Courtland Allen | courtlandallen.com | Indie Hackers创始人 | 英文 |
| Rob Walling | Rob Walling | robwalling.com | 微创业、SaaS | 英文 |
| Jason Cohen | Jason Cohen | blog.asmartbear.com | 创业、技术、产品 | 英文 |
| Buffer Blog | Buffer | buffer.com/resources | 远程工作、透明文化 | 英文 |
| ConvertKit | ConvertKit | convertkit.com/blog | 创作者经济 | 英文 |
| 利器 | 采访 | liqi.io | 创造者工具与 workflow | 中文 |
| 湾区日报 | 社区 | wanqu.co | 湾区科技资讯 | 中文 |
|  indie hacker 中文 | 社区 | - | 中文独立开发者 | 中文 |
| 利器社群 | 社区 | - | 中文创造者工具 | 中文 |
| 一人公司 | 博主 | - | 独立创业思考 | 中文 |

---

### 💼 创业与商业观察

<!-- category: business-startup -->
<!-- priority: medium -->
<!-- content_types: [strategy, analysis, trends, investment] -->

| 博客名称 | 作者/机构 | 网址/RSS | 特色内容 | 语言 |
|---------|----------|---------|---------|------|
| Stratechery | Ben Thompson | stratechery.com | 科技商业战略分析 | 英文 |
| Above Avalon | Neil Cybart | aboveavalon.com | Apple分析 | 英文 |
| AVC | Fred Wilson | avc.com | 风险投资思考 | 英文 |
| Benedict Evans | Benedict Evans | ben-evans.com | 科技趋势 | 英文 |
| Wait But Why | Tim Urban | waitbutwhy.com | 深度长文、思考 | 英文 |
| Naval Ravikant | Naval | nav.al | 创业、财富、哲学 | 英文 |
| Sam Altman | Sam Altman | blog.samaltman.com | 创业、AI | 英文 |
| Seth Godin | Seth Godin | seths.blog | 营销、领导力 | 英文 |
| a16z Blog | a16z | a16z.com | 风投、科技趋势 | 英文 |
| Sequoia Capital | Sequoia | sequoiacap.com | 投资、创业 | 英文 |
| 36氪 | 36Kr | 36kr.com | 中文科技商业新闻 | 中文 |
| 虎嗅 | 虎嗅 | huxiu.com | 深度商业分析 | 中文 |
| 晚点LatePost | 晚点 | latepost.com | 深度商业报道 | 中文 |
| 乱翻书 | 潘乱 | - | 互联网产品分析 | 中文 |
| 张潇雨 | 张潇雨 | - | 投资、创业思考 | 中文 |
| 知章 | 博主 | - | 商业分析、产品观察 | 中文 |

---

### 📚 人文思考与写作

<!-- category: humanities-thought -->
<!-- priority: medium -->
<!-- content_types: [essays, philosophy, psychology, culture] -->

| 博客名称 | 作者 | 网址/RSS | 特色内容 | 语言 |
|---------|------|---------|---------|------|
| Farnam Street | Shane Parrish | fs.blog | 思维模型、决策 | 英文 |
| The Profile | Polina Marinova | theprofile.substack.com | 人物特写 | 英文 |
| Marginal Revolution | Tyler Cowen | marginalrevolution.com | 经济学、文化 | 英文 |
| Ribbonfarm | Venkatesh Rao | ribbonfarm.com | 深度思考、系统 | 英文 |
| The Convivial Society | Michael Sacasas | theconvivialsociety.com | 技术与社会 | 英文 |
| Aeon | Aeon | aeon.co | 哲学、科学、文化 | 英文 |
| Nautilus | Nautilus | nautil.us | 科学、文化 | 英文 |
| Brain Pickings | Maria Popova | themarginalian.org | 艺术、文学、哲学 | 英文 |
| The School of Life | Alain de Botton | theschooloflife.com | 人生哲学 | 英文 |
| 看理想 | 梁文道等 | vistopia.com.cn | 文化、思想 | 中文 |
| 单读 | 许知远等 | monoreading.com | 文学、思想 | 中文 |
| 槽边往事 | 和菜头 | hecaitou.com | 写作、思考 | 中文 |
| 连岳 | 连岳 | - | 人生、情感、思考 | 中文 |
| 烧伤超人阿宝 | 阿宝 | - | 医学人文 | 中文 |
| 唐茶计划 | 李如一 | - | 独立出版、阅读 | 中文 |

---

### 🔧 效率工具与Workflow

<!-- category: productivity-tools -->
<!-- priority: medium -->
<!-- content_types: [tools, workflows, automation, reviews] -->

| 博客名称 | 作者 | 网址/RSS | 特色内容 | 语言 |
|---------|------|---------|---------|------|
| Uses This | 采访 | usesthis.com | 创造者工具采访 | 英文 |
| MacStories | Federico Viticci | macstories.net | Apple生态、自动化 | 英文 |
| The Sweet Setup | 团队 | thesweetsetup.com | 应用推荐、设置 | 英文 |
| Tools for Thought | 社区 | toolsforthought.rocks | 思维工具 | 英文 |
| Ness Labs | Anne-Laure Le Cunff | nesslabs.com | 生产力、学习 | 英文 |
| Forte Labs | Tiago Forte | fortelabs.com | 第二大脑、PKM | 英文 |
| 少数派 | 社区 | sspai.com | 中文效率工具 | 中文 |
| 利器 | 采访 | liqi.io | 创造者工具 | 中文 |
| 效率火箭 | 博主 | - | 效率工具推荐 | 中文 |
| 玩转Obsidian | 博主 | - | Obsidian教程 | 中文 |
| Notion中文社区 | 社区 | - | Notion使用技巧 | 中文 |

---

## 内容轮换计划

<!-- category: weekly-schedule -->

| 星期 | 主题 | 晨间重点 | 晚间深度 | 主要信源 |
|-----|------|---------|---------|---------|
| 周一 | 技术架构与工程 | 技术头条、新工具 | 架构案例分析 | Martin Fowler, 美团技术, Dan Luu |
| 周二 | 产品思维与设计 | 产品新观点、UX研究 | 产品设计案例 | Intercom, Lenny's Newsletter, 刘言飞语 |
| 周三 | 独立博客与人文 | 独立开发者动态 | 人文深度长文 | Indie Hackers, 利器, Wait But Why |
| 周四 | 创业与商业观察 | 商业资讯、投资动态 | 战略分析 | Stratechery, 晚点, a16z |
| 周五 | 工具与效率 | 新工具发现、Workflow | 工具深度评测 | MacStories, 少数派, Ness Labs |
| 周六 | 本周博客精华 | 本周最佳文章TOP5 | 读者反馈汇总 | 综合 |
| 周日 | 下周值得关注 | 下周预告、订阅推荐 | 月度回顾规划 | 综合 |

---

## 输出格式规范

### 晨间阅读模板 (08:30)

```markdown
☕ **晨间博客精选** | [日期] | [星期X主题]

---

📰 **技术头条**:
1. **[文章标题]** - [作者/博客]
   [2-3句话摘要]
   🔗 [链接]
   💡 关键 takeaway

2. **[文章标题]** - [作者/博客]
   [2-3句话摘要]
   🔗 [链接]
   💡 关键 takeaway

🎨 **产品/设计新思维**:
- **[文章标题]** - [来源]
  [核心观点一句话]
  🔗 [链接]

🛠️ **工具推荐**:
### [工具名称] | [类别标签]
**一句话介绍**: [核心价值]
**适用场景**: [使用场景]
🔗 [官网] | [介绍文章]

---
*晚间22:00带来深度长文*
```

### 晚间阅读模板 (22:00)

```markdown
🌙 **晚间深度阅读** | [日期] | [专题]

---

📖 **深度长文推荐**:
### [文章标题]
**作者**: [作者名] | **来源**: [博客名称]

**文章摘要**:
[300-500字的文章概述，包括：]
[- 文章讨论的核心问题]
[- 作者的主要论点]
[- 值得思考的观点]

**精彩摘录**:
> "[金句1]"

> "[金句2]"

**思考启发**:
[这篇文章对读者的启发或行动建议]

🔗 [阅读原文]

---

🏠 **独立博客精选**:
### [博客名称] - [文章标题]
**博主**: [博主名] | **更新时间**: [日期]

[简短介绍博主和文章背景]

**核心内容**:
[文章内容概述]

🔗 [文章链接] | [博客主页]

---

✨ **金句摘录**:
1. "[金句内容]" —— [作者], [出处]
2. "[金句内容]" —— [作者], [出处]
3. "[金句内容]" —— [作者], [出处]

---

📅 **明日预告**:
明天主题是 **[主题名称]**，将带来 [预告内容简述]

💬 **今日互动**:
[与今日内容相关的思考或讨论问题]

---
*明早08:30见！*
```

---

## 博客质量评估标准

### ✅ 优先收录

| 类型 | 标准 | 示例 |
|-----|------|------|
| 原创内容 | 作者原创思考，非简单转载 | 个人经验总结 |
| 深度分析 | 有深入研究和数据支撑 | 技术分析、案例研究 |
| 长期更新 | 博客持续更新超过1年 | 活跃的个人博客 |
| 实战经验 | 来自实际项目或工作 | 大厂实践、创业经历 |
| 独特观点 | 提供不同寻常的视角 | 独立思考文章 |
| 优质翻译 | 高质量外文翻译 | 经授权的优质译文 |

### ❌ 排除内容

- 内容农场或低质量SEO文章
- 未经核实的转载或抄袭
- 过度商业推广软文
- 已停止更新超过2年的博客
- 付费墙限制过强的内容

---

## RSS订阅管理

### 推荐RSS阅读器

| 工具 | 平台 | 特点 | 适用人群 |
|-----|------|------|---------|
| Feedly | 全平台 | 分类管理、团队协作 | 重度阅读者 |
| Inoreader | 全平台 | 高级过滤、规则 | 高级用户 |
| Reeder | iOS/macOS | 优雅界面、iCloud同步 | 苹果用户 |
| NetNewsWire | iOS/macOS | 开源免费、原生 | 苹果用户 |
| FreshRSS | 自托管 | 隐私保护、自建 | 技术用户 |
| Miniflux | 自托管 | 极简、高效 | 极简主义者 |

### RSS源发现工具

- **RSSHub**: 为没有RSS的网站生成订阅源
- **Follow**: 新一代RSS阅读器，支持订阅博客、社交媒体
- **Feeddd**: 中文RSS源推荐

---

## 用户档案配置

```yaml
user_profile:
  role: ""                    # 角色：开发者/设计师/产品经理/创业者/学生
  primary_interests: []       # 主要兴趣：技术/产品/创业/人文/效率
  reading_time: ""            # 阅读时间偏好：早晨/晚间/碎片时间
  language_preference: ""     # 语言偏好：中文/英文/双语
  depth_preference: ""        # 深度偏好：短文速览/深度长文/两者兼顾
  current_tools: []           # 当前使用的工具
  favorite_blogs: []          # 喜欢的博客
  saved_articles: []          # 收藏的文章

reading_habits:
  morning_reading: true       # 晨间阅读
  evening_reading: true       # 晚间阅读
  weekend_digest: true        # 周末汇总
  weekly_summary: true        # 每周总结

content_filters:
  tech_depth: ""              # 技术深度：入门/进阶/专家
  business_focus: ""          # 商业关注：初创/大厂/投资
  humanities_interest: ""     # 人文兴趣：哲学/文学/心理学
```

---

## 互动反馈机制

**每日互动**:
> 今天的哪篇文章对你最有启发？
> ⭐ 技术文章 | 🎨 设计思考 | 💼 商业观察 | 📚 人文深度

**周度调研**:
> 本周你收藏了哪些文章？
> 下周希望看到哪个领域的更多内容？

**博客推荐**:
用户可以通过 `/recommend [博客URL]` 推荐喜欢的博客

---

## 博客发现渠道

### 聚合平台
- **Hacker News**: 技术社区热门文章
- **Lobste.rs**: 程序员社区
- **Reddit r/programming**: 编程讨论
- **Lire**: 中文优质文章聚合
- **湾区日报**: 湾区科技资讯

### 通讯Newsletter
- **科技洋葱**: 中文科技资讯
- **老司机**: iOS开发资讯
- **前端周刊**: 前端技术汇总
- **Product Habits**: 产品管理
- **The Slice**: 独立创业者

### 社交媒体
- **Twitter/X**: 关注技术大V
- **即刻**: 中文互联网圈子
- **小红书**: 工具使用心得
- **豆瓣**: 人文书评文章

---

## 免责声明

> ⚠️ **重要提示**
>
> 本指南提供的博客推荐仅供参考：
> - 文章观点不代表本指南立场
> - 原创版权归原作者所有
> - 建议阅读原文获取完整信息
> - 外链内容变化与本指南无关

---

*最后更新: 2026-02-28*
*版本: 1.0*
