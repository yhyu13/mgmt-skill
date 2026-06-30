# org-skill

> 蒸馏标杆企业管理方法论 → 知识库 + 可交互工具，开源到 GitHub

## 这是什么

org-skill 把世界顶级企业的管理方法论蒸馏成结构化的知识库文件（ORG-SKILL.md），让 AI 和人都能调用。

**与女娲(nuwa-skill)的区别**：女娲蒸馏**个人**的思维模型 → 输出 SKILL.md（你读它），org-skill 蒸馏**组织**的管理方法论 → 输出 ORG-SKILL.md + 可交互工具（你用它）。

## 项目结构

```
org-skill/
├── org-skills/           # 知识库（CC BY-NC 4.0）
│   └── huawei/           # 华为管理方法论
│       ├── huawei-dste.md
│       ├── huawei-blm.md
│       ├── huawei-bem.md
│       ├── huawei-ipd.md
│       ├── huawei-mtl.md
│       ├── huawei-ltc.md
│       ├── huawei-itr.md
│       ├── huawei-isc.md
│       ├── huawei-pbc.md
│       ├── huawei-cadre.md
│       ├── huawei-incentive.md
│       ├── huawei-entropy.md
│       └── huawei-basiclaw.md
│   └── bytedance/        # 字节跳动管理方法论
│       ├── bytedance-cnc.md
│       ├── bytedance-okr.md
│       ├── bytedance-platform.md
│       ├── bytedance-talent.md
│       ├── bytedance-feishu.md
│       ├── bytedance-culture.md
│       ├── bytedance-race.md
│       ├── bytedance-abtest.md
│       ├── bytedance-compensation.md
│       ├── bytedance-growth.md
│       ├── bytedance-global.md
│       └── bytedance-philosophy.md
│   └── toyota/           # 丰田管理方法论
│       ├── toyota-way.md
│       ├── toyota-tps.md
│       ├── toyota-5s.md
│       ├── toyota-kanban.md
│       ├── toyota-a3.md
│       ├── toyota-5why.md
│       ├── toyota-andon.md
│       ├── toyota-kaizen.md
│       ├── toyota-people.md
│       └── toyota-vsm.md
│   └── netflix/          # Netflix管理方法论
│       ├── netflix-culture.md
│       ├── netflix-talent-density.md
│       ├── netflix-candor.md
│       ├── netflix-context-not-control.md
│       ├── netflix-informed-captain.md
│       ├── netflix-aligned-coupled.md
│       ├── netflix-minimal-rules.md
│       └── netflix-compensation.md
│   └── amazon/           # Amazon管理方法论
│       ├── amazon-day1.md
│       ├── amazon-leadership-principles.md
│       ├── amazon-working-backwards.md
│       ├── amazon-six-page.md
│       ├── amazon-bar-raiser.md
│       ├── amazon-single-threaded.md
│       ├── amazon-two-pizza.md
│       ├── amazon-op1-op2.md
│       ├── amazon-andon-cord.md
│       └── amazon-reversible-decisions.md
│   └── google/           # Google管理方法论
│       ├── google-data-driven.md
│       ├── google-okr.md
│       ├── google-oxygen.md
│       ├── google-aristotle.md
│       ├── google-innovation-time.md
│       ├── google-hiring.md
│       ├── google-tgif.md
│       └── google-10x.md
│   └── alibaba/         # 阿里巴巴管理方法论
│       ├── alibaba-values.md
│       ├── alibaba-hrbp.md
│       ├── alibaba-three-axes.md
│       ├── alibaba-performance.md
│       ├── alibaba-partnership.md
│       ├── alibaba-middle-office.md
│       ├── alibaba-iron-army.md
│       └── alibaba-talent-grid.md
│   └── pangdonglai/     # 胖东来管理方法论
│       ├── pdl-freedom-love.md
│       ├── pdl-profit-sharing.md
│       ├── pdl-employee-dignity.md
│       ├── pdl-transparency.md
│       ├── pdl-customer-service.md
│       ├── pdl-restraint.md
│       └── pdl-self-governance.md
├── distill/              # 蒸馏流程和模板（MIT）
│   ├── ORG-SKILL-模板.md
│   └── 蒸馏流程.md
├── tools/                # 可交互工具
│   └── free/             # 基础工具（MIT）
├── LICENSE               # MIT（代码）+ CC BY-NC 4.0（知识库）
└── README.md
```

## 已蒸馏组织

| 组织 | 方法论数 | 状态 |
|------|---------|------|
| 华为 | 12 | ✅ 已完成 |
| 字节跳动 | 12 | ✅ 已完成 |
| 丰田 | 10 | ✅ 已完成 |
| Netflix | 8 | ✅ 已完成 |
| Amazon | 10 | ✅ 已完成 |
| Google | 8 | ✅ 已完成 |
| 阿里巴巴 | 8 | ✅ 已完成 |
| 胖东来 | 7 | ✅ 已完成 |

### 华为管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 战略 | DSTE / BLM / BEM | huawei-dste / blm / bem |
| 研发 | IPD | huawei-ipd |
| 营销 | MTL | huawei-mtl |
| 销售 | LTC | huawei-ltc |
| 服务 | ITR | huawei-itr |
| 供应链 | ISC | huawei-isc |
| 人力 | PBC / 干部管理 / 科学分钱 | huawei-pbc / cadre / incentive |
| 文化 | 熵减 / 华为基本法 | huawei-entropy / basiclaw |

### 字节跳动管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 管理哲学 | Context, not Control | bytedance-cnc |
| 目标管理 | OKR体系 | bytedance-okr |
| 组织架构 | 蜂窝中台+分布式创业网络 | bytedance-platform |
| 人才 | 高人才密度 | bytedance-talent |
| 协作 | 飞书 | bytedance-feishu |
| 文化 | 字节范 | bytedance-culture |
| 创新 | 内部赛马+动态韧性 | bytedance-race |
| 产品 | 数据驱动+A/B测试 | bytedance-abtest |
| 人力 | 绩效薪酬体系 | bytedance-compensation |
| 增长 | 增长中台+算法推荐 | bytedance-growth |
| 国际化 | 本地化运营+双壳架构 | bytedance-global |
| 战略 | 务实浪漫+延迟满足 | bytedance-philosophy |

### Netflix管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 文化 | 自由与责任文化（F&R飞轮） | netflix-culture |
| 人力 | 人才密度（Dream Team + Keeper Test） | netflix-talent-density |
| 文化 | 极致坦诚（4A反馈 + 360度） | netflix-candor |
| 管理 | Context, not Control | netflix-context-not-control |
| 管理 | 知情船长决策模型 | netflix-informed-captain |
| 组织 | 高度一致，松散耦合 | netflix-aligned-coupled |
| 制度 | 极简规则 | netflix-minimal-rules |
| 人力 | 顶薪制 | netflix-compensation |

### Amazon管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 文化 | Day 1文化 | amazon-day1 |
| 文化 | 16条领导力原则 | amazon-leadership-principles |
| 研发 | 逆向工作法（PR/FAQ） | amazon-working-backwards |
| 决策 | 6页纸备忘录 | amazon-six-page |
| 人力 | 抬杆者招聘法（Bar Raiser） | amazon-bar-raiser |
| 组织 | 单线程领导 | amazon-single-threaded |
| 组织 | 两个披萨团队 | amazon-two-pizza |
| 战略 | OP1/OP2年度计划+ST目标 | amazon-op1-op2 |
| 运营 | 安灯绳（Andon Cord） | amazon-andon-cord |
| 决策 | 崇尚行动+可逆决策 | amazon-reversible-decisions |

### Google管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 文化 | 数据驱动文化 | google-data-driven |
| 战略 | OKR目标管理 | google-okr |
| 管理 | Project Oxygen（氧气项目） | google-oxygen |
| 团队 | Project Aristotle（亚里士多德项目） | google-aristotle |
| 创新 | 20%自由时间+70/20/10 | google-innovation-time |
| 人力 | 创意精英招聘法 | google-hiring |
| 沟通 | TGIF+Default Open | google-tgif |
| 创新 | 10x思维 | google-10x |

### 阿里巴巴管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 文化 | 六脉神剑价值观体系 | alibaba-values |
| 人力 | 政委体系（HRBP） | alibaba-hrbp |
| 管理 | 管理三板斧（九板斧） | alibaba-three-axes |
| 考核 | 361绩效双轨制 | alibaba-performance |
| 治理 | 合伙人制度 | alibaba-partnership |
| 组织 | 中台战略 | alibaba-middle-office |
| 执行 | 阿里铁军 | alibaba-iron-army |
| 人才 | 人才盘点九宫格 | alibaba-talent-grid |

### 胖东来管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 文化 | 自由与爱哲学 | pdl-freedom-love |
| 分配 | 极致利润共享 | pdl-profit-sharing |
| 人力 | 极致员工尊严 | pdl-employee-dignity |
| 经营 | 极致透明经营 | pdl-transparency |
| 服务 | 极致顾客服务 | pdl-customer-service |
| 战略 | 反扩张克制 | pdl-restraint |
| 治理 | 员工自治+轮值 | pdl-self-governance |

## 使用方式

### 让 AI 调用

把 ORG-SKILL.md 文件放到你的 AI 工具的知识库目录中，AI 就能基于这些方法论给出建议。

### 自己学习

每个 ORG-SKILL.md 包含：
- 核心理念（这个方法论解决什么问题）
- 框架结构（整体架构图）
- 关键模块（每个模块的定义/输入/输出/关键动作/常见误区）
- 决策启发式（如果X，则Y）
- 与其他方法论的关系
- 适用场景 + 诚实边界

### 使用可交互工具

```bash
# 打开 BEM 战略解码器
open tools/free/bem-decoder.html
```

## 贡献

欢迎贡献新的组织蒸馏！请阅读 [蒸馏流程](distill/蒸馏流程.md) 了解如何蒸馏一个新组织。

## 版权声明

- **代码（tools/ + distill/）**：MIT 协议
- **知识库（org-skills/）**：CC BY-NC 4.0 协议（署名 + 非商用）

所有 ORG-SKILL.md 文件基于公开资料整理，所有方法论版权归原著作权人所有。仅供学习参考，不得用于商业用途。

## 致谢

- [女娲(nuwa-skill)](https://github.com/alchaincyf/nuwa-skill) - SKILL.md 格式灵感来源
