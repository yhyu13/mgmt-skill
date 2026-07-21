# sources/ 原文层索引

> mgmt-skill 原文层：存权威原文，非蒸馏解读
> 创建：2026-07-21
> 规范来源：wiki/知识库建设规范.md

## 目录结构

```
sources/
├── org/                    # 组织来源
│   ├── amazon/             # Amazon
│   ├── netflix/            # Netflix
│   ├── huawei/             # 华为
│   ├── bytedance/          # 字节跳动
│   ├── alibaba/            # 阿里巴巴
│   ├── google/             # Google
│   ├── apple/              # Apple
│   ├── tesla/              # Tesla
│   ├── toyota/             # 丰田
│   ├── bridgewater/        # Bridgewater
│   └── ...
├── individual/             # 个人来源
│   ├── drucker/            # 德鲁克
│   ├── dalio/              # 达利欧
│   ├── christensen/        # 克里斯坦森
│   └── ...
└── book/                   # 书籍来源
```

## 原文层规范

1. **每个原文文件头部必须标注**：来源URL、获取日期、语言、对应蒸馏文件路径
2. **存原文不存解读**：原文层放权威原文，蒸馏层放结构化解读
3. **精选不堆砌**：每个方法论至少1个权威原文来源，不追求数量
4. **中英文优先英文**：能获取英文原文的优先存英文，中文翻译版标注来源

## 已补原文清单

| # | 来源 | 方法论 | 文件 | 语言 | 获取日期 |
|---|------|--------|------|------|---------|
| 1 | Amazon | 领导力原则（16条） | org/amazon/amazon-leadership-principles-original.md | 英文 | 2026-07-21 |
| 2 | Amazon | 贝佐斯1997股东信 | org/amazon/bezos-1997-shareholder-letter.md | 中文翻译 | 2026-07-21 |
| 3 | 华为 | 基本法（第一、二章） | org/huawei/huawei-basiclaw-original.md | 中文原文 | 2026-07-21 |
| 4 | Amazon | Day 1理念（贝佐斯2016股东信） | org/amazon/bezos-2016-day1.md | 中文翻译 | 2026-07-21 |
| 5 | Amazon | 两个披萨团队 | org/amazon/amazon-two-pizza.md | 中文+英文原话 | 2026-07-21 |
| 6 | Google | OKR（官方Playbook） | org/google/google-okr-original.md | 英文原文 | 2026-07-21 |
| 7 | 阿里巴巴 | 新六脉神剑/价值观 | org/alibaba/alibaba-values-original.md | 中文 | 2026-07-21 |
| 8 | 华为 | 基本法（第三-六章） | org/huawei/huawei-basiclaw-part2.md | 中文原文 | 2026-07-21 |
| 9 | Netflix | 文化：自由与责任 | org/netflix/netflix-culture-original.md | 中英文对照 | 2026-07-21 |
| 10 | 丰田 | 丰田之道（Toyota Way 2001） | org/toyota/toyota-way-original.md | 中文 | 2026-07-21 |
| 11 | 字节跳动 | Context, Not Control | org/bytedance/zhangyiming-context-not-control.md | 中文原文 | 2026-07-21 |
| 12 | 海底捞 | 服务管理（张勇公开演讲原话） | org/haidilao/haidilao-service-original.md | 中文 | 2026-07-21 |
| 13 | 胖东来 | 经营理念（于东来虎嗅访谈实录） | org/pangdonglai/pdl-philosophy-original.md | 中文 | 2026-07-21 |
| 14 | 美团 | 王慧文方法论（清华产品课实录） | org/meituan/meituan-wanghuiwen-original.md | 中文 | 2026-07-21 |
| 15 | Amazon | 逆向工作法/6页纸备忘录 | org/amazon/amazon-working-backwards.md | 中文+英文原文 | 2026-07-21 |
| 16 | Google | Aristotle项目（团队有效性） | org/google/google-aristotle-original.md | 中文+英文原文 | 2026-07-21 |

## 待补原文优先级清单

> **版权规则**：书籍全文有版权不补（标记❌）；官方公开文档/股东信/公开演讲/公开采访无版权问题，补齐（标记✅或⬜待补）

### P0 最优先

| # | 来源 | 方法论 | 原文来源类型 | 备注 |
|---|------|--------|------------|------|
| ✅ | Amazon | 领导力原则 | 官方页面 | 已补 |
| ✅ | Amazon | 贝佐斯1997股东信 | SEC 10-K | 已补 |
| ✅ | Netflix | 文化自由与责任 | 官方PPT | 已补（中英文对照版，含9价值观+7文化方面完整内容） |
| ✅ | 华为 | 基本法 | 公开文件 | 已补（第一二章 original + 第三-六章 part2，第1-103条全） |
| ✅ | 字节跳动 | Context, Not Control | 张一鸣公开演讲 | 已补（完整全文，含5大好处+3个Control场景+5个实践） |
| ✅ | 丰田 | 丰田之道 | 官方文件 | 已补（Toyota Way 2001，含两大支柱+五项原则+TBP十大意识+八步骤） |
| ✅ | Amazon | 逆向工作法/6页纸 | 公开博客/方法论 | 已补（Werner Vogels 2006官方博客原文 + 贝佐斯2008股东信 + Ian McAllister公开Quora回答，含PR/FAQ四步流程+模板+6页纸机制） |
| ❌ | Bridgewater/达利欧 | 原则 | 书籍 | **有版权不补**（《原则》为付费书籍） |

### P1 重要

| # | 来源 | 方法论 | 原文来源类型 | 备注 |
|---|------|--------|------------|------|
| ✅ | Amazon | Day 1理念 | 贝佐斯2016股东信 | 已补 |
| ✅ | Amazon | 两个披萨团队 | 公开采访 | 已补 |
| ✅ | Google | OKR | 官方re:Work指南 | 已补 |
| ✅ | Google | Aristotle项目 | 官方re:Work | 已补（re:Work官方指南 + 纽约时报2016深度报道原文 + Amy Edmondson心理安全学术原文，含五要素+心理安全定义+实践案例） |
| ✅ | 阿里巴巴 | 六脉神剑/价值观 | 官方文件 | 已补 |
| ✅ | 海底捞 | 服务管理 | 公开采访/报道 | 已补（张勇公开演讲原话汇编，含KPI反思/计件工资/员工授权免单权/待遇尊重承诺/嫁妆制度/善良） |
| ✅ | 胖东来 | 经营理念 | 公开采访/报道 | 已补（于东来虎嗅2024-12-13闭门会三小时访谈实录，含自由与爱/利润分享/员工尊严/利益排序/不上市/健康管理） |
| ✅ | Netflix | Context not Control | 文化文档 | 已覆盖（在Netflix文化文档原文中完整收录） |
| ✅ | 美团 | 王慧文方法论 | 公开演讲 | 已补（王慧文2020-09-25清华产品课实录，含规模效应/马太效应/战略选择/市场体量/市场集中度/业务认知四步法） |
| ❌ | 麦肯锡 | MECE/金字塔原理 | 书籍 | **有版权不补**（《金字塔原理》为付费书籍） |
| ❌ | 德鲁克 | 卓有成效的管理者 | 书籍 | **有版权不补** |
| ❌ | 稻盛和夫 | 阿米巴/经营原则 | 书籍 | **有版权不补** |
| ❌ | 克里斯坦森 | 颠覆式创新 | 书籍/论文 | **有版权不补** |

### P2 书籍类（全部有版权，不补）

| # | 来源 | 方法论 | 状态 |
|---|------|--------|------|
| ❌ | 彼得·蒂尔 | 从0到1 | **有版权不补** |
| ❌ | 吉姆·柯林斯 | 飞轮/第五级领导力 | **有版权不补** |
| ❌ | 塔勒布 | 黑天鹅 | **有版权不补** |
| ❌ | 凯文·凯利 | 必然 | **有版权不补** |
| ❌ | 菲利普·科特勒 | 营销管理 | **有版权不补** |

## 持续补充机制

- 每次对话可补2-3个原文
- 优先补 P0，再 P1，最后 P2
- 补完后在此清单标记 ✅
- 原文层与蒸馏层双向引用：原文头部标注对应蒸馏文件，蒸馏文件底部标注原文来源
