# Amazon逆向工作法（Working Backwards）/ 6页纸备忘录——公开原文汇编

> 来源：Amazon公开方法论介绍（Ian McAllister公开Quora回答 + Amazon官方博客 / Werner Vogels "All Things Distributed" 博客 + 贝佐斯2008致股东信）
> 获取日期：2026-07-21
> 语言：中文/英文
> 对应蒸馏文件：mgmt-skills/org/amazon/amazon-working-backwards.md
> 注：Working Backwards书籍（《Working Backwards》, Colin Bryar & Bill Carr, 2021）有版权不补，此处仅存公开方法论介绍（Werner Vogels 2006年官方博客原文 + 贝佐斯2008股东信 + Ian McAllister公开描述）

---

## 说明

Amazon"逆向工作法"（Working Backwards）的核心是：**从客户出发，倒推工作**——先写产品发布时的新闻稿（Press Release）和常见问题（FAQ），通过反复迭代这些文档来验证产品对客户的价值，故事说得通才写第一行代码。

该方法论没有一本"官方原版书"作为唯一权威来源（Bryar & Carr 2021年出版的《Working Backwards》是事后总结的付费书籍，有版权不补）。其权威性来自三个层级的公开来源：

1. **Amazon CTO Werner Vogels 2006年官方博客原文**（All Things Distributed，最早公开介绍Working Backwards流程的官方文章）
2. **贝佐斯2008年致股东信**（在公开股东信中正式阐述"逆向工作法"vs"技能导向法"）
3. **Ian McAllister（前Amazon产品总经理）公开Quora/LinkedIn回答**（详细描述PR/FAQ四步流程及模板）

本文档汇编以上三个层级的公开原文。

---

## 一、Werner Vogels 2006年官方博客原文（英文原文 + 中文翻译）

> 来源：Werner Vogels（Amazon CTO）个人博客 All Things Distributed
> 原文链接：https://www.allthingsdistributed.com/2006/11/working_backwards.html
> 发表日期：2006-11-01
> 说明：这是Amazon官方人士最早在公开场合系统介绍Working Backwards流程的原文

### 英文原文

**Working Backwards**

November 01, 2006

In the fine grained services approach that we use at Amazon, services do not only represent a software structure but also the organizational structure. The services have a strong ownership model, which combined with the small team size is intended to make it very easy to innovate. In some sense you can see these services as small startups within the walls of a bigger company. Each of these services require a strong focus on who their customers are, regardless whether they are externally or internally. To ensure that a service meets the needs of the customer (and not more than that) we use a process called "*Working Backwards*" in which you start with your customer and work your way backwards until you get to the minimum set of technology requirements to satisfy what you try to achieve. The goal is to drive simplicity through a continuous, explicit customer focus.

The product definition process works backwards in the following way: we start by writing the documents we'll need at launch (the press release and the faq) and then work towards documents that are closer to the implementation.

The Working Backwards product definition process is all about is fleshing out the concept and achieving clarity of thought about what we will ultimately go off and build. It typically has four steps:

1. **Start by writing the Press Release.** Nail it. The press release describes in a simple way what the product does and why it exists - what are the features and benefits. It needs to be very clear and to the point. Writing a press release up front clarifies how the world will see the product - not just how we think about it internally.

2. **Write a Frequently Asked Questions document.** Here's where we add meat to the skeleton provided by the press release. It includes questions that came up when we wrote the press release. You would include questions that other folks asked when you shared the press release and you include questions that define what the product is good for. You put yourself in the shoes of someone using the product and consider all the questions you would have.

3. **Define the customer experience.** Describe in precise detail the customer experience for the different things a customer might do with the product. For products with a user interface, we would build mock ups of each screen that the customer uses. For web services, we write use cases, including code snippets, which describe ways you can imagine people using the product. The goal here is to tell stories of how a customer is solving their problems using the product.

4. **Write the User Manual.** The user manual is what a customer will use to really find out about what the product is and how they will use it. The user manual typically has three sections, concepts, how-to, and reference, which between them tell the customer everything they need to know to use the product. For products with more than one kind of user, we write more than one user manual.

Once we have gone through the process of creating the press release, faq, mockups, and user manuals, it is amazing how much clearer it is what you are planning to build. We'll have a suite of documents that we can use to explain the new product to other teams within Amazon. We know at that point that the whole team has a shared vision on what product we are going the build.

### 中文翻译

**逆向工作法**

2006年11月1日

在Amazon使用的细粒度服务方法中，服务不仅代表软件结构，也代表组织结构。服务有很强的所有权模型，结合小团队规模，旨在使创新变得非常容易。在某种意义上，你可以把这些服务看作大公司围墙内的小型创业公司。每个服务都需要高度关注其客户是谁，无论他们是外部的还是内部的。为了确保服务满足客户的需求（且不超过这个范围），我们使用一个叫做"**逆向工作法**"的流程——你从客户出发，向后倒推，直到得到满足你试图实现目标的最小技术需求集合。目标是通过持续、明确的客户关注来驱动简洁。

产品定义流程以如下方式逆向工作：我们从撰写发布时需要的文档（新闻稿和FAQ）开始，然后逐步向更接近实现的文档推进。

逆向工作法产品定义流程的核心是充实概念，并对于我们最终要构建的东西达成清晰的思考。它通常包含四个步骤：

1. **从撰写新闻稿开始。** 把它写好。新闻稿以简单的方式描述产品做什么以及为什么存在——即功能和好处。它需要非常清晰、直击要点。预先写新闻稿可以澄清世界将如何看待这个产品——而不仅仅是我们内部如何看待它。

2. **撰写常见问题文档（FAQ）。** 这里我们为新闻稿提供的骨架添加血肉。它包括写新闻稿时出现的问题。你还会包括分享新闻稿时其他人提出的问题，以及定义产品适用场景的问题。你把自己放在使用产品的人的位置上，考虑你会有的一切问题。

3. **定义客户体验。** 精确描述客户对产品可能做的不同事情的体验。对于有用户界面的产品，我们会构建客户使用的每个屏幕的模型。对于Web服务，我们编写用例，包括代码片段，描述你能想象人们使用产品的方式。这里的目标是讲述客户如何使用产品解决问题的故事。

4. **编写用户手册。** 用户手册是客户真正用来了解产品是什么以及如何使用它的。用户手册通常有三个部分：概念、操作方法和参考，它们共同告诉客户使用产品需要知道的一切。对于有不止一种用户的产品，我们编写不止一本用户手册。

一旦我们完成了创建新闻稿、FAQ、模型和用户手册的过程，我们要构建的东西变得清晰得多，这令人惊叹。我们将拥有一套文档，可以用它向Amazon内部其他团队解释新产品。在那一刻，我们知道整个团队对我们将要构建的产品有了共同愿景。

---

## 二、贝佐斯2008年致股东信中关于"逆向工作法"的公开原文

> 来源：Amazon 2008年致股东信（公开SEC文件）
> 说明：贝佐斯在2008年股东信中正式阐述"逆向工作法"（Working backwards）与"技能导向法"（skills-forward）的对比

### 中文原文（公开翻译版）

> 在此全球经济动荡之际，我们所秉持的基本做法依然未有改变。谦虚谨慎，关注长远价值，顾客至上。关注长远价值，不仅能够促使我们提升现有的能力，并激励我们尝试新鲜事物。它使我们从反复失败中实现创新，它使我们挣脱束缚，去探索未知领域。若仅仅满足于短期内的成就感，或做出短期内的承诺，将很快被超越。然而，长期发展策略则可以与顾客至上的理念相得益彰。如果我们能够很好地了解顾客需求，并深信这种需求是有价值的，并且是长期的，那么我们的一贯做法是，多年的耐心探索，直至找到解决方案。
>
> 可以将依从顾客需求出发的"逆向工作法"（"Working backwards"）与"技能导向法"（"skills-forward"）形成鲜明对比。"技能导向法"使用现有技术和能力来驾驭商机。"技能导向"论者称："我们擅长做X"、"通过X我们还能做什么？"这确是一种有用并且一定程度上奏效的商业模式。但是，如果公司沉浸于此，就会丧失研发创新的动力。最终，现有的技能将成为昨日黄花。从顾客需求出发的"逆向工作法"，往往要求我们必须探索新技能并加以磨练，而不在乎迈出第一步时的那种不适与尴尬。

### 核心论点提炼

- **逆向工作法**：从顾客需求出发 → 倒推所需技能 → 探索新技能
- **技能导向法**：从现有技能出发 → 寻找可驾驭的商机 → 舒适但易丧失创新动力
- 贝佐斯的判断：沉浸于技能导向会丧失创新动力，逆向工作法虽不适但是长期创新之源

---

## 三、Ian McAllister公开描述的PR/FAQ流程与模板

> 来源：Ian McAllister（时任Amazon产品总经理，现任Airloom AI创始人兼CEO）公开Quora回答及LinkedIn文章
> 说明：Ian McAllister在Amazon任职十余年，创建并领导Amazon Smile，其公开Quora回答是Amazon逆向工作法流程最广泛被引用的公开介绍

### 3.1 流程总述（Ian McAllister公开描述）

**从撰写新闻稿开始。** 新闻稿以简单的方式描述了该产品的功能和存在原因，即功能和优点。它需要非常突出重点。预先写一篇新闻稿来澄清用户将如何看待产品——而不仅仅是我们如何看待产品。

**撰写FAQ。** 通过记录撰写新闻稿时想到的问题来丰富新闻稿的内容。你需要将产品的优点、别人可能提出的疑问都写进来。你将自己置身于使用该产品的角度，考虑所有你会遇到的问题。

**定义客户体验。** 详细描述客户可能会怎么用这个产品。对于具有用户界面的产品，我们会构建客户使用的每个界面的Demo。对于Web服务，我们编写用例，包括代码片段，这些代码片段描述了人们使用产品的情景。这个阶段的目标是讲述客户如何使用产品解决需求。

**编写用户手册。** 用户手册是客户用来真正了解产品是什么以及如何使用它的。用户手册通常包含三个部分：概念、操作方法和参考。手册告诉客户使用产品时他们需要知道的一切。对于具有多种用户角色的产品，我们编写多个用户角色手册。

一旦我们完成了上述内容，那么整个产品设计会变得非常清晰。我们可以使用这些文件向公司内的其他团队解释新产品。同时也让整个团队对我们正在构建的产品有着共同的愿景。

### 3.2 撰写新闻稿前的5个基础问题

在开始前，请回答下列五个基础问题，这些问题的明确答案将帮助你入门并阐明产品设计的想法：

1. 谁是你的客户？（Who is your customer?）
2. 客户的问题和当前产品的机遇是什么？（What is the customer problem or opportunity?）
3. 最重要的客户利益是什么？（What is the most important customer benefit?）
4. 你如何知道客户的需求或者期待？（How do you know what your customer needs or wants?）
5. 客户体验是什么样的？（What does the experience look like?）

### 3.3 新闻稿撰写注意事项

- 它是一篇一页叙述，不要把它写成说明书，请删掉多余的部分
- 想象你的客户阅读新闻稿的场景，选择客户能理解的词
- 与其从产品或技术入手，不如着眼于客户体验，描述它将如何使客户受益并解决客户的问题
- 避免使用比较含糊的词汇（如简单、容易、快速），对于重要的指标和数据（如时间、金钱）做到具体化
- 将最重要的信息放在首位，没有人会不读第一段
- 讲一个引人入胜的故事

### 3.4 Amazon推荐的新闻稿模板（7个组成部分）

| # | 组成部分 | 说明 |
|---|---------|------|
| 1 | **标题（Heading）** | 简短、引人注目的描述（最后写标题）。以读者（即目标客户）会理解的方式命名产品。描述产品（或服务）的市场是谁，以及他们会从中获得什么好处 |
| 2 | **摘要（Summary）** | 对产品（或服务）和收益做摘要介绍。这段内容需要高度概括，让读者不再继续阅读更多内容也能知道产品的情况。在Amazon，这部分会列出将来的发布日期（例如2021年11月11日），让读者知道它尚未发布，并设定了对发布的预期 |
| 3 | **挑战或问题（Problem）** | 要以客户为中心。描述面对的挑战或需要解决的问题 |
| 4 | **解决方案（Solution）** | 描述您的产品（或服务）如何使客户受益或优雅地解决客户的问题 |
| 5 | **引述公司中一位Leader对你的支持（Quote by leader in your company）** | 从Leader那里获得真实引述，以证明他对你的想法的支持。Leader的引述应传达新闻稿中所述的"客户利益和经验" |
| 6 | **如何入门（How to get started）** | 告诉用户入门很容易。你的目标是激励读者去尝试 |
| 7 | **客户引述（Customer quote）** | 提供来自假定客户的描述，例如他们是如何获得收益的 |

（部分版本还包含第8部分"号召行动"：总结一下，并指示读者下一步应该如何做）

### 3.5 FAQ编制要点

FAQ以新闻稿为基础，帮助你预测客户和干系人可能遇到的重要问题。它是一种帮助你了解细节并回复假设的工具。常见问题中需要包含两个单独的部分：**客户常见问题解答**和**干系人常见问题解答**。

创建常见问题的技巧：
1. 将最常见的问题放在顶部
2. 回答客户常见问题就像你在与他谈话一样
3. 询问基本问题（谁？什么？哪里？何时？如何？为什么？）

**客户常见问题必备问题：**
1. 我是怎么找到这个的？我该如何开始？
2. 如果遇到问题，我该如何获得帮助？
3. 在我的移动设备上的体验是什么？
4. 为什么我会为此感到兴奋？

**干系人常见问题必备问题：**
1. 如何提高客户体验的标准？
2. 为什么目前这个客户问题/机遇很重要？
3. 您成功的方法是什么？
4. 为什么我们的客户喜欢这种产品？

---

## 四、6页纸备忘录机制（公开资料汇编）

> 来源：Amazon公开实践 + 贝佐斯公开股东信
> 说明：6页纸备忘录是Amazon决策沟通的标准格式，PR/FAQ是其在产品开发场景下的具体形态

### 4.1 6页纸备忘录的起源

2004年，贝佐斯在Amazon高管会议上禁止使用PowerPoint。他要求所有提案必须以6页纸叙述体备忘录的形式提交——会议开始时所有人默读备忘录，然后进行讨论。这一机制与Working Backwards的PR/FAQ文档一脉相承：都强调叙述体思考、完整逻辑链、可独立阅读。

### 4.2 6页纸备忘录的核心要求（公开资料）

- **叙述体写作**：不是碎片化的bullet point，而是完整的叙事
- **完整逻辑链**：从问题到方案到执行，逻辑必须连贯，不能跳跃
- **可独立阅读**：文档不依赖口头讲解，读者独立阅读就能理解
- **长度限制**：通常不超过6页（PR+FAQ），可在附录中添加支撑数据

### 4.3 PR/FAQ与6页纸备忘录的关系

PR/FAQ是6页纸备忘录在产品开发场景下的具体形态：
- 继承6页纸的核心：叙述体（非碎片）、完整逻辑链（非跳跃）、可独立阅读（非依赖口述）
- 在6页纸基础上增加产品开发特有的结构：PR部分面向客户叙事，FAQ部分面向内部质疑
- 新闻稿 + FAQ文档最好不要超过6页，可以在附录中添加其他的支撑数据/信息

### 4.4 注意事项（公开实践）

- 不要花太多时间去完善新闻稿/FAQ文档的早期版本
- 这是一个反复的过程，可能需要多个版本的新闻稿/FAQ以及不同级别Leader的多轮审核
- 在新闻稿/FAQ上进行迭代比在产品本身上进行迭代要便宜得多（而且更快）
- 邀请相关团队和所有干系人参加评审会以获得更加全面的反馈；把新闻稿/FAQ评审会作为良好的沟通/合作机会

---

## 五、来源链接

1. **Werner Vogels 2006年官方博客原文**（Amazon CTO的All Things Distributed博客，最早公开介绍Working Backwards四步流程）https://www.allthingsdistributed.com/2006/11/working_backwards.html
2. **贝佐斯2008年致股东信**（SEC公开文件，正式阐述"逆向工作法"vs"技能导向法"）https://www.aboutamazon.com/news/company-news/2008-letter-to-shareholders
3. **Ian McAllister公开Quora回答**（时任Amazon产品总经理，详细描述PR/FAQ四步流程及模板，被多个公开来源广泛引用）
4. **可可链《产品设计方法论：Amazon逆向工作法》**（转载Ian McAllister的公开描述，含完整PR模板和FAQ要点）https://www.onekbit.com/ViewBlog/blog/BID20200812100499

---

> 注：Working Backwards方法论的核心公开来源是Werner Vogels 2006年官方博客 + 贝佐斯2008股东信 + Ian McAllister公开Quora回答。Bryar & Carr 2021年出版的《Working Backwards》书籍有版权不补。本文件按"关键公开段落+来源链接"规范收录三个层级的公开原文，符合原文层"存公开原文不存付费书籍全文"的版权要求。
