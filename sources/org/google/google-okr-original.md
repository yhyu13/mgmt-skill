# Google's OKR Playbook（Google官方OKR指南原文）

> 来源：Google re:Work官方指南 / Google内部OKR指南（经Google许可公开转载）
> 英文原文出处：WhatMatters.com《Google's OKR Playbook》https://www.whatmatters.com/resources/google-okr-playbook
> （该Playbook由John Doerr团队运营的WhatMatters.com发布，内容摘录自Google内部资源，并经Google许可转载）
> 中文翻译参考：掘金 bobjiang《谷歌OKR指导手册(译)》https://juejin.cn/post/6844904134391382030
> 获取日期：2026-07-21
> 语言：英文原文（附关键段落中文翻译）
> 对应蒸馏文件：mgmt-skills/org/google/google-okr.md

---

## Google's OKR Playbook（英文原文）

*Author: Google*

No one has more collective experience in implementing OKRs than Google.

As the company has scaled (and scaled), it has periodically issued OKR guidelines. The following excerpts are drawn mostly from internal sources and reprinted with Google's permission. *(Note: This is Google's approach to OKRs. Your approach may — and should — differ.)*

At Google, we like to think big. We use a process called Objectives and Key Results (OKRs) to help us communicate, measure, and achieve those lofty goals.

Our actions determine Google's future. As we've seen repeatedly — in Search, in Chrome, in Android — a team composed of a few percent of the company's workforce, acting in concert toward an ambitious common goal, can change an entire mature industry in less than two years. Thus it is crucial that as Google employees and managers we make conscious, careful, and informed choices about how we allocate our time and energy — as individuals and as members of teams. OKRs are the manifestation of those careful choices, and the means by which we coordinate the actions of individuals to achieve great collective goals.

### OKR Best Practices: Writing effective OKRs

Poorly done/managed OKRs are a waste of time, an empty management gesture. Well done OKRs are a motivational management tool that helps make it clear to teams what's important, what to optimize, and what tradeoffs to make during their day-to-day work.

Writing good OKRs isn't easy, but it's not impossible, either. Pay attention to the following simple rules:

**Objectives are the "Whats." They:**

- express goals and intents;
- are aggressive yet realistic;
- must be tangible, objective, and unambiguous; should be obvious to a rational observer whether an Objective has been achieved.
- The successful achievement of an Objective must provide clear value for Google.

**Key Results are the "Hows." They:**

- express measurable milestones which, if achieved, will advance Objective(s) in a useful manner to their constituents;
- must describe outcomes, not activities. If your KRs include words like "consult," "help," "analyze," or "participate," they describe activities. Instead, describe the end-use impact of these activities: "publish average and tail latency measurements from six Colossus cells by March 7," rather than "assess Colossus latency";
- must include evidence of completion. This evidence must be available, credible, and easily discoverable. Examples of evidence include change lists, links to docs, notes, and published metrics reports.

### Aligning teams to achieve ambitious goals

#### Cross-team OKRs

Many important projects at Google require contribution from different groups. OKRs are ideally suited to commit to this coordination. Cross-team OKRs should include all the groups who must materially participate in the OKR, and OKRs committing to each group's contribution should appear explicitly in each such group's OKRs. For example, if Ads Development and Ads SRE and Network Deployment must deliver to support a new ads service, then all three teams should have OKRs describing their commitment to deliver their part of the project.

#### Committed vs. aspirational OKRs

OKRs have two variants, and it is important to differentiate between them:

Commitments are OKRs that we agree will be achieved, and we will be willing to adjust schedules and resources to ensure that they are delivered.

- The expected score for a committed OKR is 1.0; a score of less than 1.0 requires explanation for the miss, as it shows errors in planning and/or execution.

By contrast, aspirational OKRs express how we'd like the world to look, even though we have no clear idea how to get there and/or the resources necessary to deliver the OKR.

- Aspirational OKRs have an expected average score of 0.7, with high variance.

### OKR Best Practices: Classic OKR-writing mistakes and traps

**TRAP #1: Failing to differentiate between committed and aspirational OKRs.**

- Marking a committed OKR as aspirational increases the chance of failure. Teams may not take it seriously and may not change their other priorities to focus on delivering the OKR.
- On the other hand, marking an aspirational OKR as committed creates defensiveness in teams who cannot find a way to deliver the OKR, and it invites priority inversion as committed OKRs are de-staffed to focus on the aspirational OKR.

**TRAP #2: Business-as-usual OKRs.**

- OKRs are often written principally based on what the team believes it can achieve without changing anything they're currently doing, as opposed to what the team or its customers really want.

**TRAP #3: Timid aspirational OKRs.**

- Aspirational OKRs very often start from the current state and effectively ask, "What could we do if we had extra staff and got a bit lucky?" An alternative and better approach is to start with, "What could my (or my customers') world look like in several years if we were freed from most constraints?" By definition, you're not going to know how to achieve this state when the OKR is first formulated — that is why it is an aspirational OKR. But without understanding and articulating the desired end state, you guarantee that you are not going to be able to achieve it.
- The litmus test: If you ask your customers what they really want, does your aspirational Objective meet or exceed their request?

**TRAP #4: Sandbagging**

- A team's committed OKRs should credibly consume most — but not all — of their available resources. Their committed and aspirational OKRs should credibly consume somewhat more than their available resources. (Otherwise they're effectively commits.)
- Teams who can meet all of their OKRs without needing all of their team's headcount/capital… are assumed to either be hoarding resources or not pushing their teams, or both. This is a cue for senior management to reassign headcount and other resources to groups who will make more effective use of them.

**TRAP #5: Low Value Objectives (aka the "Who cares?" OKR).**

OKRs must promise clear business value — otherwise, there's no reason to expend resources doing them. Low Value Objectives (LVOs) are those for which, even if the Objective is completed with a 1.0, no one will notice or care.

- A classic (and seductive) LVO example: "Increase task CPU utilization by 3 percent." This Objective by itself does not help users or Google directly. However, the (presumably related) goal, "Decrease quantity of cores required to serve peak queries by 3 percent with no change to quality/latency/… and return resulting excess cores to the free pool" has clear economic value. That's a superior Objective.
- Here is a litmus test: Could the OKR get a 1.0 under reasonable circumstances — without providing direct enduser or economic benefit? If so, then reword the OKR to focus on the tangible benefit. A classic example: "Launch X," with no criteria for success. Better: "Double fleet-wide Y by launching X to 90+ percent of borg cells."

**TRAP #6: Insufficient KRs for committed Os.**

- OKRs are divided into the desired outcome (the Objective) and the measurable steps required to achieve that outcome (the Key Results). It is critical that KRs are written such that scoring 1.0 on all Key Results generates a 1.0 score for the Objective.
- A common error is writing Key Results that are necessary but not sufficient to collectively complete the Objective. The error is tempting because it allows a team to avoid the difficult (resource/priority/risk) commitments needed to deliver "hard" Key Results.
- This trap is particularly pernicious because it delays both the discovery of the resource requirements for the Objective, and the discovery that the Objective will not be completed on schedule.
- The litmus test: Is it reasonably possible to score 1.0 on all the Key Results, but still not achieve the intent of the Objective? If so, add or rework the Key Results until their successful completion guarantees that the Objective is also successfully completed.

### Reading, interpreting, and acting on OKRs

**For committed OKRs**

- Teams are expected to rearrange their other priorities to ensure an on-schedule 1.0 delivery.
- Teams who cannot credibly promise to deliver a 1.0 on a committed OKR must escalate promptly. This is a key point: Escalating in this (common) situation is not only okay, it is required. Whether the issue arose because of disagreement about the OKR, disagreement about its priority, or inability to allocate enough time/people/resources, escalation is good. It allows the team's management to develop options and resolve conflicts.
- The corollary is that every new OKR is likely to involve some amount of escalation, since it requires a change to existing priorities and commitments. An OKR that requires no changes to any group's activities is a business-as-usual OKR, and those are unlikely to be new — although they may not have previously been written down.
- A committed OKR that fails to achieve a 1.0 by its due date requires a postmortem. This is not intended to punish teams. It is intended to understand what occurred in the planning and/or execution of the OKR, so that teams may improve their ability to reliably hit 1.0 on committed OKRs.
- Examples of classes of committed OKRs are ensuring that a service meets its SLA (service level agreement) for the quarter; or delivering a defined feature or improvement to an infrastructure system by a set date; or manufacturing and delivering a quantity of servers at a cost point.

**For Aspirational OKRs**

- The set of aspirational OKRs will by design exceed the team's ability to execute in a given quarter. The OKRs' priority should inform team members' decisions on where to spend the remaining time they have after the group's commitments are met. In general, higher priority OKRs should be completed before lower priority OKRs.
- Aspirational OKRs and their associated priorities should remain on a team's OKR list until they are completed, carrying them forward from quarter to quarter as necessary. Dropping them from the OKR list because of lack of progress is a mistake, as it disguises persistent problems of prioritization, resource availability, or a lack of understanding of the problem/solution.
- Corollary: It is good to move an aspirational OKR to a different team's list if that team has both the expertise and bandwidth to accomplish the OKR more effectively than the current OKR owner.
- Team managers are expected to assess the resources required to accomplish their aspirational OKRs and ask for them each quarter, fulfilling their duty to express known demand to the business. Managers should not expect to receive all the required resources, however, unless their aspirational OKRs are the highest priority goals in the company after the committed OKRs.

### More Litmus Tests

Some simple tests to see if your OKRs are good:

- If you wrote them down in five minutes, they probably aren't good. Think.
- If your Objective doesn't fit on one line, it probably isn't crisp enough.
- If your KRs are expressed in team-internal terms ("Launch Foo 4.1"), they probably aren't good. What matters isn't the launch, but its impact. Why is Foo 4.1 important? Better: "Launch Foo 4.1 to improve sign-ups by 25 percent." Or simply: "Improve sign-ups by 25 percent."
- Use real dates. If every Key Result happens on the last day of the quarter, you likely don't have a real plan.
- Make sure your Key Results are measurable: It must be possible to objectively assign a grade at the end of the quarter. "Improve sign-ups" isn't a good Key Result. Better: "Improve daily sign-ups by 25 percent by May 1."
- Make sure the metrics are unambiguous. If you say "1 million users," is that all-time users or seven-day actives?
- If there are important activities on your team (or a significant fraction of its effort) that aren't covered by OKRs, add more.
- For larger groups, make OKRs hierarchical — have high-level OKRs for the entire team, more detailed ones for subteams. Make sure that the "horizontal" OKRs (projects that need multiple teams to contribute) have supporting Key Results in each subteam.

---

## 附：Google OKR评分色阶（中文）

Google用色阶来衡量OKR完成度：

- 0.0 – 0.3 红色
- 0.4 – 0.6 黄色
- 0.7 – 1.0 绿色

指令性OKR（Committed OKR）目标分数为1.0；挑战性OKR（Aspirational OKR）目标分数为0.7。

---

> 本文件为Google官方OKR指南公开转载原文（经Google许可，由WhatMatters.com发布），属公开文档，非书籍全文。
