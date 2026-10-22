# Revisit

**A client retention system for a small private clinic in the Bay Area.**

![Live Demo](https://img.shields.io/badge/Live%20Demo-online-0A6B55?style=flat-square)
![Single File](https://img.shields.io/badge/Build-single%20HTML%20file-555?style=flat-square)
![No Dependencies](https://img.shields.io/badge/Dependencies-none-555?style=flat-square)
![Bilingual](https://img.shields.io/badge/UI-%E4%B8%AD%E6%96%87%20%2F%20English-555?style=flat-square)

**→ Live demo: https://sf-ryanyan.github.io/revisit/**

*Fictional data. Nothing is actually sent.*

**[English](#overview) · [中文](#中文版)**

---

## Overview

Revisit is a working web application built to answer one question a small clinic asks every week: **who should be coming back, and hasn't?**

It is not an EHR and not a practice management system. It sits beside whatever the clinic already runs and handles only the client relationship layer — contact records, appointments, consent, follow-up messages, and the reporting that shows whether any of it worked.

Everything in the demo is clickable. Seven modules, three staff roles, bilingual interface, no account needed.

## The problem

Four things go wrong in almost every small clinic.

**Clients come once and disappear.** The clinic has a records system, but records only store what happened during a visit. Nothing tells the staff that a client hasn't been back in ninety days. Three months later, nobody knows who to follow up with.

**Bookings live in three places.** Phone, website and front desk each keep their own version. Slots get double-booked, notes get lost, no-shows go unanswered.

**Marketing spend cannot be judged.** Ads run and posts go out, but nobody records where each new client came from. So the question "was that worth it?" has no answer.

**Nobody is sure what is safe to send.** Health-adjacent marketing has rules about consent, opt-out and sending hours. Without a system holding that information, the front desk sends nothing at all.

## The solution

| The problem | What Revisit does |
|---|---|
| No idea who should be coming back | Clients are segmented automatically by last visit — New, Active, Lapsed, Dormant. At ninety days they enter the win-back list on their own. |
| Bookings scattered | Phone, online and walk-in land on one calendar, with confirm, reschedule, cancel and reminder on every appointment. |
| Marketing cannot be judged | Every client carries a source. Reports turn that into channel quality and campaign conversion. |
| Unsure what is safe to send | Consent is tracked per channel — text, email, WeChat — and enforced at send time. A compliance panel shows what is still missing. |

## Why not an EHR, a generic CRM, or a spreadsheet

| | What it handles | What Revisit handles |
|---|---|---|
| **EHR / records system** | Clinical notes, diagnoses, insurance | No clinical data at all — only the relationship |
| **Generic CRM** | Sales pipelines and deals | Visit cycles: follow-up timing, consent, what "lapsed" means for a clinic |
| **Spreadsheet** | Stores names, but never reminds anyone | Segments, triggers and attributes on its own |

Revisit is a layer added beside existing systems. It replaces nothing.

## What it changes

- The front desk opens one screen and knows what today needs, without going through records.
- The owner sees every month how many new clients arrived and which channel brought them.
- Clients who would otherwise be lost quietly become a list — with messages that can actually be sent.

## Features

| Module | What it does |
|---|---|
| **Dashboard** | Today's task queue, decisions that need the owner, headline numbers |
| **Appointments** | One-week calendar, three booking sources, confirm / reschedule / cancel / remind, day notes |
| **Clients** | Auto-segmentation, consent state, packages, referrals, message history |
| **Win-back** | Channel-aware recovery of clients who stopped coming |
| **Automation** | Eight rules, compliance checks, role-gated switches |
| **Reviews** | Automatic invites, low-rating alerts, template replies |
| **Reports** | Sources, channel quality, repeat-visit funnel, campaign results |

Four things run across all of them:

- **Role-based access** — Front Desk, Marketing and Owner see different modules and different controls.
- **Per-channel consent** — tracked separately for text, email and WeChat, and enforced before anything is sent.
- **Compliance panel** — opt-out lines, sending hours, missing consent, provider agreement.
- **Source attribution** — recorded once per client, which is what makes every report meaningful.

## How to use

### Getting started

1. Open the demo. A sign-in screen asks which role to enter as.
2. Pick **Owner** the first time — it has the widest access.
3. A short "about" panel opens once. Close it; it can be reopened from the left rail any time.
4. No password, no account, no data collected.

### A five-minute tour

| # | Where | What to do | What happens |
|---|---|---|---|
| 1 | Dashboard | Click any button in **Today's tasks** | The task is handled and struck through |
| 2 | Dashboard | Click the red **Needs win-back** tile | Jumps straight to the win-back list |
| 3 | Win-back | Switch between Text / Email / WeChat | The sendable count changes — clients without consent are excluded automatically |
| 4 | Win-back | Click **Preview** | Shows the real message with a client's name filled in |
| 5 | Clients | Click any row | The full client file opens on the right |
| 6 | Client file | Open the **Messages** tab, then click **Send text** | The message appears in the history immediately |
| 7 | Appointments | Click any appointment | Confirm, reschedule (it really moves on the calendar), cancel, or send a reminder |
| 8 | Left rail | Switch role to **Front Desk**, then look for Automation | The module is gone — front desk has no access to rules |
| 9 | Reports | Read the repeat-visit funnel and channel quality table | The conclusion line at the bottom is generated from the data |

### Module by module

**Dashboard** — Six task items generated from live data, each with a button that handles it or jumps to the right place. Below that, decisions that need the owner: no-shows this month, year-end insurance benefits going unused, automation rules blocked by missing consent. Every headline number is clickable and drills into the matching list.

**Appointments** — A full week in one grid, colour-coded by status. Click any appointment to confirm it, move it to a new day and time, mark it completed, cancel it, send a reminder, or jump to that client's file. Each day has its own note field. Filter by practitioner. Add new appointments, with an option to send a confirmation text.

**Clients** — Eight filters including *no consent* and *has package*. Sortable columns, search, multi-select for bulk tagging or messaging. Click a row to open a five-tab file: overview (with three consent switches you can toggle), visit history, message log, package balance, and front-desk notes.

**Win-back** — Choose a channel first. The system then filters the ninety-day list by who has consented to that channel, states how many are excluded, and offers an opt-in invite for the rest. Each channel has its own template. Preview renders the message for a real client before anything goes out.

**Automation** — Eight rules covering follow-up, review invites, win-back, birthdays, seasonal content, referrals, no-show follow-up and year-end benefit reminders. Each shows what consent it needs and how many clients it can reach. Rules open for editing. Switches are disabled unless you are signed in as Owner.

**Reviews** — Average rating, this month's count, flagged low ratings and the unanswered queue. Ratings of three or below are marked separately. Replies can use a template in one click.

**Reports** — Four questions answered: where clients come from, which channels keep them, where clients stop returning, and what the messages actually brought back. Switch between six and twelve months; hover any bar for detail.

### Other controls

| Control | Where | What it does |
|---|---|---|
| 中文 / English | Left rail | Switches the whole interface, including sample names |
| Dark / Light | Left rail | Theme toggle; also follows the system setting |
| Demo settings | Left rail | Change the clinic name — the whole demo follows |
| Reset demo data | Left rail | Restores the original state without reloading |
| Sign out | Left rail | Returns to the role selection screen |

Refreshing the page also resets everything.

## Roles and permissions

| | Front Desk | Marketing | Owner |
|---|---|---|---|
| Dashboard | ✓ | ✓ | ✓ |
| Appointments | ✓ | — | ✓ |
| Clients | ✓ | ✓ | ✓ |
| Win-back | — | ✓ | ✓ |
| Automation | — | View only | ✓ |
| Reviews | ✓ | ✓ | ✓ |
| Reports | — | ✓ | ✓ |
| Full phone numbers | ✓ | Masked | ✓ |
| Send campaigns | — | ✓ | ✓ |
| Edit automation rules | — | — | ✓ |

## Data and privacy

- The system stores **contact details and visit dates only**. No conditions, diagnoses, prescriptions or insurance information — by design, not by omission.
- All names and numbers in the demo are fictional. Phone numbers use the **555 test range** and cannot be dialled.
- Everything lives in browser memory. **No backend, no database, no analytics, no cookies.** Nothing about a visitor is recorded.
- No message is ever actually sent. Every send action is simulated.
- The sample data models the schedule and services of a small acupuncture practice, which is where the original requirements came from.

## Technical notes

A single `index.html` file. No framework, no build step, no dependencies, no server. Plain HTML, CSS and JavaScript.

Works on desktop and mobile, follows the system light or dark theme, and switches between Chinese and English at runtime.

## Roadmap

- Importing an existing client list from a practice management system
- A waitlist that fills cancelled slots automatically
- Full package and prepaid-card lifecycle, including renewal prompts
- Multi-location switching for clinics with more than one site

## Acknowledgements

Thanks to the Bay Area clinic owner and front-desk staff who described how the work actually runs day to day. The requirements in this project came from those conversations rather than from a feature list.

## Disclaimer

This is a demonstration project. It is not a medical device, does not provide medical advice, and is not a HIPAA-compliant product. A production deployment would require a signed agreement with a compliant messaging provider and real consent management. All brands, names and data shown are fictional.

## About

**Ryan Yan** — a data analyst in the San Francisco Bay Area, building practical tools for small businesses.

Contact via GitHub profile.

---

<br>

# 中文版

**为湾区一家小型私人诊所做的客户留存系统。**

**→ 在线演示：https://sf-ryanyan.github.io/revisit/**

*所有数据均为虚构，不会真的发出任何消息。*

## 项目简介

Revisit 是一套可以直接操作的网页应用，用来回答小诊所每周都会碰到的一个问题：**谁该回来了，但还没回来？**

它不是病历系统（EHR），也不是完整的诊所管理系统。它加在诊所现有系统旁边，只负责"客户关系"这一层——联系方式、预约、接收意愿、跟进消息，以及证明这些动作到底有没有用的数据报表。

演示里所有功能都能点。七个模块，三种身份，中英双语，无需注册。

## 痛点

几乎每家小诊所都在这四件事上出问题。

**客户来过一次就消失了。** 诊所有病历系统，但病历只记录"这个人来的时候发生了什么"，不会告诉任何人"这个人九十天没来了"。三个月后，没人知道该跟进谁。

**预约散在三个地方。** 电话、网站、前台各记各的。撞时间、漏记、爽约之后也没人跟。

**营销花了钱，说不清效果。** 广告投了，内容发了，但没人记录每个新客从哪来。所以"这笔钱值不值"这个问题，永远没有答案。

**想发消息，又不确定能不能发。** 医疗相关的营销对同意、退订、发送时段都有要求。没有系统管这些信息，前台最后干脆什么都不发。

## 解决方案

| 痛点 | Revisit 怎么解决 |
|---|---|
| 不知道谁该回来 | 按最后到店时间自动分层——新客、活跃、流失、沉睡。满九十天自动进入召回名单。 |
| 预约散乱 | 电话、网上、前台进同一张日历，每条预约都能确认、改期、取消、发提醒。 |
| 说不清效果 | 每个客户都带来源。报表把来源变成渠道质量和营销转化率。 |
| 不确定能不能发 | 短信、邮件、微信三个渠道的同意状态分别记录，发送时自动过滤；合规面板显示还缺什么。 |

## 为什么不是病历系统、通用 CRM 或 Excel

| | 它们管什么 | Revisit 管什么 |
|---|---|---|
| **病历系统 / EHR** | 诊疗记录、诊断、保险 | 完全不碰临床数据，只管客户关系 |
| **通用 CRM** | 销售漏斗、成交流程 | 按就诊周期设计：复诊节奏、同意状态、诊所意义上的"流失" |
| **Excel 表格** | 能记下来，但不会提醒任何人 | 自动分层、自动触发、自动归因 |

Revisit 是加在现有系统旁边的一层，不替代任何东西。

## 它改变了什么

- 前台打开一个界面就知道今天该做什么，不用翻记录。
- 老板每个月都能看到新客有多少、分别从哪个渠道来。
- 本来会悄悄流失的客户，变成了一份名单——而且配着真的能合规发出去的消息。

## 功能一览

| 模块 | 做什么 |
|---|---|
| **总览** | 今日待办、需要老板拿主意的事、关键数据 |
| **预约** | 一周日历、三种预约来源、确认 / 改期 / 取消 / 提醒、每日备忘 |
| **客户** | 自动分层、同意状态、套餐、转介绍、沟通记录 |
| **召回** | 分渠道挽回已经不来的客户 |
| **自动化** | 八条规则、合规检查、按身份控制的开关 |
| **评价** | 自动邀评、低分预警、模板回复 |
| **报表** | 来源、渠道质量、复诊漏斗、营销效果 |

四个贯穿所有模块的设计：

- **角色权限**——前台、营销、老板看到的模块和能用的操作都不一样。
- **分渠道同意**——短信、邮件、微信分开记录，发送前强制生效。
- **合规面板**——退订提示、发送时段、同意缺失、服务商协议。
- **来源归因**——每个客户记一次来源，这是所有报表有意义的前提。

## 怎么用

### 开始

1. 打开演示，会先看到一个身份选择页。
2. 第一次建议选 **老板**，权限最全。
3. 会弹出一次简短说明，关掉即可，左栏随时能再打开。
4. 无需密码、无需注册，不收集任何信息。

### 五分钟演示路线

| # | 在哪 | 做什么 | 会发生什么 |
|---|---|---|---|
| 1 | 总览 | 点「今日待办」任意一条的按钮 | 该事项被处理并划掉 |
| 2 | 总览 | 点红色的「需要召回」数字 | 直接跳到召回名单 |
| 3 | 召回 | 在短信 / 邮件 / 微信之间切换 | 可发人数实时变化，未同意的自动排除 |
| 4 | 召回 | 点「预览」 | 看到填好真实姓名的完整消息 |
| 5 | 客户 | 点任意一行 | 右侧打开完整客户档案 |
| 6 | 客户档案 | 切到「沟通记录」，再点「发短信」 | 这条记录立刻出现在历史里 |
| 7 | 预约 | 点任意预约 | 确认、改期（日历上真的会移动）、取消、发提醒 |
| 8 | 左栏 | 把身份切成「前台」，再找自动化 | 模块消失了——前台没有这个权限 |
| 9 | 报表 | 看复诊漏斗和渠道质量对比 | 底部那句结论是从数据实时生成的 |

### 各模块能做什么

**总览**——六条从实时数据生成的待办，每条带一个按钮，点了直接处理或跳转。下面是需要老板拿主意的事：本月爽约次数、年底快清零的保险福利、因为缺少同意而开不了的规则。上方每个数字都能点，下钻到对应名单。

**预约**——一周排班在一张表里，按状态分色。点任意预约可以确认、改到新的日期和时间、标记完成、取消、发提醒，或直接跳到客户档案。每天有独立的备忘栏。可按医师筛选。新增预约时可以选择同时发确认短信。

**客户**——八个筛选条件，包括「未同意」和「有套餐」。表头可排序，可搜索，可多选后批量打标签或群发。点一行打开五个页签的档案：概览（含三个可切换的同意开关）、到店记录、沟通记录、套餐余额、前台备注。

**召回**——先选渠道。系统按该渠道的同意状态过滤九十天名单，明确告诉你排除了多少人，并为这些人提供「邀请同意」。每个渠道有独立模板。预览会用真实客户渲染消息内容。

**自动化**——八条规则，覆盖复诊提醒、评价邀请、流失召回、生日关怀、节气内容、老带新、爽约跟进和年底保险福利提醒。每条显示需要哪种同意、能覆盖多少客户。规则可点开编辑。开关只有老板身份能动。

**评价**——平均分、本月新增、低分预警、待回复数量。三星及以下单独标记。回复可以一键套用模板。

**报表**——回答四个问题：客户从哪来、哪个渠道留得住、客户在哪一步不再回来、营销到底带回多少人。可在六个月和十二个月之间切换，鼠标悬停查看每月明细。

### 其他操作

| 操作 | 在哪 | 作用 |
|---|---|---|
| 中文 / English | 左栏 | 切换整个界面，连示例姓名一起换 |
| 深色 / 浅色 | 左栏 | 主题切换，默认跟随系统 |
| 演示设置 | 左栏 | 改诊所名称，整个演示跟着变 |
| 重置演示数据 | 左栏 | 不用刷新就恢复初始状态 |
| 退出登录 | 左栏 | 回到身份选择页 |

刷新页面同样会恢复初始状态。

## 角色权限

| | 前台 | 营销 | 老板 |
|---|---|---|---|
| 总览 | ✓ | ✓ | ✓ |
| 预约 | ✓ | — | ✓ |
| 客户 | ✓ | ✓ | ✓ |
| 召回 | — | ✓ | ✓ |
| 自动化 | — | 只读 | ✓ |
| 评价 | ✓ | ✓ | ✓ |
| 报表 | — | ✓ | ✓ |
| 完整电话号码 | ✓ | 打码 | ✓ |
| 发送营销消息 | — | ✓ | ✓ |
| 修改自动化规则 | — | — | ✓ |

## 数据与隐私

- 系统**只保存联系方式和到店日期**。不保存病情、诊断、处方或保险信息——这是设计决定，不是没做。
- 演示中所有姓名和号码均为虚构。电话使用 **555 测试号段**，无法接通。
- 所有数据只存在浏览器内存里。**没有后端、没有数据库、没有统计代码、没有 Cookie**，不记录访客的任何信息。
- 不会真的发出任何消息，所有发送动作都是模拟。
- 示例数据模拟的是一家小型针灸诊所的真实排班与项目，这个项目的需求也来自那里。

## 技术说明

单个 `index.html` 文件。无框架、无构建步骤、无依赖、无服务端，纯原生 HTML、CSS 和 JavaScript。

桌面和手机都可用，自动跟随系统的浅色深色设置，中英文可随时切换。

## 后续计划

- 从现有诊所管理系统导入客户名单
- 候补名单自动填补被取消的时段
- 套餐与储值卡的完整流程，含续卡提醒
- 多门店切换

## 致谢

感谢那位湾区诊所老板和前台同事，他们讲清楚了这份工作每天实际是怎么运转的。这个项目的需求来自那些对话，而不是来自一份功能清单。

## 免责声明

本项目为演示用途。它不是医疗设备，不提供医疗建议，也不是符合 HIPAA 的产品。正式投入使用需要与合规的消息服务商签署协议，并建立真实的同意管理机制。页面中出现的所有品牌、姓名和数据均为虚构。

## 关于作者

**Ryan Yan** —— 旧金山湾区的数据分析师，为小型企业做实用工具。

联系方式见 GitHub 个人主页。
