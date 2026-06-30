# mgmt-skill

> 蒸馏管理方法论 → 知识库 + 可交互工具，开源到 GitHub

## 这是什么

mgmt-skill 把世界顶级的管理方法论蒸馏成结构化的知识库文件（MGMT-SKILL.md），让 AI 和人都能调用。

**知识来源有三类**：

| 来源类型 | 说明 | 例子 |
|---------|------|------|
| 组织 | 标杆企业的管理方法论 | 华为DSTE、Netflix自由与责任、胖东来利润共享 |
| 个人（管理者） | 管理大师/企业家的管理思想 | 德鲁克目标管理、韦尔奇领导力 |
| 个人（实践者） | 一线从业者的实战经验 | CMO获客体系、销售VP打法、独立开发者增长方法 |

**与女娲(nuwa-skill)的区别**：女娲蒸馏**怎么想** → 输出 SKILL.md（改变思维），mgmt-skill 蒸馏**怎么做** → 输出 MGMT-SKILL.md + 可交互工具（改变做法）。

**两种切法**：

| 切法 | 说明 | 用户入口 | 目录 |
|------|------|---------|------|
| 纵切 | 按来源（组织/个人） | "我要学华为" | `mgmt-skills/org/huawei/` |
| 横切 | 按管理学科 | "我要学人事管理" | `mgmt-skills/discipline/hr/` |

## 项目结构

```
mgmt-skill/
├── mgmt-skills/              # 知识库（CC BY-NC 4.0）
│   ├── org/                  # 组织纵切
│   │   ├── huawei/           # 华为管理方法论
│   │   │   ├── huawei-dste.md
│   │   │   ├── huawei-blm.md
│   │   │   ├── huawei-bem.md
│   │   │   ├── huawei-ipd.md
│   │   │   ├── huawei-mtl.md
│   │   │   ├── huawei-ltc.md
│   │   │   ├── huawei-itr.md
│   │   │   ├── huawei-isc.md
│   │   │   ├── huawei-pbc.md
│   │   │   ├── huawei-cadre.md
│   │   │   ├── huawei-incentive.md
│   │   │   ├── huawei-entropy.md
│   │   │   └── huawei-basiclaw.md
│   │   ├── bytedance/        # 字节跳动管理方法论
│   │   │   ├── bytedance-cnc.md
│   │   │   ├── bytedance-okr.md
│   │   │   ├── bytedance-platform.md
│   │   │   ├── bytedance-talent.md
│   │   │   ├── bytedance-feishu.md
│   │   │   ├── bytedance-culture.md
│   │   │   ├── bytedance-race.md
│   │   │   ├── bytedance-abtest.md
│   │   │   ├── bytedance-compensation.md
│   │   │   ├── bytedance-growth.md
│   │   │   ├── bytedance-global.md
│   │   │   └── bytedance-philosophy.md
│   │   ├── toyota/           # 丰田管理方法论
│   │   │   ├── toyota-way.md
│   │   │   ├── toyota-tps.md
│   │   │   ├── toyota-5s.md
│   │   │   ├── toyota-kanban.md
│   │   │   ├── toyota-a3.md
│   │   │   ├── toyota-5why.md
│   │   │   ├── toyota-andon.md
│   │   │   ├── toyota-kaizen.md
│   │   │   ├── toyota-people.md
│   │   │   └── toyota-vsm.md
│   │   ├── netflix/          # Netflix管理方法论
│   │   │   ├── netflix-culture.md
│   │   │   ├── netflix-talent-density.md
│   │   │   ├── netflix-candor.md
│   │   │   ├── netflix-context-not-control.md
│   │   │   ├── netflix-informed-captain.md
│   │   │   ├── netflix-aligned-coupled.md
│   │   │   ├── netflix-minimal-rules.md
│   │   │   └── netflix-compensation.md
│   │   ├── amazon/           # Amazon管理方法论
│   │   │   ├── amazon-day1.md
│   │   │   ├── amazon-leadership-principles.md
│   │   │   ├── amazon-working-backwards.md
│   │   │   ├── amazon-six-page.md
│   │   │   ├── amazon-bar-raiser.md
│   │   │   ├── amazon-single-threaded.md
│   │   │   ├── amazon-two-pizza.md
│   │   │   ├── amazon-op1-op2.md
│   │   │   ├── amazon-andon-cord.md
│   │   │   └── amazon-reversible-decisions.md
│   │   ├── google/           # Google管理方法论
│   │   │   ├── google-data-driven.md
│   │   │   ├── google-okr.md
│   │   │   ├── google-oxygen.md
│   │   │   ├── google-aristotle.md
│   │   │   ├── google-innovation-time.md
│   │   │   ├── google-hiring.md
│   │   │   ├── google-tgif.md
│   │   │   └── google-10x.md
│   │   ├── alibaba/         # 阿里巴巴管理方法论
│   │   │   ├── alibaba-values.md
│   │   │   ├── alibaba-hrbp.md
│   │   │   ├── alibaba-three-axes.md
│   │   │   ├── alibaba-performance.md
│   │   │   ├── alibaba-partnership.md
│   │   │   ├── alibaba-middle-office.md
│   │   │   ├── alibaba-iron-army.md
│   │   │   └── alibaba-talent-grid.md
│   │   └── pangdonglai/     # 胖东来管理方法论
│   │       ├── pdl-freedom-love.md
│   │       ├── pdl-profit-sharing.md
│   │       ├── pdl-employee-dignity.md
│   │       ├── pdl-transparency.md
│   │       ├── pdl-customer-service.md
│   │       ├── pdl-restraint.md
│   │       └── pdl-self-governance.md
│   │   ├── apple/           # Apple管理方法论
│   │   │   ├── apple-simplicity.md
│   │   │   ├── apple-functional-org.md
│   │   │   ├── apple-dri.md
│   │   │   ├── apple-design-driven.md
│   │   │   ├── apple-ecosystem.md
│   │   │   ├── apple-supply-chain.md
│   │   │   ├── apple-elite-team.md
│   │   │   └── apple-university.md
│   │   └── meituan/          # 美团管理方法论
│   │       ├── meituan-ground-force.md
│   │       ├── meituan-high-freq.md
│   │       ├── meituan-scientific-ops.md
│   │       ├── meituan-basics.md
│   │       ├── meituan-wanghuiwen.md
│   │       ├── meituan-infinite-game.md
│   │       └── meituan-endgame.md
│   │   ├── xiaomi/           # 小米管理方法论
│   │   │   ├── xiaomi-seven-words.md
│   │   │   ├── xiaomi-hit-product.md
│   │   │   ├── xiaomi-participation.md
│   │   │   ├── xiaomi-flat-org.md
│   │   │   ├── xiaomi-ecosystem.md
│   │   │   ├── xiaomi-ironman.md
│   │   │   └── xiaomi-trend.md
│   │   ├── mckinsey/         # 麦肯锡管理方法论
│   │   │   ├── mckinsey-mece.md
│   │   │   ├── mckinsey-pyramid.md
│   │   │   ├── mckinsey-7s.md
│   │   │   ├── mckinsey-problem-solving.md
│   │   │   ├── mckinsey-up-or-out.md
│   │   │   └── mckinsey-80-20.md
│   │   ├── bridgewater/      # 桥水管理方法论
│   │   │   ├── bridgewater-radical-transparency.md
│   │   │   ├── bridgewater-principles.md
│   │   │   ├── bridgewater-idea-meritocracy.md
│   │   │   ├── bridgewater-believability.md
│   │   │   ├── bridgewater-pain-button.md
│   │   │   └── bridgewater-radical-truth.md
│   │   ├── tencent/          # 腾讯管理方法论
│   │   │   ├── tencent-product-driven.md
│   │   │   ├── tencent-race.md
│   │   │   ├── tencent-agile.md
│   │   │   ├── tencent-ecosystem.md
│   │   │   ├── tencent-user-value.md
│   │   │   └── tencent-investment-strategy.md
│   │   ├── haidilao/         # 海底捞管理方法论
│   │   │   ├── haidilao-master-apprentice.md
│   │   │   ├── haidilao-employee-empowerment.md
│   │   │   ├── haidilao-service-as-management.md
│   │   │   ├── haidilao-hands-change-fate.md
│   │   │   └── haidilao-customer-extreme.md
│   │   └── oppo-vivo/        # OPPO/vivo管理方法论
│   │       ├── oppo-vivo-benfen.md
│   │       ├── oppo-vivo-channel.md
│   │       ├── oppo-vivo-agent-system.md
│   │       ├── oppo-vivo-duan-philosophy.md
│   │       └── oppo-vivo-product-focus.md
│   ├── individual/           # 个人蒸馏（新增）
│   │   └── (待蒸馏)
│   └── discipline/           # 学科横切（新增）
│       └── (待蒸馏)
├── distill/                  # 蒸馏流程和模板（MIT）
│   ├── MGMT-SKILL-模板.md
│   └── 蒸馏流程.md
├── tools/                    # 可交互工具
│   └── free/                 # 基础工具（MIT）
├── LICENSE                   # MIT（代码）+ CC BY-NC 4.0（知识库）
└── README.md
```

## 已蒸馏来源

### 组织纵切

| 组织 | 方法论数 | 状态 |
|------|---------|------|
| 华为 | 13 | ✅ 已完成 |
| 字节跳动 | 12 | ✅ 已完成 |
| 丰田 | 10 | ✅ 已完成 |
| Netflix | 8 | ✅ 已完成 |
| Amazon | 10 | ✅ 已完成 |
| Google | 8 | ✅ 已完成 |
| 阿里巴巴 | 8 | ✅ 已完成 |
| 胖东来 | 7 | ✅ 已完成 |
| Apple | 8 | ✅ 已完成 |
| 美团 | 7 | ✅ 已完成 |
| 小米 | 7 | ✅ 已完成 |
| 麦肯锡 | 6 | ✅ 已完成 |
| 桥水 | 6 | ✅ 已完成 |
| 腾讯 | 6 | ✅ 已完成 |
| 海底捞 | 5 | ✅ 已完成 |
| OPPO/vivo | 5 | ✅ 已完成 |

### 个人蒸馏

| 个人 | 方法论数 | 状态 |
|------|---------|------|
| (待蒸馏) | | |

### 学科横切

| 学科 | 来源数 | 状态 |
|------|--------|------|
| (待蒸馏) | | |

### 华为管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 战略 | DSTE / BLM / BEM | huawei-dste / blm / bem | strategy |
| 研发 | IPD | huawei-ipd | rd |
| 营销 | MTL | huawei-mtl | marketing |
| 销售 | LTC | huawei-ltc | sales |
| 服务 | ITR | huawei-itr | service |
| 供应链 | ISC | huawei-isc | supply-chain |
| 人力 | PBC / 干部管理 / 科学分钱 | huawei-pbc / cadre / incentive | hr |
| 文化 | 熵减 / 华为基本法 | huawei-entropy / basiclaw | culture |

### 字节跳动管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 管理哲学 | Context, not Control | bytedance-cnc | management |
| 目标管理 | OKR体系 | bytedance-okr | strategy |
| 组织架构 | 蜂窝中台+分布式创业网络 | bytedance-platform | org-design |
| 人才 | 高人才密度 | bytedance-talent | hr |
| 协作 | 飞书 | bytedance-feishu | collaboration |
| 文化 | 字节范 | bytedance-culture | culture |
| 创新 | 内部赛马+动态韧性 | bytedance-race | innovation |
| 产品 | 数据驱动+A/B测试 | bytedance-abtest | product |
| 人力 | 绩效薪酬体系 | bytedance-compensation | hr |
| 增长 | 增长中台+算法推荐 | bytedance-growth | marketing |
| 国际化 | 本地化运营+双壳架构 | bytedance-global | strategy |
| 战略 | 务实浪漫+延迟满足 | bytedance-philosophy | strategy |

### Netflix管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 文化 | 自由与责任文化（F&R飞轮） | netflix-culture | culture |
| 人力 | 人才密度（Dream Team + Keeper Test） | netflix-talent-density | hr |
| 文化 | 极致坦诚（4A反馈 + 360度） | netflix-candor | culture |
| 管理 | Context, not Control | netflix-context-not-control | management |
| 管理 | 知情船长决策模型 | netflix-informed-captain | management |
| 组织 | 高度一致，松散耦合 | netflix-aligned-coupled | org-design |
| 制度 | 极简规则 | netflix-minimal-rules | management |
| 人力 | 顶薪制 | netflix-compensation | hr |

### Amazon管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 文化 | Day 1文化 | amazon-day1 | culture |
| 文化 | 16条领导力原则 | amazon-leadership-principles | culture |
| 研发 | 逆向工作法（PR/FAQ） | amazon-working-backwards | rd |
| 决策 | 6页纸备忘录 | amazon-six-page | management |
| 人力 | 抬杆者招聘法（Bar Raiser） | amazon-bar-raiser | hr |
| 组织 | 单线程领导 | amazon-single-threaded | org-design |
| 组织 | 两个披萨团队 | amazon-two-pizza | org-design |
| 战略 | OP1/OP2年度计划+ST目标 | amazon-op1-op2 | strategy |
| 运营 | 安灯绳（Andon Cord） | amazon-andon-cord | service |
| 决策 | 崇尚行动+可逆决策 | amazon-reversible-decisions | management |

### Google管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 文化 | 数据驱动文化 | google-data-driven | culture |
| 战略 | OKR目标管理 | google-okr | strategy |
| 管理 | Project Oxygen（氧气项目） | google-oxygen | management |
| 团队 | Project Aristotle（亚里士多德项目） | google-aristotle | org-design |
| 创新 | 20%自由时间+70/20/10 | google-innovation-time | innovation |
| 人力 | 创意精英招聘法 | google-hiring | hr |
| 沟通 | TGIF+Default Open | google-tgif | culture |
| 创新 | 10x思维 | google-10x | innovation |

### 阿里巴巴管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 文化 | 六脉神剑价值观体系 | alibaba-values | culture |
| 人力 | 政委体系（HRBP） | alibaba-hrbp | hr |
| 管理 | 管理三板斧（九板斧） | alibaba-three-axes | management |
| 考核 | 361绩效双轨制 | alibaba-performance | hr |
| 治理 | 合伙人制度 | alibaba-partnership | org-design |
| 组织 | 中台战略 | alibaba-middle-office | org-design |
| 执行 | 阿里铁军 | alibaba-iron-army | sales |
| 人才 | 人才盘点九宫格 | alibaba-talent-grid | hr |

### 胖东来管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 文化 | 自由与爱哲学 | pdl-freedom-love | culture |
| 分配 | 极致利润共享 | pdl-profit-sharing | hr |
| 人力 | 极致员工尊严 | pdl-employee-dignity | hr |
| 经营 | 极致透明经营 | pdl-transparency | management |
| 服务 | 极致顾客服务 | pdl-customer-service | service |
| 战略 | 反扩张克制 | pdl-restraint | strategy |
| 治理 | 员工自治+轮值 | pdl-self-governance |

### Apple管理方法论全景

| 层级 | 方法论 | 文件 |
|------|--------|------|
| 文化 | 极简哲学 | apple-simplicity |
| 组织 | 职能型组织 | apple-functional-org |
| 管理 | DRI责任制 | apple-dri |
| 研发 | 设计驱动创新 | apple-design-driven |
| 战略 | 生态闭环战略 | apple-ecosystem |
| 运营 | 供应链极致管控 | apple-supply-chain |
| 人力 | 小团队精英制 | apple-elite-team |
| 学习 | Apple University | apple-university |

### 美团管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 销售 | 地推铁军 | meituan-ground-force | sales |
| 战略 | 高频打低频 | meituan-high-freq | strategy |
| 管理 | 科学运营 | meituan-scientific-ops | management |
| 管理 | 苦练基本功 | meituan-basics | management |
| 管理 | 王慧文方法论 | meituan-wanghuiwen | management |
| 战略 | 无限游戏 | meituan-infinite-game | strategy |
| 战略 | 终局思维 | meituan-endgame | strategy |

### 小米管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 管理 | 互联网七字诀 | xiaomi-seven-words | management |
| 产品 | 爆款战略 | xiaomi-hit-product | product |
| 营销 | 参与感 | xiaomi-participation | marketing |
| 组织 | 扁平化组织 | xiaomi-flat-org | org-design |
| 战略 | 生态链模式 | xiaomi-ecosystem | strategy |
| 战略 | 铁人三项 | xiaomi-ironman | strategy |
| 战略 | 顺势而为 | xiaomi-trend | strategy |

### 麦肯锡管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 思维 | MECE原则 | mckinsey-mece | management |
| 表达 | 金字塔原理 | mckinsey-pyramid | management |
| 诊断 | 7S模型 | mckinsey-7s | org-design |
| 方法 | 问题解决法 | mckinsey-problem-solving | management |
| 人力 | Up or Out | mckinsey-up-or-out | hr |
| 方法 | 80/20法则 | mckinsey-80-20 | management |

### 桥水管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 文化 | 极度透明 | bridgewater-radical-transparency | culture |
| 管理 | 原则体系 | bridgewater-principles | management |
| 决策 | 创意择优 | bridgewater-idea-meritocracy | management |
| 决策 | 可信度加权 | bridgewater-believability | management |
| 进化 | 痛苦+反思=进步 | bridgewater-pain-button | culture |
| 文化 | 极度求真 | bridgewater-radical-truth | culture |

### 腾讯管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 产品 | 产品驱动 | tencent-product-driven | product |
| 创新 | 赛马机制 | tencent-race | innovation |
| 组织 | 敏捷组织 | tencent-agile | org-design |
| 战略 | 生态化战略 | tencent-ecosystem | strategy |
| 文化 | 用户价值为本 | tencent-user-value | culture |
| 战略 | 投资赋能战略 | tencent-investment-strategy | strategy |

### 海底捞管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 人力 | 师徒制 | haidilao-master-apprentice | hr |
| 管理 | 员工授权 | haidilao-employee-empowerment | management |
| 服务 | 服务即管理 | haidilao-service-as-management | service |
| 人力 | 双手改变命运 | haidilao-hands-change-fate | hr |
| 服务 | 极致顾客体验 | haidilao-customer-extreme | service |

### OPPO/vivo管理方法论全景

| 层级 | 方法论 | 文件 | 学科标签 |
|------|--------|------|---------|
| 文化 | 本分文化 | oppo-vivo-benfen | culture |
| 销售 | 线下渠道深度绑定 | oppo-vivo-channel | sales |
| 销售 | 代理商体系 | oppo-vivo-agent-system | sales |
| 战略 | 段永平哲学 | oppo-vivo-duan-philosophy | strategy |
| 产品 | 产品聚焦 | oppo-vivo-product-focus | product |

## 使用方式

### 让 AI 调用

把 MGMT-SKILL.md 文件放到你的 AI 工具的知识库目录中，AI 就能基于这些方法论给出建议。

### 自己学习

每个 MGMT-SKILL.md 包含：
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

欢迎贡献新的管理方法论蒸馏！请阅读 [蒸馏流程](distill/蒸馏流程.md) 了解如何蒸馏一个新来源。

## 版权声明

- **代码（tools/ + distill/）**：MIT 协议
- **知识库（mgmt-skills/）**：CC BY-NC 4.0 协议（署名 + 非商用）

所有 MGMT-SKILL.md 文件基于公开资料整理，所有方法论版权归原著作权人所有。仅供学习参考，不得用于商业用途。

## 致谢

- [女娲(nuwa-skill)](https://github.com/alchaincyf/nuwa-skill) - SKILL.md 格式灵感来源
