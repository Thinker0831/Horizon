---
layout: default
title: "Horizon Summary: 2026-11-09 (ZH)"
date: 2026-11-09
lang: zh
---

> 从 33 条内容中筛选出 11 条重要资讯。

---

**科技新闻**
1. [Drex Max v1.1 多模态决策模型发布，声称达成 SOTA 并开放权重](#item-tech-news-1) ⭐️ 8.0/10
2. [KetchUp：基于 Rust 和 WebGPU 的开源 3D 建模工具发布](#item-tech-news-2) ⭐️ 7.0/10
3. [Llama-modchip 实现 284B 参数 LLM 在 64GB 内存无 GPU 本地推理](#item-tech-news-3) ⭐️ 7.0/10
4. [从 Claude 迁移到 Pi：AI 工具链接口变革](#item-tech-news-4) ⭐️ 7.0/10
5. [高盛限制银行家和交易员使用 Claude Code](#item-tech-news-5) ⭐️ 7.0/10
6. [Outlook.com 开始拒收无 DMARC 域名邮件](#item-tech-news-6) ⭐️ 7.0/10
7. [GRFNet：面向多通道时序分类的 PyTorch 模型开源发布](#item-tech-news-7) ⭐️ 7.0/10
8. [可玩宝可梦红宝石扩散世界模型与 System 1/2 代理架构](#item-tech-news-8) ⭐️ 7.0/10
9. [中国模型占全球开源模型企业支出 89%](#item-tech-news-9) ⭐️ 7.0/10
10. [Anthropic 报告：科学家用 Claude 以数据分析和写作为主](#item-tech-news-10) ⭐️ 7.0/10

**财经新闻**
1. [英伟达董事会对黄仁勋涉间谍指控展开独立调查](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Drex Max v1.1 多模态决策模型发布，声称达成 SOTA 并开放权重](https://www.reddit.com/r/MachineLearning/comments/1xr4hkm/artificial_analysis_multimodal_decision_model/) ⭐️ 8.0/10

Nace 团队发布了 Drex Max v1.1 多模态决策模型，声称在决策模型领域达成了最新的 SOTA（state-of-the-art）表现，并位于帕累托前沿。该模型权重采用 Open RAIL-M 许可开放，支持本地推理，且上下文窗口约为 256k，远超 Glide1.2（64k）和 Mammoth（16k）等同类模型。团队还公开了完整训练流程文档，并计划很快发布 v1.1 的开源权重。

reddit · r/MachineLearning · /u/m4rkGS · 11月8日 17:54

**「背景信息」** Drex Max 是 Nace.AI 推出的多模态决策模型，能够基于文本、JSON 和图像等多种输入格式回答问题，并为每个选项返回概率分布。此前，Drex Max v1 已在 Hugging Face 上以开放权重形式发布，并支持本地推理。该模型自称在 Decision Index 0.4 基准上取得了 67.52 的自报分数，且为 Drex v2.0 的继任者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/11/01/nace-ai-open-sources-drex-max-v1-local-inference/">Nace AI Open-Sources Drex Max v 1 : A 27B Decision Model That...</a></li>
<li><a href="https://openrouter.ai/nace-ai/drex-max">Drex Max - API Pricing &amp; Providers | OpenRouter</a></li>
<li><a href="https://huggingface.co/nace-ai/drex-max-v1">nace-ai/ drex - max - v 1 · Hugging Face</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#AI models`, `#open source`, `#multimodal`

---

<a id="item-tech-news-2"></a>
### [KetchUp：基于 Rust 和 WebGPU 的开源 3D 建模工具发布](https://ketchup3d.github.io/app/) ⭐️ 7.0/10

KetchUp 是一款全新开源的 3D 建模工具，采用 Rust 和 WebGPU 技术开发，定位为 SketchUp 的现代替代品。该项目可直接在浏览器中运行，面向需要免费、开放 3D 建模解决方案的用户和开发者。KetchUp 目前已上线，用户可通过其官网体验。其主要亮点在于利用 Rust 提供高性能 Web 端 3D 建模体验，并填补了 SketchUp 逐步远离免费和开放开发后的市场空白。

hackernews · dcoulmbe · 11月8日 22:35 · [社区讨论](https://news.ycombinator.com/item?id=50418176)

**「背景信息」** SketchUp 曾是一款广受欢迎的易用 3D 建模软件，但其免费和开放性逐步减少，引发用户对替代方案的需求。KetchUp 采用 Rust 语言和 WebGPU 技术开发，Rust 是一种注重安全性和性能的现代编程语言，而 WebGPU 则是新一代网页图形 API，支持高效的跨平台 3D 渲染。Rust 社区的 wgpu 项目为 WebGPU 在多平台上的实现提供了基础，使得在浏览器中运行高性能 3D 应用成为可能。

**「影响」** 对于习惯使用 SketchUp 但受限于其商业化和闭源政策的个人和爱好者，KetchUp 提供了一个无需安装、可自由修改和分发的现代替代方案。开发者还可借助其基于 Rust 的架构进行二次开发或集成，推动更多基于 WebGPU 的 3D 应用创新。

**「社区讨论」** 多位用户表达了对 SketchUp 逐步商业化和功能停滞的不满，对 KetchUp 作为“精神继承者”表示欢迎。有用户称赞其 Rust 实现的 Web 端 UI 表现流畅，另有反馈建议优化默认交互体验（如绘制矩形时不应强制命名对象）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/gfx-rs/wgpu">GitHub - gfx-rs/wgpu: A cross-platform, safe, pure- Rust graphics API.</a></li>

</ul>
</details>

**标签**: `#open-source`, `#3d-modeling`, `#rust`, `#webgpu`, `#software-tools`

---

<a id="item-tech-news-3"></a>
### [Llama-modchip 实现 284B 参数 LLM 在 64GB 内存无 GPU 本地推理](https://github.com/synchopate/llama-modchip) ⭐️ 7.0/10

Llama-modchip 项目实现了在仅有 64GB 内存且无 GPU 的本地硬件上运行 2840 亿参数的 DeepSeek 大语言模型（LLM）推理。这一成果依赖于模型量化和资源高效利用，使得超大模型的本地部署门槛大幅降低。该项目已开源，适用于希望在普通工作站上运行大模型的开发者和研究者。需要注意的是，具体性能表现和兼容性可能因硬件和量化策略而异。

hackernews · joshcsimmons · 11月8日 10:22 · [社区讨论](https://news.ycombinator.com/item?id=50411961)

**「背景信息」** llama-modchip 是一个开源项目，旨在通过自定义压缩和内存分块技术，使 2840 亿参数的 DeepSeek-V4-Flash 大型语言模型能够在仅有 64GB 内存、无 GPU 的 CPU 系统上本地推理运行。该项目支持多种模型和平台，并通过极致量化（如 1.71 bits per weight）和高效内存管理，显著降低了硬件门槛。此前，运行如此大规模模型通常需要昂贵的多卡 GPU 服务器或更高内存配置。

**「影响」** 开发者和个人用户无需昂贵的 GPU，即可在较为常见的高内存工作站上本地运行超大规模语言模型，有助于降低 AI 应用的硬件门槛并促进模型私有化部署。

**「社区讨论」** 有用户指出，激进的量化策略会导致模型性能非线性下降，4-bit 通常是性能与体积的最佳平衡点，低于此阈值则质量显著下降。另有评论认为该项目的实际性能与 llama.cpp 类似，但预填速度更快，且具体效果依赖于硬件配置和量化实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/synchopate/llama-modchip">GitHub - synchopate/llama-modchip: Run 284B DeepSeek-V4 ...</a></li>
<li><a href="https://www.inferwire.com/en/posts/llama-modchip-runs-284b-deepseek-model-on-64gb-ram-cpus">Llama-modchip Runs 284B DeepSeek Model on 64GB RAM CPUs</a></li>
<li><a href="https://braindetox.kr/en/posts/llama_modchip_deepseek_284b_cpu_64gb.html">llama-modchip 284B: DeepSeek-V4-Flash on 64GB RAM, No GPU</a></li>

</ul>
</details>

**标签**: `#large language models`, `#model quantization`, `#AI infrastructure`, `#open source`

---

<a id="item-tech-news-4"></a>
### [从 Claude 迁移到 Pi：AI 工具链接口变革](https://caleb.software/posts/claude-to-pi.html) ⭐️ 7.0/10

一篇技术性较强的讨论文章分析了部分高级用户从主流大语言模型（如 Claude、ChatGPT）接口迁移到替代方案（如 Pi harness）的现象。文章及社区评论详细探讨了接口设计、API 使用、模型行为和第三方封装工具的复杂性与风险，包括兼容性、API 隐藏参数、缓存机制等技术细节。该讨论反映出 AI 工具链日益复杂，开发者在选择和集成 LLM 时需权衡原生与第三方接口的优劣。Pi harness 因其灵活性和可扩展性受到部分用户青睐，但也存在与官方模型兼容性和服务条款风险。

hackernews · karagenit · 11月8日 03:11 · [社区讨论](https://news.ycombinator.com/item?id=50410107)

**「背景信息」** 近年来，开源本地大语言模型（LLM）代理工具（harness）如 Pi、OpenCode 等逐渐流行，成为开发者替代主流 LLM 接口（如 Claude、ChatGPT）的新选择。这些 harness 允许用户在本地运行和管理 AI 模型，提升了灵活性和数据隐私控制。例如，Pi harness 支持与本地 LLM 集成，能够自动化项目搭建和功能实现，适用于多种操作系统和开发环境。

**「影响」** 对于开发者和高级用户而言，采用 Pi 等第三方 harness 可以获得更高的灵活性和定制能力，但需注意潜在的兼容性问题、API 行为差异以及违反模型服务条款的风险。部分用户反馈在非原生 harness 下模型 token 消耗异常，且部分功能无法完整复现官方接口体验。

**「社区讨论」** 有用户认为第三方 harness（如 Pi）在灵活性和集成能力上优于官方接口，但也有观点指出使用非官方 harness 可能导致服务被封禁、模型行为异常及缓存失效等问题。部分开发者分享了在业务项目中自研 harness 的经验，强调 harness 设计对模型效率和功能实现的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/09/18/best-open-source-agent-harnesses-for-local-llms-in-2026/">Best Open-Source Agent Harnesses for Local LLMs in 2026</a></li>
<li><a href="https://github.com/locknet11/pi-local-harness">GitHub - locknet11/pi-local-harness: Pi wrapper tunned for ...</a></li>

</ul>
</details>

**标签**: `#large-language-models`, `#developer-tools`, `#ai-interfaces`, `#software-engineering`

---

<a id="item-tech-news-5"></a>
### [高盛限制银行家和交易员使用 Claude Code](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

高盛已决定限制其银行家和交易员对 Claude Code 的使用，原因包括安全、合规和成本方面的担忧。该措施反映了在高度监管和敏感的金融环境中部署 AI 编码代理所面临的实际挑战，尤其涉及数据隐私、金融风险以及消费型计费模式带来的预算压力。此次调整主要影响到直接接触客户和交易数据的前线金融专业人员。

hackernews · TheWiggles · 11月8日 18:16 · [社区讨论](https://news.ycombinator.com/item?id=50415628)

**「背景信息」** 据多家媒体报道，2026 年 10 月，高盛集团更新了其内部政策，限制包括 Anthropic 的 Claude Code 在内的 AI 工具的使用范围，仅允许工程师访问，禁止交易员和银行家继续使用。此前，这些非工程技术人员曾利用 Claude Code 和 GitHub Copilot 等工具开发市场模型和监控客户流，这些代码直接运行在处理客户信息的工作站上。此次调整反映出金融行业在数据安全、合规和风险管理方面对 AI 编码工具的高度关注。

**「影响」** 受影响的高盛员工将无法继续在日常工作中使用 Claude Code，可能需要寻找替代工具或恢复传统工作流程。此外，企业在选择 AI 工具时将更加重视安全、合规和可控成本，推动对计费模式和数据访问权限的严格审查。

**「社区讨论」** 有评论指出，将 AI 编码代理部署在金融专业人员的主力工作站上存在重大数据泄露风险，尤其是在同时访问敏感交易和客户信息的情况下。另有用户分享，因 AI 工具计费过高和合规风险，部分金融机构已转向计费更可控的替代方案，如 Google Gemini，并强调 AI 误用可能导致严重的合规后果甚至法律责任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gate.com/news/detail/GS/goldman-sachs-restricts-claude-code-access-in-october-traders-can-no-longer-25394829">Goldman Sachs restricts Claude Code access in October ...</a></li>
<li><a href="https://aigovernance.com/news/goldmans-claude-code-ban-exposes-ai-coding-tool-governance-gap">Goldman&#x27;s Claude Code Ban Exposes AI Coding Tool Governance…</a></li>
<li><a href="https://explainx.ai/blog/goldman-sachs-restricts-traders-bankers-ai-coding-tools-claude-code-engineers-only-2026">Goldman Sachs Restricts AI Coding Tools: What We Know ...</a></li>

</ul>
</details>

**标签**: `#enterprise-ai`, `#security`, `#finance`, `#regulation`, `#llm`

---

<a id="item-tech-news-6"></a>
### [Outlook.com 开始拒收无 DMARC 域名邮件](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Outlook.com 现已开始拒绝来自未配置 DMARC（域名基于消息认证、报告和一致性）记录的域名的邮件。这一变更影响所有向 Outlook.com 用户发送邮件但未设置 DMARC 的域名所有者，包括自建邮件服务器和部分组织。该政策调整并未公开宣布，部分用户反馈邮件被静默拒收，实际表现为 5xx 永久性投递失败。此举提升了邮件安全门槛，但对未及时配置 DMARC 的发件方造成了邮件投递中断。

hackernews · xmddmx · 11月8日 19:20 · [社区讨论](https://news.ycombinator.com/item?id=50416158)

**「背景信息」** DMARC（基于域的消息认证、报告和一致性）是一项电子邮件身份验证协议，用于防止伪造和钓鱼邮件。此前，许多邮件服务商仅建议或鼓励发件域配置 DMARC，但未强制要求。自 2026 年 11 月 5 日起，Outlook.com 及其相关服务（如 Hotmail、Live、MSN）开始拒收未设置 DMARC 记录的域名发来的邮件，这一变化影响了包括小型发件人在内的所有未配置 DMARC 的域。

**「影响」** 未设置 DMARC 的域名将无法向 Outlook.com 用户正常发送邮件，邮件管理员和自建邮件服务器的用户需尽快配置 DMARC 记录以恢复邮件可达性。未及时调整的组织可能会出现邮件丢失或业务沟通中断。

**「社区讨论」** 部分用户认为强制要求 DMARC 是合理的安全措施，但也有管理员抱怨 Outlook.com 的拒信机制不透明，且长期存在即使配置了 SPF/DKIM/DMARC 也被无故拒收的现象。有人指出，邮件服务商对自建服务器的限制越来越严，增加了独立运营邮件服务器的难度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mailroute.net/blog/outlook-rejecting-email-without-dmarc">Outlook.com Is Quietly Rejecting Email From Domains Without DMARC</a></li>
<li><a href="https://tosend.com/articles/outlook-rejects-email-without-dmarc/">Outlook.com now rejects email from domains without DMARC</a></li>
<li><a href="https://news.lavx.hu/article/outlook-com-rejects-some-email-from-domains-without-dmarc-records">Outlook.com Rejects Some Email From Domains Without DMARC ...</a></li>

</ul>
</details>

**标签**: `#email-security`, `#infrastructure`, `#policy-change`, `#software-engineering`

---

<a id="item-tech-news-7"></a>
### [GRFNet：面向多通道时序分类的 PyTorch 模型开源发布](https://www.reddit.com/r/MachineLearning/comments/1xqqj67/grfnet_pytorch_model_for_multichannel_timeseries/) ⭐️ 7.0/10

GRFNet 是一个新开源的 PyTorch 模型，专为多通道时序分类任务（如 EEG 数据）设计。该模型结合了随机与可学习的卷积核，并在空间滤波器部分引入创新：可根据传感器位置初始化通道混合权重。GRFNet 支持任意输入长度和采样率，默认配置下有 3,847 个参数，适用于小样本、高变异性的数据集。作者计划在 PhysioNet 的 EEGMMIDB 数据集上进行主体独立评测，并与 EEGNet、ShallowConvNet 等模型对比。

reddit · r/MachineLearning · /u/joekrry · 11月8日 05:13

**「背景介绍」** GRFNet 基于 ROCKET 架构，后者以随机、未训练的卷积核提取强大的时序特征而著称。GRFNet 针对 EEG 等多通道时序数据的小样本、高变异性特点，结合了可学习的空间滤波器和随机卷积核，旨在提升对这类信号的分类能力。该模型在默认配置下仅有 3,847 个参数，强调轻量化和适应性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kongchang.com/en/articles/grfnet-a-lightweight-pytorch-model-designed-for-multichannel-time-series-classification">GRFNet: A Lightweight PyTorch Model Designed for Multichannel ...</a></li>

</ul>
</details>

**标签**: `#time-series`, `#deep learning`, `#open source`, `#PyTorch`, `#EEG`

---

<a id="item-tech-news-8"></a>
### [可玩宝可梦红宝石扩散世界模型与 System 1/2 代理架构](https://www.reddit.com/r/MachineLearning/comments/1xqt0pk/i_trained_a_playable_diffusion_world_model_of/) ⭐️ 7.0/10

作者训练了一个基于扩散模型的宝可梦红宝石世界模型，能够根据最近 4 帧和按键输入生成下一帧画面，实现了可交互的游戏模拟。该模型包含 1670 万参数，分辨率为 72×80 灰度，并采用了 DIAMOND 风格的 EDM U-Net 架构。作者还实现了与 Krafton 的 PUBG Ally 类似的 System 1/2 代理架构：System 2 为规划层，能读取游戏内存并制定目标，System 1 为执行层，包含多个在世界模型中训练的小型策略网络。模型在真实游戏中 30 次尝试均成功获得第一枚徽章，但战斗部分尚未完全解决。

reddit · r/MachineLearning · /u/priyanshu123sah · 11月8日 07:48

**「相关背景」** 扩散模型是一类生成模型，近年来在图像生成等领域表现突出。System 1/2 分层代理架构源自认知科学，近期被 Krafton 在 PUBG Ally 项目中应用，用于将快速反应（System 1）与慢速规划（System 2）结合，提升游戏 AI 的灵活性和智能性。该 Reddit 项目借鉴了这一思路，将其用于宝可梦红的可玩世界模型和代理设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ajupress.com/view/20260616153131697">Krafton unveils &#x27; PUBG Ally &#x27; AI mode in two -week beta | Aju Press</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#world models`, `#diffusion models`, `#game AI`, `#agent architectures`

---

<a id="item-tech-news-9"></a>
### [中国模型占全球开源模型企业支出 89%](http://z.ai/) ⭐️ 7.0/10

根据 Menlo Ventures 的最新报告，中国开源 AI 模型占全球企业在开源模型上的支出高达 89%。其中，月之暗面 Kimi 占 61%，DeepSeek 占 15%，Z.ai 的 GLM 系列占 11%，而 Meta 的 Llama 仅占 7%。不过，开源模型整体仅占企业 AI 模型支出的 4%，大部分预算仍流向 Anthropic 和 OpenAI 的 API 服务（合计 86%）。该数据基于 9 月对近 400 名美国企业决策者的调查。

telegram · zaihuapd · 11月8日 03:26

**「背景信息」** 开源大模型在企业级市场的应用近年来持续增长，但与闭源模型相比，其市场份额仍然有限。Menlo Ventures 是一家专注于早期科技投资的风险投资公司，定期发布关于企业 AI 采用和市场趋势的报告。2026 年，企业在 AI 部署上的支出大幅增长，反映出生成式 AI 技术在全球范围内的快速普及和竞争格局的变化。

**「影响」** 对于希望采用开源 AI 模型的企业来说，中国模型已成为主流选择，但整体企业 AI 支出仍以闭源 API 服务为主，表明开源模型在企业级市场的渗透率有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://menlovc.com/">Menlo Ventures | Early-Stage Venture Capital Firm</a></li>

</ul>
</details>

**标签**: `#AI industry`, `#open source`, `#enterprise adoption`, `#market analysis`

---

<a id="item-tech-news-10"></a>
### [Anthropic 报告：科学家用 Claude 以数据分析和写作为主](https://www.anthropic.com/research/how-researchers-use-claude) ⭐️ 7.0/10

Anthropic 公布的报告分析了 2026 年 8 至 9 月间 20.7 万条科研相关会话，发现科学家主要用 Claude 进行数据分析和写作。具体来看，数据分析占 Claude 使用的 33.7%、Claude Code 的 48.1%，写作占 Claude 的 32%。正式科学（如计算机、数学）用户人均使用量高于实验学科（如化学、医学）。报告还估算，广泛采用现有 AI 能力可使部分领域研究产出翻倍，若 AI 能完全接管非体力工作，计算机等领域产出最高可提升至 15 倍。

telegram · zaihuapd · 11月9日 01:29

**「背景信息」** Anthropic 是一家专注于开发大语言模型（LLM）的人工智能公司，其 Claude 系列模型被广泛应用于文本生成、数据分析等任务。此前，AI 公司如 Anthropic 和 OpenAI 定期发布关于用户如何使用其产品（如 Claude、ChatGPT）的报告，但这些报告通常只披露部分数据，具体使用细节和影响仍有限。此次报告基于 2026 年 8 至 9 月间 20.7 万条科研相关会话，分析了 Claude 在科学研究中的实际应用场景和潜在生产力提升。

**「影响」** 对于正式科学领域的研究人员，积极采用 Claude 及其代码工具有望显著提升数据分析和写作效率，部分领域的研究产出可能实现倍增甚至更高增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.technologyreview.com/2026/08/18/1142226/how-people-use-ai/480/">We still don’t know how people are really using AI</a></li>
<li><a href="https://blockchain.news/news/anthropic-ai-scientific-research-claude">Anthropic Report Explores AI&#x27;s Role in Accelerating Scientific Research</a></li>

</ul>
</details>

**标签**: `#AI applications`, `#research productivity`, `#data analysis`, `#scientific writing`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [英伟达董事会对黄仁勋涉间谍指控展开独立调查](https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity) ⭐️ 7.0/10

英伟达董事会已启动独立调查，核查首席执行官黄仁勋在承认婚外情后是否成为外国情报行动目标，调查期间黄仁勋将继续担任首席执行官。

telegram · zaihuapd · 11月8日 21:39

**「背景」** 此前，英伟达首席执行官黄仁勋向公司员工承认婚外情后，董事会因有报道称涉事女性可能与中国情报机构有关，决定启动独立调查。该调查旨在查明黄仁勋是否成为外国情报行动的目标，并由外部律师协助进行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/08/nvidia-jensen-huang-investigation-china-spy.html">Nvidia investigates CEO Jensen Huang&#x27;s relationship with ...</a></li>
<li><a href="https://www.nytimes.com/2026/11/08/technology/nvidia-investigation-jensen-huang-china.html">Nvidia Opens Investigation Into Jensen Huang’s Relationship ...</a></li>
<li><a href="https://sfstandard.com/2026/11/08/nvidia-jensen-huang-affair-board-investigation-chinese-spy/">Nvidia launches probe as Jensen Huang admits affair with ...</a></li>

</ul>
</details>

**标签**: `#corporate governance`, `#national security`, `#NVIDIA`, `#executive leadership`, `#investigation`

---