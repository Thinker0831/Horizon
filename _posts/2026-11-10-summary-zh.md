---
layout: default
title: "Horizon Summary: 2026-11-10 (ZH)"
date: 2026-11-10
lang: zh
---

> 从 44 条内容中筛选出 24 条重要资讯。

---

**科技新闻**
1. [DeepMind 发布 AlphaProof Code 自动化形式化验证系统](#item-tech-news-1) ⭐️ 9.0/10
2. [谷歌 Gemini 4 Carbon 模型正式面向公众开放](#item-tech-news-2) ⭐️ 9.0/10
3. [现代 Web 指南 1.0 发布，助力编码代理采用原生特性](#item-tech-news-3) ⭐️ 8.0/10
4. [Claude Code 泄露 2539 个真实凭据](#item-tech-news-4) ⭐️ 8.0/10
5. [Fireworks 遭遇新一轮黑客攻击，客户数据外泄](#item-tech-news-5) ⭐️ 8.0/10
6. [稀宇科技开源 MiniMax H3 Image 4K 图像生成模型](#item-tech-news-6) ⭐️ 8.0/10
7. [Synaptics 专利诉讼致 DisplayLink 开源驱动开发中止](#item-tech-news-7) ⭐️ 7.0/10
8. [Blender 5.3 发布，支持 Gaussian Splat](#item-tech-news-8) ⭐️ 7.0/10
9. [AMD Zen 6 架构升级与内存控制器改进分析](#item-tech-news-9) ⭐️ 7.0/10
10. [Val Town 宣布关闭平台运营](#item-tech-news-10) ⭐️ 7.0/10
11. [Meta AI 发布高效小型模型 Muse Ember](#item-tech-news-11) ⭐️ 7.0/10
12. [TimesFM 3.0、Chronos-2 和 Toto 2.0 在股市预测中未优于简单基线](#item-tech-news-12) ⭐️ 7.0/10
13. [苹果 Logic Pro 推出 50 美元 AI 用量包](#item-tech-news-13) ⭐️ 7.0/10
14. [华为擎云 HM650 台式机全系国产组件发布](#item-tech-news-14) ⭐️ 7.0/10
15. [OpenAI 部署 35 秒内叫停风险 AI 任务系统](#item-tech-news-15) ⭐️ 7.0/10
16. [Grok 4.8 强化学习阶段及技术栈重写](#item-tech-news-16) ⭐️ 7.0/10
17. [Anthropic 改为白名单制并排除中国大陆及港澳](#item-tech-news-17) ⭐️ 7.0/10

**财经新闻**
1. [美联储官员暗示 12 月或加息，可能幅度更大](#item-finance-news-1) ⭐️ 8.0/10
2. [加州选民否决 5%亿万富翁税提案](#item-finance-news-2) ⭐️ 8.0/10
3. [台积电 10 月营收同比大增 59.7%](#item-finance-news-3) ⭐️ 8.0/10
4. [Polymarket 年化营收突破 18 亿美元](#item-finance-news-4) ⭐️ 7.0/10
5. [2026 年前三季度中国新能源车出口大增](#item-finance-news-5) ⭐️ 7.0/10
6. [Anthropic 撤回高达 693 亿美元 IPO 申请](#item-finance-news-6) ⭐️ 7.0/10
7. [多家银行上调美元存款利率，部分高于美联储基准](#item-finance-news-7) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [DeepMind 发布 AlphaProof Code 自动化形式化验证系统](https://deepmind.google/blog/introducing-alphaproof-code/) ⭐️ 9.0/10

DeepMind 推出了 AlphaProof Code，这是一款用于复杂代码库自动化形式化验证的 AI 系统。该系统据称能够为先前由人类编写的复杂代码自动生成形式化证明，旨在提升软件的可靠性和安全性。官方博客宣布了这一能力，但尚未披露具体的适用范围、支持的编程语言或实际验证案例的详细数据。该系统目前处于发布初期，尚无独立测评结果。

hackernews · ilreb · 11月10日 12:11 · [社区讨论](https://news.ycombinator.com/item?id=50439193)

**「背景介绍」** AlphaProof Code 是 DeepMind 推出的多智能体 AI 框架，专为软件的形式化规范与验证而设计。该系统已被用于对 libsignal（Signal 协议的参考实现）在机器码级别进行关键安全属性的形式化证明。其工作方式类似于研究团队：由人类专家与 AI 协作确定需要证明的内容，再由一组 AI 代理完成具体的证明任务。

**「影响」** 对于需要高可靠性的软件开发者和组织，AlphaProof Code 有望显著降低形式化验证的门槛，提高关键系统的安全性和正确性。但用户在实际应用时需关注其验证范围、支持的属性类型以及潜在的误判风险。

**「社区讨论」** 部分开发者对 AlphaProof Code 的实际有效性表示质疑，认为其可能只验证了有限的属性或存在遗漏，担心 AI 生成的证明可能掩盖了实际漏洞。也有评论认为这是 AI 在软件工程领域的有益尝试，但强调需要警惕 AI 形式化验证的局限性和潜在误用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/introducing-alphaproof-code/">Formal Verification of Signal’s Protocol with... — Google DeepMind</a></li>
<li><a href="https://google-deepmind.github.io/code-verification/">AlphaProof Code : Verifying Signal’s Security at the Machine- Code ...</a></li>
<li><a href="https://storage.googleapis.com/gdm-deepmind-com-prod-public/media/documents/Formal_Verification_of_Signal_4.pdf">AlphaProof Code : Verifying Signal’s Security at</a></li>

</ul>
</details>

**标签**: `#formal verification`, `#AI tools`, `#software engineering`, `#machine learning`

---

<a id="item-tech-news-2"></a>
### [谷歌 Gemini 4 Carbon 模型正式面向公众开放](https://deepmind.google/models/model-cards/gemini-4-carbon/) ⭐️ 9.0/10

谷歌已正式向公众开放其最新旗舰 AI 模型 Gemini 4 Carbon。该模型主打网络安全、长时程智能体工作流，适用于复杂知识工作、软件工程和科学推理，并在 CursorBench 4.0 等多项基准测试中排名第一。Gemini 4 Carbon 通过 Gemini API、Google AI Studio 及 Gemini for business 提供，定价与 Argon 相同：输入 2 美元/百万 token，输出 10 美元/百万 token。此外，该模型已在 Antigravity 预览中支持 /swarm 多智能体协作。

telegram · zaihuapd · 11月10日 15:48

**「背景信息」** Gemini 4 Carbon 是谷歌基于 Gemini 4 Argon 开发的最新旗舰 AI 模型，专为复杂推理、代码生成和多智能体工作流设计。此前，Gemini 4 Argon 已作为高性能模型面向开发者和企业用户开放，而 Gemini 4 Carbon 在多个基准测试中表现更优，并以相同价格通过 Gemini API、Google AI Studio 及 Gemini for business 提供服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/">Gemini 4 Carbon is now available</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-carbon/">Gemini 4 Carbon - Model Card — Google DeepMind</a></li>

</ul>
</details>

**标签**: `#AI models`, `#Google`, `#machine learning`, `#software engineering`, `#industry news`

---

<a id="item-tech-news-3"></a>
### [现代 Web 指南 1.0 发布，助力编码代理采用原生特性](https://github.com/GoogleChrome/modern-web-guidance) ⭐️ 8.0/10

Google Chrome 团队联合 Firefox、MDN 和 Edge 发布了开源项目“modern-web-guidance”1.0，旨在帮助编码代理和开发者用现代 Web 平台原生特性替代过时的 JavaScript 实现。该项目包含 200 多篇由专家手工编写的最佳实践指南，并提供 CLI 工具，可用于知识检索、遗留代码扫描和技能集成。官方宣称，集成该指南后，主流 AI 编码代理在 200 项前端任务上的通过率从 55% 提升至 92%。该工具包可通过 npm 安装，支持本地快速搜索和遗留模式检测。

hackernews · paulirish · 11月10日 18:01 · [社区讨论](https://news.ycombinator.com/item?id=50443812)

**「背景信息」** 现代 Web Guidance 是一个由 Google Chrome 团队主导、开源的项目，旨在为开发者和编码代理（coding agents）提供关于现代浏览器 API、布局和性能的最佳实践与兼容性数据。该项目以 TypeScript 编写，并通过 CLI 工具或 npm 包分发，帮助用户直接在开发流程中获取最新的 Web 平台知识。该指南由多家主流浏览器厂商和 MDN 参与协作，内容持续更新以反映 Web 技术的演进。

**「影响」** 开发者和 AI 编码代理可更高效地采用浏览器原生能力，减少对冗余 JavaScript 代码和第三方依赖的依赖，从而提升代码现代性和可维护性。对于需要兼容多浏览器的项目，部分新特性在 Firefox 或 Safari 上尚未稳定，需注意兼容性风险。

**「社区讨论」** 有用户担忧该项目可能加剧 Chrome 在 Web 标准制定中的主导地位，导致 AI 代理生成的代码偏向 Chrome 支持的特性，影响跨浏览器兼容性。另有建议希望官方提供无需安装的在线文档索引，便于直接检索和集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/GoogleChrome/modern-web-guidance">GitHub - GoogleChrome / modern - web - guidance : Keep your coding...</a></li>
<li><a href="https://developer.chrome.com/docs/modern-web-guidance">Modern Web Guidance | Chrome for Developers</a></li>
<li><a href="https://www.libhunt.com/r/modern-web-guidance-src">Modern - web - guidance -src Alternatives and Reviews</a></li>

</ul>
</details>

**标签**: `#web development`, `#open source`, `#browser technology`, `#AI agents`

---

<a id="item-tech-news-4"></a>
### [Claude Code 泄露 2539 个真实凭据](https://www.ithome.com/1/024/888.htm) ⭐️ 8.0/10

安全公司 Apiiro 披露，Claude Code 因将获准执行的 Shell 命令写入本地设置文件，导致 1,994 个 GitHub 代码库中泄露了 2,539 个真实凭据，包括数据库密码和 API Token。超过 10 万份本地设置文件被上传至公共仓库，其中约 1,100 份包含机密数据。该问题源于设置文件未被正确配置为 Git 忽略，进而随项目提交暴露。Claude Code 团队表示正在研究预防措施，并考虑内置密钥扫描功能。

telegram · zaihuapd · 11月10日 11:20

**「事件背景」** Claude Code 是一款 AI 编程助手，允许用户批准并执行 Shell 命令。此前有用户在 2025 年 8 月于 GitHub 提交 issue，指出 Claude Code 会将已批准的 Bash 命令（包括明文凭据）直接写入本地设置文件 settings.local.json。若这些文件未被正确配置为 Git 忽略项，上传到公共仓库后就可能导致敏感信息泄露。近期安全公司 Apiiro 发现，数千条真实凭据因此暴露在 GitHub 上。

**「影响」** 受影响的开发者和组织需立即检查并清理公开仓库中的 Claude Code 设置文件，防止凭据被滥用。同时，建议加强本地配置文件的 Git 忽略规则，并关注后续官方的安全更新和密钥扫描功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybernews.com/security/ai-agents-leaking-secrets-on-github/">Claude Code secrets leak: thousands exposed on GitHub | Cybernews</a></li>
<li><a href="https://labs.cloudsecurityalliance.org/research/csa-research-note-claude-code-settings-secret-leak-20261108/">Approved Once, Leaked Forever: Secrets in Claude Code ...</a></li>

</ul>
</details>

**标签**: `#security`, `#software engineering`, `#devops`, `#incident response`

---

<a id="item-tech-news-5"></a>
### [Fireworks 遭遇新一轮黑客攻击，客户数据外泄](https://finance.sina.com.cn/stock/usstock/c/2026-11-10/doc-iniyfzhx2605532.shtml) ⭐️ 8.0/10

Fireworks 公司确认遭遇新一轮黑客攻击，部分客户账单信息、AI 模型权重和数据集被泄露。目前，Fireworks 正与帕洛阿尔托网络旗下的 Unit 42 团队联合展开调查。Harvey 公司声明其客户数据未受影响，但其他客户和终端用户是否受波及尚不明确。此次事件发生时，Fireworks 年化营收已达 10 亿美元，并计划以至少 300 亿美元估值启动新一轮融资。

telegram · zaihuapd · 11月10日 13:00

**「背景信息」** Fireworks 此前已披露 2026 年 10 月发生过安全事件，攻击者通过第三方云服务商入侵其开发环境，导致客户账户信息、账单记录、数据集及部分模型权重外泄。公司已针对该事件采取了安全加固措施，但本次披露显示影响范围进一步扩大。相关调查和安全通报显示，部分敏感数据如信用卡信息未被存储，因此未受影响。

**「影响分析」** 部分年付数百万美元的大客户据称正在考虑迁移服务，事件可能对 Fireworks 的企业客户信任、业务运营及即将进行的高估值融资造成直接影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cybersecuritynews.com/fireworks-ai-data-breach/">Hackers Breach Fireworks AI Through Third-Party Cloud ...</a></li>
<li><a href="https://fireworks.ai/security/bulletins/october-2026-security-incident-update">Update on October 2026 security incident | Fireworks AI</a></li>
<li><a href="https://breachhistory.com/blog/fireworks-data-breach-november-2026">Fireworks Data Breach: Billing and Model Weights (Nov 2026)</a></li>

</ul>
</details>

**标签**: `#security`, `#data breach`, `#AI industry`, `#enterprise software`

---

<a id="item-tech-news-6"></a>
### [稀宇科技开源 MiniMax H3 Image 4K 图像生成模型](https://huggingface.co/MiniMaxAI/MiniMax-H3-Image) ⭐️ 8.0/10

稀宇科技正式开源了 MiniMax H3 Image 图像生成模型，并在 Hugging Face 上发布权重。该模型支持最高 4096×4096 分辨率（4K）、最多 16 张参考图输入、复杂指令理解和图像编辑，标准模式下可在约 10 秒内生成一张 4K 图像。官方还同步推出 Highspeed 高速版本，标准模式生成速度为主流工具的 1.5–2 倍，高速模式可达 3–4 倍，模型已通过 API 和多款产品接入，标准版 4K 单张价格约 0.069 美元，首周优惠价约 0.034 美元。

telegram · zaihuapd · 11月10日 15:39

**「背景」** MiniMax H3 Image 是稀宇科技基于 H3 架构开发的开源图像生成模型，支持文本生成图像、参考图像生成和图像编辑等功能。该模型原生支持 4096×4096（约 1600 万像素）分辨率，并允许最多输入 16 张参考图像以增强复杂指令理解和细节表现。此次发布包括标准版和高速版，均已在 Hugging Face 平台及 API 上开放获取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3-image">MiniMax H 3 - Image : Bringing 4 K Image Generation into the...</a></li>
<li><a href="https://news.sulat.com/2026/11/11/minimax-releases-h3-image-open-weights/">MiniMax releases H 3 - Image as open weights - Sulat AI &amp; Tech News</a></li>
<li><a href="https://h3image.online/">MiniMax H 3 Image : open -weights 16MP / 4 K image model — API...</a></li>

</ul>
</details>

**标签**: `#generative-ai`, `#open-source`, `#image-generation`, `#machine-learning`

---

<a id="item-tech-news-7"></a>
### [Synaptics 专利诉讼致 DisplayLink 开源驱动开发中止](https://lwn.net/SubscriberLink/1102549/acbc92e00cee3a3f/) ⭐️ 7.0/10

由于 Synaptics 提出专利主张，开源 DisplayLink 驱动的开发工作已被迫中止。这一法律行动引发了硬件和开源社区对专利合规性及未来硬件支持的担忧。受影响的主要是 Linux 等系统上依赖 DisplayLink 技术的用户和开发者，目前尚无解决方案或替代驱动发布。该事件反映了专利执法对开源硬件支持项目的直接影响。

hackernews · speckx · 11月10日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50443824)

**「背景信息」** DisplayLink 是一种允许通过 USB 等接口扩展显示器的技术，广泛用于各种扩展坞和外设。此前，社区开发者曾基于开源方式为 DisplayLink 设备开发驱动程序，但近期有开发者因涉嫌侵犯 Synaptics 专利而收到律师函，被要求停止相关开源驱动的开发和分发。Synaptics 官方已提供部分平台的专有驱动，但开源驱动的法律风险和可用性问题一直是 Linux 等系统用户关注的焦点。

**「影响」** 依赖 DisplayLink 硬件的 Linux 及其他系统用户将面临驱动支持中断，可能影响相关设备的正常使用。开源开发者需谨慎评估专利风险，相关项目短期内难以继续推进。

**「社区讨论」** 部分评论者质疑 Synaptics 要求开发者承担专利侵权调查费用的合理性，认为此举缺乏法律依据。也有用户指出，DisplayLink 本身已因技术和经济原因逐渐被新一代接口（如 Thunderbolt 和 USB4）取代，认为该专利诉讼加速了其淘汰。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/peripherals/docking-stations-hubs/synaptics-sends-cease-and-desist-order-to-creator-of-open-source-displaylink-driver-dares-him-to-publicize-its-threats-dev-reverse-engineers-displaylink-using-claude-ai-and-rust-synaptics-threatens-to-bill-creator-for-legal-documentation">Synaptics sends cease-and-desist order to creator of open - source ...</a></li>
<li><a href="https://www.phoronix.com/news/Synaptics-Blocks-Vino-Driver">Synaptics Appears To Use Legal Threats To Block Open - Source ...</a></li>
<li><a href="https://www.synaptics.com/products/displaylink-graphics/embedded/sdk">Software Tools | Synaptics</a></li>

</ul>
</details>

**标签**: `#patents`, `#open-source`, `#hardware`, `#legal`

---

<a id="item-tech-news-8"></a>
### [Blender 5.3 发布，支持 Gaussian Splat](https://www.blender.org/download/releases/5-3/) ⭐️ 7.0/10

Blender 5.3 正式发布，新增对 Gaussian Splat（高斯点云渲染）的支持，并带来几项重要的工作流增强。此次更新为 3D 图形和技术用户提供了新的渲染技术，提升了几何节点、列表和闭包等功能，改善了复杂管线下的使用体验。Gaussian Splat 支持使 Blender 能够处理和渲染基于点云的新型 3D 数据格式，拓展了其在建模、渲染和潜在机器学习应用中的能力。该版本现已开放下载，适用于 Blender 支持的各主流平台。

hackernews · amlib · 11月10日 16:15 · [社区讨论](https://news.ycombinator.com/item?id=50442426)

**「背景信息」** 高斯点云（Gaussian Splatting）是一种用于高效渲染和表示三维点云数据的技术，近年来在计算机图形领域获得关注。Blender 5.3 版本首次引入了对高斯点云的原生支持，包括导入、几何节点集成以及在 Workbench、EEVEE 和 Cycles 渲染引擎中的渲染能力。这一实现使得用户可以直接在 Blender 内部处理和渲染高斯点云数据，提升了与点云相关的工作流程效率和灵活性。

**「影响」** 对于需要处理大规模点云数据或探索新型渲染技术的 3D 艺术家和技术开发者，Blender 5.3 的 Gaussian Splat 支持将显著提升其工作效率和创作空间。几何节点的增强也为复杂项目的可视化编程带来更多灵活性和易用性。

**「社区讨论」** 有用户反馈 Gaussian Splat 功能在测试中表现成熟且与 Blender 界面高度集成，未发现明显不一致。另有开发者认为几何节点的增强极大改善了复杂工作流，尤其是在与列表和闭包结合使用时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.blender.org/docs/release_notes/5.3/rendering/">Rendering - Blender Developer Documentation</a></li>
<li><a href="https://digitalproduction.com/2026/09/22/blender-5-3-brings-gaussian-splats-home/">Gaussian Splats in Blender 5.3: Native Import and Rendering</a></li>

</ul>
</details>

**标签**: `#3d-graphics`, `#software-release`, `#rendering`, `#open-source`

---

<a id="item-tech-news-9"></a>
### [AMD Zen 6 架构升级与内存控制器改进分析](https://chipsandcheese.com/p/amds-zen-6-family-feeding-the-beast) ⭐️ 7.0/10

AMD Zen 6 处理器家族将带来多项架构改进，包括全新设计的 I/O 芯片组（chiplet）、升级的内存控制器，以及核心微架构的平衡优化。新一代 I/O 芯片组预计采用更先进的制程工艺，有望显著提升内存带宽和支持更高的内存速度，解决现有 AM5 平台在高于 3600 MT/s 内存频率下的性能瓶颈。此外，Zen 6 还调整了整数乘法单元和 PDEP/PEXT 指令吞吐量，并在每个芯片组内集成多达 32 个核心，配备更大的 L3 缓存。

hackernews · pixelpoet · 11月10日 17:02 · [社区讨论](https://news.ycombinator.com/item?id=50443090)

**「背景信息」** AMD Zen 架构是该公司自 2017 年以来持续演进的高性能 CPU 微架构，广泛应用于桌面、服务器和移动平台。Zen 6 是继 Zen 5 之后的下一代架构，据报道将带来显著的 IPC（每时钟指令数）提升、核心数量增加以及内存和 I/O 子系统的重大改进。此前 Zen 5 已引入更先进的分支预测和执行单元，Zen 6 则在此基础上进一步优化核心微结构和系统带宽。

**「影响」** 对于硬件工程师和高性能计算用户而言，Zen 6 的内存控制器和 I/O 芯片组升级将改善多通道内存性能，提升整体系统带宽和可扩展性，尤其适合需要高并发和大容量内存支持的应用场景。

**「社区讨论」** 多位评论者关注 Zen 6 新内存控制器对高频内存支持的提升，认为这是 AM5 平台用户最期待的改进之一。也有技术讨论聚焦于核心微架构的平衡调整，如整数单元数量减少、指令级并行性优化，以及每芯片组 32 核心设计对 NUMA 架构和系统调度的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wccftech.com/amd-zen-6-architecture-ipc-cores-memory-performance-epyc-venice/">AMD Zen 6 Architecture Brings A Phenomenal 27% IPC Increase...</a></li>
<li><a href="https://www.techpowerup.com/review/amd-zen-6-technical-deep-dive/">AMD Zen 6 Technical Deep Dive | TechPowerUp</a></li>

</ul>
</details>

**标签**: `#hardware`, `#cpu`, `#microarchitecture`, `#systems`

---

<a id="item-tech-news-10"></a>
### [Val Town 宣布关闭平台运营](https://blog.val.town/winding-down) ⭐️ 7.0/10

面向开发者的端用户编程平台 Val Town 宣布即将关闭。该平台基于 Deno 运行时，曾获得 700 万美元风险投资，主要用于快速原型开发和云端代码执行。此次关闭反映了此类开发者工具平台在商业可持续性方面面临的挑战。Deno 团队加入 Cloudflare 后将于明年停止维护 Deno 运行时，这也是 Val Town 关闭的技术背景之一。

hackernews · tosh · 11月10日 17:31 · [社区讨论](https://news.ycombinator.com/item?id=50443427)

**「背景信息」** Val Town 是一个基于云的脚本平台，允许开发者用 TypeScript 快速编写和部署函数，无需构建步骤或管理基础设施。该平台支持定时任务、API、Webhook、邮件等功能，主要面向希望快速上线小型后端逻辑的开发者。Val Town 也被一些开发者工具公司用于演示、Webhook 和轻量级集成。

**「影响」** Val Town 用户需尽快迁移其代码和项目，因平台即将停止服务且依赖的 Deno 运行时也将不再维护。开发者和相关社区需关注云端代码托管和端用户编程领域的可持续性问题。

**「社区讨论」** 多位评论者认为，端用户编程平台商业化极为困难，即使获得大量融资也难以实现规模化。部分用户表达了对 Val Town 社区活动和团队透明度的认可，并对团队未来发展表示祝福。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://makerstack.co/reviews/val-town-review/">Val Town Review 2026: 7.6/10, from $10/mo</a></li>
<li><a href="https://www.val.town/features">Features | Val Town</a></li>
<li><a href="https://aicoolies.com/tools/val-town">Val Town : Features, Pricing &amp; Alternatives — aicoolies</a></li>

</ul>
</details>

**标签**: `#developer-tools`, `#end-user-programming`, `#startup-shutdown`, `#deno`

---

<a id="item-tech-news-11"></a>
### [Meta AI 发布高效小型模型 Muse Ember](https://simonwillison.net/2026/Nov/10/muse-ember/) ⭐️ 7.0/10

Meta AI 推出了 Muse Ember，这是其目前最小且最高效的 AI 模型，专为复杂推理和自动化代理任务（如工具调用、代码子任务、路由、信息抽取和长文档解析）设计。Muse Ember 1.0 支持最长 100 万输入 token，短提示下的定价与 GPT-6 Luna 和 Claude Haiku 5.5 相同（每百万输入 token $0.10，输出 $0.50），但超过 20 万 token 后价格上调。人工分析数据显示，Muse Ember 在智能指数与任务成本的平衡上处于效率前沿，性价比优于同类竞品。该模型还提供六档推理能力，适应不同复杂度需求。

rss · Simon Willison · 11月10日 07:28

**「背景信息」** Muse Ember 是 Meta AI 最新发布的一款轻量级高效模型，专为复杂推理和高频重复性任务（如工具调用、代码子任务、路由和文档处理）设计。该模型定位于高吞吐量、日常自动化和智能体工作流，旨在以较低成本提供高效执行能力。此前，Meta 的 Muse 系列模型以更大规模和更高价格为主，Muse Ember 则补充了面向高效、经济场景的产品线。

**「影响」** 开发者和企业可用更低成本获得高效推理能力，尤其适合需要长文本处理和复杂自动化的场景。Muse Ember 的定价和性能优势可能促使用户从更昂贵的模型迁移，推动市场对高性价比小型模型的关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.meta.ai/models/muse-ember">Muse Ember | Meta</a></li>
<li><a href="https://research.meta.ai/blog/muse-ember">Introducing Our Smallest, Most Efficient Model: Muse Ember</a></li>
<li><a href="https://techcrunch.com/2026/11/09/meta-releases-muse-ember-a-new-lightweight-model-for-agent-execution/">Meta releases Muse Ember, a new lightweight model for agent ...</a></li>

</ul>
</details>

**标签**: `#AI models`, `#model efficiency`, `#industry news`, `#pricing`

---

<a id="item-tech-news-12"></a>
### [TimesFM 3.0、Chronos-2 和 Toto 2.0 在股市预测中未优于简单基线](https://www.reddit.com/r/MachineLearning/comments/1xsqztt/i_benchmarked_timesfm_30_chronos2_and_toto_20_on/) ⭐️ 7.0/10

一位用户对三款主流时间序列基础模型（TimesFM 3.0、Chronos-2、Toto 2.0）在 24 只美国股票和 ETF 上的预测能力进行了基准测试，涵盖日线和分钟级数据。实验采用零样本、默认配置、无微调，比较对象为简单基线（如最后价格、单向预测和随机游走）。结果显示，这些模型在预测股票价格涨跌方向上的准确率与随机猜测相当（约 50%），且在简单交易策略下的收益远低于买入并持有。即使在更高频率的数据上，模型表现也未优于一行均值回归等简单方法。

reddit · r/MachineLearning · /u/AdelSexy · 11月10日 16:14

**「背景」** TimesFM 3.0 是 Google 推出的最新一代零样本时间序列基础模型，旨在实现多变量和单变量预测，并在多个公开基准上取得了领先表现。Chronos-2 和 Toto 2.0 也是近期发布的通用时间序列预测模型，均主打无需微调即可在多种数据集上进行预测。此前，这些模型在标准数据集上表现优异，但其在金融市场等高噪声、难以预测的实际场景中的有效性尚未被广泛验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://research.google/blog/timesfm-3-a-zero-shot-foundation-model-for-multivariate-forecasting/">TimesFM - 3 : A zero -shot foundation model for multivariate forecasting</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#time series`, `#benchmarking`, `#financial data`

---

<a id="item-tech-news-13"></a>
### [苹果 Logic Pro 推出 50 美元 AI 用量包](https://www.theverge.com/tech/1030084/apple-intelligence-usage-packs-ai-features-creator-studio-logic-pro) ⭐️ 7.0/10

苹果在 Logic Pro 中上线了售价 49.99 美元的 AI 用量包，允许用户购买更多基于云端（如 OpenAI 或 Gemini 模型）的 AI 功能使用额度。该用量包仅限购买账户使用，未用完的额度可逐月结转，但 12 个月后会过期。这是首个对 Apple Intelligence 额外用量收费的苹果应用，预计本月还将扩展至 Pixelmator Pro、Final Cut Pro 等其他创意软件。

telegram · zaihuapd · 11月10日 01:53

**「背景信息」** Logic Pro 是苹果面向音乐制作专业用户的旗舰软件。此前，苹果已在 Logic Pro 中集成了基于云端的 AI 功能，但这些功能有免费额度限制。此次推出的 49.99 美元 AI 用量包，是苹果首次对额外 Apple Intelligence 用量进行收费，用户可在额度用尽后通过一次性购买获得更多 AI 功能使用权。

**「影响」** Logic Pro 用户如需持续使用云端 AI 功能，需额外付费购买用量包，否则将受额度限制。此举标志着苹果在创意软件中引入 AI 功能分级付费模式，用户需关注额度管理和有效期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://madrobot.blog/2026/11/09/apple-intelligence-usage-packs-extra-ai/">Apple intelligence usage packs: $49.99 for more AI in Logic Pro</a></li>
<li><a href="https://www.cultofmac.com/news/apple-intelligence-usage-packs-logic-pro">Apple’s ‘intelligence usage packs’ put a price on extra AI</a></li>
<li><a href="https://www.gadgets360.com/ai/news/apple-introduces-paid-ai-usage-packs-for-logic-pro-more-apps-to-follow-12308768">Apple Starts Charging for Extra AI Usage in Logic Pro With ...</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI monetization`, `#creative software`, `#business models`

---

<a id="item-tech-news-14"></a>
### [华为擎云 HM650 台式机全系国产组件发布](https://www.techspot.com/news/114490-huawei-new-desktop-pc-contains-only-chinese-components.html) ⭐️ 7.0/10

华为宣布其擎云 HM650 台式机全系采用中国制造的组件，并搭载自研的鸿蒙操作系统。该机型配备 16GB 长鑫存储 LPDDR5 内存、256GB 或 512GB 固态硬盘，以及由中芯国际以 7 纳米 N+2 工艺代工的麒麟 X90 芯片（基于 Armv8 授权）。不过，芯片制造仍依赖海外技术，且鸿蒙系统无法原生运行 Windows .exe 程序，企业用户需自行确认软件和外设的兼容性。

telegram · zaihuapd · 11月10日 03:46

**「背景信息」** 近年来，华为因受到美国等国家的出口管制，推动了国产化硬件和自主操作系统的研发。此前，华为已推出自研麒麟系列芯片和鸿蒙操作系统，但在台式机领域实现全国产组件尚属首次。此次擎云 HM650 台式机被称为首款全部采用中国制造组件的桌面电脑，搭载麒麟 X90 处理器和鸿蒙系统，标志着中国在信息技术自主可控方面迈出新步伐。

**「影响」** 对于追求国产化硬件和操作系统的企业用户，该产品提供了新的选择，但在软件兼容性和部分核心技术自主性方面仍存在局限，采购和部署前需充分评估实际需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.notebookcheck.net/The-first-fully-Chinese-desktop-Huawei-launches-PC-with-Kirin-X90-and-HarmonyOS.1445194.0.html">The first fully Chinese desktop : Huawei ... - Notebookcheck News</a></li>
<li><a href="https://basic-tutorials.com/news/huawei-qingyun-hm650-first-harmonyos-pc-made-entirely-from-chinese-parts/">Huawei Qingyun HM 650 : First HarmonyOS PC Made... - Basic Tutorials</a></li>
<li><a href="https://www.theregister.com/systems/2026/11/09/huawei-says-its-made-a-100-percent-chinese-pc/5308335">Huawei says it’s made a 100 percent Chinese PC</a></li>

</ul>
</details>

**标签**: `#hardware`, `#operating-systems`, `#supply-chain`, `#china-tech`

---

<a id="item-tech-news-15"></a>
### [OpenAI 部署 35 秒内叫停风险 AI 任务系统](https://interestingengineering.com/ai-robotics/openai-control-room-35-second-model-shutdown) ⭐️ 7.0/10

OpenAI 已在其内部研究设施部署了“控制室”系统，能够在收到停止指令后，最迟 35 秒内阻止有风险的 AI 智能体任务继续获取模型输出。该系统通过唯一任务 ID 管理训练、评估和数据处理任务，并在推理引擎处理请求前确认任务是否获准继续。所有前沿强化学习任务还配备了独立模型监控器，能够检测模型行为并在发现潜在问题时报警。OpenAI 还在努力进一步缩短因授权请求缓存带来的延迟，目标是将其降至 0。

telegram · zaihuapd · 11月10日 05:47

**「背景信息」** AI 研究和部署过程中，存在模型行为不可预测、潜在风险难以及时控制的问题。为此，业界逐步重视基础设施级别的安全控制措施，例如在每次推理请求前强制进行授权检查，并在授权服务不可用时默认拒绝请求，以优先保障系统可控性而非可用性。OpenAI 此次推出的“控制室”系统正是在此背景下，针对 AI 任务的安全与可控性需求而设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://emergent.sh/news/openai-control-room-35-second-kill-switch">OpenAI Control Room: 35-Second Kill Switch for Research</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#operational systems`, `#machine learning`, `#risk management`

---

<a id="item-tech-news-16"></a>
### [Grok 4.8 强化学习阶段及技术栈重写](https://x.com/elonmusk/status/2120088070443655190) ⭐️ 7.0/10

埃隆·马斯克宣布，Grok 4.8 版本已完成预训练并进入强化学习（RL）阶段。此次更新的核心在于完全弃用 JAX/SGLang，转而用 C/C++ 从零重写了整个强化学习与推理栈。马斯克表示，这一重写导致开发周期延长，但目前评测分数已开始上升。4.8 版本将于本周晚些时候向部分 Bot 用户灰度发布，与 4.7 版本几乎没有相似之处。

telegram · zaihuapd · 11月10日 12:28

**「背景信息」** Grok 4.8 是 xAI 推出的新一代大型语言模型，早在 2026 年 9 月，马斯克就曾透露该模型拥有 2.5 万亿参数，并计划在全新 C/C++ 软件栈上进行训练。此前的 Grok 版本主要基于 JAX/SGLang 实现，而 4.8 版本则彻底转向 C/C++，并在预训练完成后进入强化学习阶段。此次更新也是自 9 月以来首次公布具体进展和上线时间表。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/grok-4-8-soft-rollout-rl-cpp-stack-november-2026">Grok 4.8 Soft Rollout: RL Done, Bot Test This Week - explainx.ai</a></li>
<li><a href="https://www.explainx.ai/blog/grok-4-8-2-5-trillion-parameters-cpp-training-stack-2026">Grok 4.8: 2.5T Params, C++ Stack, RL Next (Sept 2026 ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#reinforcement-learning`, `#software-engineering`, `#large-language-models`

---

<a id="item-tech-news-17"></a>
### [Anthropic 改为白名单制并排除中国大陆及港澳](https://www.anthropic.com/legal/supported-regions) ⭐️ 7.0/10

Anthropic 宣布自 11 月 12 日起，其 AI 产品（包括 Claude.ai、Claude Code、Cowork、API 及通过云平台和授权经销商提供的 Claude 模型）将仅在官方白名单列出的 185 个国家和地区开放使用。中国大陆、香港和澳门均未被列入支持名单，台湾地区则在名单内。政策规定，人在不支持地区使用、在不支持地区注册或设总部的实体及其人员使用、以及被不支持地区主体控股的公司人员使用，均属违规。该名单并未完全照搬美国制裁名单，显示为 Anthropic 自主合规标准。

telegram · zaihuapd · 11月10日 13:44

**「背景信息」** Anthropic 是一家知名的人工智能公司，其产品包括 Claude.ai、Claude Code、Cowork 及 API 等。此前，Anthropic 的服务在全球范围内较为开放，但近期公司发布了《支持地区政策》，明确规定仅允许名单上的 185 个国家和地区访问其产品。该政策还特别强调，身处未支持地区的个人、注册地或总部在未支持地区的实体及其人员、以及被未支持地区主体控股的公司人员均被禁止使用其服务。

**「影响」** 中国大陆、香港和澳门的用户及企业将无法合法访问或使用 Anthropic 的 AI 产品和服务，包括 API 接入和云平台部署。国际企业需注意员工出差、公司注册地及控股结构，以避免违反新政策。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/legal/supported-regions">Supported Regions Policy - Anthropic</a></li>
<li><a href="https://www.gate.com/news/detail/anthropic-enforces-whitelist-policy-on-november-12-banning-claude-access-25535601">Anthropic Enforces Whitelist Policy on November 12, Banning ...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#regional access`, `#compliance`, `#Anthropic`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [美联储官员暗示 12 月或加息，可能幅度更大](https://www.cnbc.com/2026/11/10/fed-governor-waller-sees-december-hike-likely.html) ⭐️ 8.0/10

美国联邦储备委员会理事沃勒表示，12 月很可能加息，并称如果通胀高于预期，将考虑加息 50 个基点，而不是通常的 25 个基点。沃勒强调，若未按预期加息，将损害美联储的政策公信力。

rss · CNBC Finance · 11月10日 17:13

**「背景」** 克里斯托弗·沃勒自 2020 年起担任美国联邦储备委员会（美联储）理事，任期至 2030 年，负责参与制定美国货币政策。美联储通过调整基准利率来应对通胀和经济增长变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Christopher_Waller">Christopher Waller - Wikipedia</a></li>
<li><a href="https://www.federalreserve.gov/aboutthefed/bios/board/waller.htm">Federal Reserve Board - Christopher J. Waller</a></li>
<li><a href="https://www.federalreservehistory.org/people/christopher-waller">Christopher J. Waller - Federal Reserve History</a></li>

</ul>
</details>

**标签**: `#Federal Reserve`, `#interest rates`, `#monetary policy`, `#inflation`, `#economic outlook`

---

<a id="item-finance-news-2"></a>
### [加州选民否决 5%亿万富翁税提案](https://www.theguardian.com/us-news/2026/nov/09/california-tax-billionaires-prop-40) ⭐️ 8.0/10

加州选民否决了第 40 号提案，该提案原计划对截至 2026 年 1 月净资产超过 10 亿美元的人群一次性征收 5%税款，用于医疗、教育和食品援助。

telegram · zaihuapd · 11月10日 07:12

**「背景」** 加州第 40 号提案是一项拟对净资产超过 10 亿美元的个人和信托一次性征收 5%税收的公投，税收将用于资助州医疗、教育和食品援助项目。该提案在 2026 年 11 月的选举中成为加州最具争议的议题之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ballotpedia.org/California_Proposition_40,_One-Time_Wealth_Tax_for_State-Funded_Healthcare,_Education,_and_Food_Assistance_Programs_Initiative_%282026%29">California Proposition 40, One-Time Wealth Tax for State ...</a></li>
<li><a href="https://calmatters.org/california-voter-guide-2026/proposition-40-billionaire-tax/">Voter guide to Proposition 40: Billionaire tax - CalMatters</a></li>

</ul>
</details>

**标签**: `#tax policy`, `#ballot initiative`, `#California`, `#wealth`, `#public finance`

---

<a id="item-finance-news-3"></a>
### [台积电 10 月营收同比大增 59.7%](https://pr.tsmc.com/chinese/news/3349) ⭐️ 8.0/10

台积电公布 2026 年 10 月营收为 5868.9 亿新台币，同比增加 59.7%，为公司实际业绩。

telegram · zaihuapd · 11月10日 08:07

**「背景」** 台积电是全球最大的半导体代工厂，2025 年 10 月营收为 3674.7 亿新台币，2026 年 10 月营收同比大幅增长。此前公司营收已连续多月保持增长态势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.design-reuse.com/news/202529634-tsmc-october-2025-revenue-report/">TSMC October 2025 Revenue Report</a></li>

</ul>
</details>

**标签**: `#earnings`, `#semiconductors`, `#technology`, `#company results`

---

<a id="item-finance-news-4"></a>
### [Polymarket 年化营收突破 18 亿美元](https://www.cnbc.com/2026/11/10/polymarket-annualized-revenue-us-growth.html) ⭐️ 7.0/10

预测市场平台 Polymarket 表示，其年化营收已超过 18 亿美元，为 2026 年 11 月的最新数据，高于今年 6 月披露的 10 亿美元以上。该公司美国本土交易所的快速增长推动了这一业绩，但目前正接受美国商品期货交易委员会的调查。

rss · CNBC Finance · 11月10日 13:00

**「背景」** Polymarket 是一家主要的预测市场平台，允许用户就各种事件结果进行交易，其美国本土交易所自 2026 年 5 月上线后推动了收入和交易量的快速增长。此前，Polymarket 的国际平台并未受到美国商品期货交易委员会（CFTC）监管，且公司正因合规问题接受监管调查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://polymarket.com/">Polymarket | The World’s Largest Prediction Market</a></li>
<li><a href="https://money.usnews.com/investing/articles/what-are-prediction-markets-predictit-polymarket-and-kalshi">What Are Prediction Markets ? Kalshi, PredictIt and Polymarket</a></li>

</ul>
</details>

**标签**: `#fintech`, `#earnings`, `#regulation`, `#markets`, `#funding`

---

<a id="item-finance-news-5"></a>
### [2026 年前三季度中国新能源车出口大增](https://finance.sina.com.cn/tech/roll/2026-10-26/doc-iniwpfnc2438186.shtml) ⭐️ 7.0/10

2026 年前三季度，中国新能源乘用车出口达到 388.7 万辆，同比增长 138.8%，为车企销量增长提供了重要支撑。

telegram · zaihuapd · 11月10日 02:56

**「背景」** 2025 年中国新能源车出口量超过 120 万辆，2026 年出口量有望进一步增长，主要原因是国内市场增速放缓，车企通过出口来维持产能和投资。此前，国内新能源车销量增速已降至个位数水平，出口成为行业增长的重要动力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ievchina.com/insights/china-ev-export-boom-2026-navigating-trade-barriers-seizing-new-markets/">China EV Export Boom 2026: Navigating Trade Barriers, Seizing ...</a></li>

</ul>
</details>

**标签**: `#automotive`, `#exports`, `#China`, `#economic data`, `#electric vehicles`

---

<a id="item-finance-news-6"></a>
### [Anthropic 撤回高达 693 亿美元 IPO 申请](https://www.reuters.com/business/anthropic-aims-raise-up-693-billion-blockbuster-ipo-2026-11-10/) ⭐️ 7.0/10

Anthropic 撤回了原计划募资最高 693 亿美元的首次公开募股（IPO）申请，称定价信息不准确并将更新相关文件。

telegram · zaihuapd · 11月10日 06:25

**「背景」** Anthropic 此前向银行分发了计划上市的文件，拟以每股 70 至 80 美元发行约 8.67 亿股，最高募资 693 亿美元，但随后公司称定价信息不准确并撤回了该文件。此前未有如此大规模的 IPO 计划被公开撤回。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech-insider.org/anthropic-ipo-retracted-math-60-7-to-69-3-billion-2026/">Anthropic IPO Math: $60.7B to $69.3B Retracted [2026]</a></li>
<li><a href="https://shattered.io/anthropic-ipo-retraction-what-69-3-billion-would-mean-2026/">Anthropic IPO Retraction: What $69.3B Would Mean [2026]</a></li>
<li><a href="https://shattered.io/anthropic-retracts-ipo-filing-pricing-867m-shares-70-80-range-2026/">Anthropic Retracts IPO Pricing: 867M Shares [2026]</a></li>

</ul>
</details>

**标签**: `#IPO`, `#technology`, `#capital markets`, `#corporate finance`

---

<a id="item-finance-news-7"></a>
### [多家银行上调美元存款利率，部分高于美联储基准](https://finance.sina.com.cn/roll/2026-11-10/doc-iniyfzhx2584501.shtml) ⭐️ 7.0/10

多家中国境内银行近期上调美元存款利率，其中大众银行深圳分行 12 个月美元定存利率升至 4.2%，已高于美联储 2026 年 9 月设定的 3.75%-4%基准区间。

telegram · zaihuapd · 11月10日 10:57

**「背景」** 2026 年 9 月，美联储将基准利率目标区间上调至 3.75%-4%，推动全球美元利率水平上升。此后，部分中国境内银行为应对外币存款流失压力，选择上调美元存款利率。 

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.federalreserve.gov/newsevents/pressreleases/monetary20260916a1.htm">Federal Reserve Board - Implementation Note issued September ...</a></li>

</ul>
</details>

**标签**: `#banking`, `#interest rates`, `#monetary policy`, `#currency`

---