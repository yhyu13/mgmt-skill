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
