---
layout: default
title: "Horizon Summary: 2026-11-16 (ZH)"
date: 2026-11-16
lang: zh
---

> 从 37 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [Meta FAIR 与 NYU：多模态视觉编码器预训练可选，专用参数不可或缺](#item-tech-news-1) ⭐️ 8.0/10
2. [多人游戏用本地世界模型实时生成玩家视角](#item-tech-news-2) ⭐️ 8.0/10
3. [美团开源 LongCat-2.5，完全用国产芯片训练](#item-tech-news-3) ⭐️ 8.0/10
4. [旧 Bitly 短链被劫持引发安全担忧](#item-tech-news-4) ⭐️ 7.0/10
5. [Protomaps 简化并降低自托管地图瓦片成本](#item-tech-news-5) ⭐️ 7.0/10
6. [MacBook Pro OLED 屏幕 PWM 闪烁问题分析](#item-tech-news-6) ⭐️ 7.0/10
7. [微软 365 故障致酒店氯气泄漏，15 人中毒](#item-tech-news-7) ⭐️ 7.0/10
8. [B300 GPU 上 cudaMemcpy 提速 5 倍新工具发布](#item-tech-news-8) ⭐️ 7.0/10
9. [推理模型训练外早停新方法：输出层线性探针](#item-tech-news-9) ⭐️ 7.0/10
10. [Marimba：开源轻量级语音决策模型发布](#item-tech-news-10) ⭐️ 7.0/10
11. [MariaDB 驱动的多语言维基百科历史对齐项目亮相黑客松](#item-tech-news-11) ⭐️ 7.0/10
12. [特斯拉 Cybercab 推出 299 美元/月自动驾驶订阅](#item-tech-news-12) ⭐️ 7.0/10
13. [传鲁比奥与 Anthropic 涉推动黄仁勋离职与芯片出口限制](#item-tech-news-13) ⭐️ 7.0/10
14. [华为云上线开源盘古模型 openPangu-2.1-Pro](#item-tech-news-14) ⭐️ 7.0/10

**财经新闻**
1. [Cantor Fitzgerald 因与 Nvidia 相关交易及高管关系受到审查](#item-finance-news-1) ⭐️ 8.0/10
2. [美法官允许美光、三星等 DRAM 价格操纵案继续审理](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Meta FAIR 与 NYU：多模态视觉编码器预训练可选，专用参数不可或缺](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Meta FAIR 与纽约大学（NYU）联合开展的大规模实证研究，训练了 200 多个多模态大语言模型（MLLM），系统分析了视觉编码器预训练和架构选择的作用。结果显示，视觉编码器的单独预训练在受控算力预算下并非必要，无论采用对比、自监督还是描述生成等多种预训练目标，最终在视觉问答（VQA）任务上与从零训练的编码器表现相当。即使免费延长预训练时间，也未提升 VQA 表现，但视觉专用参数（即仅视觉 token 使用的参数）是不可或缺的，缺失时模型在各规模下均显著落后。视觉分支参数可直接融合进 LLM 前几层，无需独立编码器，且推理延迟更低。

reddit · r/MachineLearning · /u/trungh98 · 11月15日 17:38

**「背景介绍」** 多模态大模型（MLLMs）近年来成为人工智能领域的研究热点，尤其是在视觉与语言结合的任务中。此前，Meta FAIR 和 NYU 的研究已探索从零开始联合训练视觉与语言模型的效果，并发现统一的多模态架构在某些条件下优于将视觉编码器“外挂”到语言模型的做法。相关研究还指出，视觉任务在大规模训练中对数据量的需求远高于语言任务，这推动了对视觉编码器预训练和参数分配方式的进一步系统性研究。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aigazine.net/industry/meta-fair-and-nyu-present-advances-in-multimodal-ai-pretraining-with-moe-architecture--s">Meta FAIR and NYU Present Advances in Multimodal AI Pretraining ...</a></li>
<li><a href="https://toknow.ai/posts/meta-fair-beyond-language-modeling-multimodal-pretraining/">Meta FAIR Finds That Training Vision and Language Together From...</a></li>

</ul>
</details>

**标签**: `#multimodal models`, `#vision encoders`, `#machine learning research`, `#model architecture`

---

<a id="item-tech-news-2"></a>
### [多人游戏用本地世界模型实时生成玩家视角](https://www.reddit.com/r/MachineLearning/comments/1xx4ta3/we_made_a_multiplayer_game_where_each_players/) ⭐️ 8.0/10

一个多人游戏原型现已开放测试，玩家需使用 RTX 3080 或更高配置（或实验性 Mac 版本），每位玩家的游戏视角由其本地 GPU 上运行的世界模型实时生成。该模型基于近 3958 小时、16Hz 对齐的 10 人 CS:GO 机器人比赛数据集训练，游戏状态通过轻量级服务器同步，渲染则依赖扩散变换器。当前仅支持一张小地图和手枪，细节表现有限，但已可多人游玩。数据集和游戏均已开放下载，供研究者和开发者使用。

reddit · r/MachineLearning · /u/bengal7ion · 11月15日 19:46

**「背景介绍」** 传统多人游戏通常依赖中心化服务器和本地渲染引擎来生成玩家视角。而本项目采用了世界模型（world model）和扩散变换器（diffusion transformers），让每位玩家的视角由本地 GPU 运行的 AI 模型实时生成，无需传统渲染引擎。根据开发者在社交媒体上的介绍，这种架构允许玩家通过网络同步游戏状态，但每个人的画面由各自的模型推理生成，体现了生成式 AI 在游戏领域的新应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/v0rt3ch/status/2122031717712085388">vor.tech on X: &quot;1/ We made a playable multiplayer game using ...</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#world models`, `#diffusion transformers`, `#multiplayer systems`, `#open dataset`

---

<a id="item-tech-news-3"></a>
### [美团开源 LongCat-2.5，完全用国产芯片训练](https://the-decoder.com/meituan-releases-a-1-6-trillion-parameter-agent-model-that-never-touched-an-nvidia-gpu/) ⭐️ 8.0/10

美团 LongCat 团队正式开源了 LongCat-2.5 大模型的权重，并声明其训练过程完全未使用英伟达 GPU，而是采用华为升腾加速卡等中国芯片。LongCat-2.5 是一款支持文本、图像和视频输入的多模态智能体模型，每个 token 激活约 480 亿参数，权重以 MIT 许可证发布，允许商用。在 Terminal Bench v2.1 测试中，该模型得分 88.4，略低于 Claude Opus 5 的 89.1。

telegram · zaihuapd · 11月15日 11:08

**「背景信息」** LongCat-2.5 是美团于 2026 年 11 月发布的大型多模态语言模型，具备 1M token 的上下文窗口，并支持文本、图像和视频输入。该模型以其大规模参数量和多模态能力为特点，且已通过 API 平台和部分第三方平台提供试用。此前版本未公开强调完全基于中国芯片训练，此次明确未用英伟达 GPU，突显其硬件自主性。

**「影响」** 开发者和企业可在无需依赖英伟达 GPU 的情况下，基于国产硬件部署和训练 LongCat-2.5，并在商业项目中使用其开源权重。这为中国本土 AI 生态提供了更多自主可控的选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm-stats.com/models/longcat-2.5">LongCat - 2 . 5 Benchmarks, Pricing &amp; Context Window</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI models`, `#hardware`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [旧 Bitly 短链被劫持引发安全担忧](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 7.0/10

近期有报道称，旧的 Bitly 短链接正在被劫持，这引发了关于 URL 缩短服务安全性和可靠性的担忧。被劫持的短链可能被用于恶意用途，影响依赖这些链接的个人和组织。该问题凸显了第三方短链服务在长期链接完整性和安全方面的风险，尤其是当原始账户失效或服务商发生变更时。此事件提醒开发者和内容发布者注意短链的持久性和管理。

hackernews · hspeiser · 11月15日 22:11 · [社区讨论](https://news.ycombinator.com/item?id=50511395)

**「背景信息」** Bitly 是一种常用的 URL 缩短服务，允许用户将长链接转换为更短的格式，便于分享。然而，随着时间推移，部分旧链接可能因账户失效、域名变更或服务商管理不善而失去原有指向，导致被攻击者利用进行“链接劫持”。链接劫持（Broken Link Hijacking）是一种攻击方式，攻击者通过接管失效或过期的链接目标，将原本可信的短链重定向到恶意或不当内容上，从而危害用户安全和品牌信誉。相关报道显示，这一问题已影响到企业社交媒体历史内容，造成不良影响。

**「影响」** 依赖 Bitly 等第三方短链服务的用户和组织，可能面临链接被恶意重定向、内容丢失或品牌信誉受损的风险。建议重要内容或长期链接尽量避免使用外部短链服务，或定期检查和归档相关链接。

**「社区讨论」** 有用户认为外包的短链服务比自建方案更容易导致链接失效和安全隐患，主张避免使用短链。另有讨论指出，类似问题也出现在组织放弃的域名或 CNAME 上，被不法分子利用进行钓鱼或垃圾信息传播。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nypost.com/2026/11/15/lifestyle/corporate-social-media-hacked-in-bizarre-bitly-link-hijacking-scheme/">Corporate social media hacked in bizarre Bitly link - hijacking scheme</a></li>
<li><a href="https://www.youtube.com/watch?v=grLWfIbXAys">How I was found broken link hijacking less than 2 minutes... - YouTube</a></li>
<li><a href="https://www.drlinkcheck.com/blog/broken-link-hijacking">Broken Link Hijacking : How Broken Links Can Be a Security Risk</a></li>

</ul>
</details>

**标签**: `#security`, `#web infrastructure`, `#url shorteners`, `#internet hygiene`

---

<a id="item-tech-news-5"></a>
### [Protomaps 简化并降低自托管地图瓦片成本](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

Protomaps 让开发者能够更便宜、更容易地自托管地图瓦片，为需要隐私、控制权或成本敏感的用户提供了商业地图服务的替代方案。该工具支持自定义主题，易于集成，并且运行成本极低，适合个人开发者和小型项目。与传统的地图 API 相比，Protomaps 不依赖第三方服务，用户可完全掌控地图数据的存储与访问。社区反馈显示，Protomaps 已被实际替换 Google Maps 和 Maptiler 等服务，显著降低了费用。

hackernews · bcye · 11月15日 19:26 · [社区讨论](https://news.ycombinator.com/item?id=50509837)

**「背景信息」** Protomaps 是一个开源项目，旨在让前端开发者能够轻松自助托管地图瓦片。与 Mapbox 或 Google Maps API 等商业地图服务不同，Protomaps 通过将矢量地图瓦片打包为单一文件（PMTiles 格式），并利用 HTTP 范围请求进行分发，无需服务器搭建，也无需第三方依赖或 API 密钥，用户只需承担自身的存储和带宽费用。其底图数据基于 OpenStreetMap，适合需要隐私、成本可控和自主可控地图服务的开发者。

**「影响」** 开发者和小型企业可以通过 Protomaps 以极低的成本自托管地图服务，避免高额的商业地图 API 账单，并提升数据隐私和自主可控性。对于需要高分辨率全球卫星图像的场景，存储和带宽成本仍然较高，需权衡使用范围。

**「社区讨论」** 有用户表示，Protomaps 替代 Google Maps 后大幅降低了费用，并称其易用且可定制。也有开发者指出，高分辨率卫星图像自托管时存储需求巨大，难以完全依赖低成本方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>
<li><a href="https://protomaps.com/about">Protomaps - The open source map in a file</a></li>
<li><a href="https://docs.protomaps.com/">Protomaps Documentation | Protomaps Docs</a></li>

</ul>
</details>

**标签**: `#open-source`, `#mapping`, `#web-development`, `#tools`

---

<a id="item-tech-news-6"></a>
### [MacBook Pro OLED 屏幕 PWM 闪烁问题分析](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

一篇技术分析文章详细探讨了 MacBook Pro OLED 屏幕的 PWM（脉宽调制）闪烁问题，包括具体的技术测量和对用户体验的影响。文章指出，OLED 屏幕采用 PWM 控制亮度，可能导致部分用户出现视觉不适，尤其是对闪烁敏感的人群。分析还涉及 PWM 频率的具体数值及其在不同亮度下的表现，并讨论了该现象对可访问性的潜在影响。该问题已引发技术社区的广泛讨论和关注。

hackernews · MacAnorak · 11月15日 13:15 · [社区讨论](https://news.ycombinator.com/item?id=50506719)

**「背景信息」** PWM（脉宽调制）是一种常用于 OLED 显示屏亮度调节的技术，通过快速切换屏幕亮灭来实现不同的亮度水平。近期，Notebookcheck 等第三方实验室测量发现，14 英寸 MacBook Pro 的 PROLED XDR 显示屏在 99%及以下亮度时采用 240Hz 的 PWM 调光，这一频率相对较低。相比之下，上一代 Mini-LED 显示屏的 PWM 频率高达 14,880Hz，因此新款 OLED 面板的调光频率低了约 62 倍，这可能导致对 PWM 敏感的用户出现眼睛疲劳、头痛或恶心等不适症状。

**「社区讨论」** 有用户对 PWM 频率的具体数值和测量方法提出质疑，认为实际有效频率可能高于部分测试结果。多位评论者分享了自己或家人对屏幕闪烁的敏感体验，强调该问题对部分用户可能造成头痛、恶心等明显不适，并呼吁厂商关注屏幕技术对易感人群的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.appleheadlines.com/macbook-pro-oled-eye-strain-pwm-flicker/">MacBook Pro OLED Eye Strain &amp; PWM Flicker: 7 Moves - AH</a></li>
<li><a href="https://daily.dev/posts/the-macbook-pro-s-oled-pwm-problem-when-a-better-display-becomes-worse-to-use-bxu5e2tu9">The MacBook Pro&#x27;s OLED PWM Problem: When a &#x27;Better&#x27;...</a></li>

</ul>
</details>

**标签**: `#hardware`, `#display technology`, `#user experience`, `#accessibility`

---

<a id="item-tech-news-7"></a>
### [微软 365 故障致酒店氯气泄漏，15 人中毒](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

据报道，微软 365 的服务中断导致一家酒店未能及时收到自动化安全系统发出的氯气超量警报邮件，最终造成泳池氯气泄漏，15 名住客中毒。此次事件暴露出该酒店安全关键系统对云端邮件服务的高度依赖，缺乏本地或多重备份机制。事故发生在德国 Phantasialand 酒店，自动加氯系统因未被及时干预而持续过量投放氯气。微软 365 故障为诱因，但系统设计缺陷是事故的根本原因。

hackernews · DeepLogin · 11月15日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=50509411)

**「事件背景」** 据报道，德国一家主题公园酒店因自动化安全系统依赖的微软 365 云服务发生长时间故障，导致关键的化学品过量警报邮件未能送达工作人员，最终造成 15 名客人因氯气中毒受伤。此次事件的直接原因是泳池自动加药系统出现故障，过量投放了氯气，而本应通过邮件发出的维护安全警报因微软云服务中断未被及时获知。该事件凸显了安全关键系统对云服务依赖的潜在风险。

**「实际影响」** 受影响的酒店需重新评估其安全关键系统的通信和报警机制，避免单点云服务失效导致严重后果。其他依赖云服务的自动化设施也应检视自身的冗余和本地应急措施。

**「社区讨论」** 多位评论者认为，酒店将安全报警完全依赖于云端邮件服务是严重设计失误，微软并非事故主因。部分专业人士指出，类似自动加氯系统本就容易因传感器或通信故障导致过量投放，必须有本地人工或多重备份保障。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://timesofindia.indiatimes.com/technology/tech-news/a-hotel-in-germany-reports-chlorine-gas-poisoning-after-email-warning-system-fails-due-to-microsoft-365-outage-guests-taken-to-hospital/articleshow/135864509.cms">A hotel in Germany reports Chlorine gas poisoning after email ...</a></li>
<li><a href="https://windowsforum.com/news/outlook-outage-blocked-phantasialand-pool-alerts-before-chlorine-incident-injured-15.452435/">Outlook Outage Blocked Phantasialand Pool Alerts Before ...</a></li>
<li><a href="https://www.yahoo.com/news/world/articles/microsoft-365-outage-leads-chlorine-154113086.html?fr=sycsrp_catchall">Microsoft 365 outage leads to chlorine gas poisoning of 15 ...</a></li>

</ul>
</details>

**标签**: `#cloud-dependency`, `#system-design`, `#automation`, `#safety-critical`

---

<a id="item-tech-news-8"></a>
### [B300 GPU 上 cudaMemcpy 提速 5 倍新工具发布](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

一款新工具可将 B300 GPU 上 cudaMemcpy 的 pageable 数据传输速度提升至原来的 5 倍。在实际基准测试中，1GB 张量从 CPU 传输到 GPU 的速度由 10.2 GB/s 提升至 51.5 GB/s。该工具适用于需要大量数据搬运的机器学习和高性能计算场景，用户可通过命令行集成使用。当前发布未提供详细技术原理说明。

reddit · r/MachineLearning · /u/makneeee · 11月15日 18:20

**「背景介绍」** cudaMemcpy 是 NVIDIA CUDA 平台中用于在主机（CPU）和设备（GPU）之间传输数据的核心 API。通常，使用 pageable（可分页）内存进行数据传输时，速度会受到操作系统内存管理机制的影响，导致性能低于使用 pinned（锁页）内存。B300 是 NVIDIA 的一款高性能 GPU，广泛应用于机器学习和高性能计算场景。此前，提升 pageable 内存传输速率一直是性能优化的难点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agihunt.info/en/p/1a1e07bf9febb7c90bad763fb45">cudamemcpy-tuner speeds up pageable cudaMemcpy… · AGI Hunt</a></li>
<li><a href="https://agihunt.info/p/1a1e07bf9febb7c90bad763fb45">开源工具让 B300 上 cudaMemcpy 分页拷贝提速 5 倍 · AGI Hunt</a></li>
<li><a href="https://stackoverflow.com/questions/19268428/pinned-memory-in-cuda-and-cudamemcpy">gpu - Pinned memory in CUDA and cudamemcpy () - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#GPU`, `#performance`, `#machine learning`, `#tools`

---

<a id="item-tech-news-9"></a>
### [推理模型训练外早停新方法：输出层线性探针](https://www.reddit.com/r/MachineLearning/comments/1xx1xdm/trainingfree_early_exit_for_reasoning_models_a/) ⭐️ 7.0/10

一项 Reddit 帖子介绍了一种无需训练即可实现推理模型早停的新方法：通过修改输出层中特定（&lt;/think&gt;）token 的权重行，将线性探针直接嵌入模型权重。该方法无需重新训练模型，也不需要推理时额外代码，适用于如 Qwen3.5-4B、DeepSeek V4.1 Flash 等主流大模型。初步实验显示，在数学和代码任务中，模型在保持准确率的同时，推理 token 数减少 40%-84%。目前结果基于小样本，主要在数学任务上验证，泛化能力和极端场景下的表现尚需进一步评估。

reddit · r/MachineLearning · /u/Good-Presentation-23 · 11月15日 17:52

**「背景介绍」** 以往的推理模型早停方法通常依赖于输出层启发式或经过训练的探针模型，通过跳过冗余推理步骤来减少过度思考，但这些方法往往需要额外的推理计算或外部标注数据。近期也有无训练的早停方法尝试直接在模型输出层插入探针，以在无需额外推理或代码修改的情况下实现早停，但存在模型仍可能继续生成推理内容的局限（如虚假的链式思考终止）。本次提出的方法是在输出层特定权重行内嵌入线性探针，属于这一类无训练、结构简单的早停技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2602.02010v1">NEAT: Neuron-Based Early Exit for Large Reasoning Models</a></li>
<li><a href="https://aiweekly.co/alerts/paper-injected-think-doesnt-cleanly-halt-lrm-reasoning">Paper: Injected Doesn&#x27;t Cleanly Halt LRM Reasoning</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#language models`, `#model efficiency`, `#reasoning`

---

<a id="item-tech-news-10"></a>
### [Marimba：开源轻量级语音决策模型发布](https://www.reddit.com/r/MachineLearning/comments/1xwzsm4/marimba_a_system_one_model_for_speech_r/) ⭐️ 7.0/10

Marimba 是一个新发布的开源轻量级语音模型，专为音频上的快速、类型化决策（如是/否、选项或分数）而设计。该模型基于冻结的 Qwen3-ASR-0.6B，支持多种语音相关任务，包括零样本（zero-shot）下的词语和语言判断，以及语音活动、说话轮次结束、说话人变化和人数检测等。Marimba 提供了开放权重（Apache-2.0 许可）、代码、基准测试，并即将发布论文，用户可通过 pip 安装 marimba-audio。该模型适用于需要高效语音分析的开发者和研究者。

reddit · r/MachineLearning · /u/solanotodesch · 11月15日 16:30

**「背景」** Qwen3-ASR-0.6B 是 Qwen 团队开发的一款开源、多语言语音识别模型，主打轻量级和开放权重，适用于语音转文本等任务。该模型作为 Marimba 的基础，被“冻结”后用于高效、快速地处理语音相关的多种任务。Qwen3-ASR-0.6B 以其紧凑体积和开放生态，为开发者和研究者提供了灵活的语音处理能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mindstudio.ai/models/qwen3-asr-0-6b-deepinfra">Qwen 3 ASR 0 . 6 B — AI Model | MindStudio</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3-0.6B">Text Generation model with 0.8 B parameters. Download, explore files...</a></li>
<li><a href="https://benchlm.ai/models/qwen3-asr-0-6b">Qwen 3 - ASR 0 . 6 B Context, Specs &amp; Sources (September 2026)</a></li>

</ul>
</details>

**标签**: `#speech-recognition`, `#open-source`, `#machine-learning`, `#audio-processing`

---

<a id="item-tech-news-11"></a>
### [MariaDB 驱动的多语言维基百科历史对齐项目亮相黑客松](https://www.reddit.com/r/MachineLearning/comments/1xwttxo/hackathon_project_for_mariadbs_wikipedia_through/) ⭐️ 7.0/10

在 Espoo 举办的 Junction 黑客松上，开发者推出了 Parallax 项目，实现了对芬兰语、瑞典语、德语、英语、俄语、爱沙尼亚语和乌克兰语七种维基百科版本的历史对齐与比较。该项目利用 MariaDB 的系统版本表存储每个版本的句子，并用 bge-m3 模型生成 1024 维句向量，通过 SQL 自连接和 VEC\_DISTANCE\_COSINE 函数在任意历史时间点匹配各语言版本的相似句子。项目还集成了 Gemini 3.8 Flash 模型对候选句对进行语义判别和翻译，支持跨语言内容追踪和历史分析。该系统目前已处理 87 万余条修订，句向量嵌入速度约为每秒 4555 句。

reddit · r/MachineLearning · /u/Loxbey · 11月15日 12:03

**「背景信息」** MariaDB 是一个开源关系型数据库管理系统，支持系统版本表（system-versioned tables），可用于追踪数据随时间的变化。MariaDB 基金会定期举办黑客松活动，鼓励开发者利用其数据库功能进行创新项目。此次“Wikipedia Through Time”挑战要求参赛者结合向量检索和系统版本表技术，探索多语言维基百科内容的历史对齐与比较。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MariaDB">MariaDB - Wikipedia</a></li>
<li><a href="https://github.com/danielbacsur/junction-x-wikipedia-hackathon">GitHub - danielbacsur/junction-x-wikipedia-hackathon: A time ...</a></li>
<li><a href="https://mariadb.org/projects/hackathons/">MariaDB Hackathons - MariaDB.org</a></li>

</ul>
</details>

**标签**: `#natural-language-processing`, `#multilingual`, `#databases`, `#hackathon`

---

<a id="item-tech-news-12"></a>
### [特斯拉 Cybercab 推出 299 美元/月自动驾驶订阅](https://www.tesla.com/configurator/api/v4/terms?category=autonomy_subs&amp;amp;locale=en_US&amp;amp;model=cc&amp;amp;saleType=Sale) ⭐️ 7.0/10

特斯拉正式公布了 Cybercab 自动驾驶出租车的订阅协议，车辆售价为 29,990 美元，但用户需每月支付 299 美元订阅费，否则车辆将无法运行。特斯拉有权提前一个月通知调整订阅价格，若用户欠费或违规使用，可能被暂停或取消订阅，累计三次警告将导致自动驾驶功能停用一周。Cybercab 仅允许在指定区域内运营，且禁止接入未经授权的网约车、配送或租赁平台。

telegram · zaihuapd · 11月15日 01:10

**「背景信息」** 特斯拉 Cybercab 是该公司最新推出的自动驾驶出租车产品，定位于 Robotaxi 车队，采用无方向盘和踏板的设计。根据特斯拉官方支持页面，Cybercab 旨在推动自动驾驶出行新时代，并已向部分个人用户开放购买，售价为 29,990 美元，需额外支付每月 299 美元的自动驾驶订阅费用。此前，特斯拉的自动驾驶功能（如 FSD）主要面向普通车主，且仍需人工监督，而 Cybercab 则强调完全自动驾驶和严格的订阅管理。

**「影响」** 用户在购买 Cybercab 后，必须持续支付订阅费用才能正常使用车辆，且运营范围和用途受到严格限制，这对传统车辆所有权和使用习惯带来重大变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tesla.com/support/robotaxi/cybercab">Cybercab Frequently Asked Questions | Tesla Support</a></li>
<li><a href="https://www.zerohedge.com/technology/tesla-opens-cybercab-orders-select-customers-personal-use">Tesla Opens Cybercab Orders To &quot;Select Customers...&quot; | ZeroHedge</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#software licensing`, `#AI hardware`, `#technology industry`

---

<a id="item-tech-news-13"></a>
### [传鲁比奥与 Anthropic 涉推动黄仁勋离职与芯片出口限制](https://www.washingtonpost.com/technology/2026/11/13/behind-jensen-huangs-spy-scandal-shadow-war-trumps-ear-china/) ⭐️ 7.0/10

据《华盛顿邮报》报道，英伟达创始人黄仁勋的离职疑似与美国政界及 Anthropic 等科技公司高管的幕后操作有关。报道称，黄仁勋因反对对华芯片出口限制并与特朗普关系密切，激怒了美国国安官员和对华鹰派，促使参议员鲁比奥等人通过情报备忘录向总统施压。与此同时，Anthropic 被怀疑向媒体提供调查线索，推动相关丑闻曝光，因其一直主张对华芯片出口实施更严厉限制，并推动在 GPU 中加入固件级追踪机制。当前，相关芯片出口限制法案的阻力已减弱，国会正推动将更严格的条款纳入国防法案。

telegram · zaihuapd · 11月15日 08:08

**「背景信息」** 近期，英伟达 CEO 黄仁勋因个人丑闻和与美国政府在对华芯片出口政策上的分歧而辞职，引发了关于其离职背后是否存在政治操作的广泛猜测。美国国会参议员鲁比奥据称曾基于 CIA 情报撰写强硬备忘录，推动对黄仁勋施压，而媒体和行业评论认为 Anthropic 及其高管可能向记者提供了调查线索，因其与英伟达在对华芯片政策上存在直接利益冲突。此前，黄仁勋曾公开反对在芯片中加入追踪和后门功能，并成功游说放宽对华芯片出口，而 Anthropic 一直主张更严格的出口限制和技术管控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=7UX_h-DVUuc">Who Took Down Jensen Huang , and Why? - YouTube</a></li>
<li><a href="https://www.zerohedge.com/ai/was-jensen-taken-out-over-open-source-sacks-says-anthropics-safetyist-allies-want-all-models-and">Was Jensen Taken Out Over Open Source? Sacks Says... | ZeroHedge</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/14/jensen-huang-affair-nvidia-nightmare">‘ Jensen Huang lost his mind’: how AI ’s smartest man... | The Guardian</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#hardware`, `#technology industry`, `#geopolitics`

---

<a id="item-tech-news-14"></a>
### [华为云上线开源盘古模型 openPangu-2.1-Pro](https://mp.weixin.qq.com/s/8JfFmscBTDl_mPQMycD8Nw) ⭐️ 7.0/10

华为云于 11 月 15 日在 MaaS 模型即服务平台上线了开源盘古模型 openPangu-2.1-Pro。该模型针对 Agent 开发、AI 编码和推理优化进行了能力升级，基于 10 万余条专项数据优化了 Skills 触发与工具调用。openPangu-2.1-Pro 重点适配鸿蒙 ArkTS 开发、升腾算子生成，并已集成至智果 AgentArts、码道 CodeArts、果办 OfficeAce 等华为产品。推理服务定价为输入 0.8 元/百万 tokens、输出 3.2 元/百万 tokens，缓存命中输入为 0.016 元/百万 tokens。

telegram · zaihuapd · 11月15日 16:03

**「背景介绍」** 盘古（Pangu）模型是华为推出的大型语言模型系列，最初面向政务、金融、制造等行业应用，并基于华为云平台提供服务。openPangu-2.1-Pro 是该系列在华为云 MaaS（模型即服务）平台上的新版本，重点升级了对鸿蒙生态任务和升腾硬件底层算子的支持，旨在增强模型在特定场景下的适配能力和推理效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/en/item/openPangu-2.1-Pro/7509035">openPangu-2.1-Pro（Huawei Cloud Pangu Series Large Language ...</a></li>
<li><a href="https://www.huaweicloud.com/intl/en-us/product/pangu.html">PanguLM_Large Models-HUAWEI CLOUD</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI models`, `#cloud platforms`, `#software engineering`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [Cantor Fitzgerald 因与 Nvidia 相关交易及高管关系受到审查](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 8.0/10

在美国情报部门警告和出口管制加强的背景下，Cantor Fitzgerald 因其与 Nvidia 的业务往来及领导层关系受到关注，该公司 2025 年 9 月至 2026 年 3 月间持有的 Nvidia 股票数量下降了近 50%，据 CNBC 分析其证券申报文件显示。

rss · CNBC Finance · 11月15日 19:58

**「背景」** 美国商务部长霍华德·卢特尼克因与前英伟达（Nvidia）CEO 黄仁勋的私人关系及其家族企业与英伟达的业务往来，正面临外界对其在对华芯片出口管控方面监督不力的质疑。近期，财政部长和国会成员也公开表达了对卢特尼克在相关出口管制决策中的角色和利益冲突的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/lutnick-nvidia-ai-chips-china/">Lutnick should have prevented the diversion of sensitive ...</a></li>
<li><a href="https://finance.yahoo.com/technology/ai/articles/scott-bessent-lutnick-clash-over-235529522.html?fr=sycsrp_catchall">Scott Bessent and Lutnick clash over Nvidia chips and China</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/13/nvidia-scandal-sparks-us-national-security-concerns-china">Nvidia scandal: Howard Lutnick under pressure over alleged ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Cantor Fitzgerald`, `#export controls`, `#conflict of interest`, `#technology sector`

---

<a id="item-finance-news-2"></a>
### [美法官允许美光、三星等 DRAM 价格操纵案继续审理](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 7.0/10

美国法官驳回了美光、三星和 SK 海力士关于撤销 DRAM 价格操纵集体诉讼的动议，认为存在三家公司合谋的合理证据，因此案件将继续审理。

telegram · zaihuapd · 11月15日 16:39

**「背景」** 此前，三家主要内存芯片制造商美光、三星和 SK 海力士被指控在一年内多次同步限制 DRAM（动态随机存取存储器）供应，导致价格大幅上涨，原告为 17 名个人和小企业。该案为美国加州北区法院受理的集体反垄断诉讼，三家公司曾请求法院驳回诉讼但被拒绝。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/articles/judge-denies-motion-dismiss-dram-152445837.html?fr=sycsrp_catchall">Judge denies motion to dismiss DRAM price-fixing lawsuit ...</a></li>
<li><a href="https://wccftech.com/federal-judge-rejects-memory-makers-defense-samsung-micron-sk-hynix-dram-shortage-lawsuit/">Federal Judge Rejects Memory Makers’ Defense To ... - Wccftech</a></li>
<li><a href="https://www.techpowerup.com/354863/samsung-sk-hynix-and-micron-fail-to-get-dram-antitrust-suit-dismissed">Samsung, SK hynix, and Micron Fail to Get DRAM Antitrust Suit ...</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#semiconductors`, `#legal`, `#market regulation`

---