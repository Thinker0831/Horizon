---
layout: default
title: "Horizon Summary: 2026-11-19 (ZH)"
date: 2026-11-19
lang: zh
---

> 从 42 条内容中筛选出 19 条重要资讯。

---

**科技新闻**
1. [Nginx HTTP/2 未认证远程代码执行漏洞披露](#item-tech-news-1) ⭐️ 9.0/10
2. [Java4Shell 高危漏洞影响新一代服务器 CPU](#item-tech-news-2) ⭐️ 9.0/10
3. [OpenAI 模型应用于芯片设计](#item-tech-news-3) ⭐️ 8.0/10
4. [Google 发布 Gemini 4 Neon 模型](#item-tech-news-4) ⭐️ 7.0/10
5. [AI 在审计试验中提问能力超越 KPMG 会计师](#item-tech-news-5) ⭐️ 7.0/10
6. [ExitPath：开源替代 Slack、Notion 和 Microsoft 365 的资源汇总](#item-tech-news-6) ⭐️ 7.0/10
7. [德意志银行调查项目采用开源工具与大规模数据处理](#item-tech-news-7) ⭐️ 7.0/10
8. [微软发布七款新 AI 模型，主打性价比](#item-tech-news-8) ⭐️ 7.0/10
9. [Quad9 因 DNS 封锁退出法国引发基础设施监管争议](#item-tech-news-9) ⭐️ 7.0/10
10. [KVM x86 MMU 上下文处理曝安全漏洞（CVE-2026-99312）](#item-tech-news-10) ⭐️ 7.0/10
11. [DaisyRose-27B 开源 27B 参数大语言模型发布](#item-tech-news-11) ⭐️ 7.0/10
12. [小米大模型 MiMo 或将分拆，负责人去留未定](#item-tech-news-12) ⭐️ 7.0/10

**财经新闻**
1. [美联储会议纪要显示或将继续加息并关注 AI 对通胀影响](#item-finance-news-1) ⭐️ 8.0/10
2. [美联储官员沃勒称或需加息 50 个基点以遏制通胀](#item-finance-news-2) ⭐️ 8.0/10
3. [中美俄领导人于深圳 APEC 峰会会晤，聚焦贸易与科技政策](#item-finance-news-3) ⭐️ 8.0/10
4. [英国下议院通过移民与庇护法案，延长定居年限](#item-finance-news-4) ⭐️ 8.0/10
5. [中韩自贸协定服务与投资谈判实质性结束](#item-finance-news-5) ⭐️ 8.0/10
6. [美国芯片新规导致字节跳动 4.8 亿美元 GPU 贷款暂停](#item-finance-news-6) ⭐️ 7.0/10
7. [腾讯三季度营收低于预期，AI 支出大幅增加](#item-finance-news-7) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Nginx HTTP/2 未认证远程代码执行漏洞披露](https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities) ⭐️ 9.0/10

研究人员披露了影响 Nginx HTTP/2 的多个关键未认证远程代码执行（RCE）漏洞，其中 CVE-2026-123007 涉及 HTTP/2 流控内存破坏，允许攻击者在 worker 进程中执行任意命令。Nginx 1.30.7 和 1.31.9 已于 11 月 18 日修复了 10 个相关 CVE，Rapid7 已发布漏洞利用代码（PoC），但目前尚无野外利用报告。受影响用户如无法升级，建议立即禁用对外 HTTP/2 支持。部分漏洞还可与 Linux 内核缺陷串联，最终获取主机 root 权限。

hackernews · speedping · 11月18日 15:19 · [社区讨论](https://news.ycombinator.com/item?id=50547374)

**「背景信息」** Nginx 是全球广泛使用的开源 Web 服务器和反向代理服务器。此次披露的关键漏洞（CVE-2026-123633 和 CVE-2026-123007）均影响 Nginx 对 HTTP/2 协议的实现，允许未经认证的攻击者远程执行代码。这些漏洞自 Nginx 1.9.5 首次引入 HTTP/2 支持以来一直存在，直到 1.30.7 和 1.31.9 版本于 2026 年 11 月 18 日发布补丁才被修复。

**「影响」** 运行 Nginx 并启用 HTTP/2 的服务器面临被远程攻击者未经认证执行任意代码的风险，严重时可导致主机完全失陷。管理员需尽快升级至已修复版本或临时禁用 HTTP/2，以防止潜在攻击。

**「社区讨论」** 有用户指出漏洞补丁在开源仓库提前一周公开，攻击者有机会提前利用；也有观点认为 HTTP/2 并非默认启用，实际受影响比例有限，但在互联网规模下依然影响巨大。部分讨论还关注了串联利用的 Linux SCTP 内核漏洞，目前尚无公开 CVE 编号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities">Unauthenticated Remote Code Execution in NGINX ... | Wiz Blog</a></li>
<li><a href="https://xint.io/blog/nginx2root-remote-code-execution">NGINX 2 Root: New Remote Code Execution Vulnerabilities in nginx ...</a></li>
<li><a href="https://nginx2shell.com/">Remote code execution in NGINX HTTP / 2 ( CVE - 2026 - 123633 ...)</a></li>

</ul>
</details>

**标签**: `#security`, `#web servers`, `#nginx`, `#vulnerabilities`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [Java4Shell 高危漏洞影响新一代服务器 CPU](https://censys.com/advisory/cve-2026-114938/) ⭐️ 9.0/10

Java 被曝出高危远程代码执行漏洞（CVE-2026-114938，俗称“Java4Shell”），CVSS 4.0 评分高达 9.2，影响 Java 17（17.0.6 及以上）、21、25、27 版本，以及 Oracle Java 8 Performance Pack。标准 Java 8/11 通常不受影响。该漏洞仅影响支持 AVX-512 VBMI 指令集的 x86-64 服务器处理器，主要为 2021 年及以后发布的 Intel Xeon（Ice Lake 及更新）和 2022 年及以后发布的 AMD Zen 4 EPYC/Ryzen，ARM64 架构不受影响。

telegram · zaihuapd · 11月18日 03:55

**「背景信息」** CVE-2026-114938（“Java4Shell”）是 2026 年 11 月 17 日公开披露的一个关键远程代码执行（RCE）漏洞，影响 OpenJDK 的多个主流版本。该漏洞允许攻击者在无需认证的情况下远程执行任意代码，CVSS 4.0 评分高达 9.2，属于极高风险级别。此前，Java 社区曾因 Log4Shell 等漏洞引发广泛关注，但 Java4Shell 影响范围更集中于新一代 Java 版本和特定硬件平台。

**「影响」** 运行受影响 Java 版本且部署在新一代 Intel 或 AMD 服务器上的企业和开发者需立即评估风险，考虑升级、打补丁或采取临时缓解措施，以防止远程攻击者利用该漏洞执行恶意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wiz.io/blog/cve-2026-114938-rce-java4shell-openjdk">CVE - 2026 - 114938 OpenJDK RCE ( Java 4 Shell ): Everything... | Wiz Blog</a></li>
<li><a href="https://www.aikido.dev/blog/java-17-rce-vulnerability-cve-2026-114938">Java 4 Shell Java RCE: Fix &amp; Versions ( CVE - 2026 - 114938 )</a></li>
<li><a href="https://techcommunity.microsoft.com/blog/azurenetworksecurityblog/addressing-java4shell-cve-2026-114938-upgrade-guidance-and-azure-waf-mitigations/4574305">Addressing Java 4 Shell CVE - 2026 - 114938 : upgrade guidance and...</a></li>

</ul>
</details>

**标签**: `#security`, `#Java`, `#vulnerability`, `#software engineering`, `#hardware`

---

<a id="item-tech-news-3"></a>
### [OpenAI 模型应用于芯片设计](https://openai.com/index/advancing-chip-design-with-our-models/) ⭐️ 8.0/10

OpenAI 正在利用其 AI 模型推动芯片设计领域的发展，探索通过自动化和优化电子设计自动化（EDA）流程来提升硬件开发效率。官方信息表明，这些模型被用于简化和加速芯片设计任务，但目前尚未明确公开具体的设计成果或模型细节。该举措可能影响传统硬件行业的工作流程和竞争格局，尤其是在 AI 与硬件深度融合的背景下。现阶段，OpenAI 并未将相关模型或设计完全开放给市场。

hackernews · vighneshiyer · 11月18日 17:45 · [社区讨论](https://news.ycombinator.com/item?id=50549493)

**「背景信息」** OpenAI 近期利用其 AI 模型（如 GPT-6 Astra）优化了 Jalapeño 芯片中的电路，并改进了 RISC-V 核心设计，展示了 AI 辅助芯片设计的进展。这一举措表明，AI 技术正被应用于电子设计自动化（EDA）流程，以提升硬件开发效率和创新能力。

**「社区讨论」** 有用户质疑 OpenAI 是否会与客户形成竞争关系，并指出其模型并未完全开放。另有开发者分享了将芯片设计视为软件问题、利用 AI 代理自动化 EDA 流程的实际经验，认为这种方法在模拟和设计自动化方面效果良好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/advancing-chip-design-with-our-models/">Advancing chip design with OpenAI models | OpenAI</a></li>

</ul>
</details>

**标签**: `#AI applications`, `#chip design`, `#EDA`, `#hardware`

---

<a id="item-tech-news-4"></a>
### [Google 发布 Gemini 4 Neon 模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/) ⭐️ 7.0/10

Google 推出了 Gemini 4 Neon，这是其 AI 模型系列中的新成员。虽然官方尚未披露详细的技术参数或具体用途，但社区讨论显示该模型在智能和易用性方面较前代产品有所提升。Neon 被定位为比 Carbon 更智能，但在某些研究级推理任务上表现略逊一筹。该发布属于 Gemini 系列的渐进式更新，主要面向对 AI 模型差异化和实际应用感兴趣的开发者和研究者。

hackernews · yigitdemirag · 11月18日 21:34 · [社区讨论](https://news.ycombinator.com/item?id=50552424)

**「背景信息」** Gemini 4 Neon 是 Google 推出的 Gemini AI 模型系列中的新成员，专为复杂编程、分析推理和企业级生产工作流设计。与专注于长期项目的 Carbon 以及处理日常任务的 Hydrogen 不同，Neon 旨在在深度与效率之间取得平衡，并以较低成本提供前沿级智能。该模型强调链式推理能力，适用于需要复杂思考和分析的场景。

**「影响」** 对于需要在不同任务间权衡智能水平与推理能力的用户和开发者，Gemini 4 Neon 提供了新的选择，但也加剧了模型命名和定位的混乱，可能增加实际选型和应用的难度。

**「社区讨论」** 部分用户认为频繁更换模型名称和定位让人困惑，难以快速匹配实际需求。也有用户表示，Neon 在易用性和任务执行效率上有明显提升，但对模型命名体系和实际智能水平仍有疑问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-neon/">Gemini 4 Neon - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/">Introducing Gemini 4 Neon</a></li>
<li><a href="https://artificialanalysis.ai/models/gemini-4-neon">Gemini 4 Neon Models - Intelligence, Performance... | Artificial Analysis</a></li>

</ul>
</details>

**标签**: `#AI models`, `#Google`, `#machine learning`, `#industry developments`

---

<a id="item-tech-news-5"></a>
### [AI 在审计试验中提问能力超越 KPMG 会计师](https://europeanbusinessmagazine.com/ai-agents-better-questions-kpmg/) ⭐️ 7.0/10

在一项由 KPMG 主导的审计试验中，AI 代理在提出审计问题方面表现优于 KPMG 的人类会计师。这一结果显示，AI 在细致、繁琐的审计领域具备显著应用潜力。该试验表明，AI 代理能够更全面地覆盖审计细节，提升问题发现的广度和深度。目前尚无证据表明该能力已在行业范围内广泛应用。

hackernews · Betelbuddy · 11月18日 15:49 · [社区讨论](https://news.ycombinator.com/item?id=50547777)

**「背景信息」** KPMG 最近在对一家英国上市公司的首次 AI 驱动审计中，比较了 AI 技术与其自身会计师在审计过程中提出问题的能力。根据报道，AI 能够在某些财务细节上提出更深入的问题，并在部分领域比人类会计师挖掘得更深。这一试点项目旨在探索 AI 在传统审计流程中的实际应用潜力。

**「影响」** 对于会计师事务所和审计行业而言，AI 代理有望提升审计流程的效率和覆盖面，尤其在处理大量细节和重复性任务时表现突出。人类审计师可能需要调整工作重心，更加关注判断性和高阶分析任务。

**「社区讨论」** 有评论认为，AI 在记忆细节和覆盖所有审计要点方面具有天然优势，适合处理繁琐且易遗漏的工作。也有观点指出，审计不仅仅是发现问题，更重要的是判断哪些问题具有重大影响，这一能力仍需人类经验补足。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ft.com/content/5168b3e9-75d0-4be0-9ccd-d327d6b16c05?syn-25a6b1a6=1">AI asked ‘better questions’ than KPMG accountants in pilot audit</a></li>

</ul>
</details>

**标签**: `#artificial-intelligence`, `#automation`, `#professional-services`, `#audit`

---

<a id="item-tech-news-6"></a>
### [ExitPath：开源替代 Slack、Notion 和 Microsoft 365 的资源汇总](https://exitpath-ruddy.vercel.app/) ⭐️ 7.0/10

ExitPath 是一个开源项目，汇总了针对 Slack、Notion 和 Microsoft 365 等主流 SaaS 办公套件的开源替代方案。该网站为希望迁移到开源工具的组织和个人提供了集中参考，涵盖了协作、文档、邮件等多个领域。ExitPath 目前主要作为资源导航和社区讨论平台，帮助用户了解各替代方案的功能差异和迁移难点。该项目适用于关注数据控制、隐私或成本优化的软件工程师和 IT 决策者。

hackernews · zerocool0101 · 11月18日 16:04 · [社区讨论](https://news.ycombinator.com/item?id=50547980)

**「背景信息」** 许多企业和个人用户依赖于如 Slack、Notion 和 Microsoft 365 等主流 SaaS 生产力平台，但这些平台通常存在数据锁定、隐私和成本等问题。ExitPath 项目旨在为用户提供从这些专有平台迁移到开源替代方案的路线图，并对迁移难度进行分级，帮助用户评估和规划替代方案的可行性和实施成本。该项目涵盖了包括 Slack、Notion、Microsoft 365、Google Workspace、Dropbox 和 GitHub 在内的 16 个主流工具，并为每个工具推荐了 30 种开源替代品，如 Mattermost、AppFlowy、Nextcloud 和 Forgejo 等。

**「影响」** 有意从专有办公套件迁移到开源解决方案的用户，可以通过 ExitPath 快速了解和比较不同开源工具，节省调研时间，并提前识别如日历、单点登录（SSO）等功能缺口，便于制定更可行的替代和部署方案。

**「社区讨论」** 多位用户指出，开源替代方案在部署难度、用户体验、日历功能和企业级身份管理（如 SSO）等方面存在明显短板，成为大规模迁移的主要障碍。部分用户也分享了对具体工具（如 Zulip）的实际体验和改进建议，强调开源工具需在易用性和功能完整性上进一步提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://exitpath-ruddy.vercel.app/">ExitPath — find your way out of big-platform lock-in</a></li>
<li><a href="https://numootech.com/en/article/tl-mwmbf8su-8arf2">ExitPath — Open-source alternatives to Slack, Notion, and ...</a></li>
<li><a href="https://zeli.app/story/50547980">ExitPath - Open-source migration routes · Hacker News | Zeli</a></li>

</ul>
</details>

**标签**: `#open-source`, `#productivity`, `#software-engineering`, `#tools`

---

<a id="item-tech-news-7"></a>
### [德意志银行调查项目采用开源工具与大规模数据处理](https://www.inside-db.com/) ⭐️ 7.0/10

一项针对德意志银行的深度调查新闻项目披露，团队利用了如 OpenAleph（基于 ElasticSearch）和 FollowTheMoney 等开源工具，对约 1500 万份主要为 Outlook 邮箱导出的文件进行大规模数据处理与分析。这些工具由 DARC 维护，专为调查新闻场景设计，支持复杂的文档管理和信息检索。项目未公开原始数据，仅向合作媒体提供访问权限，强调数据安全与合规性。

hackernews · gyre007 · 11月18日 15:38 · [社区讨论](https://news.ycombinator.com/item?id=50547620)

**「背景信息」** OpenAleph 是一个专为调查新闻编辑部和研究机构设计的开源平台，能够帮助用户高效检索和分析大量文档和结构化数据。该平台最初由 OCCRP 发起，基于 ElasticSearch 构建，并支持如 FollowTheMoney 这样的专用数据模式，便于揭示复杂的金融关系和数据关联。此次对德意志银行的调查项目正是利用 OpenAleph 及其相关技术，对超过 1500 万份文件进行处理和分析。

**「影响」** 该项目为调查记者和数据工程师提供了可借鉴的开源技术栈和数据架构实践，尤其适用于处理大规模、结构复杂的文档数据。未公开原始数据的做法也引发了关于新闻透明度与数据隐私的讨论。

**「社区讨论」** 有评论者认为不公开原始数据可能导致报道存在选择性偏见，影响公众对事实的全面认知。另有参与者详细介绍了技术实现细节，强调了 OpenAleph 和 FollowTheMoney 在实际调查中的作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openaleph.org/">Welcome - OpenAleph</a></li>
<li><a href="https://github.com/openaleph/openaleph">GitHub - openaleph / openaleph : The open source platform that...</a></li>
<li><a href="https://www.inside-db.com/">Inside Deutsche Bank</a></li>

</ul>
</details>

**标签**: `#data engineering`, `#open source`, `#investigative journalism`, `#information retrieval`

---

<a id="item-tech-news-8"></a>
### [微软发布七款新 AI 模型，主打性价比](https://microsoft.ai/news/microsoft-ignite-2026/) ⭐️ 7.0/10

微软宣布推出七款全新 AI 模型，官方宣称这些模型在价格与性能方面具有竞争力，并可与当前领先的 Opus 和 Sol 模型媲美。此次发布面向 AI 和软件工程领域的从业者及企业，但目前尚未公布具体的技术细节或基准测试数据。该消息引发了业界和技术社区的广泛讨论，关注点集中在模型性能、市场竞争格局以及微软在 AI 领域的战略布局。

hackernews · gmays · 11月18日 16:08 · [社区讨论](https://news.ycombinator.com/item?id=50548021)

**「背景信息」** 微软在 Ignite 2026 大会上发布了七款全新 AI 模型，主打高性价比。据官方介绍，其中 MAI Cyber 2 Flash 模型在 CyberGymE2E 基准测试中，以不到 2% 的任务成本实现了与 GPT-6 Astra 相当的质量。这些模型面向企业和开发者，旨在提升 AI 应用的可负担性和性能表现。

**「社区讨论」** 部分用户认为微软新模型已接近 Opus 和 Sol 的性能，称赞其进步，但也有声音质疑微软缺乏创新和市场影响力，建议开放部分模型以争取市场份额。另有开发者表达对 AI 工具普及带来的职业困扰和行业变化的担忧，反映出技术进步对个人和行业生态的复杂影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/microsoft-ignite-2026/">Seven new world class models at scalable... | Microsoft AI</a></li>

</ul>
</details>

**标签**: `#AI models`, `#Microsoft`, `#machine learning`, `#industry news`

---

<a id="item-tech-news-9"></a>
### [Quad9 因 DNS 封锁退出法国引发基础设施监管争议](https://techstackups.com/articles/quad9-leaves-france-dns-blocking/) ⭐️ 7.0/10

公共 DNS 解析服务 Quad9 宣布因法国法院强制要求其实施 DNS 封锁以打击盗版内容，决定退出法国市场。此举凸显了围绕互联网基础设施在内容监管和反盗版措施中的角色所引发的持续争议。Quad9 的退出意味着法国用户将无法再通过该服务解析域名，反映出基础设施层面介入内容审查的技术和法律局限性。该事件为全球范围内关于 DNS 解析器是否应承担内容过滤责任的讨论提供了新的案例。

hackernews · ritzaco · 11月18日 13:18 · [社区讨论](https://news.ycombinator.com/item?id=50545958)

**「背景信息」** Quad9 是一家非营利 DNS 解析服务提供商，因法国法院要求其屏蔽涉嫌未经授权传播体育赛事的域名，决定于 2026 年 11 月 24 日起停止为法国用户提供服务。这一法院裁决是应 beIN Sports 的诉求作出的，要求 DNS 解析商对特定域名实施封锁。Quad9 的撤离将影响其在法国的网络安全过滤和普通 DNS 解析服务。

**「社区讨论」** 有评论认为，除直接起诉盗版者外，其他打击盗版的措施往往成为政府压制不受欢迎言论的后门。另有观点指出，提升正版内容体验才是减少盗版的有效途径，而强制 DNS 封锁既难以根治盗版，也可能损害互联网自由。部分讨论还聚焦于应将责任归咎于法院还是立法者，认为法院只是执行现有法律，真正的问题或许在于立法本身。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberinsider.com/quad9-to-leave-france/">Quad9 to leave France after court orders piracy-related DNS ...</a></li>
<li><a href="https://thecybersecguru.com/online-privacy/quad9-leaves-france-bein-sports-dns-blocking/">Quad9 Exits France: Why the beIN Sports DNS Ruling Matters ...</a></li>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-will-leave-france-after-court-orders-piracy-blocking-penalty/">DNS Resolver Quad9 Will Leave France After Court Orders ...</a></li>

</ul>
</details>

**标签**: `#internet infrastructure`, `#policy`, `#censorship`, `#DNS`

---

<a id="item-tech-news-10"></a>
### [KVM x86 MMU 上下文处理曝安全漏洞（CVE-2026-99312）](https://www.cve.org/CVERecord?id=CVE-2026-99312) ⭐️ 7.0/10

KVM（基于内核的虚拟机）在 x86 架构下的 MMU（内存管理单元）上下文处理被曝存在安全漏洞（CVE-2026-99312）。该漏洞涉及在模拟 INIT 操作时未无条件重置 MMU 上下文，可能影响虚拟化环境的安全性。目前公开的技术细节有限，原始 CVE 页面暂时无法访问。该问题主要影响运行 Linux 内核并使用 KVM 进行虚拟化的系统管理员和开发者。

hackernews · Kozmik1 · 11月18日 16:06 · [社区讨论](https://news.ycombinator.com/item?id=50548004)

**「背景信息」** KVM（Kernel-based Virtual Machine）是 Linux 内核中的虚拟化模块，允许在 x86 架构上运行虚拟机。此次披露的 CVE-2026-99312 漏洞涉及 KVM 在模拟 INIT 信号时未无条件重置 MMU（内存管理单元）上下文，可能影响虚拟化环境的安全性。该漏洞已被 Linux 内核社区修复，目前未有公开的利用代码。

**「社区讨论」** 有用户质疑该 CVE 的实际危害，认为内核项目对潜在攻击利用点过于敏感地分配 CVE 编号。另有观点建议不要禁用嵌套虚拟化，认为其安全性仍优于其他方案，并指出相关报道存在 AI 生成内容，呼吁由人工重新撰写。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://app.opencve.io/cve/CVE-2026-99312">CVE-2026-99312 - Vulnerability Details - OpenCVE</a></li>
<li><a href="https://www.thehackerwire.com/vulnerability/CVE-2026-99312/">CVE-2026-99312: Vulnerability Details - Exploit Status &amp; Fix ...</a></li>
<li><a href="https://www.rapid7.com/db/vulnerabilities/cve-2026-99312/">CVE-2026-99312: Linux: In the Linux kernel, the following ...</a></li>

</ul>
</details>

**标签**: `#security`, `#virtualization`, `#linux`, `#kernel`

---

<a id="item-tech-news-11"></a>
### [DaisyRose-27B 开源 27B 参数大语言模型发布](https://www.radixark.com/blog/daisyrose-27b) ⭐️ 7.0/10

DaisyRose-27B 是一款新发布的开源大语言模型，拥有 270 亿参数。该模型据称在 144 张 H200 GPU 上训练了 18 天，目前已在 Hugging Face 上提供下载。社区讨论聚焦于其训练方法、评测方式以及与同类模型（如 Sabi-noema、Qwen3.8）的对比。当前尚未提供 gguf 格式权重，部分用户表示期待后续支持。

hackernews · de\_sty · 11月18日 19:39 · [社区讨论](https://news.ycombinator.com/item?id=50551046)

**「背景介绍」** DaisyRose-27B 是基于 Qwen3.8-27B 模型，通过 RadixArk 的 Miles 开源强化学习框架进行后训练得到的。该模型在 144 张 H200 GPU 上，利用 1,200 个精心挑选的长序列智能体任务，经过 18 天训练，显著提升了 Terminal-Bench 4.1 的 pass@1 分数。此次训练采用了完全异步的强化学习方式，使智能体和模型可以并行工作，提升了训练效率。

**「影响」** 对于需要高性能开源大模型的开发者和研究者，DaisyRose-27B 提供了新的选择，尤其适合有大规模算力资源的团队进行二次开发或评测。由于暂未提供 gguf 格式，部分轻量级部署用户需等待后续支持。

**「社区讨论」** 有用户质疑过度依赖评测数据集可能导致模型泛化能力下降，并建议发布更多未参与训练的基准测试结果。另有用户关注训练所需硬件资源之高，以及与同类模型的实际性能对比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://todayforai.com/en/items/art-d6667117-06c">RadixArk Open-Sources DaisyRose-27B Agent Model Trained in 18 ...</a></li>
<li><a href="https://www.aigpu.cloud/en/blog/radixark-daisyrose-27b-rl-post-training">RadixArk&#x27;s DaisyRose-27B Doubles Agent Benchmark Scores with ...</a></li>
<li><a href="https://daily.dev/posts/daisyrose-27b-1-200-task-rl-took-qwen3-8-from-5-6-to-12-on-terminal-bench-4-1-m8yz1a39l">DaisyRose-27B: 1,200-task RL took Qwen3.8 from 5.6% to...</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#open-source`, `#machine-learning`, `#model-training`

---

<a id="item-tech-news-12"></a>
### [小米大模型 MiMo 或将分拆，负责人去留未定](https://mp.weixin.qq.com/s/7LwGupEtmtLzWKQM1-vEfQ) ⭐️ 7.0/10

据多方消息，小米的大模型业务 MiMo 正处于是否分拆的关键阶段，目前已有多家风投和 CVC 与其初步接触，但集团尚未确定具体的分拆融资方案。MiMo 负责人罗福莉与小米集团创始人雷军在分拆问题上存在分歧，罗福莉本人已与部分投资人和财务顾问接触，不排除未来单独创业的可能。MiMo 团队约有百余人，核心研究员二三十人，其 V2-Pro 模型参数超万亿，在 Artificial Analysis 品牌全球排名第五。投资人普遍认为 MiMo 的市场定位尚不明确，但其在小米智能家居和智能座舱生态中有形成闭环的潜力。

telegram · zaihuapd · 11月18日 04:11

**「背景信息」** 小米的 MiMo 大模型业务是公司近年来在人工智能领域的重要布局，团队由罗福莉领导，核心成员具有深厚的技术背景。近期有多家知名风投和企业投资机构与小米就 MiMo 业务的潜在分拆和独立融资进行了初步接触，但小米集团尚未公布明确的分拆方案。当前，集团高层与 MiMo 负责人在分拆事宜上存在分歧，导致决策进展缓慢。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chaincatcher.com/en/article/2305793">Xiaomi was reported to be discussing...</a></li>
<li><a href="https://www.lookonchain.com/feeds/82786">Xiaomi&#x27;s MiMo is reportedly planning a separate financing ...</a></li>
<li><a href="https://news.qq.com/rain/a/20261118A0DPRD00">罗福莉想带MiMo分拆融资，雷军还没松口_腾讯新闻</a></li>

</ul>
</details>

**标签**: `#AI industry`, `#corporate strategy`, `#large language models`, `#China tech`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储会议纪要显示或将继续加息并关注 AI 对通胀影响](https://www.cnbc.com/2026/11/18/fed-minutes-october-2026.html) ⭐️ 8.0/10

美联储 10 月会议纪要显示，官员们预计未来还需加息以应对通胀风险，并首次将人工智能相关需求列为重要通胀风险来源。会议最终以 10 票对 2 票决定将联邦基金利率维持在 3.75%-4%区间。

rss · CNBC Finance · 11月18日 19:41

**「背景」** 美联储此前已多次加息以应对高于目标的通胀，并在 2026 年持续关注人工智能相关投资对物价的影响，部分官员认为 AI 需求已成为推高通胀的新风险因素。近期美联储会议纪要显示，决策层对 AI 带来的通胀和金融稳定风险表达了更高关注度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.richmondfed.org/research/national_economy/macro_minute/2026/ai_imprint_on_prices_and_inflation">AI&#x27;s Imprint on Prices and Inflation | Richmond Fed</a></li>
<li><a href="https://en.cryptonomist.ch/2026/07/09/federal-reserve-inflation-concerns-ai/">Federal Reserve Inflation Concerns Over AI-Driven Chipflation</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/speech/cook20260928a.htm">An Update on AI and the Economy - Federal Reserve Board</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#Interest Rates`, `#Inflation`, `#Artificial Intelligence`, `#Monetary Policy`

---

<a id="item-finance-news-2"></a>
### [美联储官员沃勒称或需加息 50 个基点以遏制通胀](https://www.cnbc.com/2026/11/18/federal-reserve-governor-christopher-waller.html) ⭐️ 8.0/10

美联储理事沃勒表示，为应对持续高企的通胀，央行可能需要在 12 月会议上将基准利率上调 0.5 个百分点，这一幅度高于市场普遍预期的 0.25 个百分点。沃勒称当前通胀形势严峻，需采取更激进措施。

rss · CNBC Finance · 11月18日 15:13

**「背景」** 克里斯托弗·沃勒自 2020 年起担任美联储理事，目前美联储正面临高于 2%目标的持续通胀压力。此前，美联储在 2025 年曾三次降息以应对就业市场担忧，但近期通胀因地缘冲突和能源价格上涨再次升温。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Christopher_Waller">Christopher Waller - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2026/11/18/federal-reserve-governor-christopher-waller.html">Fed’s Waller says central bank may need to ‘shock people’ with...</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#inflation`, `#monetary policy`, `#economic outlook`

---

<a id="item-finance-news-3"></a>
### [中美俄领导人于深圳 APEC 峰会会晤，聚焦贸易与科技政策](https://www.cnbc.com/2026/11/18/apec-trump-xi-putin-shenzhen.html) ⭐️ 8.0/10

美国总统特朗普、中国国家主席习近平和俄罗斯总统普京在中国深圳出席 APEC 峰会，重点讨论贸易协议执行和科技限制等议题；美中双方此前宣布将互相降低价值 300 亿美元商品的关税，但尚未公布生效日期。

rss · CNBC Finance · 11月18日 06:04

**「背景」** 此次亚太经合组织（APEC）峰会在中国深圳举行，美国总统特朗普、中国国家主席习近平和俄罗斯总统普京将首次三方会晤，讨论贸易、科技和地缘政治等关键议题。此前一年，中美曾在韩国 APEC 峰会期间达成为期一年的贸易休战协议，并延长至 2027 年 1 月。此次会议背景下，中美关系因科技出口管制和关税问题持续紧张，全球能源和安全局势也因伊朗和俄乌战争承压。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sputnikglobe.com/20261118/putins-key-statements-at-the-apec-business-summit-1125088068.html">Putin ’s Key Statements at the APEC Business Summit - 18.11. 2026 ...</a></li>
<li><a href="https://www.theguardian.com/world/live/2026/nov/18/apec-summit-live-updates-xi-putin-trump-world-leaders-gather-in-china?page=with:block-6afd64c78f08258efcd2521b">Apec summit live: Xi welcomes Trump on China visit as Putin claims...</a></li>
<li><a href="https://www.cnbc.com/2026/11/18/apec-trump-xi-putin-shenzhen.html">Three things to watch as Trump , Xi and Putin meet in China</a></li>

</ul>
</details>

**标签**: `#geopolitics`, `#trade policy`, `#APEC`, `#US-China relations`, `#technology regulation`

---

<a id="item-finance-news-4"></a>
### [英国下议院通过移民与庇护法案，延长定居年限](https://www.bloomberg.com/news/articles/2026-11-17/uk-s-house-of-commons-passes-controversial-immigration-bill) ⭐️ 8.0/10

英国下议院以 290 票对 94 票通过《移民与庇护法案》，将大多数移民申请定居的基准居住年限从 5 年延长至 10 年，这是最终审议结果，法案将提交上议院进一步审查。

telegram · zaihuapd · 11月18日 05:51

**「背景」** 英国《移民与庇护法案》此前已在下议院进行多轮辩论，旨在调整移民和庇护流程，并对相关政策进行收紧。该法案需在上议院进一步审查后，才可成为正式法律。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.naijaukhub.com/news/immigration-asylum-bill-second-reading">Immigration and Asylum Bill Second Reading Debate... | NaijaUKHub</a></li>

</ul>
</details>

**标签**: `#immigration policy`, `#UK legislation`, `#labor market`, `#public policy`

---

<a id="item-finance-news-5"></a>
### [中韩自贸协定服务与投资谈判实质性结束](https://x.com/Jaemyung_Lee/status/2122988472994791476) ⭐️ 8.0/10

2026 年 11 月 18 日，中韩两国宣布自贸协定服务与投资后续谈判实质性结束，中国承诺在电影、游戏等领域给予韩国最惠国待遇，并扩大旅游、法律、建筑、金融等领域开放。

telegram · zaihuapd · 11月18日 10:02

**「背景」** 中韩自贸协定（FTA）自 2015 年生效后，双方于 2018 年 3 月启动了服务和投资领域的后续谈判，旨在扩大市场准入和深化经济合作，此次谈判历时 8 年 8 个月才实质性结束。此前，协定主要涵盖货物贸易，服务和投资领域的进一步开放一直是两国经济关系深化的重要议题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://biz.chosun.com/en/en-policy/2026/11/18/3HXWCB2DJJGY5JHJZMFZGGB3CQ/">South Korea and China reach deal on services and investment ...</a></li>

</ul>
</details>

**标签**: `#trade agreement`, `#China`, `#South Korea`, `#services sector`, `#investment`

---

<a id="item-finance-news-6"></a>
### [美国芯片新规导致字节跳动 4.8 亿美元 GPU 贷款暂停](https://www.bloomberg.com/news/articles/2026-11-17/banks-pause-480-million-chip-loan-tied-to-china-s-bytedance) ⭐️ 7.0/10

受美国最新 AI 芯片出口管制影响，五家银行暂停了为字节跳动采购 GPU 的 4.8 亿美元贷款，该贷款原计划用于马来西亚数据中心。贷款方 Aolani Cloud 表示正与监管机构和融资伙伴评估新规以确保合规。

telegram · zaihuapd · 11月18日 05:11

**「背景」** 美国近期出台了针对人工智能芯片的新出口管制，限制中国企业获取先进的美国芯片，导致相关金融和供应链活动受到影响。此前，字节跳动计划通过新加坡云服务商 Aolani Cloud 在马来西亚采购英伟达 GPU，并获得 4.8 亿美元贷款支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-17/banks-pause-480-million-chip-loan-tied-to-china-s-bytedance">Banks Pause $480 Million Chip Loan Tied to China’s ByteDance</a></li>
<li><a href="https://www.gate.com/news/detail/NVDA/bytedance-480m-loan-stalled-after-us-tightens-ai-chip-export-rules-25700410">ByteDance $480M Loan Stalled After US Tightens AI Chip Export ...</a></li>

</ul>
</details>

**标签**: `#US-China relations`, `#semiconductors`, `#regulation`, `#corporate finance`, `#technology sector`

---

<a id="item-finance-news-7"></a>
### [腾讯三季度营收低于预期，AI 支出大幅增加](https://api3.cls.cn/share/article/2537922?os=android&amp;amp;sv=8.8.5&amp;amp;app=cailianpress&amp;amp;selected=) ⭐️ 7.0/10

腾讯 2026 年第三季度营收为 2073 亿元，同比增长 8%，低于市场预期，资本开支达到 814.33 亿元，远高于市场预估的 554 亿元，单季自由现金流为负 691 亿元。

telegram · zaihuapd · 11月18日 09:20

**「背景」** 腾讯是一家中国领先的互联网和科技公司，定期发布季度财报以披露其营收、利润和主要业务进展。此前市场普遍关注其在人工智能领域的投入及相关产品表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tencent.com/wp-content/uploads/2026/11/Tencent-Announces-2026-Third-Quarter-Results.pdf">For Immediate Release - Tencent</a></li>

</ul>
</details>

**标签**: `#earnings`, `#capital expenditure`, `#AI`, `#China`, `#technology`

---