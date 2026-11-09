---
layout: default
title: "Horizon Summary: 2026-11-09 (ZH)"
date: 2026-11-09
lang: zh
---

> 从 32 条内容中筛选出 9 条重要资讯。

---

**科技新闻**
1. [KetchUp：基于 Rust 和 WebGPU 的开源 SketchUp 替代品发布](#item-tech-news-1) ⭐️ 7.0/10
2. [高盛限制银行和交易员使用 Claude Code](#item-tech-news-2) ⭐️ 7.0/10
3. [284B DeepSeek 模型可在 64GB 内存无 GPU 本地运行](#item-tech-news-3) ⭐️ 7.0/10
4. [Outlook.com 开始静默拒收无 DMARC 域名邮件](#item-tech-news-4) ⭐️ 7.0/10
5. [Drex Max v1.1 多模态决策模型发布，声称达成 SOTA 并开放权重](#item-tech-news-5) ⭐️ 7.0/10
6. [GRFNet：面向多通道时序分类的 PyTorch 模型开源发布](#item-tech-news-6) ⭐️ 7.0/10
7. [美议员呼吁立法禁止 AI 递归自我改进](#item-tech-news-7) ⭐️ 7.0/10
8. [中国模型占全球开源模型企业支出 89%](#item-tech-news-8) ⭐️ 7.0/10

**财经新闻**
1. [英伟达董事会调查黄仁勋是否遭外国情报锁定](#item-finance-news-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [KetchUp：基于 Rust 和 WebGPU 的开源 SketchUp 替代品发布](https://ketchup3d.github.io/app/) ⭐️ 7.0/10

KetchUp 是一个开源的 3D 建模工具，采用 Rust 和 WebGPU 技术开发，可直接在浏览器中运行。它定位为 SketchUp（广泛使用的专有 3D 建模软件）的替代方案，强调跨平台和高性能。用户无需安装本地应用即可进行 3D 建模，适用于希望在网页端进行设计的开发者和爱好者。目前已可在线访问。

hackernews · dcoulmbe · 11月8日 22:35 · [社区讨论](https://news.ycombinator.com/item?id=50418176)

**「背景信息」** SketchUp 是一款广泛使用的专有 3D 建模软件，因其易用性和广泛的社区资源受到欢迎。KetchUp 作为开源替代方案，采用 Rust 语言和 WebGPU 技术，后者是一种现代 Web 图形 API，能够在浏览器中实现高性能 3D 渲染。Rust 与 WebGPU 的结合为跨平台、高性能的浏览器 3D 建模工具提供了新的技术路径。

**「影响」** 对于需要轻量级、易用且无需安装的 3D 建模工具的用户，KetchUp 提供了一个新的开源选择，尤其适合教育、业余爱好者和开发者快速原型设计。其基于现代技术栈，有望推动更多高性能 Web 端 3D 应用的开发。

**「社区讨论」** 有用户称赞 KetchUp 的 Rust UI 在浏览器中的表现流畅，甚至认为 Rust 可能是未来跨平台 Web 和移动应用的关键技术。部分用户建议增加功能展示和示例文件，以提升新用户的上手体验，也有用户反馈默认操作流程（如绘制矩形时强制命名）不够友好。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pooya.ai/webgpu/">Rust WebGPU Examples &amp; Tutorials | wgpu &amp; WGSL</a></li>

</ul>
</details>

**标签**: `#open-source`, `#3d-modeling`, `#rust`, `#webgpu`, `#software-tools`

---

<a id="item-tech-news-2"></a>
### [高盛限制银行和交易员使用 Claude Code](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

高盛已决定限制其银行和交易员对 Claude Code 的使用，原因涉及安全、合规和成本等多方面考量。该举措反映出在金融等高度敏感行业中，企业级 AI 工具的部署面临实际的操作、监管和财务挑战。此次调整主要影响到直接接触客户、交易和内部敏感信息的前线金融专业人员。高盛此举并非完全禁止 AI 工具，而是针对特定风险场景采取了更严格的管控措施。

hackernews · TheWiggles · 11月8日 18:16 · [社区讨论](https://news.ycombinator.com/item?id=50415628)

**「背景信息」** 此前，高盛允许包括交易员和银行家在内的员工使用 Claude Code 和 GitHub 等 AI 编程工具，用于监控客户流、构建交易模型和生成内容报告等任务。根据近期多家媒体报道，高盛在 2026 年 10 月对这些工具的访问权限进行了限制，仅允许软件工程师继续使用，结束了此前面向更广泛员工群体的试点阶段。这一政策调整是在评估了生产力提升与风险管理因素后做出的，反映出金融行业在采用 AI 编程助手时对安全、合规和成本的高度关注。

**「影响」** 受影响的高盛员工将无法在日常工作中继续使用 Claude Code，需寻找替代工具或回归传统流程，可能导致部分自动化和效率提升项目暂停或调整。对于其他金融机构而言，此举也为 AI 工具的合规和风险管理提供了警示和参考。

**「社区讨论」** 有评论指出，将 AI 编码代理部署在金融专业人员的主力工作站上存在重大数据泄露风险，尤其是在涉及客户、交易和内部网络的场景下。另有用户分享，部分机构因 AI 工具计费过高而收紧使用权限，并倾向选择计费更可控的替代方案，如 Google Gemini。此外，有实际案例显示，AI 工具在合规文档处理中的错误可能导致严重法律后果，甚至团队被解雇。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gate.com/news/detail/GS/goldman-sachs-restricts-claude-code-access-in-october-traders-can-no-longer-25394829">Goldman Sachs restricts Claude Code access in October ...</a></li>
<li><a href="https://www.siliconreport.com/goldman-sachs-cuts-off-most-staff-from-claude-code-and-github">Goldman Sachs cuts off most staff from Claude Code and GitHub</a></li>
<li><a href="https://explainx.ai/blog/goldman-sachs-restricts-traders-bankers-ai-coding-tools-claude-code-engineers-only-2026">Goldman Sachs Restricts AI Coding Tools: What We Know ...</a></li>

</ul>
</details>

**标签**: `#AI adoption`, `#enterprise security`, `#finance industry`, `#regulatory compliance`

---

<a id="item-tech-news-3"></a>
### [284B DeepSeek 模型可在 64GB 内存无 GPU 本地运行](https://github.com/synchopate/llama-modchip) ⭐️ 7.0/10

llama-modchip 项目实现了在仅有 64GB 内存、无 GPU 的本地硬件上运行 2840 亿参数的 DeepSeek 大语言模型。该项目依赖模型量化等技术以降低硬件门槛，允许用户在普通工作站上进行推理。虽然具体性能和兼容性细节尚不完全明确，但该项目已在开源社区引发了关于量化策略和硬件权衡的讨论。

hackernews · joshcsimmons · 11月8日 10:22 · [社区讨论](https://news.ycombinator.com/item?id=50411961)

**「背景信息」** llama-modchip 是一个开源项目，旨在让用户能够在仅有 64GB 内存且无独立 GPU 的普通 CPU 设备上本地运行 2840 亿参数的 DeepSeek-V4-Flash 语言模型。该项目通过激进的模型量化（如 1.71 bits per weight）和 CPU 优先的推理策略，大幅降低了对硬件的要求。此前，运行如此大规模模型通常需要昂贵的高端 GPU 和更高的内存配置。

**「影响」** 开发者和研究人员现在可以在无需高端 GPU 的情况下，本地实验和部署超大规模语言模型，这有助于降低 AI 研究和应用的硬件成本门槛。但实际性能和模型质量会受到量化方式和内存配置的显著影响，用户需根据自身需求权衡。

**「社区讨论」** 评论者普遍关注量化对模型性能的影响，有人指出 4-bit 量化通常是性能与模型体积的最佳平衡点，低于此会显著降低效果。也有用户质疑该项目的实际功能和与现有工具（如 llama.cpp）的差异，认为文档对量化细节描述不清。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/synchopate/llama-modchip">GitHub - synchopate/llama-modchip: Run 284B DeepSeek-V4 ...</a></li>
<li><a href="https://braindetox.kr/en/posts/llama_modchip_deepseek_284b_cpu_64gb.html">llama-modchip 284B: DeepSeek-V4-Flash on 64GB RAM, No GPU</a></li>
<li><a href="https://www.promptzone.com/mei_bui/llama-modchip-run-284b-deepseek-on-64gb-ram-no-gpu-required-3plk">Llama-modchip: Run 284B DeepSeek on 64GB RAM, No GPU Required</a></li>

</ul>
</details>

**标签**: `#large language models`, `#model quantization`, `#local inference`, `#hardware requirements`, `#open source`

---

<a id="item-tech-news-4"></a>
### [Outlook.com 开始静默拒收无 DMARC 域名邮件](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Outlook.com 现已悄然开始拒收来自未配置 DMARC（域名基于消息认证、报告和一致性）策略的域名的邮件。此变更影响所有向 Outlook.com 用户发送邮件但未部署 DMARC 的域名，且邮件被拒收时不会有明显提示。该政策调整对邮件投递率和邮件基础设施管理带来直接影响，尤其对尚未实施 DMARC 的组织和个人尤为重要。

hackernews · xmddmx · 11月8日 19:20 · [社区讨论](https://news.ycombinator.com/item?id=50416158)

**「背景信息」** DMARC（基于域的消息认证、报告和一致性）是一项电子邮件身份验证协议，旨在帮助防止伪造和钓鱼邮件。此前，许多邮件服务商建议但未强制要求发件域配置 DMARC。现在，Outlook.com 开始直接拒收未配置 DMARC 的域名发来的邮件，这一做法提升了邮件安全门槛，但也对未及时部署 DMARC 的域造成了影响。

**「影响」** 未配置 DMARC 的域名将无法向 Outlook.com 用户正常投递邮件，且发件方和收件方可能无法察觉邮件被静默丢弃，增加了沟通失败和故障排查难度。邮件管理员需尽快为其域名部署 DMARC 策略以确保邮件可达。

**「社区讨论」** 部分管理员认为微软静默丢弃邮件的做法容易导致发件方误以为邮件已成功送达，增加了排查难度。也有观点认为强制要求 DMARC 是提升安全的合理措施，但对未及时部署的用户造成了不便。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.factae.eu/en/article/outlook-com-quietly-rejects-emails-from-domains-without-dmarc-182744">Outlook . com quietly rejects emails from domains without DMARC</a></li>

</ul>
</details>

**标签**: `#email`, `#security`, `#infrastructure`, `#policy`

---

<a id="item-tech-news-5"></a>
### [Drex Max v1.1 多模态决策模型发布，声称达成 SOTA 并开放权重](https://www.reddit.com/r/MachineLearning/comments/1xr4hkm/artificial_analysis_multimodal_decision_model/) ⭐️ 7.0/10

Drex Max v1.1 是一款新发布的开源多模态决策模型，声称在决策模型领域达到了最新的 SOTA（state-of-the-art）性能，并实现了帕累托前沿。该模型支持约 256k 的上下文窗口，权重以 Open RAIL-M 许可证开放，支持本地推理（包括在 Mac 上运行），并提供了详细的训练方法论文和资源。虽然这些技术亮点和性能主张具有吸引力，但目前主要信息来自 Reddit 公告，缺乏独立验证，但开放的权重和文档为研究者和开发者提供了实际参考。

reddit · r/MachineLearning · /u/m4rkGS · 11月8日 17:54

**「背景信息」** Drex Max 是由 Nace.AI 推出的多模态决策模型，具备 270 亿参数和 255 路输出头，能够处理文本、JSON 及图像输入，并为每个选项输出概率。该模型以 Open RAIL-M 许可证开源，支持本地推理，包括在 Mac 上运行，并可通过 Python 在 NVIDIA GPU 上部署。此前版本 Drex Max v1 已在 Hugging Face 和 GitHub 上发布，v1.1 进一步提升了性能和兼容性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/nace-ai/drex-max-v1">nace-ai/drex-max-v1 · Hugging Face</a></li>
<li><a href="https://github.com/nace-ai/drex-decision-models/tree/main/models/drex-max-v1">drex-decision-models/models/drex-max-v1 at main · nace-ai ...</a></li>
<li><a href="https://www.nace.ai/drex">Drex Max, the decision model that sees | Nace.AI</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#open source`, `#decision models`, `#model release`

---

<a id="item-tech-news-6"></a>
### [GRFNet：面向多通道时序分类的 PyTorch 模型开源发布](https://www.reddit.com/r/MachineLearning/comments/1xqqj67/grfnet_pytorch_model_for_multichannel_timeseries/) ⭐️ 7.0/10

GRFNet 是一个开源的 PyTorch 模型，专为多通道时序数据（如 EEG 脑电信号）分类设计。该架构结合了 ROCKET 方法的随机未训练卷积核、可学习的空间滤波器，并支持根据传感器位置初始化权重。模型默认支持 22 个通道和 4 个分类任务，参数量为 3,847，可适应任意输入长度和采样率。目前作者正基于 PhysioNet 的 EEGMMIDB 数据集进行主体独立评估，并计划与 EEGNet 和 ShallowConvNet 进行对比。

reddit · r/MachineLearning · /u/joekrry · 11月8日 05:13

**「背景信息」** 多通道时间序列分类，尤其是脑电（EEG）等生物信号分析，因数据集规模小、个体差异大和信号采集条件多变而具有挑战性。ROCKET 方法通过随机、未训练的卷积核提取时间序列特征，已被证明在此类任务中有效。PyTorch 是一个广泛使用的深度学习框架，支持灵活的模型开发和开源协作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=LyJtbe__2i0">PyTorch 101 Crash Course For Beginners in 2026 - YouTube</a></li>
<li><a href="https://www.udemy.com/course/pytorch-deep-learning/">PyTorch : Deep Learning and Artificial Intelligence</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#open source`, `#time-series`, `#PyTorch`

---

<a id="item-tech-news-7"></a>
### [美议员呼吁立法禁止 AI 递归自我改进](https://x.com/AlexBores/status/2118494668769878037) ⭐️ 7.0/10

美国民主党议员 Alex Bores 公开呼吁国会在今年内立法，禁止人工智能递归自我改进（RSI），即 AI 自动构建下一代 AI。Bores 援引 OpenAI 和 Anthropic 的时间表，称自动化 AI 研究员和 AI 主导前沿模型开发可能分别在 2028 年和 2027 年实现，并引用 METR 报告支持 AI 研发加速的可信度。他强调，当前 AI 的错误或对齐偏差可能在每一代中被放大，因此立法禁令十分紧迫。

telegram · zaihuapd · 11月8日 01:30

**「递归自我改进（RSI）与监管讨论背景」** 递归自我改进（RSI）指的是 AI 系统能够自动改进自身或开发更强大的下一代 AI，无需人类直接干预。近年来，随着 AI 能力的快速提升，关于是否应立法限制或禁止 RSI 的讨论逐渐增多。部分政策制定者和专家担忧，若不加监管，RSI 可能导致不可控的超级智能或放大现有 AI 的对齐和安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/10/26/magazine/ai-companies-law-regulations.html">What Should the Rules for A . I . Companies Actually Be?</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#AI safety`, `#regulation`, `#recursive self-improvement`

---

<a id="item-tech-news-8"></a>
### [中国模型占全球开源模型企业支出 89%](http://z.ai/) ⭐️ 7.0/10

根据 Menlo Ventures 最新报告，中国开源 AI 模型占全球企业在开源模型上的支出高达 89%。其中，月之暗面 Kimi 占 61%，DeepSeek 占 15%，Z.ai 的 GLM 系列占 11%，而 Meta 的 Llama 仅占 7%。不过，开源模型整体仅占企业模型支出的 4%，大部分预算（86%）仍流向 Anthropic 和 OpenAI 的 API 服务。该数据基于 9 月对近 400 名美国企业决策者的调查。

telegram · zaihuapd · 11月8日 03:26

**「背景信息」** Menlo Ventures 的报告显示，2025 年第三季度至 2026 年第三季度，前沿模型（如 Anthropic、OpenAI 等）在企业 AI 支出中的份额显著上升，从 35% 增至 63%，而开源模型则主要由中国厂商主导。此前，Anthropic 曾在企业市场份额上超越 OpenAI，显示出企业用户对不同类型模型的偏好正在发生变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://menlovc.com/perspective/2026-the-state-of-enterprise-ai/">2026: The State of Enterprise AI | Menlo Ventures</a></li>
<li><a href="https://www.zdnet.com/article/anthropic-openai-enterprise-market-share-2025/">While Google and OpenAI battle for model dominance... - ZDNET</a></li>

</ul>
</details>

**标签**: `#AI industry`, `#open source`, `#enterprise adoption`, `#market analysis`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [英伟达董事会调查黄仁勋是否遭外国情报锁定](https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity) ⭐️ 7.0/10

英伟达董事会已成立独立委员会并聘请外部律师，调查首席执行官黄仁勋是否成为外国情报行动的目标；黄仁勋承认对妻子不忠并公开道歉，目前将继续担任首席执行官，直至调查结果公布。

telegram · zaihuapd · 11月8日 21:39

**「背景」** 此前，英伟达首席执行官黄仁勋承认对妻子不忠，并在媒体报道他可能成为外国情报行动目标后，英伟达董事会宣布将成立独立委员会并配合外部律师展开调查。该调查旨在查明黄仁勋是否受到外国间谍活动影响，属于公司治理和国家安全相关的重大事项。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity">Nvidia Board to Probe Spying Case After CEO Jensen Huang ...</a></li>
<li><a href="https://www.ft.com/content/1397e2f4-d7f5-4cbb-a4d9-04ecf661d1aa?syn-25a6b1a6=1">Nvidia’s Jensen Huang admits to affair after allegations of ...</a></li>
<li><a href="https://www.bbc.com/news/articles/c3dxw10rjn9no">Nvidia launches investigation into CEO&#x27;s affair with ... - BBC</a></li>

</ul>
</details>

**标签**: `#corporate governance`, `#national security`, `#NVIDIA`, `#leadership`

---