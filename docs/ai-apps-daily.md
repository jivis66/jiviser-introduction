# AI应用Daily 咨询指南

> **用途**: 本文件用于配置AI助手收集和推荐最新的AI工具、应用案例及行业动态
> **推送时间**: 每日 08:00 (晨间速览) 和 21:00 (晚间深度)
> **推送渠道**: Telegram
> **输出语言**: 中文（外文内容需翻译）
> **内容形式**: 每日3-5条精选资讯 + 1个深度案例 + 1个实用工具推荐

---

## 元数据配置

```yaml
schedule:
  - "08:00"  # 晨间速览：行业快讯、新工具发布
  - "21:00"  # 晚间深度：案例解析、使用教程
timezone: "local"
output_format: "ai-news-digest"
content_mix:
  morning:
    - 行业头条（1-2条重大新闻）
    - 新工具/更新发现（1-2个）
    - 今日热点话题
  evening:
    - 深度案例解析（1个详细案例）
    - 实用工具推荐（1个带教程）
    - 明日预告
rotation:
  monday: "AI编程与开发工具"
  tuesday: "AI设计与创意"
  wednesday: "AI效率与办公"
  thursday: "AI对话与LLM"
  friday: "AI视频与音频"
  saturday: "本周精华回顾"
  sunday: "下周趋势预测"
preferences:
  exclude: ["炒作概念", "未经验证的谣言", "过度商业推广"]
  prioritize: ["实用工具", "真实案例", "开源项目", "深度评测"]
focus_areas:
  - ai_coding          # AI编程
  - ai_design          # AI设计
  - ai_productivity    # AI效率
  - ai_llm             # 大语言模型
  - ai_multimedia      # AI音视频
delivery:
  channel: "telegram"
  format: "markdown"
  include_screenshots: true
```

---

## 信息源列表

### 💻 AI编程与开发

<!-- category: ai-coding -->
<!-- priority: high -->
<!-- content_types: [tools, tutorials, code-examples, reviews] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| GitHub Trending | 代码平台 | github.com/trending | 每日热门AI项目 | 开发者 |
| Hacker News | 社区 | news.ycombinator.com | 技术圈热点讨论 | 技术从业者 |
| Dev.to AI专区 | 博客平台 | dev.to/t/ai | 开发者AI应用文章 | 程序员 |
| LangChain Blog | 框架官方 | blog.langchain.com | LLM应用开发 | AI应用开发者 |
| Vercel AI SDK | 开发工具 | sdk.vercel.ai/docs | AI应用部署 | 全栈开发者 |
| Cursor官方更新 | IDE | cursor.com/changelog | Cursor新功能 | AI编程用户 |
| Windsurf Editor | IDE | codeium.com/windsurf | 新兴AI IDE动态 | 探索新工具者 |
| Sourcegraph Cody | 代码助手 | sourcegraph.com/cody | 企业级代码AI | 企业开发者 |
| 掘金AI专区 | 中文社区 | juejin.cn/ai | 中文AI开发文章 | 中文开发者 |
| 知乎AI编程话题 | 中文问答 | zhihu.com/topic/ai编程 | 中文讨论与评测 | 中文用户 |
| AI Coding Newsletter | 邮件 | aicoding.substack.com | AI编程周报 | 订阅用户 |
| Reddit r/ClaudeCode | 社区 | reddit.com/r/ClaudeCode | Claude编程讨论 | Claude用户 |
| Reddit r/VibeCoding | 社区 | reddit.com/r/VibeCoding | AI编程趋势 | 趋势关注者 |

---

### 🎨 AI设计与创意

<!-- category: ai-design -->
<!-- priority: high -->
<!-- content_types: [tools, showcases, tutorials, prompts] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| Midjourney | 图像生成 | midjourney.com | 最新功能、社区作品 | 设计师 |
| Figma AI博客 | 设计工具 | figma.com/blog | AI设计功能更新 | UI/UX设计师 |
| Adobe Firefly | 创意套件 | adobe.com/firefly | Adobe AI工具 | 创意工作者 |
| Canva AI | 设计平台 | canva.com/ai | 在线设计AI | 非专业设计师 |
| Stability AI | 图像模型 | stability.ai/blog | SD模型更新 | 技术爱好者 |
| Recraft | 设计工具 | recraft.ai | AI矢量设计 | 品牌设计师 |
| Krea.ai | 实时生成 | krea.ai | 实时AI设计 | 创意探索者 |
| Freepik AI | 素材平台 | freepik.com/ai | AI素材生成 | 内容创作者 |
| 站酷AI专区 | 中文设计 | zcool.com.cn/ai | 中文AI设计作品 | 中文设计师 |
| UI中国AI | 中文UI | ui.cn/ai | UI设计AI应用 | UI设计师 |
| PromptHero | 提示词 | prompthero.com | 设计提示词库 | 提示词工程师 |
| LiblibAI | 中文SD | liblib.art | 中文SD模型 | Stable Diffusion用户 |
| 吐司AI | 中文生成 | tusiart.com | 中文生图社区 | 中文创作者 |

---

### 🚀 AI效率与办公

<!-- category: ai-productivity -->
<!-- priority: high -->
<!-- content_types: [tools, workflows, integrations, reviews] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| Notion AI | 笔记工具 | notion.so/product/ai | Notion AI功能 | 知识工作者 |
| Obsidian AI插件 | 笔记工具 | obsidian.md/plugins?search=ai | 本地笔记AI | 隐私重视者 |
| Raycast AI | 启动器 | raycast.com/ai | 快捷AI助手 | Mac用户 |
| Alfred Workflows | 效率工具 | alfred.app/workflows | AI工作流 | 效率控 |
| Zapier AI | 自动化 | zapier.com/ai | AI自动化集成 | 自动化需求者 |
| Make (Integromat) | 自动化 | make.com/en/ai | 可视化AI自动化 | 无代码用户 |
| n8n AI | 自动化 | n8n.io/ai | 开源自动化AI | 自托管用户 |
| Microsoft Copilot | 办公套件 | microsoft.com/copilot | Office AI集成 | 企业用户 |
| Google Workspace AI | 办公套件 | workspace.google.com/solutions/ai | Google办公AI | Google用户 |
| Superhuman AI | 邮件 | superhuman.com/ai | AI邮件处理 | 邮件重度用户 |
| Grammarly | 写作 | grammarly.com | AI写作辅助 | 英文写作者 |
| 飞书智能伙伴 | 中文办公 | feishu.cn/ai | 飞书AI功能 | 国内团队 |
| 钉钉AI助理 | 中文办公 | dingtalk.com/ai | 钉钉AI功能 | 国内企业 |
| 讯飞星火 | 中文AI | xinghuo.xfyun.cn | 国产大模型应用 | 中文用户 |
| 文心一言 | 中文AI | yiyan.baidu.com | 百度AI应用 | 国内用户 |
| 智谱清言 | 中文AI | chatglm.cn | GLM模型应用 | 中文用户 |
| Kimi AI | 中文AI | kimi.moonshot.cn | 长文本处理 | 文档处理者 |
| 通义千问 | 中文AI | tongyi.aliyun.com | 阿里AI应用 | 国内用户 |

---

### 🤖 AI对话与LLM

<!-- category: ai-llm -->
<!-- priority: high -->
<!-- content_types: [models, apis, benchmarks, research] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| OpenAI Blog | 官方 | openai.com/blog | GPT模型更新 | AI从业者 |
| OpenAI API Docs | 开发者 | platform.openai.com/docs | API更新 | 开发者 |
| Anthropic Blog | 官方 | anthropic.com/news | Claude更新 | Claude用户 |
| Google AI Blog | 官方 | ai.googleblog.com | Google AI研究 | 研究者 |
| Gemini API | 开发者 | ai.google.dev | Gemini开发 | Google生态 |
| Hugging Face | 开源社区 | huggingface.co/blog | 开源模型 | 开源爱好者 |
| Together AI | 推理平台 | together.ai/blog | 模型推理 | 应用开发者 |
| Groq | 推理加速 | groq.com | 超快推理 | 性能敏感用户 |
| Cohere | 企业模型 | cohere.com/blog | 企业级LLM | 企业用户 |
| Perplexity Blog | 搜索AI | perplexity.ai/hub/blog | AI搜索更新 | 知识探索者 |
| AI21 Labs | 模型 | ai21.com/blog | Jurassic模型 | 替代方案探索 |
| Mistral AI | 开源模型 | mistral.ai/news | 欧洲开源LLM | 开源支持者 |
| Replicate | 模型平台 | replicate.com/blog | 模型托管部署 | 快速部署者 |
| LMSYS Arena | 评测 | chat.lmsys.org | 模型对战排名 | 模型选择者 |
| Paper with Code | 研究 | paperswithcode.com | 最新研究代码 | 研究者 |
| arXiv AI | 论文 | arxiv.org/list/cs.AI/recent | 最新AI论文 | 学术用户 |
| 机器之心 | 中文媒体 | jiqizhixin.com | 中文AI新闻 | 中文读者 |
| 量子位 | 中文媒体 | qbitai.com | 中文AI快讯 | 中文读者 |
| 新智元 | 中文媒体 | ai.sina.com.cn | 中文AI资讯 | 中文读者 |

---

### 🎬 AI视频与音频

<!-- category: ai-multimedia -->
<!-- priority: medium -->
<!-- content_types: [tools, showcases, tutorials, reviews] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| Runway | 视频生成 | runwayml.com/blog | Gen-3等视频AI | 视频创作者 |
| Pika Labs | 视频生成 | pika.art | Pika视频生成 | 短视频创作者 |
| HeyGen | 数字人 | heygen.com | AI数字人视频 | 营销人员 |
| Synthesia | 数字人 | synthesia.io/blog | 企业数字人 | 企业培训 |
| ElevenLabs | 语音 | elevenlabs.io/blog | AI语音合成 | 播客/配音 |
| Suno | 音乐生成 | suno.ai | AI音乐创作 | 音乐爱好者 |
| Udio | 音乐生成 | udio.com | AI音乐生成 | 音乐创作者 |
| Stable Audio | 音频 | stability.ai/stable-audio | AI音效音乐 | 音频创作者 |
| Descript | 音视频编辑 | descript.com/blog | AI音视频编辑 | 内容创作者 |
| CapCut AI | 视频剪辑 | capcut.com | AI剪辑功能 | 短视频用户 |
|剪映AI | 中文视频 | capcut.cn | 抖音官方剪辑 | 国内创作者 |
| 快影AI | 中文视频 | kuaishou.com/kuaiying | 快手官方剪辑 | 快手用户 |
| 讯飞听见 | 中文语音 | tingxie.iflyrec.com | 语音转文字 | 会议纪要 |
| 魔音工坊 | 中文配音 | morin.vip | AI中文配音 | 中文视频 |
| 剪映图文成片 | 中文AI | capcut.cn | 图文转视频 | 快速创作 |

---

### 📱 AI应用生态

<!-- category: ai-ecosystem -->
<!-- priority: medium -->
<!-- content_types: [apps, plugins, extensions, integrations] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| Product Hunt AI | 产品发现 | producthunt.com/topics/ai | 每日AI新品 | 产品探索者 |
| Futurepedia | 工具目录 | futurepedia.io | AI工具目录 | 工具搜索者 |
| TheresAnAIForThat | 工具发现 | theresanaiforthat.com | AI应用场景 | 场景探索者 |
| Toolify AI | 工具目录 | toolify.ai | AI工具排行 | 工具对比者 |
| TopAI.tools | 工具目录 | topai.tools | AI工具精选 | 质量导向者 |
| Awesome AI | GitHub | github.com/awesome-ai | AI资源合集 | 资源收集者 |
| AI Tools Directory | 目录 | aitoolsdirectory.com | 分类工具目录 | 分类浏览者 |
| GPTs Store | 应用商店 | chatgpt.com/gpts | ChatGPT应用 | GPT用户 |
| Poe | 聚合平台 | poe.com | 多模型聊天 | 模型对比者 |
| You.com | 搜索AI | you.com | AI搜索引擎 | 搜索用户 |
| Perplexity | 搜索AI | perplexity.ai | 对话式搜索 | 研究者 |
| Bing AI | 搜索 | bing.com/chat | 微软AI搜索 | 微软用户 |
| Arc Browser AI | 浏览器 | arc.net/max | 智能浏览器 | 浏览器用户 |
| Brave Leo | 浏览器 | brave.com/leo-ai | 隐私AI助手 | 隐私重视者 |
| Merlin | 浏览器插件 | getmerlin.in | 浏览器AI助手 | 浏览器重度用户 |
| Monica | 浏览器插件 | monica.im | 全能AI插件 | Chrome用户 |
| Elmo Chat | 浏览器插件 | elmo.chat | 网页AI总结 | 阅读者 |
| ChatGPT Sidebar | 插件 | chatgpt-sidebar.com | 侧边栏AI | 研究者 |
|沉浸式翻译 | 中文插件 | immersivetranslate.com | 双语翻译 | 外文阅读者 |
| 划词翻译 | 中文插件 | hcfy.ai | 浏览器翻译 | 中文用户 |

---

## 内容轮换计划

<!-- category: weekly-schedule -->

| 星期 | 主题 | 早间速览重点 | 晚间深度内容 | 主要信源 |
|-----|------|-------------|-------------|---------|
| 周一 | AI编程与开发 | 新工具发布、GitHub热门 | Cursor/V Windsurf深度教程 | GitHub, HN, Cursor Blog |
| 周二 | AI设计与创意 | Midjourney/SD新功能 | 设计案例解析、提示词技巧 | Midjourney, Figma, 站酷 |
| 周三 | AI效率与办公 | Notion/飞书新功能 | 自动化工作流搭建教程 | Notion, Zapier, 飞书 |
| 周四 | AI对话与LLM | GPT/Claude更新 | API开发实战、模型对比 | OpenAI, Anthropic, HF |
| 周五 | AI视频与音频 | Runway/Pika新功能 | 视频制作案例、工具对比 | Runway, ElevenLabs |
| 周六 | 本周精华回顾 | 本周热门工具TOP5 | 深度评测合集 | Product Hunt, 综合 |
| 周日 | 下周趋势预测 | 下周值得关注的新品 | 行业趋势分析 | 投资动态, 研究论文 |

---

## 输出格式规范

### 晨间速览模板 (08:00)

```markdown
🌅 **AI晨间速览** | [日期] | [星期X主题]

---

📰 **行业头条**:
1. **[新闻标题]**
   [一句话摘要]
   🔗 [来源链接]

2. **[新闻标题]**
   [一句话摘要]
   🔗 [来源链接]

🆕 **新发现**:
- **[工具名称]**: [一句话描述] [标签: #编程 #设计 #效率]
  🔗 [官网链接]

- **[工具名称]**: [一句话描述] [标签: #视频 #音频 #国产]
  🔗 [官网链接]

🔥 **今日热点**:
[当前AI圈讨论最多的话题简述]

💡 **今日一句话**:
[一句启发性的观点/建议]

---
*晚间21:00带来深度解析*
```

### 晚间深度模板 (21:00)

```markdown
🌙 **AI晚间深度** | [日期] | [专题名称]

---

📖 **深度案例**:
### [案例标题]

**背景**:
[案例背景介绍]

**应用场景**:
[具体使用场景描述]

**实现方式**:
1. [步骤1]
2. [步骤2]
3. [步骤3]

**效果展示**:
[成果描述或截图/视频链接]

**经验总结**:
[关键经验点]

🔗 [完整案例链接]

---

🛠️ **工具推荐**:
### [工具名称] | [类别标签]

**一句话介绍**:
[工具核心价值]

**核心功能**:
- [功能1]
- [功能2]
- [功能3]

**适用人群**:
[适合谁使用]

**上手教程**:
1. [快速开始步骤]
2. [关键设置]
3. [实用技巧]

**价格**:
[免费/付费情况]

🔗 [官网] | [教程] | [社区]

---

📅 **明日预告**:
明天主题是 **[主题名称]**，将带来 [预告内容简述]

📝 **今日互动**:
[与今日内容相关的互动问题]

---
*明早08:00见！*
```

---

## 信息筛选标准

### ✅ 优先收录

| 类型 | 标准 | 示例 |
|-----|------|------|
| 新工具发布 | 有实际可用产品，非纯概念 | 官方Release Notes |
| 重要更新 | 改变用户体验的重大版本 | v2.0发布 |
| 实用教程 | 有具体操作步骤，可复现 | 图文/视频教程 |
| 真实案例 | 有具体数据或成果展示 | 用户案例研究 |
| 开源项目 | GitHub Star > 500 | Trending项目 |
| 深度评测 | 多维度对比测试 | 实测文章 |

### ❌ 排除内容

- 纯概念产品，无实际可用版本
- 过度夸大的营销内容
- 无来源的技术谣言
- 明显广告软文（除非产品本身优秀）
- 重复发布的旧闻

---

## 用户档案配置

```yaml
user_profile:
  role: ""                    # 角色：开发者/设计师/产品经理/学生/爱好者
  primary_use_case: ""        # 主要用途：工作/学习/创作/娱乐
  preferred_platforms: []     # 偏好平台：Web/Mac/Windows/iOS/Android
  language_preference: ""     # 语言偏好：中文/英文/双语
  skill_level: ""             # 技术水平：新手/进阶/专家
  budget: ""                  # 预算：免费/月付<50/月付<200/企业
  specific_interests: []      # 具体关注领域
  current_tools: []           # 当前使用的AI工具
  pain_points: []             # 工作中的痛点

notification_preferences:
  morning_digest: true        # 早间速览
  evening_deep_dive: true     # 晚间深度
  breaking_news: true         # 重大突发
  tool_recommendations: true  # 工具推荐
  tutorials: true             # 教程内容
```

---

## 互动反馈机制

**每日互动**:
> 这个工具对你有帮助吗？
> ⭐ 很有用 | 👍 还不错 | ⭐ 不感兴趣

**周度调研**:
> 本周你尝试了哪些AI工具？有什么发现？
> 下周你希望看到哪个领域的深度内容？

**即时反馈**:
- `/tool [工具名]` - 查询特定工具信息
- `/compare [工具A] vs [工具B]` - 对比工具
- `/tutorial [主题]` - 获取主题教程

---

## 社区与资源

### 中文AI社区
- **即刻AI话题**: 中文AI从业者聚集地
- **知乎AI话题**: 深度讨论
- **知识星球**: 付费AI社群
- **微信AI公众号**: 机器之心、量子位、新智元
- **B站AI区**: 视频教程
- **小红书AI话题**: 使用心得

### 国际社区
- **Reddit r/ArtificialIntelligence**: 综合AI讨论
- **Reddit r/LocalLLaMA**: 本地模型
- **Discord AI社区**: Midjourney、Stable Diffusion等
- **Twitter/X AI圈**: 实时动态
- **LinkedIn AI**: 职业角度

---

## 免责声明

> ⚠️ **重要提示**
>
> 本指南提供的信息仅供参考：
> - 工具推荐不构成购买建议
> - 使用前请自行评估安全性和隐私政策
> - AI生成内容可能存在错误，请自行验证
> - 付费工具请根据实际需求选择

---

*最后更新: 2026-02-28*
*版本: 1.0*
