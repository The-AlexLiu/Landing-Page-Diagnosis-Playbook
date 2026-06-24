# Landing Page Diagnosis Playbook

一套面向增长、投放、内容策略和产品体验的落地页内容诊断方法。

我把落地页看成转化链路中的一个关键承接点，而不是单独的一张销售页面。用户从广告、搜索、邮件、站内入口或销售链接进入页面时，已经带着预期。诊断的重点不是先判断页面好不好看，而是判断页面有没有接住用户的问题，并推动他走到合理的下一步。

---

## 这个项目解决什么问题

很多落地页复盘会停留在比较主观的层面：

- 标题不够吸引；
- 页面不够高级；
- 按钮不够明显；
- 卖点不够突出。

这些判断可能有道理，但很难直接指导执行。这个项目把落地页拆成可检查、可评分、可复盘的诊断框架，用来回答更具体的问题：

- 用户从哪里来，页面有没有承接入口承诺？
- 首屏能不能在几秒内讲清楚价值？
- 用户为什么会不信，页面有没有提前解除风险？
- CTA 是否符合用户当前阶段？
- 页面问题能否用广告数据、GA4、热图或用户反馈验证？
- 哪些问题应该立即修，哪些问题应该测试，哪些还需要补数据？

---

## 适用场景

| 页面类型 | 主要诊断目标 |
|---|---|
| 广告落地页 | 承接素材/关键词意图，提升 CVR、CPA、ROAS |
| 独立站商品页 | 强化商品理解、信任证据、购买路径 |
| 活动页 | 说明优惠、规则、时间、参与路径 |
| SaaS 官网 | 把产品能力翻译成用户任务和业务结果 |
| App 下载页 | 快速解释下载理由和核心使用场景 |
| B2B 线索页 | 降低表单阻力，补充案例、交付和隐私说明 |
| 内容增长页 | 承接标题承诺，引导订阅、下载或下一步阅读 |
| 服务办理页 | 帮用户判断条件、材料、步骤和结果查询 |

---

## 12 个诊断维度

| 维度 | 主要看什么 | 常见问题 |
|---|---|---|
| 来源意图匹配 | 页面是否接住广告、搜索词、入口承诺 | 广告讲优惠，页面讲品牌故事 |
| 首屏价值主张 | 用户几秒内能不能理解价值 | 标题抽象、首屏无 CTA、利益不清楚 |
| 信息架构 | 内容顺序是否符合用户决策 | 证据太后、规则太散、重点被埋 |
| 可扫描性 | 小标题、列表、表格是否好读 | 大段文字、卖点堆叠、没有层级 |
| 可信证据 | 有没有让用户相信的材料 | 评价空泛、案例无结果、数据无口径 |
| 产品/服务解释 | 用户是否理解具体怎么用 | 只写功能名，不写场景和结果 |
| CTA 与行动路径 | 下一步是否明确、顺手、可追踪 | 按钮多、文案虚、点击后无反馈 |
| 风险解除 | 用户顾虑是否被提前回答 | 价格、售后、隐私、退款不清楚 |
| 移动端体验 | 手机上是否好看、好点、加载快 | 首屏白屏、弹窗遮挡、按钮太小 |
| 合规与透明 | 是否存在夸大、隐藏、诱导 | 隐藏费用、默认勾选、虚假稀缺 |
| 数据追踪 | 能不能判断问题出在哪里 | UTM 丢失、事件重复、归因口径不明 |
| 品牌一致性 | 页面是否和品牌、产品、客服口径一致 | 广告、页面、客服说法不一样 |

---

## 快速使用方式

### 1. 先做 30 分钟快诊

适合投放前检查、页面上线前 review、广告异常时快速定位。

| 步骤 | 操作 | 输出 |
|---|---|---|
| 1 | 收集广告素材、关键词或入口截图 | 来源承诺清单 |
| 2 | 用手机打开最终 URL | 移动端首屏截图 |
| 3 | 对照首屏内容 | 判断是否承接来源意图 |
| 4 | 点击主 CTA | 检查路径、参数、反馈 |
| 5 | 快速扫信任信息 | 价格、评价、案例、售后、隐私 |
| 6 | 检查追踪 | GA4、Pixel、Tag Assistant |
| 7 | 输出优先级 | 立即修、观察、测试、暂停 |

### 2. 再做深度评分

使用 [`templates/diagnosis-checklist.csv`](templates/diagnosis-checklist.csv) 导入 Google Sheet 或 Excel，按 12 个维度逐项评分，并记录证据。

建议评分规则：

| 分数 | 判断 |
|---:|---|
| 0 | 缺失，或明显误导，可能影响转化、审核或用户完成任务 |
| 1 | 有内容但不完整，用户需要猜 |
| 2 | 基本可用，但表达泛、证据弱、路径不够清楚 |
| 3 | 合格，能承接主要用户任务 |
| 4 | 清晰、有证据、路径顺，移动端体验良好 |
| 5 | 高度匹配用户意图，并且有数据持续验证 |

### 3. 最后输出执行优先级

| 类型 | 适用情况 |
|---|---|
| 立即执行 | 页面打不开、CTA 不可点、价格不一致、UTM 丢失 |
| 观察等待 | 样本不足，或广告组仍在学习期 |
| 小预算测试 | 有明确假设，但需要验证 |
| 暂停或降预算 | 页面问题会直接浪费预算或带来审核风险 |
| 需要补充数据 | 缺广告素材、缺 GA4、缺转化定义、缺利润数据 |

---

## 项目结构

```text
.
├── README.md
├── docs
│   ├── portfolio-notes.md
│   └── research-framework.md
└── templates
    └── diagnosis-checklist.csv
```

| 文件 | 说明 |
|---|---|
| [`README.md`](README.md) | 项目主展示页，适合快速阅读 |
| [`docs/portfolio-notes.md`](docs/portfolio-notes.md) | 作品集版经验沉淀，适合面试或作品集正文 |
| [`docs/research-framework.md`](docs/research-framework.md) | 更完整的调研版方法论，包含更多细节和参考资料 |
| [`templates/diagnosis-checklist.csv`](templates/diagnosis-checklist.csv) | 可导入表格的诊断评分清单 |

---

## 作品集展示建议

如果把这套方法用于作品集，我建议不要只展示“我改了一个页面”，而是展示完整的问题解决过程：

1. **项目背景**：页面类型、业务目标、流量来源、核心 KPI。
2. **问题定义**：把“页面不转化”拆成可验证的问题。
3. **诊断方法**：展示 12 维度框架、数据来源和截图标注方式。
4. **核心发现**：列出 3 到 5 个影响最大的断点。
5. **优化方案**：按首屏、证据、CTA、风险解除、移动端、追踪拆解。
6. **结果复盘**：展示 CVR、CPA、ROAS、表单率、加购率或任务完成率变化。
7. **边界说明**：样本不足、归因差异、无法验证的数据都要说明。

这套方法想表达的能力不是“会写落地页文案”，而是：

- 能把页面问题放回完整转化链路里看；
- 能从广告素材、关键词、用户意图和页面内容之间找断点；
- 能把抽象问题拆成可检查、可排序、可验证的事项；
- 能同时考虑短期投放结果和长期用户信任；
- 能用数据、截图、用户行为和业务目标支撑建议。

---

## 参考资料

- Nielsen Norman Group: Web usability, information scent, trustworthiness, web writing  
  https://www.nngroup.com/articles/
- Google Ads Help: Quality Score, Landing Page Experience, ad and landing page alignment  
  https://support.google.com/google-ads/
- Google Search Central: Core Web Vitals, page experience, A/B testing  
  https://developers.google.com/search/docs/
- W3C WCAG 2.2: Accessibility guidelines  
  https://www.w3.org/TR/WCAG22/
- FTC: Bringing Dark Patterns to Light  
  https://www.ftc.gov/reports/bringing-dark-patterns-light
- GOV.UK Service Manual: Service design and content design  
  https://www.gov.uk/service-manual
- Baymard Institute: Ecommerce UX research  
  https://baymard.com/
- Microsoft Clarity: Heatmaps and session recordings  
  https://clarity.microsoft.com/

