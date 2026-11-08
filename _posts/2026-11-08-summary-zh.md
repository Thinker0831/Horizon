---
layout: default
title: "Horizon Summary: 2026-11-08 (ZH)"
date: 2026-11-08
lang: zh
---

> 从 39 条内容中筛选出 17 条重要资讯。

---

**科技新闻**
1. [Ant Ling 发布 Ling-3.2-flash：560B 参数原生多模态 MoE 模型](#item-tech-news-1) ⭐️ 9.0/10
2. [MaxxBench 批判 DeepSWE 基准测试方法](#item-tech-news-2) ⭐️ 8.0/10
3. [苹果发布人形机器人系统 HALO，采用双千问模型并开源](#item-tech-news-3) ⭐️ 8.0/10
4. [GitHub 新架构支持每秒 7200 次推送](#item-tech-news-4) ⭐️ 8.0/10
5. [微软研究院关闭 AI Frontiers 小组](#item-tech-news-5) ⭐️ 7.0/10
6. [Coldframe：模拟超市冷柜控制器的蜜罐项目发布](#item-tech-news-6) ⭐️ 7.0/10
7. [Mac 未公开守护进程构建用户社交关系图](#item-tech-news-7) ⭐️ 7.0/10
8. [Claude Code“勿再询问”功能导致密码泄露至 GitHub](#item-tech-news-8) ⭐️ 7.0/10
9. [Pointer Networks 在组合优化中的表现与局限](#item-tech-news-9) ⭐️ 7.0/10
10. [微软逐步终止租用甲骨文 AI 算力协议](#item-tech-news-10) ⭐️ 7.0/10
11. [Claude Code 被曝搜索时泄露用户邮箱](#item-tech-news-11) ⭐️ 7.0/10
12. [OnlyFake AI 假证平台创始人认罪被驱逐出境](#item-tech-news-12) ⭐️ 7.0/10
13. [Anthropic 因 Claude Max 用量宣传被判须应诉](#item-tech-news-13) ⭐️ 7.0/10
14. [美议员呼吁立法禁止 AI 递归自我改进](#item-tech-news-14) ⭐️ 7.0/10

**财经新闻**
1. [全国 3.35 万座寺院启动财务大检查](#item-finance-news-1) ⭐️ 8.0/10
2. [伯克希尔哈撒韦第三季度回购大幅增加，盈利下滑](#item-finance-news-2) ⭐️ 7.0/10
3. [软银与 ABB 拟分拆中国业务以挽救机器人收购案](#item-finance-news-3) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Ant Ling 发布 Ling-3.2-flash：560B 参数原生多模态 MoE 模型](https://www.reddit.com/r/MachineLearning/comments/1xpye7g/ant_ling_introduces_ling32flash_560b25b_native/) ⭐️ 9.0/10

Ant Ling 正式发布了 Ling-3.2-flash，这是一款拥有 5600 亿总参数、250 亿激活参数的原生多模态 MoE（专家混合）模型，支持最长 100 万 token 的上下文窗口。该模型原生支持文本、图像和视频输入，并在 MathVision、OmniDocBench 1.5、MedXpertQA-MM 等多个基准测试中取得了优异成绩。Ling-3.2-flash 还展示了 PDF 转代码、GUI 操作、3D 重建和多智能体协作等应用场景，API 兼容 OpenAI 和 Anthropic 标准。

reddit · r/MachineLearning · /u/the-hollow-soul · 11月7日 05:21

**「背景信息」** 混合专家（MoE, Mixture of Experts）架构是一种在大规模语言模型中常用的技术，通过只激活部分参数来提升推理效率和模型容量。多模态模型能够同时处理文本、图像和视频等多种输入类型，近年来在人工智能领域受到广泛关注。此前，主流多模态大模型的上下文窗口通常远小于 100 万（1M）token，且参数规模和 API 兼容性有限。

**标签**: `#multimodal`, `#large language models`, `#AI research`, `#MoE`, `#benchmarking`

---

<a id="item-tech-news-2"></a>
### [MaxxBench 批判 DeepSWE 基准测试方法](https://maxxbench.unlap.ai/research/why-maxxbench/) ⭐️ 8.0/10

MaxxBench 对当前流行的大型语言模型（LLM）基准 DeepSWE 的可靠性进行了深入批判，指出其存在方法学缺陷和实现漏洞。文章强调，DeepSWE 的分数可能无法真实反映模型的泛化能力，部分原因在于测试参数和任务规范的单一性，以及基准本身存在的 bug。该分析呼吁采用更健壮的评估方法，例如通过变更任务规范来检验模型表现的稳定性，并建议开发者警惕基准分数的表面意义。

hackernews · antiuniverse · 11月7日 17:19 · [社区讨论](https://news.ycombinator.com/item?id=50406222)

**「背景信息」** DeepSWE 是一个专为评估前沿代码生成代理（如大型语言模型）而设计的软件工程基准。与早期的 SWE-bench Pro 等基准相比，DeepSWE 的任务更具现实复杂性，要求模型生成更长的代码和输出。该基准还通过减少数据泄漏等方式，力图更准确地反映模型在真实开发任务中的表现。

**「影响」** AI 研究者和开发者在引用 DeepSWE 等基准分数时需更加谨慎，建议结合多样化的测试和参数变动来评估模型的实际能力。对于依赖这些基准进行模型选择或优化的团队，可能需要重新审视其评估流程，以避免因基准缺陷导致的误判。

**「社区讨论」** 多位评论者指出，较小模型在参数变化下表现波动更大，反映出过拟合和泛化能力不足的问题。部分用户对 DeepSWE 存在 bug 表示担忧，并认为当前主流基准测试的可靠性值得质疑，呼吁采用更复杂和多变的评测环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://deepswe.net/">DeepSWE Benchmark : GPT vs Claude for Agentic Coding</a></li>

</ul>
</details>

**标签**: `#AI evaluation`, `#benchmarks`, `#large language models`, `#software engineering`

---

<a id="item-tech-news-3"></a>
### [苹果发布人形机器人系统 HALO，采用双千问模型并开源](https://weibo.com/1642634100/RqjjGllvw) ⭐️ 8.0/10

苹果研究团队公开了人形机器人自主控制系统 HALO，并在宇树 G1 机器人上实现了仿真到现实的动作迁移。HALO 采用三层架构：顶层使用千问 Qwen3.6-35B-A3B 进行任务编排，中层用 Qwen3.5-2B 生成具体动作，底层为强化学习训练的动作跟踪器。团队已开源数据生成、模型训练和部署的全部代码，便于研究和工程社区复现与扩展。

telegram · zaihuapd · 11月7日 13:35

**「背景信息」** 千问（Qwen）是由阿里云开发的大型语言模型家族，涵盖了大语言模型（LLM）、多模态模型（LMM）等多种人工智能相关技术。Qwen 模型具备对话、图像与视频理解、文档处理等多项功能，并已被应用于机器人导航等实际场景。此次苹果 HALO 系统采用的 Qwen3.6-35B-A3B 和 Qwen3.5-2B，均属于该系列模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen">Org profile for Qwen on Hugging Face, the AI community building the...</a></li>
<li><a href="https://qwen.ai/">Qwen</a></li>
<li><a href="https://github.com/QwenLM/Qwen-RobotNav">GitHub - QwenLM/ Qwen -RobotNav: Official Repo for Qwen -RobotNav</a></li>

</ul>
</details>

**标签**: `#robotics`, `#AI systems`, `#machine learning`, `#open source`

---

<a id="item-tech-news-4"></a>
### [GitHub 新架构支持每秒 7200 次推送](https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/) ⭐️ 8.0/10

GitHub 推出了代号为 Rubicon 的新 Git 存储架构，专为支持大量 AI 智能体并发操作单个仓库而设计。在内部测试中，该架构可支持 5000 个智能体协作，每秒处理高达 7200 次推送，同时保持较低的读取延迟。新架构将 Git 对象存储在 Azure Blob Storage 上，引用状态由 Ref-CAS 管理，并通过虚拟副本和后台节点进行数据包压缩。目前该架构处于有限私有预览阶段，未来将逐步扩大推广范围。

telegram · zaihuapd · 11月7日 14:12

**「背景信息」** 随着 AI 智能体在软件开发中的广泛应用，GitHub 需要应对单个仓库高并发操作带来的存储和性能挑战。据 GitHub 官方博客介绍，过去一年中，AI 智能体极大改变了热门仓库的访问模式，促使 GitHub 在不影响现有服务的前提下，重新设计底层存储架构以支持更高的并发和可扩展性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/">Inside GitHub &#x27;s new Git storage architecture - The GitHub Blog</a></li>

</ul>
</details>

**标签**: `#infrastructure`, `#version-control`, `#scalability`, `#AI-workflows`

---

<a id="item-tech-news-5"></a>
### [微软研究院关闭 AI Frontiers 小组](https://hunch.net/?p=13764006) ⭐️ 7.0/10

微软研究院（Microsoft Research）已解散其 AI Frontiers 小组，这一小组专注于 AI 基础性前沿研究。此次调整表明微软正将重心从探索性 AI 研究转向对现有模型（尤其是 Transformer 类模型）的规模化扩展，这与当前业界普遍优先发展大规模模型的趋势一致。该变化反映出公司在资源分配和研究方向上的重大转变。

hackernews · srean · 11月7日 18:02 · [社区讨论](https://news.ycombinator.com/item?id=50406563)

**「背景信息」** 微软研究院（Microsoft Research）长期以来以推动人工智能基础研究著称，AI Frontiers 小组专注于探索性和前沿性 AI 技术的突破。近年来，业界普遍将重心转向基于 Transformer 的大规模模型扩展，许多大型科技公司也在调整研究方向以优先支持可快速落地和商业化的 AI 技术。

**「影响」** 受影响的研究人员可能需要转向更贴近产品化和规模化的 AI 项目，而非基础性、探索性研究。AI 领域的多样化创新空间可能因此进一步收窄，尤其是在大型科技公司内部。

**「社区讨论」** 多位评论者表达了对探索性 AI 研究被边缘化的担忧，认为当前行业过度聚焦于 Transformer 模型的规模化，忽视了其他潜在的创新路径。一些人还指出，这种转变可能损害了微软研究院长期以来鼓励自由探索的文化。

**标签**: `#AI research`, `#industry trends`, `#Microsoft`, `#transformer models`

---

<a id="item-tech-news-6"></a>
### [Coldframe：模拟超市冷柜控制器的蜜罐项目发布](https://github.com/hedgerow-dev/coldframe) ⭐️ 7.0/10

Coldframe 是一个用 Python 编写的蜜罐项目，专门模拟超市冷柜控制器（如 Danfoss AK-SM 800A 和 Dixell XWEB），用于研究针对工业系统的攻击行为。该项目通过精确还原真实设备的 HTTP 头顺序、页面标题、证书字段和 TLS 版本等细节，提升了伪装的真实性，并能识别多项已知漏洞（如 CVE-2025-41450）和默认登录尝试。Coldframe 仅依赖标准库，基于公开研究成果开发，目前已上线两台实例，主要被通用扫描器和 Shodan 爬虫访问。该项目适用于关注工业物联网安全的研究者和从业者。

hackernews · hedgerow-dev · 11月7日 17:27 · [社区讨论](https://news.ycombinator.com/item?id=50406292)

**「背景信息」** 蜜罐（honeypot）是一种网络安全工具，通过模拟真实设备或服务来吸引攻击者，从而研究其攻击手法并提升防御能力。近年来，工业控制系统（ICS）和物联网（IoT）设备频繁成为攻击目标，尤其是超市冷藏控制器等关键基础设施设备。Coldframe 项目正是在此背景下，针对现实中工业冷藏系统遭受攻击的事件，开发出高度仿真的蜜罐以便更好地理解和防护相关威胁。

**「影响」** 工业安全研究人员和安全团队可以利用 Coldframe 更真实地捕捉和分析针对冷链控制系统的攻击手法，有助于提前发现和防御相关威胁。由于该蜜罐高度还原真实设备，攻击者更难识别其为诱捕系统，从而提升了数据收集的有效性。

**「社区讨论」** 有用户质疑依赖 Shodan 数据还原设备真实性的有效性，认为许多互联网上的设备本身就是蜜罐或已被攻陷。项目作者则补充，现实中超市等场所缺乏专业安全团队，设备安全更多依赖厂商默认配置和维护，反映了工业设备安全管理的普遍短板。

**标签**: `#honeypots`, `#industrial-security`, `#IoT`, `#cybersecurity`

---

<a id="item-tech-news-7"></a>
### [Mac 未公开守护进程构建用户社交关系图](https://8rank.ai/game/apple-intelligence-personal-knowledge-graph) ⭐️ 7.0/10

有报道称，自 2022 年以来，每台 Mac 都内置了未公开的守护进程，这些进程会收集用户及其社交关系的信息，构建详细的个人知识图谱。该功能未在官方文档中披露，涉及用户身份、联系人、互动方式、活动时间地点等多维度数据。此举引发了关于隐私和透明度的技术与伦理讨论，尤其是在用户不知情的情况下自动收集和分析个人数据。

hackernews · infwhispers · 11月7日 09:46 · [社区讨论](https://news.ycombinator.com/item?id=50403097)

**「背景信息」** 据相关技术分析，macOS 系统自 2022 年起包含了两个未公开文档的守护进程，这些进程会在用户主目录下的 ~/Library/IntelligencePlatform 目录中维护个人知识图谱。该目录包含 51 个以明文存储的 SQLite 数据库，但受 TCC（透明度、同意与控制）全盘访问权限保护。这些数据库记录了用户及其社交关系的详细信息，相关行为引发了关于隐私和合规性的讨论，尤其是在 GDPR 等法规背景下。

**「影响」** Mac 用户的个人和社交数据可能被系统自动收集和分析，而用户对此过程缺乏知情权和控制权，增加了隐私泄露和数据滥用的风险。开发者和隐私关注者需警惕系统底层未公开的数据处理行为，评估其对合规性和用户信任的影响。

**「社区讨论」** 部分用户认为此类数据收集若为可选功能会更易接受，但在默认开启且不透明的情况下令人担忧。也有评论指出，这类知识图谱有助于本地 AI 助手（如 Siri）理解用户指令，但隐私和社交环境的边界应受到尊重。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50403097">Every Mac comes with an ( undocumented ) family member classifier</a></li>
<li><a href="https://8rank.ai/game/apple-intelligence-personal-knowledge-graph">Anatomy of Apple&#x27;s Personal Knowledge Graph — Eighth Rank</a></li>

</ul>
</details>

**标签**: `#privacy`, `#macOS`, `#system internals`, `#personal data`

---

<a id="item-tech-news-8"></a>
### [Claude Code“勿再询问”功能导致密码泄露至 GitHub](https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again) ⭐️ 7.0/10

Claude Code 的“Don&\#x27;t Ask Again（勿再询问）”功能导致 1,122 个包含密码的文件被公开上传至 GitHub。这些泄露主要发生在用户将本地 .claude/settings.local.json 配置文件（本应仅限本地使用）手动提交到公共代码仓库时，且文件中包含了敏感信息。Claude Code 官方表示该配置文件默认已被自动加入 .gitignore，但部分用户绕过此保护手动上传，且目前 Claude Code 并未内置自动密钥清理功能。

hackernews · shmulc · 11月7日 20:45 · [社区讨论](https://news.ycombinator.com/item?id=50407882)

**「事件背景」** Claude Code 是一个集成于终端的 AI 编程助手，能够理解代码库并通过自然语言命令协助开发者完成例行任务，包括处理 git 工作流。其“Don&\#x27;t Ask Again”功能允许用户对某些命令永久授权，减少交互确认。根据相关文档，.claude/settings.local.json 文件本应仅保存在本地，并被自动加入 .gitignore，防止被提交到代码仓库。然而，部分用户手动创建并将该文件及包含敏感信息的命令提交到了公共 GitHub 仓库，导致凭证泄露。

**「影响」** 受影响的开发者和团队需要立即检查自己的公共代码仓库，确保未误将包含敏感信息的 Claude Code 配置文件上传，并考虑采用专门的密钥管理工具或自动化密钥扫描工具来防止类似泄露。

**「社区讨论」** Claude Code 团队成员强调，配置文件本应仅限本地使用且已自动 gitignore，泄露多因用户手动上传。部分用户建议通过密码管理器、API 代理或隔离环境等方式加强安全防护，社区也讨论了 AI 工具权限管理与自动密钥清理的必要性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/anthropics/claude-code/issues">Issues · anthropics/ claude - code · GitHub</a></li>
<li><a href="https://support.claude.com/">Home | Claude Help Center</a></li>

</ul>
</details>

**标签**: `#security`, `#AI tools`, `#software engineering`, `#source control`

---

<a id="item-tech-news-9"></a>
### [Pointer Networks 在组合优化中的表现与局限](https://www.reddit.com/r/MachineLearning/comments/1xqgg4v/combinatorial_optimization_with_pointer_networks/) ⭐️ 7.0/10

一项技术分析评估了 Pointer Networks 在解决 NP 难题（如二维欧几里得旅行商问题）中的表现，并将其与 Google OR-Tools 等经典求解器进行了基准对比。结果显示，Pointer Networks 能够在毫秒级时间内生成高质量、近似最优的解，但随着问题规模从 N=20 扩展到 N=200，解的质量显著下降。分析指出，LSTM 编码器对坐标集的顺序性和近期性偏置与几何图的排列不变性不匹配，是导致性能下降的理论根源。该研究为机器学习方法在组合优化领域的实际应用和局限性提供了具体数据和理论解释。

reddit · r/MachineLearning · /u/an2ancan · 11月7日 20:44

**「背景信息」** Pointer Networks 是一种神经网络架构，最初被提出用于解决组合优化问题，如旅行商问题（TSP）。与传统的优化算法（如 Google OR-Tools）不同，Pointer Networks 通过学习输入序列之间的关系，直接生成问题的解序列。该方法通常采用序列到序列（seq2seq）结构，并利用注意力机制来“指向”输入中的元素，从而构建解答路径。近年来，研究者们尝试用神经方法加速 NP-hard 问题的近似求解，但模型在大规模问题上的泛化能力和解质量仍存在挑战。

**标签**: `#machine learning`, `#combinatorial optimization`, `#pointer networks`, `#benchmarking`

---

<a id="item-tech-news-10"></a>
### [微软逐步终止租用甲骨文 AI 算力协议](https://www.bloomberg.com/news/articles/2026-11-06/microsoft-is-winding-down-oracle-deal-to-rent-ai-cloud-capacity) ⭐️ 7.0/10

微软正在逐步终止与甲骨文租用 AI 算力的协议，近几个月未续签相关合同。知情人士透露，主要原因是甲骨文提供的硬件仍采用老一代英伟达芯片，已无法满足微软对 AI 计算的需求。该协议最初于 2023 年宣布，主要用于支持 Bing 搜索的 AI 版本。甲骨文方面表示 AI 基础设施需求依然强劲，并在 9 月以高于原价 20% 的价格续签了部分 GPU 合同，但微软对此未作回应。

telegram · zaihuapd · 11月7日 02:00

**「背景信息」** 微软与甲骨文的 AI 算力租赁协议最初于 2023 年宣布，旨在为 Bing 搜索的 AI 版本提供计算资源。当时，这一合作被视为全球算力短缺背景下，微软向竞争对手租用服务器的早期案例。随着 AI 基础设施需求持续增长，硬件的更新换代成为影响合作持续性的关键因素。

**「影响」** 受协议终止消息影响，甲骨文股价一度下跌约 3%。对于依赖最新 AI 硬件的企业用户而言，甲骨文现有基础设施的吸引力可能下降，微软则需寻找更符合其技术要求的算力供应商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zerohedge.com/markets/microsoft-pulls-plug-oracle-ai-rental-post-election-data-center-fallout-spreads">Microsoft Pulls The Plug On Oracle AI Rental As... | ZeroHedge</a></li>

</ul>
</details>

**标签**: `#cloud infrastructure`, `#AI hardware`, `#industry news`, `#enterprise agreements`

---

<a id="item-tech-news-11"></a>
### [Claude Code 被曝搜索时泄露用户邮箱](https://github.com/anthropics/claude-code/issues/107757) ⭐️ 7.0/10

有开发者发现，Claude Code 在进行网页搜索时，会将用户的登录邮箱地址包含在联网请求中发送出去，导致用户收到大量垃圾邮件。Anthropic 工程师回应称，此做法原为解决模型乱填作者名的问题，但已于 2.1.317 版本中增加拦截措施，尽管该措施可被 Python 脚本绕过。公司计划在下一个版本中彻底移除上下文中的登录邮箱信息。此前该问题已被报告，涉及邮箱泄露给 Wikipedia、美国证券交易委员会等第三方网站。

telegram · zaihuapd · 11月7日 08:09

**「背景信息」** Claude Code 是由 Anthropic 公司开发的 AI 编程助手，属于 Claude 系列大语言模型工具之一，广泛应用于辅助软件开发。该工具允许用户通过终端与 AI 进行交互，执行代码生成和联网请求等操作。由于其集成了用户身份信息以优化模型表现，相关隐私和安全问题成为开发者关注的焦点。

**「影响」** 受影响的开发者可能会因邮箱泄露而遭遇垃圾邮件甚至钓鱼攻击，建议用户在官方发布修复版本前谨慎使用相关联网功能，或采取临时防护措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_%28AI%29">Claude (AI) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#privacy`, `#AI tools`, `#software engineering`

---

<a id="item-tech-news-12"></a>
### [OnlyFake AI 假证平台创始人认罪被驱逐出境](https://www.404media.co/an-ai-fraud-kingpins-confessions/) ⭐️ 7.0/10

AI 假证平台 OnlyFake 的创始人 Nazarenko 因开发并运营自动化伪造证件服务被美国法院定罪并驱逐出境。OnlyFake 利用生成式 AI，以低至 15 美元的价格生成美国 50 州驾照、美国护照及全球约 56 国证件，曾被朝鲜虚假 IT 工作者等滥用。Nazarenko 在美国被捕并认罪，最终被判服刑一年后驱逐出境，且终身不得再入境美国。

telegram · zaihuapd · 11月7日 10:54

**「背景信息」** OnlyFake 是由乌克兰公民 Yurii Nazarenko 创办的 AI 驱动假证平台，允许用户生成美国 50 个州的驾照、美国护照及约 56 个其他国家的数字身份证件。该平台自 2021 年至 2024 年间运营，累计生成超过 1 万份假证，获利数十万美元。此次案件是美国司法部门首次针对数字假证平台提起指控之一，凸显生成式 AI 在网络犯罪中的新型应用及其带来的监管挑战。

**「影响」** 此次判决显示，利用生成式 AI 进行大规模证件伪造将面临严厉法律后果，并引发国际社会对 AI 滥用和身份安全的关注。相关平台用户和开发者需警惕法律风险，监管机构也可能加强对 AI 生成内容的审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/ukrainian-man-pleads-guilty-to-running-ai-powered-fake-id-site/">Ukrainian man pleads guilty to running AI -powered fake ID site</a></li>
<li><a href="https://me.pcmag.com/en/ai/35593/us-nabs-man-behind-onlyfake-which-trafficked-in-ai-powered-digital-fake-ids">US Nabs Man Behind OnlyFake , Which Trafficked in AI -Powered...</a></li>
<li><a href="https://securityaffairs.com/188734/cyber-crime/ukrainian-hacker-pleads-guilty-to-running-onlyfake-ai-id-scam-site.html">Ukrainian hacker pleads guilty to running OnlyFake AI ID scam site</a></li>

</ul>
</details>

**标签**: `#AI misuse`, `#cybersecurity`, `#generative AI`, `#legal issues`

---

<a id="item-tech-news-13"></a>
### [Anthropic 因 Claude Max 用量宣传被判须应诉](https://thenextweb.com/news/anthropic-claude-max-lawsuit-ruling-usage-claims) ⭐️ 7.0/10

美国加州北区联邦法院裁定，Anthropic 必须就 Claude Max 套餐用量宣传涉嫌误导用户的指控应诉。原告称，Claude Max 的 100 美元和 200 美元套餐分别宣称比 Pro 档多用 5 倍和 20 倍，但实际按周计算仅为 3.5 倍和 6 倍。法官认为，按会话计算的说明隐藏在销售页面的两个超链接之后，用户按月付费有理由理解为按月计算。法院允许过失虚假陈述和违约指控继续审理，但驳回了加州不正当经营和虚假广告的两项指控。

telegram · zaihuapd · 11月7日 12:44

**「背景信息」** Anthropic 是一家总部位于美国旧金山的人工智能公司，专注于开发大语言模型，其主要产品为 Claude 系列。该公司由前 OpenAI 成员于 2021 年创立，致力于 AI 安全和透明度。此次诉讼涉及其 Claude Max 套餐的用量宣传，原告质疑其广告中关于不同价格档位用量倍数的表述具有误导性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI industry`, `#legal`, `#Anthropic`, `#transparency`

---

<a id="item-tech-news-14"></a>
### [美议员呼吁立法禁止 AI 递归自我改进](https://x.com/AlexBores/status/2118494668769878037) ⭐️ 7.0/10

美国民主党议员 Alex Bores 呼吁国会在 2024 年立法，禁止 AI 递归自我改进（RSI），即 AI 自动构建下一代 AI。Bores 援引 OpenAI、Anthropic 和 METR 的行业预测，指出 AI 能力可能在未来几年内迅速提升，存在安全和对齐风险。他强调，AI 的错误或偏差可能在每一代中被放大，因此立法刻不容缓。目前这仅为立法倡议，尚未形成具体法律。

telegram · zaihuapd · 11月8日 01:30

**「递归自我改进（RSI）简介」** 递归自我改进（RSI）指的是 AI 系统能够自动改进自身架构或能力，进而开发出更强大的下一代 AI。该概念被认为可能导致 AI 能力的快速指数级提升，同时也带来人类难以控制的风险。Anthropic 等机构指出，完全实现 RSI 可能会显著增加人类对 AI 系统失控的风险，因此成为 AI 安全和监管领域的重要讨论议题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/institute/recursive-self-improvement">Our progress toward recursive self - improvement , and its implications.</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#AI safety`, `#regulation`, `#industry trends`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [全国 3.35 万座寺院启动财务大检查](https://www.163.com/dy/article/LB2VSRQD0556HNS1.html) ⭐️ 8.0/10

中国已对全国 3.35 万座寺院和 9000 余座道观启动财务大检查，要求年收入达到一定规模的宗教场所必须引入第三方审计，并严格限制商业活动和财务透明度。相关政策还规定，寺院住持亲属不得参与经营，所有收支需定期向信众公示。

telegram · zaihuapd · 11月7日 15:02

**「背景」** 此前，宗教场所的商业化和财务透明度问题在中国一直受到关注，相关部门已多次提出加强监管和规范管理。

**标签**: `#regulation`, `#policy`, `#religious organizations`, `#China`, `#financial audit`

---

<a id="item-finance-news-2"></a>
### [伯克希尔哈撒韦第三季度回购大幅增加，盈利下滑](https://www.cnbc.com/2026/11/07/berkshire-hathaway-q3-2026-earnings-buybacks.html) ⭐️ 7.0/10

伯克希尔哈撒韦公司 2026 年第三季度股票回购金额达到 96 亿美元，较上一季度的 45 亿美元翻倍，而同期公司整体盈利同比下降 28%至 221.12 亿美元。该公司在公告中披露，运营利润和保险业务利润均出现下滑。

rss · CNBC Finance · 11月7日 15:23

**「背景」** 伯克希尔哈撒韦是一家总部位于美国内布拉斯加州奥马哈的多元化控股公司，业务涵盖保险、铁路、能源等多个领域。该公司由格雷格·阿贝尔领导，长期以稳健的资本管理和大规模股票投资闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Berkshire_Hathaway">Berkshire Hathaway - Wikipedia</a></li>

</ul>
</details>

**标签**: `#earnings`, `#buybacks`, `#conglomerates`, `#investment`, `#stock performance`

---

<a id="item-finance-news-3"></a>
### [软银与 ABB 拟分拆中国业务以挽救机器人收购案](https://www.bloomberg.com/news/articles/2026-11-07/softbank-abb-weigh-china-carve-out-to-salvage-robotics-deal) ⭐️ 7.0/10

软银与 ABB 正考虑将 ABB 机器人业务的中国部分分拆为独立实体，以挽救被中国监管机构叫停的 54 亿美元收购案。

telegram · zaihuapd · 11月7日 11:24

**「背景」** 此前，软银计划以 54 亿美元收购 ABB 的机器人业务，但该交易本周被中国外商投资安全审查机制叫停。

**标签**: `#M&amp;A`, `#robotics`, `#regulation`, `#China`, `#technology`

---