---
layout: default
title: "Horizon Summary: 2026-11-15 (ZH)"
date: 2026-11-15
lang: zh
---

> 从 34 条内容中筛选出 16 条重要资讯。

---

**科技新闻**
1. [SpaceX 星舰首次实现轨道返回后机械臂捕获](#item-tech-news-1) ⭐️ 9.0/10
2. [Meta FAIR 与 NYU：多模态视觉编码器设计系统性研究](#item-tech-news-2) ⭐️ 8.0/10
3. [多人游戏用本地世界模型实时生成玩家视角](#item-tech-news-3) ⭐️ 8.0/10
4. [美团开源 LongCat-2.5，未用英伟达 GPU 训练](#item-tech-news-4) ⭐️ 8.0/10
5. [华为云发布开源盘古模型 openPangu-2.1-Pro](#item-tech-news-5) ⭐️ 8.0/10
6. [MacBook Pro OLED 屏幕 PWM 闪烁问题引发关注](#item-tech-news-6) ⭐️ 7.0/10
7. [Microsoft 365 故障致酒店 15 人氯气中毒](#item-tech-news-7) ⭐️ 7.0/10
8. [B300 上 cudaMemcpy 可提速 5 倍的新工具发布](#item-tech-news-8) ⭐️ 7.0/10
9. [推理模型训练免早停新方法：线性探针嵌入输出层](#item-tech-news-9) ⭐️ 7.0/10
10. [Marimba：开源高效语音决策模型发布](#item-tech-news-10) ⭐️ 7.0/10
11. [多语言维基百科历史版本句子比对工具发布](#item-tech-news-11) ⭐️ 7.0/10
12. [TimeCues Studio：开源音乐结构标注工具发布](#item-tech-news-12) ⭐️ 7.0/10
13. [特斯拉 Cybercab 推出 299 美元/月自动驾驶强制订阅](#item-tech-news-13) ⭐️ 7.0/10
14. [传 Anthropic 与美官员联手推动黄仁勋下台及 AI 芯片出口限制](#item-tech-news-14) ⭐️ 7.0/10

**财经新闻**
1. [坎托·菲茨杰拉德与英伟达关系引发美国政府审查](#item-finance-news-1) ⭐️ 7.0/10
2. [美法官允许美光、三星等 DRAM 价格操纵案继续审理](#item-finance-news-2) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [SpaceX 星舰首次实现轨道返回后机械臂捕获](https://www.spacex.com/launches/starship-flight-15) ⭐️ 9.0/10

SpaceX 宣布，星舰在第 15 次试飞中首次实现了轨道返回后由发射塔机械臂直接捕获，飞船完成约 22.5 小时飞行并绕地球 14 圈后安全返回得克萨斯州发射基地。这一突破标志着 SpaceX 在大型航天器回收与重复使用技术上取得了重要进展。本次任务还成功部署了 26 颗新一代星链 V3 卫星，但超重型助推器未能按计划回收，最终在墨西哥湾溅落，未实现两级同时回收。

telegram · zaihuapd · 11月14日 23:49

**「背景」** 此前，SpaceX 的星舰项目一直致力于实现大型航天器的可重复使用。传统上，火箭回收多采用降落伞或推进器着陆等方式，但直接由发射塔机械臂捕获返回的航天器尚属首次。此次捕获不仅验证了机械臂捕捉技术的可行性，也为未来更高频次、低成本的航天发射奠定了基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.foxbusiness.com/technology/spacex-makes-history-starship-spacecraft-caught-launch-tower-first-time">SpaceX makes history with first -ever Starship spacecraft catch at...</a></li>
<li><a href="https://www.nine.com.au/world-news/usa/spacex-s-starship-captured-by-launch-pad-arms-in-a-dramatic-first-as-it-returns-from-orbit-20261115-p61e8f.html">SpaceX ’s Starship captured by launch pad arms in a dramatic first as...</a></li>
<li><a href="https://www.nytimes.com/2026/11/14/science/spacex-starship-first-catch.html">SpaceX Makes History With Successful Rocket Catch in Texas</a></li>

</ul>
</details>

**标签**: `#space technology`, `#hardware`, `#automation`, `#industry news`

---

<a id="item-tech-news-2"></a>
### [Meta FAIR 与 NYU：多模态视觉编码器设计系统性研究](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Meta FAIR 与纽约大学（NYU）对多模态大语言模型（MLLMs）中的视觉编码器设计进行了系统性分析，训练了 200 多个模型，统一数据和算力预算。研究发现，视觉编码器的单独预训练并非必要，无论采用对比学习、自监督或图像字幕等多种预训练目标，最终在视觉问答（VQA）任务上与从零训练的编码器表现相当。相反，模型必须为视觉分支分配专用参数，否则在所有规模下性能显著下降，且需要约三倍算力才能追平。

reddit · r/MachineLearning · /u/trungh98 · 11月15日 17:38

**「背景介绍」** 多模态大语言模型（MLLMs）通常结合视觉编码器和语言模型，以实现图文理解等任务。此前，业界在视觉编码器的设计上存在分歧：有的模型（如 Gemma 4 12B）去除了视觉编码器，有的（如 Kimi K3）则从头训练编码器，还有的（如 Inkling 2 Small）重新引入了编码器。主流做法往往将视觉编码器单独预训练，并在多模态训练中固定或微调，但不同模型的数据、算力和训练流程差异较大，导致难以直接比较各自设计选择的优劣。

**标签**: `#multimodal-models`, `#vision-encoders`, `#machine-learning-research`, `#model-architecture`, `#AI`

---

<a id="item-tech-news-3"></a>
### [多人游戏用本地世界模型实时生成玩家视角](https://www.reddit.com/r/MachineLearning/comments/1xx4ta3/we_made_a_multiplayer_game_where_each_players/) ⭐️ 8.0/10

一个多人游戏原型现已开放测试，玩家需使用 RTX 3080 或更高配置的显卡（也有实验性 Mac 版本），每位玩家的游戏视角由本地运行的世界模型和扩散变换器实时生成。该模型基于近 4,000 小时、10 人 CS:GO 机器人对战的公开数据集训练，所有 POV 和输入以 16 Hz 对齐。游戏通过轻量级服务器同步状态，玩家本地根据服务器状态、操作和前一帧生成画面。目前仅支持一张小地图和手枪，细节表现有限，但已可多人游玩。数据集和测试版均已开放下载。

reddit · r/MachineLearning · /u/bengal7ion · 11月15日 19:46

**「背景介绍」** 扩散变换器（Diffusion Transformer）是一种结合了扩散模型和变换器架构的生成式人工智能方法，近年来被用于图像生成和世界建模等任务。世界模型（World Model）指的是通过机器学习方法对环境动态进行建模，使得智能体能够基于模型预测未来状态或生成环境视图。此前，扩散模型已被证明在生成高保真视觉细节方面具有优势，尤其是在强化学习和游戏环境的模拟中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2412.03572">Navigation World Models</a></li>
<li><a href="https://github.com/eloialonso/diamond">GitHub - eloialonso/diamond: DIAMOND ( DIffusion As a Model Of...)</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#world models`, `#diffusion models`, `#multiplayer gaming`, `#computer systems`

---

<a id="item-tech-news-4"></a>
### [美团开源 LongCat-2.5，未用英伟达 GPU 训练](https://the-decoder.com/meituan-releases-a-1-6-trillion-parameter-agent-model-that-never-touched-an-nvidia-gpu/) ⭐️ 8.0/10

美团 LongCat 团队正式开源了 LongCat-2.5 多模态智能体模型的权重，并采用 MIT 许可证，允许商用。官方声明该模型全程使用华为升腾加速卡训练，未用英伟达 GPU。LongCat-2.5 支持文本、图像和视频输入，每个 token 激活约 480 亿参数，在 Terminal Bench v2.1 测试中得分 88.4，略低于 Claude Opus 5 的 89.1。该模型专为自主完成复杂多步骤任务（如编程）设计。

telegram · zaihuapd · 11月15日 11:08

**「背景信息」** LongCat-2.5 是美团推出的一款原生多模态大模型，专为长时序智能体任务（如复杂编程）设计。该模型支持文本、图像和视频输入，单 token 激活约 480 亿参数，具备 100 万 token 的上下文窗口。此前，主流大模型训练多依赖英伟达 GPU，而 LongCat-2.5 全程采用华为升腾加速卡，体现了中国在 AI 算力自主化方面的探索。

**「影响」** 开发者和企业可在无需英伟达 GPU 的情况下，基于中国本土硬件复现和部署该模型，降低了对特定硬件供应链的依赖，并可合法商用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.longcatai.org/">LongCat AI - LongCat - 2 . 5 Native Multimodal Agent Model (1.6T)</a></li>
<li><a href="https://llm-stats.com/models/longcat-2.5">LongCat - 2 . 5 Benchmarks, Pricing &amp; Context Window</a></li>

</ul>
</details>

**标签**: `#open source`, `#large language models`, `#hardware alternatives`, `#AI research`, `#China tech`

---

<a id="item-tech-news-5"></a>
### [华为云发布开源盘古模型 openPangu-2.1-Pro](https://mp.weixin.qq.com/s/8JfFmscBTDl_mPQMycD8Nw) ⭐️ 8.0/10

华为云于 11 月 15 日在 MaaS 模型即服务平台上线了开源盘古模型 openPangu-2.1-Pro，重点提升了 Agent 开发、AI 编码和推理优化能力。该模型基于 10 万余条专项数据优化了 Skills 触发与工具调用，特别适配鸿蒙 ArkTS 开发和升腾算子生成，并已集成至智果 AgentArts、码道 CodeArts、果办 OfficeAce 等产品。推理输入费用为 0.8 元/百万 tokens，输出为 3.2 元/百万 tokens，缓存命中输入仅需 0.016 元/百万 tokens。该模型以开源形式发布，面向开发者和企业用户。

telegram · zaihuapd · 11月15日 16:03

**「背景信息」** openPangu-2.1-Pro 是华为云 MaaS 平台推出的开源盘古模型的升级版本。此前，openPangu-2.0-Pro 作为 MoE（混合专家）模型，基于升腾硬件训练，拥有 5050 亿总参数和 18 亿激活参数，支持 512k 上下文长度，并以 34 万亿 tokens 进行预训练。2023 年 11 月初，华为云曾宣布将逐步下线 Pangu 2.0 相关模型，建议用户迁移至其他替代方案，因此 2.1-Pro 的上线为用户提供了新的升级选择。

**「影响」** 开发者和企业可利用 openPangu-2.1-Pro 在华为云平台上更高效地进行 AI Agent 开发和 AI 编码，尤其是在鸿蒙系统和升腾硬件环境下，降低了推理成本并提升了工具集成度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/openpangu/openPangu-2.0-Pro/blob/main/README_EN.md">README_EN.md · openpangu/ openPangu - 2 .0- Pro at main</a></li>
<li><a href="https://www.kucoin.com/news/flash/huawei-cloud-to-discontinue-pangu-2-0-models-recommends-deepseek-and-glm-alternatives">Huawei Cloud to Discontinue Pangu 2 .0 Models ... | KuCoin</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI models`, `#cloud platforms`, `#software engineering`

---

<a id="item-tech-news-6"></a>
### [MacBook Pro OLED 屏幕 PWM 闪烁问题引发关注](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

新款 MacBook Pro 采用 OLED 屏幕，但其脉宽调制（PWM）频率较低，导致部分用户出现视觉不适和闪烁敏感问题。文章分析了 PWM 频率（如 240Hz、480Hz、960Hz）及其对用户体验的影响，并指出 OLED 屏幕在高端笔记本普及后，相关健康和可用性问题日益突出。社区讨论涉及技术细节、用户主观体验以及对苹果产品设计选择的质疑。该问题主要影响对屏幕闪烁敏感的用户，尤其是在低亮度或特定使用场景下。

hackernews · MacAnorak · 11月15日 13:15 · [社区讨论](https://news.ycombinator.com/item?id=50506719)

**「背景信息」** OLED 显示屏常采用脉宽调制（PWM）来调节亮度，这种方式会导致屏幕在低亮度下出现肉眼可见或不可见的闪烁。部分用户对 PWM 闪烁高度敏感，可能出现眼睛疲劳、头痛等不适症状。随着 OLED 屏幕在高端笔记本（如 MacBook Pro）中的普及，关于 PWM 闪烁对用户体验影响的讨论也日益增多，苹果社区和其他品牌用户均有类似反馈。

**「影响」** 对闪烁敏感的用户在使用新款 MacBook Pro OLED 屏幕时，可能会出现眼睛疲劳、注意力难以集中等不适症状，部分用户甚至可能因此无法正常使用该设备。开发者和硬件设计师需关注 PWM 频率设置对用户健康的潜在影响。

**「社区讨论」** 有用户质疑实际 PWM 频率的测量方法和解释，认为 OLED 屏幕的 PWM 行为比部分测试结果更复杂。部分评论者分享了自身对屏幕闪烁的敏感体验，并对苹果采用低 PWM 频率的决策表示惊讶和担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://discussions.apple.com/thread/254749941?page=2">Severe Eye Strain due to OLED PWM Dimming - Apple Community</a></li>

</ul>
</details>

**标签**: `#hardware`, `#display technology`, `#user experience`, `#Apple`

---

<a id="item-tech-news-7"></a>
### [Microsoft 365 故障致酒店 15 人氯气中毒](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

由于 Microsoft 365 服务中断，某酒店的安全系统未能通过电子邮件及时发出氯气过量警报，导致自动加药系统向泳池过量投放氯气，最终造成 15 名住客中毒。此次事件暴露出该酒店安全关键系统对云端邮件服务的高度依赖，缺乏本地或多渠道冗余机制。该事故引发了业界对安全系统架构设计和云服务可靠性的广泛讨论。

hackernews · DeepLogin · 11月15日 18:36 · [社区讨论](https://news.ycombinator.com/item?id=50509411)

**「事件背景」** 据报道，德国一家酒店的桑拿区维护安全系统依赖于 Microsoft 365（Outlook）发送自动警报邮件。当酒店泳池的加药系统发生故障，导致过量投放氯气时，原本应通过邮件通知工作人员的安全警报因 Microsoft 365 云服务中断未能送达，最终导致 15 名客人吸入氯气受伤。此次事件凸显了关键安全系统对云服务依赖的风险。

**「实际影响」** 受影响的酒店需重新评估其安全系统的通信和报警机制，增加本地备份或多渠道通知手段，以防止类似因云服务中断导致的安全事故再次发生。

**「社区讨论」** 多位评论者认为，安全关键系统完全依赖单一云服务是严重的设计失误，强调应采用更具弹性和冗余的架构。部分技术人员指出，酒店应对自身系统负责，而不应将责任归咎于云服务提供商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.yahoo.com/news/world/articles/microsoft-365-outage-leads-chlorine-154113086.html?fr=sycsrp_catchall">Microsoft 365 outage leads to chlorine gas poisoning of 15 ...</a></li>
<li><a href="https://windowsforum.com/news/outlook-outage-blocked-phantasialand-pool-alerts-before-chlorine-incident-injured-15.452435/">Outlook Outage Blocked Phantasialand Pool Alerts Before ...</a></li>
<li><a href="https://techbytes.app/posts/microsoft-365-outage-leads-to-chlorine-gas-poisoning-of-15/">Microsoft 365 outage leads to chlorine gas poisoning of 15 ...</a></li>

</ul>
</details>

**标签**: `#cloud reliability`, `#system architecture`, `#IoT`, `#safety-critical systems`

---

<a id="item-tech-news-8"></a>
### [B300 上 cudaMemcpy 可提速 5 倍的新工具发布](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

一款新工具实现了在 B300 GPU 上对 cudaMemcpy pageable 传输速度的显著提升，实测将 1GB 张量从 CPU 传输到 GPU 的速度从 10.2 GB/s 提升到 51.5 GB/s，提升约 5 倍。该工具已开源，并提供了详细的代码和基准测试，适用于需要高效数据搬运的机器学习工作流。

reddit · r/MachineLearning · /u/makneeee · 11月15日 18:20

**「背景介绍」** cudaMemcpy 是 NVIDIA CUDA 平台中用于在主机（CPU）和设备（GPU）之间传输数据的核心 API，尤其在机器学习等高性能计算场景中广泛使用。传统上，pageable 内存的 cudaMemcpy 传输速度受限，尤其在 B300 等 GPU 上，通常只能达到约 10 GB/s 的速率。近期有开发者发布了名为 cudamemcpy-tuner 的开源工具，显著提升了 B300 上 pageable cudaMemcpy 的传输速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agihunt.info/en/p/1a1e07bf9febb7c90bad763fb45">cudamemcpy-tuner speeds up pageable cudaMemcpy… · AGI Hunt</a></li>

</ul>
</details>

**标签**: `#GPU`, `#performance`, `#machine-learning`, `#tools`

---

<a id="item-tech-news-9"></a>
### [推理模型训练免早停新方法：线性探针嵌入输出层](https://www.reddit.com/r/MachineLearning/comments/1xx1xdm/trainingfree_early_exit_for_reasoning_models_a/) ⭐️ 7.0/10

一项 Reddit 帖子提出了一种无需训练即可实现推理模型早停的新方法：通过线性探针（linear probe）直接修改输出层中&lt;/think&gt;标记对应的权重行。该方法仅需一次性编辑权重文件，无需额外推理代码，适用于如 Qwen3.5-4B 和 DeepSeek V4.1 Flash 等模型。实测在数学和代码任务中，模型在保持准确率的同时，平均减少了 40%至 84%的推理 token 数。该方法的创新点在于将探针直接嵌入输出层权重，无需额外组件，且可在原始模型推理记录上离线评估效果。

reddit · r/MachineLearning · /u/Good-Presentation-23 · 11月15日 17:52

**「背景介绍」** 在大语言模型（LLM）进行链式推理（CoT）时，模型常常在找到正确答案后继续生成大量冗余的“思考”内容。为提升推理效率，近期已有研究提出了无需额外训练的动态早停方法，使模型在推理量足够时自动提前终止生成。这类方法通常通过分析隐藏状态，判断模型是否已完成主要推理任务，从而实现早停。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2504.15895v2">Dynamic Early Exit in Reasoning Models - arXiv.org</a></li>
<li><a href="https://arxiv.org/html/2504.15895v1">Dynamic Early Exit in Reasoning Models - arXiv.org</a></li>
<li><a href="https://openreview.net/forum?id=NpU7ZXafRi">Dynamic Early Exit in Reasoning Models - OpenReview</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#large language models`, `#model optimization`, `#reasoning`

---

<a id="item-tech-news-10"></a>
### [Marimba：开源高效语音决策模型发布](https://www.reddit.com/r/MachineLearning/comments/1xwzsm4/marimba_a_system_one_model_for_speech_r/) ⭐️ 7.0/10

Marimba 是一个基于 Qwen3-ASR-0.6B 冻结骨干的开源语音分析模型，专为高效、轻量级的语音决策任务设计。该模型支持零样本（zero-shot）语音识别、语音活动检测、说话人变化与数量判断等多种语音相关任务，并已开放代码、模型权重和基准测试，采用 Apache-2.0 许可证。用户可通过 pip 安装 marimba-audio 并在线体验。Marimba 适用于需要快速、结构化语音决策的开发者和研究者。

reddit · r/MachineLearning · /u/solanotodesch · 11月15日 16:30

**「背景」** 自动语音识别（ASR）模型近年来在语音理解和处理任务中广泛应用，常见评估指标包括词错误率、推理速度和模型体积。Qwen3-ASR-0.6B 是一款开源的中小型语音识别模型，支持多种语音任务。Marimba 基于该模型，结合零样本推理和多任务能力，进一步拓展了语音模型在决策型任务中的应用场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/spaces/hf-audio/open_asr_leaderboard">Open ASR Leaderboard - a Hugging Face Space by hf-audio</a></li>

</ul>
</details>

**标签**: `#speech-recognition`, `#open-source`, `#machine-learning`, `#model-release`

---

<a id="item-tech-news-11"></a>
### [多语言维基百科历史版本句子比对工具发布](https://www.reddit.com/r/MachineLearning/comments/1xwttxo/hackathon_project_for_mariadbs_wikipedia_through/) ⭐️ 7.0/10

在 Espoo 举办的 Junction 黑客松上，一个名为 Parallax 的项目实现了对维基百科七种语言（芬兰语、瑞典语、德语、英语、俄语、爱沙尼亚语和乌克兰语）历史版本的句子级比对。该工具利用系统版本表存储 87 万余条修订，将每个句子嵌入为 1024 维向量，并通过 SQL 查询结合向量相似度和 Gemini 3.8 Flash 大模型进行跨语言、跨时间点的内容对齐和差异分析。项目还对模型判别准确性进行了初步人工评估，并开源了代码和演示。该方案主要面向需要多语言、时序文本分析的数据库和机器学习社区。

reddit · r/MachineLearning · /u/Loxbey · 11月15日 12:03

**「背景信息」** MariaDB 是一个开源关系型数据库管理系统，支持系统版本表（system-versioned tables），可用于追踪数据随时间的变化。Hackathon 是一种短时间内集中协作开发项目的活动，通常持续 24 至 48 小时。本项目是在 Junction 2026 黑客松上为 MariaDB 的“Wikipedia Through Time”挑战开发，结合了向量检索和系统版本表技术以实现多语言、多版本的维基百科内容比对。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MariaDB">MariaDB - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hackathon">Hackathon - Wikipedia</a></li>
<li><a href="https://github.com/danielbacsur/junction-x-wikipedia-hackathon">GitHub - danielbacsur/junction-x-wikipedia-hackathon: A time ...</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#databases`, `#natural language processing`, `#multilingual`, `#open source`

---

<a id="item-tech-news-12"></a>
### [TimeCues Studio：开源音乐结构标注工具发布](https://www.reddit.com/r/MachineLearning/comments/1xwh3mw/acm_multimedia_2026_timecues_studio_a_free/) ⭐️ 7.0/10

TimeCues Studio 是一款新发布的免费开源 Web 应用，专为音乐结构详细标注和算法评测设计。该工具支持基于节拍的时间线标注、分轨可视化、算法对比（如 allin1 和 MSAF）、协作工作流，并可导出为 Audacity 标签、MIDI 或 JSON 格式。用户可通过 Docker Compose 一键部署，或直接在线体验，无需注册。该项目采用 MIT 许可证，适用于音乐信息检索、机器学习模型训练及音视频同步等场景。

reddit · r/MachineLearning · /u/SapirCa · 11月14日 23:59

**「背景介绍」** 音乐结构标注是音乐信息检索（MIR）领域的重要任务，涉及对音频文件中不同部分（如段落、重复、过渡等）进行精确标记。此前，研究人员和开发者常用如 Audacity 等通用音频编辑器或自建脚本进行标注，但这些工具通常缺乏专为结构标注和算法评测设计的功能。TimeCues Studio 作为一个开源的网络应用，旨在为算法开发团队和音乐分析研究者提供集成的标注、算法对比和原型开发环境，支持团队协作和多种导出格式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2609.10338">TimeCues Studio : A Workspace for Music Annotation and Algorithm...</a></li>
<li><a href="https://github.com/sapirca/timecues-studio">GitHub - sapirca/ timecues - studio · GitHub</a></li>

</ul>
</details>

**标签**: `#open-source`, `#music information retrieval`, `#machine learning tools`, `#data annotation`

---

<a id="item-tech-news-13"></a>
### [特斯拉 Cybercab 推出 299 美元/月自动驾驶强制订阅](https://www.tesla.com/configurator/api/v4/terms?category=autonomy_subs&amp;amp;locale=en_US&amp;amp;model=cc&amp;amp;saleType=Sale) ⭐️ 7.0/10

特斯拉正式公布了 Cybercab 自动驾驶订阅协议，要求用户在支付 29,990 美元购车款后，每月还需支付 299 美元订阅费，否则车辆将无法运行。特斯拉有权提前一个月通知调整订阅价格，若用户欠费或违规使用，可能被暂停或取消订阅，累计三次警告将导致自动驾驶功能停用一周。Cybercab 仅允许在指定区域内运营，且禁止未经授权接入网约车、配送或租赁平台。

telegram · zaihuapd · 11月15日 01:10

**「背景信息」** 特斯拉 Cybercab 是一款专为自动驾驶设计的两座车型，用户需支付 29,990 美元购车款，并每月额外支付 299 美元的强制订阅费以启用无人驾驶功能。该订阅不仅涵盖自动驾驶，还包括高级联网、轮胎和挡风玻璃服务及道路救援，但保险、充电和车辆注册需用户自理。若未按时续费或违反协议，车辆将被远程停用，且仅允许在特定区域内运营，禁止接入未经授权的网约车、配送或租赁平台。

**「影响」** Cybercab 车主必须持续支付订阅费用才能正常使用车辆，且需遵守严格的运营和平台接入限制，否则将面临功能停用等处罚。这对用户的用车自由度和成本控制提出了新的挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.notateslaapp.com/news/5015/teslas-cybercab-autonomy-subscription-everything-included">Tesla’s Cybercab Autonomy Subscription: Everything Included</a></li>
<li><a href="https://electrek.co/2026/11/14/tesla-cybercab-autonomy-subscription-agreement-terms/">Tesla Cybercab&#x27;s autonomy agreement is insane: $299/mo or it ...</a></li>
<li><a href="https://teslanorth.com/2026/11/13/tesla-cybercab-autonomy-subscription-terms/">Tesla Cybercab Terms Require a Paid Monthly Subscription</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#AI`, `#business models`, `#hardware`, `#technology industry`

---

<a id="item-tech-news-14"></a>
### [传 Anthropic 与美官员联手推动黄仁勋下台及 AI 芯片出口限制](https://www.washingtonpost.com/technology/2026/11/13/behind-jensen-huangs-spy-scandal-shadow-war-trumps-ear-china/) ⭐️ 7.0/10

据《华盛顿邮报》报道，英伟达创始人黄仁勋的离职疑似与美国国安官员和 Anthropic 高管的幕后操作有关。报道称，黄仁勋因反对对华 AI 芯片出口限制并与特朗普关系密切，激怒了美国鹰派，促使参议员鲁比奥等人通过 CIA 情报向总统施压。与此同时，Anthropic 被怀疑向媒体提供调查线索，推动对黄仁勋不利的报道。当前，国会正借此事件推动更严厉的 AI 芯片出口管制和芯片追踪技术立法，但相关指控尚未获得当事方回应，具体细节仍存疑。

telegram · zaihuapd · 11月15日 08:08

**「背景信息」** 近期，英伟达创始人兼前 CEO 黄仁勋卷入间谍丑闻，引发美国政界和科技行业关注。据《华盛顿邮报》报道，参议员鲁比奥等对华强硬派利用情报推动对黄仁勋的调查，削弱了其在华盛顿反对芯片出口限制的影响力。与此同时，Anthropic 等 AI 公司一直积极游说白宫，主张加强对华芯片出口管控，并推动在 GPU 芯片中加入追踪和防走私技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.washingtonpost.com/technology/2026/11/13/behind-jensen-huangs-spy-scandal-shadow-war-trumps-ear-china/">Behind Jensen Huang’s spy scandal, a shadow war for Trump’s ...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#hardware`, `#industry news`, `#US-China relations`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [坎托·菲茨杰拉德与英伟达关系引发美国政府审查](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 7.0/10

坎托·菲茨杰拉德及其领导层因与英伟达的关系受到美国政府审查，尤其是在 2025 年 9 月至 2026 年 3 月期间，该公司报告持有的英伟达股票数量下降了 49%，据 CNBC 分析称。美国政府担忧技术出口至中国及潜在利益冲突，目前尚无证据表明存在非法行为。

rss · CNBC Finance · 11月15日 19:58

**「背景」** 美国商务部长霍华德·卢特尼克因其与英伟达（Nvidia）的关系以及对人工智能芯片出口中国的监管态度受到批评。近期，英伟达 CEO 黄仁勋因与涉嫌协助中国获取美国 AI 芯片的 Megaspeed 公司高管关系曝光而辞职，进一步加剧了相关争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/11/12/us/politics/lutnick-nvidia-commerce-china-chips.html">Howard Lutnick Took Softer Line on Nvidia as Calls for Tougher...</a></li>
<li><a href="https://www.newsweek.com/scott-bessent-howard-lutnick-nvidia-scandal-12712195">Scott Bessent Puts Howard Lutnick on Spot Over Nvidia ... - Newsweek</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Cantor Fitzgerald`, `#US-China relations`, `#Technology policy`, `#Corporate governance`

---

<a id="item-finance-news-2"></a>
### [美法官允许美光、三星等 DRAM 价格操纵案继续审理](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 7.0/10

美国法官驳回了美光、三星和 SK 海力士关于撤销 DRAM 价格操纵集体诉讼的动议，认为存在三家公司合谋的合理证据。该案指控三家芯片制造商在一年内多次同步限制供应，导致 DRAM 价格最高上涨 500%。

telegram · zaihuapd · 11月15日 16:39

**「背景」** 此前，三家主要内存芯片制造商美光、三星和 SK 海力士被指控自 2022 年以来通过协调减少 DRAM（动态随机存取存储器）供应，涉嫌操纵价格，导致美国消费者和小企业提起集体诉讼。此次法官驳回撤诉动议，意味着案件将进入进一步审理阶段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/articles/judge-denies-motion-dismiss-dram-152445837.html?fr=sycsrp_catchall">Judge denies motion to dismiss DRAM price-fixing lawsuit ...</a></li>
<li><a href="https://wccftech.com/federal-judge-rejects-memory-makers-defense-samsung-micron-sk-hynix-dram-shortage-lawsuit/">Federal Judge Rejects Memory Makers’ Defense To ... - Wccftech</a></li>
<li><a href="https://hoodline.com/2026/11/judge-lets-dram-price-fixing-suit-against-samsung-micron-sk-hynix-move-forward/">Judge Allows DRAM Price-Fixing Suit Vs Samsung, Micron, SK Hynix</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#semiconductors`, `#legal`, `#price fixing`

---