---
layout: default
title: "Horizon Summary: 2026-11-15 (ZH)"
date: 2026-11-15
lang: zh
---

> 从 38 条内容中筛选出 15 条重要资讯。

---

**科技新闻**
1. [SpaceX 星舰首次实现轨道级机械臂捕获回收](#item-tech-news-1) ⭐️ 9.0/10
2. [Lovable 应用曝出护照信息与 20 万条私信数据泄露](#item-tech-news-2) ⭐️ 8.0/10
3. [Cloudflare 开源 AI 代理浏览器 Kitesurf](#item-tech-news-3) ⭐️ 8.0/10
4. [Meta 因违规读取相册被意大利罚款 8.05 亿欧元](#item-tech-news-4) ⭐️ 8.0/10
5. [Google Antigravity 推出 /teamwork 协作 AI 工作流功能](#item-tech-news-5) ⭐️ 7.0/10
6. [PyPI 项目页改版，强化安全与溯源信息](#item-tech-news-6) ⭐️ 7.0/10
7. [DeepSeek V3：约 200 行纯 JAX 实现开源](#item-tech-news-7) ⭐️ 7.0/10
8. [Project Zero 调整漏洞披露周期至 30 天](#item-tech-news-8) ⭐️ 7.0/10
9. [TimeCues Studio：开源音乐结构标注与算法评测工具发布](#item-tech-news-9) ⭐️ 7.0/10
10. [短期价格预测论文应对比市场隐含预测基线](#item-tech-news-10) ⭐️ 7.0/10
11. [OpenAI 解散机器人团队，转向通用模型驱动机器人](#item-tech-news-11) ⭐️ 7.0/10
12. [W5000 全球最大无人货机完成试飞](#item-tech-news-12) ⭐️ 7.0/10
13. [Google 高管用 Gemini 让 Windows 11 跑上折叠 iPhone](#item-tech-news-13) ⭐️ 7.0/10

**财经新闻**
1. [Anthropic IPO 拒绝中国内地及香港投资者](#item-finance-news-1) ⭐️ 8.0/10
2. [英伟达 CEO 辞职与国会监管影响 AI 相关股票](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SpaceX 星舰首次实现轨道级机械臂捕获回收](https://www.spacex.com/launches/starship-flight-15) ⭐️ 9.0/10

SpaceX 于 2026 年 11 月 13 日完成了星舰（Starship）第 15 次试飞，首次实现了轨道级飞船由发射塔机械臂直接捕获回收。飞船在绕地球约 14 圈、飞行约 22.5 小时后返回得州基地，被机械臂成功夹住，未采用落地或落海方式。此次任务还部署了 26 颗新一代星链 V3 卫星，但超重型助推器因技术问题未能回收，最终在墨西哥湾溅落并爆炸。该成果标志着 SpaceX 在大型航天器可重复使用技术上取得重大突破，但双回收目标尚未实现。

hackernews · ls612 · 11月14日 21:22 · [社区讨论](https://news.ycombinator.com/item?id=50500963)

**「背景信息」** SpaceX 的星舰（Starship）项目旨在实现大型航天器的完全可重复使用，降低太空运输成本。此前，SpaceX 已多次尝试通过发射塔机械臂（俗称“筷子”）捕获返回的助推器和飞船，但均未完全成功。本次第 15 次试飞是首次实现星舰飞船轨道返回后由机械臂直接捕获，标志着该技术取得关键性突破。

**「影响」** 此次机械臂捕获星舰的成功，为未来实现完全可重复使用的轨道级运载系统奠定了基础，有望大幅降低太空发射成本并提升任务频率。开发者和航天机构可关注后续双回收与重复飞行的进展，以评估其对商业航天和卫星部署的实际影响。

**「社区讨论」** 有评论认为，星舰的设计实现了航天飞机未能完成的完全可重复使用目标，并避免了历史上的重大安全隐患。部分用户指出，若热防护系统表现良好，未来实现双回收和多次复用将极大改变航天经济格局，开启新纪元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=VEvzBhRyB94">SpaceX Catches Starship for the First Time Ending Flight Test 15</a></li>
<li><a href="https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-flight-15-chopsticks-double-catch-super-heavy-ship">SpaceX launches Starship on ambitious 22-hour Flight 15 ... | Space</a></li>

</ul>
</details>

**标签**: `#spaceflight`, `#hardware`, `#systems engineering`, `#industry impact`

---

<a id="item-tech-news-2"></a>
### [Lovable 应用曝出护照信息与 20 万条私信数据泄露](https://www.crissyfield.de/research/lovable-en/) ⭐️ 8.0/10

Lovable 应用因行级安全（Row-Level Security）配置不足，导致用户护照信息和超过 20 万条私信等敏感数据被暴露。此次安全漏洞揭示了平台默认配置（如 Supabase）和自动化开发工具在安全性上的不足。Lovable 官方表示，其平台已内置自动扫描和修复功能，用户可选择自动修复或阻止存在安全问题的应用上线。社区讨论聚焦于平台方和开发者在安全责任上的分工，以及云平台默认安全策略的合理性。

hackernews · armcat · 11月14日 17:43 · [社区讨论](https://news.ycombinator.com/item?id=50499017)

**「事件背景」** Lovable 是一个 AI 驱动的应用开发平台，允许用户快速生成和部署 Web 应用。2026 年 11 月，安全研究人员扫描了超过 15 万个由 Lovable 平台生成的应用，发现大量数据库未设置登录验证，导致护照号码、支付信息、聊天记录等敏感数据被公开访问。此次数据泄露的根本原因在于数据库访问规则缺失，而非 Lovable 平台本身被黑客入侵，且与 Supabase 等云数据库平台的默认配置有关。

**「实际影响」** 受影响用户的敏感数据（包括护照信息和私信）已被泄露，开发者需关注平台默认安全配置并主动加强安全措施。使用 Supabase 等平台的项目应检查并修正默认的安全策略，防止类似问题再次发生。

**「社区讨论」** Lovable 安全负责人强调平台已提供自动扫描和修复工具，但有用户指出 Supabase 的默认配置存在历史遗留问题，部分老项目仍未修复。部分评论认为，AI 生成应用因部署门槛低、数量多，成为数据泄露的高风险对象，平台应提升默认安全标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybernews.com/security/lovable-ai-apps-expose-personal-information/">Lovable AI apps exposed sensitive data in open databases ...</a></li>
<li><a href="https://dev.to/yashvikothari/lovable-data-leak-2026-24664-ai-apps-exposed-80000-user-records-via-supabase-2l7a">Lovable Data Leak 2026: 24,664 AI Apps Exposed 80,000+ User ...</a></li>
<li><a href="https://startupfortune.com/lovable-ai-apps-left-passport-and-payment-data-open-to-anyone/">Lovable AI Apps Left Passport and Payment Data Open to ...</a></li>

</ul>
</details>

**标签**: `#security`, `#data breach`, `#application development`, `#cloud platforms`

---

<a id="item-tech-news-3"></a>
### [Cloudflare 开源 AI 代理浏览器 Kitesurf](https://www.phoronix.com/news/Cloudflare-Kitesurf-Open-Source) ⭐️ 8.0/10

Cloudflare 已以 Apache 2.0 协议开源了 Kitesurf，这是一款专为 AI 代理设计的无状态浏览器。Kitesurf 基于 Cloudflare Workers 构建，无需传统浏览器容器即可解析 HTML、处理 CSS 并执行 JavaScript。与 Chromium 等传统浏览器相比，Kitesurf 占用更少的 CPU 和内存资源，并可在全球 Workers 网络上弹性扩展。相关源代码现已在 GitHub 上公开。

telegram · zaihuapd · 11月14日 09:33

**「背景信息」** Kitesurf 是 Cloudflare 专为 AI 代理开发的实验性无头浏览器引擎，旨在为 AI 系统提供高效的网页交互能力。它完全基于 Cloudflare Workers 构建，最初作为 Cloudflare Agents Week 的一部分发布，并已以开源形式提供，允许开发者本地运行或在 Cloudflare Workers 上自行部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf-open-source/">Kitesurf is now open source | Cloudflare Blog</a></li>
<li><a href="https://www.everydev.ai/tools/kitesurf">Kitesurf - Headless Browser for AI Agents | EveryDev. ai</a></li>

</ul>
</details>

**标签**: `#open-source`, `#AI agents`, `#web browsers`, `#cloud infrastructure`

---

<a id="item-tech-news-4"></a>
### [Meta 因违规读取相册被意大利罚款 8.05 亿欧元](https://www.garanteprivacy.it/home/docweb/-/docweb-display/docweb/10321080) ⭐️ 8.0/10

意大利隐私监管机构对 Meta 处以 8.05 亿欧元罚款，原因是其 Facebook Android 应用在未经用户具体同意的情况下，读取了约 2000 万意大利用户的相册照片、视频及元数据。涉事功能为 2023 年上线的相册推荐，默认开启且授权提示不明确。监管机构要求 Meta 在 60 天内将该功能改为默认关闭，并单独征得用户同意，否则不得对未有效授权的用户启用该功能。

telegram · zaihuapd · 11月14日 14:37

**「背景」** Meta 旗下 Facebook 的 Android 应用于 2023 年推出了相册推荐功能，该功能默认开启，并在用户授权提示上未做到足够明确和具体。意大利隐私监管机构认定该功能在未经用户明确同意的情况下访问了约 2000 万意大利用户的相册照片、视频及元数据，违反了欧盟数据保护法规（GDPR）中关于用户知情同意的要求。

**「影响」** 受此处罚影响，Meta 需对 Facebook Android 应用在意大利的相册推荐功能进行调整，开发团队必须实现默认关闭并单独征求用户同意的机制，否则该功能将无法对未授权用户开放。其他地区的开发者和平台也需关注类似隐私合规风险，避免因默认授权或授权提示不明确而受到监管处罚。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apnews.com/article/italy-meta-android-facebook-feature-9b3073c52464d5cd0e8facbc57285194">Italy fines Meta $887M over access to users&#x27; photos | AP News</a></li>
<li><a href="https://abcnews.com/Technology/wireStory/meta-fined-887-million-italy-android-gallery-photos-138145127">Meta fined $887M in Italy over Android gallery photos, videos ...</a></li>
<li><a href="https://www.politico.eu/article/italy-hits-meta-with-e805m-fine-over-privacy-law-violation/">Italy hits Meta with €805m fine over privacy law violation</a></li>

</ul>
</details>

**标签**: `#privacy`, `#regulation`, `#mobile development`, `#technology industry`

---

<a id="item-tech-news-5"></a>
### [Google Antigravity 推出 /teamwork 协作 AI 工作流功能](https://research.google/blog/advancing-science-engineering-with-antigravitys-teamwork-feature/) ⭐️ 7.0/10

Google 的 Antigravity 平台现已推出 /teamwork 功能，支持科学与工程领域的多智能体协作式 AI 工作流。该功能允许多个 AI 代理在数学、科学、编程和工程任务中协同工作，展示了在复杂任务分解和团队自动化方面的进步。虽然官方博客展示了实际应用案例，但社区认为该功能目前的进展属于渐进式提升，尚未实现颠覆性突破。/teamwork 功能正持续迭代，未来将支持更动态的智能体团队构建。

hackernews · acossta · 11月14日 13:20 · [社区讨论](https://news.ycombinator.com/item?id=50496811)

**「背景信息」** Google Antigravity 是谷歌推出的软件开发平台，允许人工智能代理以不同程度的自主性编写、运行和测试代码。其 /teamwork 功能支持在 Antigravity 平台上部署协作型多智能体团队，用于处理大型项目、多文件重构和复杂研究任务。2026 年 8 月，谷歌首次公开介绍了 Teamwork 作为多智能体编排框架，强调代理之间可以自主提出、批判和完善彼此的工作，这一能力基于 Gemini 3.7 Flash 模型的发布。

**「影响」** 科学家和工程师可利用 /teamwork 功能更高效地组织和自动化复杂项目中的多角色 AI 协作，但当前用户需关注其与其他平台（如 Claude 动态工作流）的差异及功能局限，实际应用时可能仍需人工指导。

**「社区讨论」** 部分用户认为 /teamwork 在多智能体协作方面有潜力，但与现有工具相比仍显落后，缺乏自动模式等关键功能。也有观点认为，该功能有望简化跨学科协作流程，让领域专家更快实现项目目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Antigravity">Google Antigravity - Wikipedia</a></li>
<li><a href="https://antigravity.google/docs/teamwork/">Teamwork agent teams (/teamwork) | Google Antigravity Docs</a></li>
<li><a href="https://antigravity.google/blog/teamwork-when-ai-becomes-a-research-partner">Teamwork: when AI becomes a research partner - antigravity.google</a></li>

</ul>
</details>

**标签**: `#AI systems`, `#collaborative workflows`, `#software engineering`, `#multi-agent systems`

---

<a id="item-tech-news-6"></a>
### [PyPI 项目页改版，强化安全与溯源信息](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI 已正式上线新版项目页面，重点提升了安全信号和溯源信息的展示。此次更新为所有 Python 包用户提供更清晰的包签名、来源和可信度指示，旨在增强开源依赖的信任度和供应链透明度。新版页面现已对所有项目开放，用户可直接在页面上查看相关安全与溯源标识。该功能主要面向开发者、维护者及依赖 Python 包的组织。

hackernews · rbanffy · 11月14日 15:40 · [社区讨论](https://news.ycombinator.com/item?id=50497892)

**「背景信息」** PyPI（Python Package Index）是 Python 社区最主要的软件包托管和分发平台。此前，PyPI 已引入了“provenance”（来源证明）机制，通过可验证的声明（attestations）记录每个发布文件的构建或发布细节，以提升包的安全性和可追溯性。此次页面改版进一步将这些安全和来源信号以更直观的方式展示在项目页面上，便于用户判断包的可信度和供应链安全状况。

**「影响」** 开发者和组织可以更直观地识别包的安全状态和来源信息，从而降低因依赖被篡改或来源不明包而带来的供应链风险。部分用户需关注自身 CI/CD 流程与 PyPI 新增的签名和溯源机制的兼容性。

**「社区讨论」** 有用户担忧新机制可能导致过度依赖中心化云服务，影响生态多样性；也有开发者支持 sigstore 等无密钥签名方式的普及，期待更多 CI/CD 服务商支持相关安全标准。部分意见指出，当前溯源机制主要防范被劫持的项目，但对本身恶意的包无能为力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.pypi.org/using-pypi/package-security/provenance/">Checking Provenance (package origin) - PyPI User Documentation</a></li>
<li><a href="https://habr.com/ru/companies/codescoring/articles/1107380/">[46. 2026 ] Обзор новых правил безопасности в пакетных... / Хабр</a></li>

</ul>
</details>

**标签**: `#python`, `#security`, `#open-source`, `#software-supply-chain`

---

<a id="item-tech-news-7"></a>
### [DeepSeek V3：约 200 行纯 JAX 实现开源](https://github.com/Vaibhaav-Tiwari/deepseek-v3-jax) ⭐️ 7.0/10

一位开发者在 GitHub 上发布了 DeepSeek V3 的极简纯 JAX 实现，代码量约 200 行，旨在为学习和实验现代深度学习模型提供便捷入口。该项目无需依赖复杂框架，适合希望深入理解模型原理的开发者和研究者，尤其对 JAX 和 ROCm 用户友好。该实现并非官方发布，而是社区成员基于公开信息的简化复现，主要用于教育和实验目的。

hackernews · VaibhaavTiwari · 11月14日 15:04 · [社区讨论](https://news.ycombinator.com/item?id=50497589)

**「背景介绍」** DeepSeek V3 是一种大规模混合专家（Mixture-of-Experts, MoE）语言模型，总参数量达 6710 亿，但每个 token 实际激活的参数仅为 370 亿，从而兼顾了模型能力与推理效率。其架构采用了多头潜在注意力（Multi-head Latent Attention, MLA）和 DeepSeekMoE 技术，这些创新最早在 DeepSeek V2 中得到验证。DeepSeek V3 以高效推理和成本效益为目标，相关模型和论文已完全开源。

**「影响」** 对于希望在非 NVIDIA 硬件（如 AMD 显卡）上使用 JAX 进行深度学习实验的用户，该项目提供了可行的端到端训练起点，降低了环境配置和模型理解的门槛。部分用户反馈在 Fedora+ROCm 环境下可顺利运行，并分享了相关配置经验。

**「社区讨论」** 评论者普遍认为该项目极具教育价值，便于从第一性原理学习模型结构和推理过程。一些用户分享了在 AMD 显卡和 ROCm 环境下的成功运行经验，并指出该实现对非 CUDA 用户尤其有用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepwiki.com/deepseek-ai/DeepSeek-V3/1.2-model-architecture-overview">Model Architecture Overview | deepseek-ai/DeepSeek-V3 | DeepWiki</a></li>
<li><a href="https://arxiv.org/abs/2412.19437">[2412.19437] DeepSeek-V3 Technical Report - arXiv.org DeepSeek-V3 Technical Report - arXiv.org deepseek-ai/DeepSeek-V3 · Hugging Face DeepSeek-V3 - Hugging Face GitHub - deepseek-ai/DeepSeek-V3 · GitHub</a></li>

</ul>
</details>

**标签**: `#machine-learning`, `#jax`, `#open-source`, `#deep-learning`

---

<a id="item-tech-news-8"></a>
### [Project Zero 调整漏洞披露周期至 30 天](https://projectzero.google/2026/11/disclosure-policy.html) ⭐️ 7.0/10

Google Project Zero 宣布将逐步缩短其漏洞披露窗口：自 2027 年 2 月 2 日起，漏洞将在报告给厂商后 60 天公开，自 2028 年 1 月 3 日起缩短至 30 天。目前政策为 90 天。该政策适用于所有被 Project Zero 报告的安全漏洞，旨在加快厂商修复安全问题的速度。

hackernews · hacb · 11月14日 11:13 · [社区讨论](https://news.ycombinator.com/item?id=50496051)

**「背景信息」** 自 2021 年以来，Google Project Zero 一直采用“90+30”漏洞披露政策，即厂商有最多 90 天时间修复漏洞，外加 30 天的补丁推广期。该政策旨在推动厂商更快修复安全问题，并确保用户能及时获得补丁。随着 AI 辅助漏洞发现和利用技术的发展，威胁环境发生了变化，促使 Project Zero 重新评估披露窗口的合理性。

**「影响」** 受影响的软件厂商和开源项目需在更短时间内修复被报告的安全漏洞，否则漏洞细节将在 30 至 60 天后公开，增加了未及时修复时的安全风险和舆论压力。

**「社区讨论」** 有评论认为部分厂商（如 Ubuntu）可能难以在更短周期内完成修复，也有人主张应立即披露漏洞以促使厂商尽快响应。另有观点担忧大型公司可能借此策略推动自家产品的采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://projectzero.google/2026/11/disclosure-policy.html">Policy and Disclosure: 2026 Edition - Project Zero</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability-disclosure`, `#software-industry`, `#policy`

---

<a id="item-tech-news-9"></a>
### [TimeCues Studio：开源音乐结构标注与算法评测工具发布](https://www.reddit.com/r/MachineLearning/comments/1xwh3mw/acm_multimedia_2026_timecues_studio_a_free/) ⭐️ 7.0/10

TimeCues Studio 是一款免费开源的网页应用，专为音乐结构标注和算法评测设计，现已发布。该工具支持在节拍对齐的时间线上标注歌曲的各类结构（如段落、提示、循环等），并可与算法（如 allin1 和 MSAF）输出进行对比评测。用户可单独或协作完成标注，并支持导出为 Audacity 标签、MIDI 或 JSON 格式。该项目采用 MIT 许可证，支持 Docker 一键部署，并提供在线演示和详细文档。

reddit · r/MachineLearning · /u/SapirCa · 11月14日 23:59

**「背景介绍」** 音乐结构标注是音乐信息检索（MIR）领域的重要任务，涉及对音频文件中不同部分（如段落、重复、过渡等）进行人工或自动化标记。此前，研究人员常用如 Audacity 等通用音频编辑器进行标注，或依赖各自开发的工具，缺乏专为音乐结构标注和算法评测设计的开源协作平台。TimeCues Studio 正是在此背景下开发，旨在为算法开发团队和研究者提供统一的标注、算法对比和原型测试环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.10338">[2609.10338] TimeCues Studio : A Workspace for Music Annotation ...</a></li>
<li><a href="https://github.com/sapirca/timecues-studio">GitHub - sapirca/ timecues - studio · GitHub</a></li>

</ul>
</details>

**标签**: `#open source`, `#music information retrieval`, `#machine learning tools`, `#data annotation`

---

<a id="item-tech-news-10"></a>
### [短期价格预测论文应对比市场隐含预测基线](https://www.reddit.com/r/MachineLearning/comments/1xw6fk9/should_shorthorizon_price_forecasting_papers/) ⭐️ 7.0/10

一则讨论帖质疑当前短期价格预测论文普遍采用的基线方法，建议应将市场隐含预测（如期权隐含波动率或众包预测）作为更有意义的对比基线，而不仅仅是与随机游走、ARIMA 等简单模型比较。发帖者指出，许多论文只关注点预测的 RMSE，而忽视了区间预测的覆盖率，这在如比特币等高波动资产中更为重要。该观点强调，若无法超越市场自身的预测，模型优于简单基线的意义有限。帖子还提出数据可得性可能是阻碍此类基线普及的原因之一。

reddit · r/MachineLearning · /u/happypeanut-t · 11月14日 16:23

**「背景」** 在金融时间序列预测领域，学术论文常用随机游走、ARIMA 等传统模型作为基线进行性能对比。然而，市场隐含预测（如期权价格反映的市场预期）已被广泛认为整合了大量公开信息，代表了市场参与者的集体智慧。

**标签**: `#machine learning`, `#finance`, `#forecasting`, `#research methodology`

---

<a id="item-tech-news-11"></a>
### [OpenAI 解散机器人团队，转向通用模型驱动机器人](https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/) ⭐️ 7.0/10

OpenAI 已解散其独立的机器人团队，将相关研究员重新分配至更通用的研究团队。公司表示，随着 GPT-6 Astra 等通用前沿模型已能直接操控机器人执行任务，已无需专门的机器人团队。此前 OpenAI 曾于 2024 年重建机器人团队并与 Figure 合作，但该合作已于 2025 年 2 月终止。目前 OpenAI 仍在自研人形机器人，计划于 2027 年首次公开展示。

telegram · zaihuapd · 11月14日 04:00

**「背景信息」** OpenAI 近年来一直在机器人领域进行探索，曾于 2020 年解散过一次机器人团队，2024 年又重建团队并与 Figure 合作，但该合作于 2025 年初终止。此次调整的背景是，OpenAI 认为其最新的通用 AI 模型（如 GPT-6 Astra）已具备直接操控机器人执行任务的能力，因此不再需要专门的机器人团队。公司将相关研究员分配到更广泛的研究方向，旨在加速机器人相关技术的发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://casrai.org/news/openai-disbands-robotics-team-2026">OpenAI Disbands Its Robotics Team: What It Means — CASRAI</a></li>
<li><a href="https://tech.yahoo.com/ai/articles/exclusive-openai-disbands-stand-alone-170530559.html">Exclusive: OpenAI disbands its stand-alone robotics team as ...</a></li>
<li><a href="https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/">Exclusive: OpenAI disbands stand-alone robotics team as ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#robotics`, `#AI models`, `#industry news`

---

<a id="item-tech-news-12"></a>
### [W5000 全球最大无人货机完成试飞](https://www.ithome.com/1/027/068.htm) ⭐️ 7.0/10

白鲸航线宣布，W5000 大型无人货运飞机在内蒙古成功完成技术验证试飞，涵盖爬升、平飞、转弯、下降和着陆等全部科目。W5000 号称全球最大业载无人货机，最大起飞重量 10.8 吨，最大业载 5 吨，设计航程 2600 公里，采用涡桨动力和自主驾驶、地面监控模式。企业计划于 2027 年上半年完成适航取证。该机组设计允许一组人员同时监控 6 至 7 架飞机。

telegram · zaihuapd · 11月14日 05:00

**「背景介绍」** W5000 是由白鲸航线（Air White Whale）研发的大型无人货运飞机，采用双涡桨动力，最大起飞重量为 10.8 吨，最大业载 5 吨，货舱容积超过 65 立方米。此前，该机型于 2024 年 10 月首次在常州生产基地亮相，定位为高效、低成本的无人空中物流平台，旨在推动货运无人机在长距离运输领域的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chinadaily.com.cn/a/202410/22/WS6717074aa310f1265a1c8dd2.html">Firm unveils unmanned cargo drone - Chinadaily.com.cn</a></li>
<li><a href="https://interestingengineering.com/innovation/china-worlds-largest-cargo-drone">World’s largest cargo drone with 5-ton payload capacity unveiled</a></li>
<li><a href="https://dronexl.co/nn/2024/10/27/chinese-firm-unveils-5-ton-payload-cargo-drone/">Chinese Firm Unveils Massive 5-Ton Payload Cargo Drone</a></li>

</ul>
</details>

**标签**: `#autonomous systems`, `#hardware`, `#aviation`, `#AI applications`

---

<a id="item-tech-news-13"></a>
### [Google 高管用 Gemini 让 Windows 11 跑上折叠 iPhone](https://www.windowslatest.com/2026/11/14/windows-11-can-run-on-apples-foldable-iphone-and-googles-ai-boss-proved-it-using-gemini-years-after-microsoft-gave-up-on-windows-phones/) ⭐️ 7.0/10

Google AI Studio 产品设计负责人 Ammaar Reshi 利用 Gemini 4 Carbon 和开源项目 WindowsiOS，在苹果折叠手机 iPhone Duo 上本地运行了 Windows 11 24H2，并公开了操作视频。该方案无需越狱，通过 JIT 翻译运行 ARM64 代码，并借助微软 Prism 支持部分传统 Windows 应用。安装镜像约 12 GB，需配合 Apple Silicon Mac 及开发工具。此次演示展示了跨平台系统移植和 AI 工具在操作系统兼容性上的新突破。

telegram · zaihuapd · 11月14日 06:52

**「相关背景」** WindowsiOS 是一个开源项目，旨在让微软 Windows 11 ARM64 版本以接近原生的 JIT 速度在未越狱的现代 iOS 设备上运行。据其官方仓库介绍，该项目已在折叠屏 iPhone Duo（iPhone 19，搭载 Apple A20 Pro，iOS 27 TXM）上完成端到端验证，无需使用 Hypervisor.framework。Gemini 4 Carbon 是 Google 的一款 AI 工具，在此次演示中被用于辅助开发和部署该系统移植方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ammaarreshi/WindowsiOS">GitHub - ammaarreshi/ WindowsiOS : Native Windows 11 ARM64 on...</a></li>
<li><a href="https://www.ixbt.com/news/2026/11/15/gemini-4-carbon-za-dva-casa-prevratila-iphone-duo-v-noutbuk-s-windows-11-daze-dzeilbreik-ne-ponadobilsia.html">Gemini 4 Carbon за два часа превратила iPhone Duo в ноутбук...</a></li>

</ul>
</details>

**标签**: `#cross-platform`, `#operating systems`, `#AI tools`, `#hardware`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Anthropic IPO 拒绝中国内地及香港投资者](https://m.economictimes.com/markets/us-stocks/news/anthropic-ipo-share-orders-from-china-are-said-to-be-rebuffed/articleshow/135809948.cms) ⭐️ 8.0/10

Anthropic 首次公开募股（IPO）将不接受中国内地及香港投资者下单，知情人士称此举与国际武器贸易条例（ITAR）相关的出口管制有关。公司计划以 1.4 万亿美元估值募资至多 904 亿美元，IPO 定价日为 11 月 18 日，次日上市。

telegram · zaihuapd · 11月14日 10:18

**「背景」** 此前，受美国国际武器贸易条例（ITAR）等出口管制影响，SpaceX 等公司上市时也曾对中国内地和香港投资者实施类似限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://the-decoder.com/banks-bar-chinese-and-hong-kong-investors-from-anthropic-ipo-over-us-export-controls/">Banks bar Chinese and Hong Kong investors from Anthropic IPO ...</a></li>

</ul>
</details>

**标签**: `#IPO`, `#regulation`, `#technology`, `#capital markets`, `#geopolitics`

---

<a id="item-finance-news-2"></a>
### [英伟达 CEO 辞职与国会监管影响 AI 相关股票](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 7.0/10

英伟达 CEO 辞职和美国国会可能加强对数据中心的监管，引发 AI 相关股票和 ETF（交易型基金）出现波动，其中 Roundhill Neocloud ETF 自 2026 年 8 月上市以来累计下跌 39%。分析师预计，如果英伟达面临持续压力，其他 AI 芯片公司如 AMD 和 Alphabet 可能受益。

rss · CNBC Finance · 11月14日 15:50

**「背景」** 2026 年 11 月，英伟达（Nvidia）创始人兼首席执行官黄仁勋宣布辞职，由公司执行副总裁兼首席财务官 Colette Kress 担任临时 CEO。此前，市场对美国国会可能加强对数据中心和芯片出口的监管已有关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/live/2026/nov/13/nvidia-jensen-huang-to-testify-before-congress-live-latest-updates">Calls for crackdown on China chip exports – as it happened | Nvidia</a></li>
<li><a href="https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Announces-CEO-Transition/">NVIDIA Corporation - NVIDIA Announces CEO Transition</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI`, `#ETFs`, `#Tech Regulation`, `#Market Reaction`

---