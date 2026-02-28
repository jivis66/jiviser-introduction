# Reddit AI Subreddits 监控清单

> **用途**: 本文件用于配置AI助手监控Reddit上AI相关子版块的高价值帖子
> **更新频率**: 每日下午5点
> **输出语言**: 中文（非中文内容需翻译）

---

## 元数据配置

```yaml
schedule: "17:00"  # 每天运行时间
timezone: "local"
output_format: "summary"
translation:
  enabled: true
  target_language: "zh-CN"
  source_languages: ["en", "ja", "ko", "de", "fr"]
preferences:
  exclude: ["memes", "low-effort", "spam"]
  prioritize: ["tutorials", "news", "discussions", "showcase"]
delivery:
  channel: "telegram"
  format: "markdown"
```

---

## 监控目标

### 🧠 一般 AI 讨论

<!-- category: general-ai -->
<!-- priority: high -->
<!-- content_types: [news, discussion, tutorials] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/ArtificialIntelligence | 大型综合AI社区，讨论最新发展动态 | 行业新闻、技术突破 |
| r/PromptEngineering | 提示词工程技巧与策略分享 | 提示词教程、最佳实践 |
| r/GenerativeAI | 生成式AI内容与工具讨论 | 创意应用、灵感分享 |
| r/AIToolTesting | AI工具使用经验分享 | 新工具评测、使用案例 |
| r/AiAssisted | 实际AI用户的实践讨论 | 真实用例、工作流 |
| r/AICuriosity | 最新工具、新闻和发展动态 | 工具推荐、求助讨论 |

---

### 🤖 大型语言模型 (LLMs)

<!-- category: llm -->
<!-- priority: high -->
<!-- content_types: [news, coding, prompts, discussions] -->

#### OpenAI 生态
| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/ChatGPT | 最大的ChatGPT专属社区 | 使用技巧、提示词帮助 |
| r/ChatGPTPro | 专业级ChatGPT和LLM使用 | 高级工作流、研究 |
| r/ChatGPTPromptGenius | 提示词优化教学 | 提示词技巧、最佳结果 |
| r/OpenAI | OpenAI全生态讨论 | GPT、Sora、DALL-E 3 |

#### Google 生态
| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/GeminiAI | Google Gemini LLM讨论 | 使用技巧、灵感 |
| r/Bard | Google Bard（已更名为Gemini） | 历史内容、迁移信息 |

#### Anthropic 生态
| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/Anthropic | Claude背后的公司讨论 | 公司动态、技术理念 |
| r/ClaudeAI | Claude使用与编程讨论 | 编程辅助、日常使用 |

#### 其他重要LLM
| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/PerplexityAI | Perplexity AI搜索与研究 | 简短答案、研究用例 |
| r/DeepSeek | DeepSeek中文LLM社区 | 中文优化、替代方案 |
| r/Microsoft365Copilot | Microsoft 365 Copilot | 办公集成、问题求助 |
| r/Grok | Grok最新动态 | 用户案例、新闻 |
| r/MistralAI | 欧洲Mistral LLM | 开源模型、欧洲AI |
| r/QwenAI | 阿里巴巴Qwen模型 | 新模型、使用案例 |
| r/LocalLLaMA | Meta Llama本地运行 | 本地部署、新功能 |
| r/Kimi | 月之暗面Kimi助手 | 中文助手、新功能发布 |

---

### 🖼️ 图像与视频生成

<!-- category: image-video -->
<!-- priority: medium -->
<!-- content_types: [showcase, tutorials, prompts] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/Midjourney | 热门文生图生成器作品 | 艺术作品、提示词灵感 |
| r/NanoBanana | Google图片生成器社区 | 提示词、图像灵感 |
| r/Veo3 | Google Veo 3视频生成器 | 视频作品、使用技巧 |
| r/StableDiffusion | 开源图像生成巨大社区 | 本地运行、技术讨论 |
| r/Dalle2 | DALL-E各版本讨论（含DALL-E 3） | 作品展示、版本对比 |
| r/LeonardiAI | 多模型图像视频生成工具 | 功能讨论、作品分享 |
| r/HiggsfieldAI | Higgsfield视频生成 | 视频灵感、用户作品 |
| r/KlingAIVideos | Kling AI视频生成 | 视频分享、求助讨论 |
| r/AIGeneratedArt | 多模型AI艺术混合社区 | 综合灵感、跨平台 |
| r/AIImages | 各类AI生成器图像 | 提示词灵感、作品展示 |
| r/Aivideos | AI视频展示与分享 | 视频项目、创作技巧 |
| r/AIArt | AI艺术创作社区 | 惊人作品、艺术讨论 |

---

### 🎵 音乐生成

<!-- category: music -->
<!-- priority: low -->
<!-- content_types: [showcase, tutorials, news] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/SunoAI | Suno AI音乐生成最大社区 | 音乐作品、创作技巧 |
| r/UdioMusic | Udio官方社区（活跃度下降） | 平台动态、遗留内容 |
| r/AIMusic | 多平台AI音乐讨论 | 新闻、工具对比 |

---

### ✍️ AI 辅助写作

<!-- category: writing -->
<!-- priority: medium -->
<!-- content_types: [tutorials, discussions, tips] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/WritingWithAI | 作家AI写作指导社区 | 文案技巧、内容创作 |
| r/AIWritingHub | 小型AI内容写作社区 | 日常讨论、互动内容 |
| r/BookwritingAI | AI书籍写作社区 | 长篇创作、写作流程 |

---

### 🌐 SEO 与营销

<!-- category: seo-marketing -->
<!-- priority: medium -->
<!-- content_types: [tutorials, news, strategies] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/SEO | AI时代的SEO优化 | AI工具应用、策略更新 |
| r/BigSEO | 大型SEO从业者社区 | 实用信息、问题解答 |
| r/TechSEO | 技术SEO讨论 | 技术实现、深度优化 |
| r/MarketingAutomation | AI营销自动化 | 营销策略、工具集成 |

---

### ⚙️ 工作流与自动化

<!-- category: automation -->
<!-- priority: high -->
<!-- content_types: [workflows, tutorials, integrations] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/Automation | AI与任务自动化综合 | 工作自动化、日常使用 |
| r/AI_Agents | LLM自主/半自主代理 | Agent开发、工具使用 |
| r/AI_Automations | AI工作流与商业策略 | 工作流分享、商业应用 |
| r/n8n | n8n工作流自动化平台 | 平台使用、集成方案 |
| r/Zapier | Zapier自动化平台 | 工具连接、自动化技巧 |

---

### 💻 AI 辅助编程

<!-- category: coding -->
<!-- priority: high -->
<!-- content_types: [tutorials, showcases, debugging, tips] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/VibeCoding | 最大AI编程社区 | 编程策略、代码分享 |
| r/ClaudeCode | Claude编程专用社区 | Claude代码能力、技巧 |
| r/ChatGPTCoding | ChatGPT编程讨论 | 代码帮助、调试技巧 |
| r/OnlyAIcoding | 无编程技能者策略 | 学习资源、入门指南 |
| r/VibeCodeDevs | AI编程技巧与项目 | 技巧窍门、项目展示 |
| r/Cursor | Cursor AI编程平台 | IDE使用、应用开发 |
| r/Google_antigravity | Google AI驱动IDE | 代理优先开发、新功能 |

---

### 📚 研究与深度讨论

<!-- category: research -->
<!-- priority: medium -->
<!-- content_types: [news, research, discussions] -->

| Subreddit | 描述 | 关注重点 |
|-----------|------|----------|
| r/Artificial | AI新闻与讨论 | 最新发展、行业动态 |
| r/MachineLearning | 机器学习社区（2009年起） | 研究论文、技术深入 |
| r/Singularity | 技术奇点与未来技术 | 前沿预测、深度讨论 |

---

## 输出格式规范

### 每日摘要应包含:

1. **热门帖子概览** - 每个子版块1-3个高互动帖子
2. **分类总结** - 按上述类别分组
3. **重点推荐** - 标记最具价值的讨论
4. **行动项** - 需要关注或尝试的内容

### 内容过滤规则:

- ❌ **排除**: 纯表情包、低质量内容、垃圾信息
- ✅ **优先**: 教程、新闻、深度讨论、作品展示
- 🔄 **翻译**: 所有非中文内容翻译为中文
- 📊 **排序**: 按互动量（点赞+评论）降序

---

## 用户偏好学习

> **注意**: 以下部分由AI助手根据用户反馈动态更新

```yaml
user_preferences:
  liked_topics: []      # 记录用户喜欢的主题类型
  disliked_topics: []   # 记录用户不喜欢的内容
  preferred_format: ""   # 用户偏好的摘要格式
  translation_quality: "" # 翻译风格偏好
  priority_categories: [] # 高优先级关注的类别
```

**每日确认问题模板**:
> 今日推荐的帖子是否符合您的兴趣？有哪些您希望看到更多/更少的内容？

---

## 外部资源参考

以下是人工策划的AI社区清单，涵盖多平台：

- **最佳 AI Subreddits**: 学习AI、获取新闻、技巧、提示词指南
- **最佳 AI YouTube 频道**: 新闻、发展、教程
- **最佳 AI Discord 服务器**: 学习讨论（如使用Discord）
- **最佳 AI X 账号**: 新闻、技巧、用例、教程
- **最佳 AI Facebook 粉丝页/社团**: 新闻、工具发布、讨论
- **最佳 AI 电子报**: 每日/每周新闻汇总
- **最佳 AI 工具目录**: 探索数千个AI工具

---

*最后更新: 2026-02-28*
*版本: 2.0*
