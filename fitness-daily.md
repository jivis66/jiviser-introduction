# 运动健康Daily 咨询指南

> **用途**: 本文件用于配置AI助手提供运动健康、跑步、公路车相关的每日咨询与建议
> **推送时间**: 每日 07:00 (晨间激励) 或 20:00 (晚间复盘)
> **推送渠道**: Telegram
> **输出语言**: 中文
> **内容形式**: 每日1条核心建议 + 1个知识要点 + 可选训练计划

---

## 元数据配置

```yaml
schedule:
  - "07:00"  # 晨间激励
  - "20:00"  # 晚间复盘（可选）
timezone: "local"
output_format: "daily-fitness-tip"
content_mix:
  daily_structure:
    - 今日主题（运动健康/跑步/公路车轮换）
    - 核心建议（1条 actionable 建议）
    - 知识要点（科学原理解释）
    - 训练提示（可选，基于用户目标）
    - 来源链接
rotation:
  monday: "跑步训练"
  tuesday: "公路车技术与装备"
  wednesday: "运动康复与伤病预防"
  thursday: "力量训练与核心"
  friday: "骑行路线与活动"
  saturday: "周末长距离训练建议"
  sunday: "恢复与营养"
preferences:
  exclude: ["高风险动作", "无科学依据的偏方", "过度训练建议"]
  prioritize: ["科学训练", "伤病预防", "循序渐进", "实用技巧"]
user_goals:
  running: ""      # 跑步目标（减脂/5K/10K/半马/全马）
  cycling: ""      # 骑行目标（休闲/通勤/爬坡/长途）
  fitness_level: "" # 当前水平（新手/进阶/资深）
delivery:
  channel: "telegram"
  format: "markdown"
  include_video: true  # 如有教学视频链接
```

---

## 信息源列表

### 🏃 跑步与马拉松

<!-- category: running -->
<!-- priority: high -->
<!-- content_types: [training-plans, injury-prevention, gear-reviews, science] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| Runner's World | 杂志/网站 | runnersworld.com | 权威跑步训练计划、装备评测、伤病预防 | 全水平跑者 |
| Hal Higdon | 训练计划 | halhigdon.com | 经典马拉松训练计划，从5K到全马 | 备赛跑者 |
| McMillan Running | 训练 | mcmillanrunning.com | 科学配速计算、个性化训练建议 | 数据驱动跑者 |
| The Run Experience | 视频/YouTube | youtube.com/@TheRunExperience | 跑姿分析、力量训练、伤病康复 | 视觉学习者 |
| Sweat Science (Alex Hutchinson) | 科学博客 | sweatscience.com | 运动科学研究解读，破除迷思 | 科学爱好者 |
| 跑步学院 | 中文公众号 | - | 中国本土跑者教育、训练营 | 中文用户 |
| 慧跑 | 中文平台 | hui-run.com | 跑步数据分析、训练指导 | 数据化跑者 |
| 跑野大爆炸 | 中文媒体 | runyeyeye.com | 国内外跑步新闻、赛事报道 | 跑步爱好者 |

---

### 🚴 公路车与骑行

<!-- category: cycling -->
<!-- priority: high -->
<!-- content_types: [technique, gear, routes, maintenance, racing] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| GCN (Global Cycling Network) | 视频/YouTube | youtube.com/@gcn | 骑行技术、装备评测、训练建议 | 全水平骑手 |
| GCN Racing | 赛事 | youtube.com/@gcnracing | 职业赛事报道、技术分析 | 赛事爱好者 |
| Cycling Weekly | 杂志 | cyclingweekly.com | 英国权威骑行媒体，装备与训练 | 英语读者 |
| BikeRadar | 评测 | bikeradar.com | 详尽的自行车与装备评测 | 装备党 |
| TrainerRoad Blog | 训练 | trainerroad.com/blog | 功率训练、科学骑行训练方法 | 严肃训练者 |
| The Pro's Closet | 装备 | theproscloset.com | 二手车、装备知识 | 装备爱好者 |
| 骑行家 | 中文媒体 | cyclingchina.net | 国内骑行新闻、赛事、装备 | 中文骑手 |
| 美骑网 | 中文平台 | biketo.com | 国内最大骑行社区，路线/装备/评测 | 中文用户 |
| 公路车吧精华 | 论坛 | tieba.baidu.com/f?kw=公路车 | 国内骑友经验分享、问答 | 入门/进阶 |

---

### 💪 运动健康与体能

<!-- category: fitness-health -->
<!-- priority: high -->
<!-- content_types: [strength, mobility, nutrition, recovery, injury-prevention] -->

| 来源名称 | 类型 | 网址/RSS | 特色内容 | 适合人群 |
|---------|------|---------|---------|---------|
| Barbell Medicine | 医学/力量 | barbellmedicine.com | 医学博士主理，力量训练与康复 | 科学训练者 |
| Squat University | 康复 | squatuniversity.com | Dr. Aaron Horschig，深蹲与伤病预防 | 力量训练者 |
| The Ready State (Kelly Starrett) | 灵活性 | thereadystate.com | 灵活性、恢复、疼痛管理 | 需要恢复者 |
| Precision Nutrition | 营养 | precisionnutrition.com | 循证运动营养建议 | 关注饮食者 |
| Examine.com | 补剂 | examine.com | 运动补剂科学研究数据库 | 补剂使用者 |
| Strength Running | 力量 | strengthrunning.com | 跑者专项力量训练 | 跑者 |
| Peloton Digital | 训练 | onepeloton.com | 室内骑行/跑步课程 | 室内训练者 |
| Zwift Insider | 虚拟骑行 | zwiftinsider.com | Zwift平台攻略、路线、活动 | Zwift用户 |

---

### 🏥 运动医学与康复

<!-- category: sports-medicine -->
<!-- priority: medium -->
<!-- content_types: [injury-treatment, prevention, rehab-protocols] -->

| 来源名称 | 类型 | 网址 | 特色内容 | 适合人群 |
|---------|------|------|---------|---------|
| British Journal of Sports Medicine | 学术期刊 | bjsm.bmj.com | 最新运动医学研究 | 专业人士 |
| Running Physio (Tom Goom) | 物理治疗 | running-physio.com | 跑步伤病评估与康复 | 伤病恢复中 |
| The Running Clinic | 教育 | therunningclinic.com | 跑步步态分析、伤痛管理 | 慢性伤痛者 |
| 运动康复陈文杰 | 中文/视频 | B站/小红书 | 中文运动康复科普 | 中文用户 |
| 上海体育学院运动康复 | 学术 | - | 国内权威运动康复知识 | 专业学习者 |

---

## 内容轮换计划

<!-- category: weekly-schedule -->

| 星期 | 主题 | 核心内容 | 参考来源 |
|-----|------|---------|---------|
| 周一 | 跑步训练 | 配速策略、间歇训练、长距离安排 | Runner's World, Hal Higdon |
| 周二 | 公路车技术 | 爬坡技巧、下坡安全、团队骑行 | GCN, Cycling Weekly |
| 周三 | 伤病预防 | 常见伤痛识别、预防措施、何时停训 | Squat University, Running Physio |
| 周四 | 力量与核心 | 跑者/骑手专项力量、核心稳定 | Strength Running, Barbell Medicine |
| 周五 | 装备与维护 | 装备选购、保养知识、性价比推荐 | BikeRadar, 美骑网 |
| 周六 | 周末训练建议 | 长距离骑行/跑步路线规划、补给策略 | The Run Experience, TrainerRoad |
| 周日 | 恢复与营养 | 主动恢复、拉伸、营养补充、睡眠 | The Ready State, Precision Nutrition |

---

## 特殊主题储备

<!-- category: special-topics -->

### 新手入门系列
- 如何开始第一次5K跑步
- 公路车选购指南（预算分级）
- 基础装备清单（跑步/骑行）
- 正确的骑行姿势设定

### 进阶提升系列
- 乳酸阈值训练详解
- FTP测试与功率训练基础
- 马拉松周期化训练
- 爬坡技术与呼吸节奏

### 伤病管理系列
- 跑者膝(ITBS)的识别与康复
- 跟腱炎的预防与恢复
- 骑行腰痛的原因与解决
- 足底筋膜炎的自我处理

### 赛事准备系列
- 首马/首百准备清单
- 比赛日策略与配速
- 长途骑行补给计划
- 赛前减量(Taper)指南

---

## 输出格式规范

### 每日咨询模板

```markdown
🏃‍♂️ **今日运动咨询** | [主题名称]

📅 **星期X** | 专注领域: [跑步/骑行/康复/力量]

---

🎯 **核心建议**:
[1条具体、可操作的建议，如:
"今天的轻松跑请控制在最大心率的65-70%，时长45分钟，不要急于提速"]

📚 **知识要点**:
**[知识点标题]**
[科学原理简要解释，150字以内，如:
"轻松跑(Easy Run)的主要目的是建立有氧基础。在这个强度下，身体主要使用脂肪作为燃料，同时促进毛细血管增生和线粒体密度提升。过快的配速会转入无氧区间，失去基础训练的效果。"]

💡 **今日训练提示**:
- 如果今天计划跑步: [具体建议]
- 如果今天计划骑行: [具体建议]
- 如果今天休息: [恢复建议]

⚠️ **注意事项**:
[伤病预警、天气提醒或其他重要提示]

🔗 **延伸阅读**:
- [相关文章1标题](链接)
- [相关文章2标题](链接)
- [视频教程标题](YouTube/B站链接)

---

📊 **本周进度**:
周一 ✅ | 周二 ✅ | 周三 ⏳ | 周四 ⬜ | 周五 ⬜ | 周六 ⬜ | 周日 ⬜

*明天07:00见，记得按时训练！*
```

---

## 用户档案配置

```yaml
user_profile:
  running:
    current_level: ""        # 新手/5K完赛/10K完赛/半马完赛/全马完赛
    weekly_mileage: 0        # 当前周跑量(公里)
    goal_race: ""            # 目标赛事
    goal_time: ""            # 目标成绩
    preferred_terrain: ""    # 公路/跑道/越野
    injuries_history: []     # 伤病历史

  cycling:
    current_level: ""        # 休闲/通勤/进阶/竞技
    weekly_distance: 0       # 当前周骑行量(公里)
    ftp_watts: 0             # 功能性阈值功率
    bike_type: ""            # 公路车/山地车/折叠车
    preferred_riding: ""     # 平路/爬坡/长途/团骑
    indoor_trainer: false    # 是否有骑行台

  general:
    age: 0
    resting_hr: 0            # 静息心率
    max_hr: 0                # 最大心率(实测或估算)
    available_time: ""       # 每周可训练时间
    limitations: []          # 身体限制或特殊情况
```

---

## 互动反馈机制

**每日确认问题模板**:
> 今天的建议对你有帮助吗？你目前的训练重点是：
> A) 提升跑步配速  B) 增加骑行功率  C) 伤病恢复  D) 减脂塑形

**周度复盘问题**:
> 本周完成训练 ___ 次 | 总距离 ___ 公里
> 身体状况: 很好/良好/有疲劳/有伤痛
> 下周希望关注的话题：___

---

## 安全免责声明

<!-- category: disclaimer -->

> ⚠️ **重要提示**
>
> 本指南提供的所有运动建议仅供参考，不构成医疗建议。
> - 开始任何新的运动计划前，请咨询医生
> - 如有持续性疼痛，请立即停止训练并就医
> - 循序渐进，避免过度训练
> - 个人体质差异大，请根据自身情况调整

---

## 社区与活动

### 国内跑步/骑行社区
- **悦跑圈**: 国内最大跑步APP，有线上挑战赛
- **Strava**: 全球运动社交平台，记录与分享
- **Keep**: 国内健身APP，有跑步/骑行课程
- **Garmin Connect**: 佳明用户生态
- **顽鹿/Onelap**: 国内骑行虚拟平台

### 推荐赛事日历（国内）
- 马拉松赛事: 关注"马拉松报名"等公众号
- 骑行活动: 关注各地自行车协会、美骑网
- Gran Fondo: 长距离骑行挑战活动

---

*最后更新: 2026-02-28*
*版本: 1.0*
*免责声明: 运动有风险，训练需谨慎*
