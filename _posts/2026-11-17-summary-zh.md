---
layout: default
title: "Horizon Summary: 2026-11-17 (ZH)"
date: 2026-11-17
lang: zh
---

> 从 48 条内容中筛选出 23 条重要资讯。

---

**科技新闻**
1. [Optimizely 被攻破，Zoom 与 GitLab 等网站遭恶意软件投放](#item-tech-news-1) ⭐️ 8.0/10
2. [Marimba：单一冻结编码器的多任务语音模型发布](#item-tech-news-2) ⭐️ 8.0/10
3. [美国堵住远程访问先进 AI 芯片出口漏洞](#item-tech-news-3) ⭐️ 8.0/10
4. [山东大学团队提出首个哥德巴赫猜想条件性证明](#item-tech-news-4) ⭐️ 8.0/10
5. [卡内基梅隆大学将计算机科学课程免费上线 YouTube](#item-tech-news-5) ⭐️ 7.0/10
6. [Windows 11 收集开发者工具与编码代理的遥测数据](#item-tech-news-6) ⭐️ 7.0/10
7. [Jiff 1.0：Rust 的新日期时间库发布](#item-tech-news-7) ⭐️ 7.0/10
8. [无需微调的实时爵士 AI 伴奏：采样时引导音乐 Transformer](#item-tech-news-8) ⭐️ 7.0/10
9. [苹果启动健康 AI 使用研究，招募 20 万人](#item-tech-news-9) ⭐️ 7.0/10
10. [腾讯总办推动 AI 时代组织扁平化，减少管理岗位](#item-tech-news-10) ⭐️ 7.0/10
11. [腾讯混元发布 Hy4 flash，主打高性价比日常任务](#item-tech-news-11) ⭐️ 7.0/10
12. [美等十国签署《旧金山宣言》共保 AI 供应链](#item-tech-news-12) ⭐️ 7.0/10
13. [亚马逊警告 AI 代理利用 Artex 框架窃取 API 密钥](#item-tech-news-13) ⭐️ 7.0/10
14. [Apple 智能功能登陆国行 iPad 与 Mac，新增安全修复与使用上限](#item-tech-news-14) ⭐️ 7.0/10

**科技博客**
1. [NVIDIA cuPotential 加速分子动力学模拟的实践与分析](#item-tech-blog-1) ⭐️ 8.0/10

**财经新闻**
1. [中国 10 月经济数据全面低于预期，经济放缓加剧](#item-finance-news-1) ⭐️ 8.0/10
2. [英特尔因股价暴跌遭股东集体诉讼](#item-finance-news-2) ⭐️ 8.0/10
3. [伯克希尔哈撒韦三季度增持达美航空并减持美国银行](#item-finance-news-3) ⭐️ 7.0/10
4. [美国原油价格因中东出口恢复降至每桶 85 美元](#item-finance-news-4) ⭐️ 7.0/10
5. [英伟达高层动荡与国会政策或重塑 AI 板块格局](#item-finance-news-5) ⭐️ 7.0/10
6. [Cantor Fitzgerald 因与 Nvidia 关系及出口管制受审查](#item-finance-news-6) ⭐️ 7.0/10
7. [2026 年第三季度中国外资直接投资现净流出](#item-finance-news-7) ⭐️ 7.0/10
8. [英伟达董事会未考虑让黄仁勋回归 CEO](#item-finance-news-8) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Optimizely 被攻破，Zoom 与 GitLab 等网站遭恶意软件投放](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/) ⭐️ 8.0/10

知名网站优化服务 Optimizely 遭遇重大安全入侵，导致其脚本在包括 Zoom 和 GitLab 在内的多个大型网站上分发恶意软件。此次事件暴露了第三方脚本供应链的严重安全风险，尤其是当脚本管理权限下放给非工程团队时。受影响网站的用户可能在不知情的情况下暴露于恶意内容，具体受影响范围和持续时间尚未披露。

hackernews · kristjansson · 11月16日 23:00 · [社区讨论](https://news.ycombinator.com/item?id=50524767)

**「事件背景」** Optimizely 是一家广泛应用于网站 A/B 测试和优化的第三方服务平台。2026 年 11 月 16 日，攻击者在 Optimizely Web 实验平台中植入了恶意 JavaScript 代码，该代码通过 Optimizely 的脚本分发机制传播到包括 Zoom、GitLab、BBC、CNN、Salesforce、IKEA、HSBC 等在内的 178 家大型网站。安全监测公司 Report URI 指出，这些恶意脚本可窃取用户输入的加密货币钱包地址和银行卡信息，暴露了第三方脚本供应链的严重安全风险。

**「实际影响」** 受影响网站的用户在访问时可能被植入恶意脚本，尤其是在 iOS 设备上，部分脚本还会尝试利用特定系统漏洞。网站运营方需紧急审查并替换第三方脚本，防止进一步的安全威胁。

**「社区讨论」** 有开发者批评将脚本管理权限交给市场部门导致安全隐患，并呼吁大型网站应自行托管关键脚本而非依赖第三方。另有用户建议通过 NoScript 等工具减少暴露风险，也有人指出 Optimizely 及受影响网站缺乏有效的安全审查和发布流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shiftdelete.net/en/optimizely-malware">Optimizely Malware Hit 178 Sites: What It Stole and What to Do</a></li>
<li><a href="https://cybersecuritynews.com/optimizely-websites-hijacked/">Hackers Infect 178 Major Websites via Optimizely to Steal ...</a></li>

</ul>
</details>

**标签**: `#security`, `#web-infrastructure`, `#supply-chain`, `#incident-response`

---

<a id="item-tech-news-2"></a>
### [Marimba：单一冻结编码器的多任务语音模型发布](https://www.reddit.com/r/MachineLearning/comments/1xxsqro/marimba_a_system_one_model_for_speech_r/) ⭐️ 8.0/10

Marimba 是一款新型语音模型，采用单一冻结的 Qwen3-ASR-0.6B 编码器，每 8 秒音频窗口仅需一次编码即可支持多种类型的音频查询，包括术语检测、语言识别、说话人变化与计数等，无需针对特定术语训练。该模型在 9 项公开测试中有 6 项表现与 Qwen3-Omni 30B 持平或更优，在语言识别（FLEURS 数据集 100%）和说话人变化检测（AMI/VoxConverse AUROC 0.966-0.980）等任务上表现突出。Marimba 的代码和权重已开源，支持 pip 安装和 Hugging Face 在线体验。模型在场景分类等未见任务上表现为随机水平，且部分测试（如 turn-end）为自有数据集内分布。

reddit · r/MachineLearning · /u/solanotodesch · 11月16日 15:47

**「背景」** Marimba 是一种新型语音模型，旨在通过单一冻结的 Qwen3-ASR-0.6B 编码器实现多任务音频查询，包括术语检测、语言识别、说话人变化等。它与 Qwen3-Omni 30B 这一更大规模的多模态基础模型进行了对比，后者能够处理文本、图像、音频和视频等多种输入，并在多个基准测试中表现优异。Marimba 的创新之处在于无需针对特定术语进行训练即可实现零样本检测，并通过校准概率输出多类型问题的答案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.alphaxiv.org/abs/2611.18330">Marimba : A System One Model for Speech | alphaXiv</a></li>
<li><a href="https://huggingface.co/collections/Qwen/qwen3-omni">Qwen 3 - Omni - a Qwen Collection</a></li>
<li><a href="https://github.locker/QwenLM/Qwen3-Omni">Qwen 3 - Omni on GitHub (QwenLM/ Qwen 3 - Omni ) — FAQ &amp; Similar...</a></li>

</ul>
</details>

**标签**: `#speech-recognition`, `#machine-learning`, `#AI-models`, `#research`

---

<a id="item-tech-news-3"></a>
### [美国堵住远程访问先进 AI 芯片出口漏洞](https://www.reuters.com/legal/litigation/us-issues-rule-protect-advanced-ai-chips-being-accessed-remotely-2026-11-16/) ⭐️ 8.0/10

美国商务部于 11 月 16 日发布临时最终规则，将先进 AI 芯片及服务器的出口管制范围扩展至远程访问场景，防止通过第三国数据中心绕开出口限制。该规则由财政部和国家安全委员会主导起草，意味着即使芯片物理上未出口，远程调用也受限。此外，向印尼、马来西亚、新加坡、泰国和巴西再出口 AI 芯片也需申请许可。此举进一步收紧了中国等国家获取先进 AI 硬件的渠道。

telegram · zaihuapd · 11月16日 14:44

**「背景信息」** 此前，美国已对先进 AI 芯片的出口实施管制，主要针对中国等国家，防止其获取高性能计算硬件。然而，企业通过第三国数据中心远程访问受限芯片的做法成为监管漏洞。此次新规正是在此前出口限制基础上，进一步堵住了通过远程调用绕过管制的渠道。

**「影响」** 受新规影响，国际 AI 云服务和跨境数据中心将面临更严格的合规要求，相关企业需重新评估其 AI 硬件部署和远程服务策略，以避免违反美国出口管制规定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-16/us-moves-to-limit-remote-access-to-advanced-ai-chips">US Moves to Curb China’s Remote Access to Nvidia’s AI Chips</a></li>
<li><a href="https://edition.cnn.com/2026/11/16/politics/ai-chips-restrictions-china">Trump administration tightens restrictions on flow of AI chips ahead of...</a></li>
<li><a href="https://reason.com/2026/11/16/trumps-new-chip-export-rule-targets-china-but-exempts-tiktoks-parent-company/">Trump’s new chip export rule exempts TikTok’s parent company</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#export controls`, `#technology policy`, `#international regulation`

---

<a id="item-tech-news-4"></a>
### [山东大学团队提出首个哥德巴赫猜想条件性证明](https://mrc.sdu.edu.cn/info/1018/2193.htm) ⭐️ 8.0/10

山东大学李嘉民、刘建亚团队宣布，在广义黎曼猜想（GRH）成立并满足两种附加谱假设之一的前提下，首次给出了二元哥德巴赫猜想对所有充分大的偶数成立的条件性证明。该证明还限定两素数需位于该偶数的三分之一至三分之二之间。论文强调，这一结果不同于以往的经典筛法和圆法，且单靠广义黎曼猜想并不足以推出结论，因此目前仍非无条件证明。

telegram · zaihuapd · 11月16日 16:01

**「背景介绍」** 哥德巴赫猜想是数论中著名的未解难题，内容为每个大于 2 的偶数都可以表示为两个素数之和。尽管该猜想已被验证至极大范围，但至今尚无无条件的完整证明。此前的研究多采用筛法和圆法等经典方法，且通常仅能在某些假设或特定范围内给出部分结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thinkacademy.ca/blog/blog/2026/08/06/goldbach-conjecture-guide/">The Goldbach Conjecture : Math&#x27;s Most Famous Unsolved Problem</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#theory`, `#research`, `#algorithms`

---

<a id="item-tech-news-5"></a>
### [卡内基梅隆大学将计算机科学课程免费上线 YouTube](https://www.cs.cmu.edu/learn/) ⭐️ 7.0/10

卡内基梅隆大学（CMU）现已将其计算机科学课程的完整学期讲座免费发布在 YouTube 上，涵盖多个主题领域。该项目由 CS Learn 团队推动，采用自动化工具简化课程制作流程，每周将有新课程上线，更多内容计划于明年一月推出。与以往类似的开放课程项目相比，此次不仅包含基础课程，还涵盖高级课程如机器学习系统等。课程目前主要提供视频讲座，后续将补充项目作业和配套教材。

hackernews · pcompeau · 11月16日 20:43 · [社区讨论](https://news.ycombinator.com/item?id=50522980)

**「背景信息」** 麻省理工学院（MIT）等高校早已通过开放课程（如 MIT OpenCourseWare）向公众免费提供计算机科学等领域的完整课程内容。此前，卡内基梅隆大学也曾推出面向中学的 CS Academy 项目，提供互动式计算机科学课程，但主要面向中学阶段。此次将完整大学计算机科学课程系统性地免费发布到 YouTube，进一步拓展了高等教育资源的开放获取范围。

**「影响」** 全球学习者和自学者现在可以免费获得 CMU 高质量的计算机科学课程资源，尤其是那些难以获得顶尖高校教育机会的人群。开发者和教育者可利用这些课程进行自我提升或教学参考，但目前缺乏自动化反馈和完整作业体系，实际学习效果可能受限。

**「社区讨论」** 部分用户认为，尽管 AI 工具日益普及，系统性学习计算机科学基础仍然不可替代。也有评论指出，只有视频讲座而缺乏项目和反馈机制会影响学习深度，期待后续补充完整的课程作业和更高级别课程内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=hztO5vaBTRs">Demonstration of Carnegie Mellon CS Academy - YouTube</a></li>
<li><a href="https://www.openculture.com/freeonlinecourses">1,700 Free Online Courses from Top Universities | Open Culture</a></li>

</ul>
</details>

**标签**: `#computer-science-education`, `#open-access`, `#software-engineering`, `#artificial-intelligence`

---

<a id="item-tech-news-6"></a>
### [Windows 11 收集开发者工具与编码代理的遥测数据](https://xusheng.dev/posts/windows-coding-agent-telemetry/) ⭐️ 7.0/10

有报道指出，Windows 11 正在收集关于用户所用编码代理（coding agents）和开发者工具的遥测数据。这一做法引发了开发者社区对隐私的担忧，并促使部分开发者考虑转向其他操作系统。具体收集的数据类型、用途及用户控制选项尚未详细披露，但该行为已引发广泛讨论。

hackernews · cwaffles · 11月16日 22:58 · [社区讨论](https://news.ycombinator.com/item?id=50524736)

**「背景信息」** Windows 11 和其前身 Windows 10 一直因默认收集用户遥测数据而受到关注。遥测数据通常包括系统使用情况、应用程序活动等信息，微软称其用于改进产品体验。社区中已有多种工具和方法（如 PowerShell 脚本、第三方工具）用于阻止或减少 Windows 的遥测数据收集，反映出用户对隐私的持续担忧。

**「影响」** 受此影响，一些开发者正在考虑迁移到 Linux 等替代操作系统，以规避 Windows 11 的数据收集行为。这可能导致部分开发者生态向更注重隐私的平台转移，尤其是在对工具和工作流敏感的用户群体中。

**「社区讨论」** 多位评论者表示，因对隐私的担忧，他们已计划或正在将开发环境从 Windows 迁移到 Linux，并分享了迁移经验和相关资源。部分用户认为 Windows 11 的数据收集范围可能远超当前已知，进一步加剧了对微软平台的不信任。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/N0tHorizon/WindowsTelemetryBlocker">N0tHorizon/WindowsTelemetryBlocker: A PowerShell based tool to...</a></li>
<li><a href="https://www.youtube.com/watch?v=-E-WC_UvHXE">Windows 11 : Kill Telemetry , Widgets &amp; Bloat - YouTube</a></li>

</ul>
</details>

**标签**: `#privacy`, `#operating-systems`, `#developer-tools`, `#software-engineering`

---

<a id="item-tech-news-7"></a>
### [Jiff 1.0：Rust 的新日期时间库发布](https://burntsushi.net/jiff/) ⭐️ 7.0/10

Jiff 1.0 正式发布，为 Rust 语言带来一个稳定且经过深思熟虑设计的日期时间库。Jiff 由知名开发者 burntsushi 编写，作为 Chrono 的新替代方案，旨在解决 Rust 生态中长期存在的日期时间处理痛点。1.0 版本的发布意味着该库已达到生产可用的稳定阶段，适用于需要精确时间处理的开发者和科学计算场景。Jiff 明确声明并非适用于所有用例，强调专业工程实践。

hackernews · burntsushi · 11月16日 16:53 · [社区讨论](https://news.ycombinator.com/item?id=50519744)

**「背景介绍」** 在 Rust 生态中，处理日期和时间的主要库长期以来是 Chrono，但其 API 设计和时区处理方式一直存在争议。Jiff 是由知名开发者 BurntSushi 开发的新日期时间库，旨在通过将时区处理作为核心设计，自动解决许多与夏令时相关的常见问题。Jiff 还支持通过 crate 特性自定义标准库、serde 支持以及是否将时区数据库嵌入二进制文件等功能。

**「影响」** Rust 开发者现在有了 Chrono 之外的稳定日期时间库选择，特别适合对时间精度和 API 设计有更高要求的项目。对于需要处理多种时间尺度或科学计算的用户，Jiff 可能简化了以往需要手动实现的复杂时间转换逻辑。

**「社区讨论」** 有前 Chrono 维护者表示，Chrono 的 API 改进阻力大，导致维护压力大，对 Jiff 的出现表示感激。部分用户赞赏 Jiff 明确自身适用范围，认为这是专业工程的体现；也有开发者关注 Jiff 对多种时间尺度（如 TAI、UT1）的支持，期待其在科学计算领域的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://burntsushi.net/jiff/">A datetime library for Rust - Andrew Gallant&#x27;s Blog</a></li>
<li><a href="https://github.com/burntsushi/jiff">GitHub - BurntSushi/ jiff : A datetime library for Rust that encourages...</a></li>

</ul>
</details>

**标签**: `#rust`, `#datetime`, `#libraries`, `#software engineering`

---

<a id="item-tech-news-8"></a>
### [无需微调的实时爵士 AI 伴奏：采样时引导音乐 Transformer](https://www.reddit.com/r/MachineLearning/comments/1xxkyh3/steering_a_pretrained_music_transformer_at/) ⭐️ 7.0/10

一款名为 duetto 的实时爵士伴奏系统利用预训练的 Anticipatory Music Transformer（Thickstun 等，2023），通过采样时的规则化 logit 编辑实现模型输出的引导，无需对模型进行微调。该方法在每次采样前通过规则层屏蔽不允许的音符并对特定音高或节奏进行偏置，使模型能够根据玩家的实时输入进行互动伴奏。系统支持 MIDI 键盘，能够在低延迟下完成实时演奏，相关代码已开源供非商业用途。该方法展示了在符号音乐生成领域通过采样时控制实现模型行为定制的创新实践。

reddit · r/MachineLearning · /u/GGAllin43 · 11月16日 09:19

**「背景」** Anticipatory Music Transformer（AMT）是一种基于 Transformer 的音乐生成模型，最初由 Thickstun 等人在 2023 年提出。该模型通过在大规模 Lakh MIDI 音乐数据集上训练，能够实现自动回归音乐生成，并具备“填充控制”能力，即在给定部分旋律的情况下生成伴奏或补全音乐片段。AMT 的预训练模型可直接用于多种音乐生成任务，无需针对特定应用进行微调。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2306.08620">[2306.08620] Anticipatory Music Transformer - arXiv.org</a></li>
<li><a href="https://github.com/jthickstun/anticipation">GitHub - jthickstun/anticipation: Anticipatory Autoregressive ... Anticipatory Music Transformer - arXiv.org Anticipatory Music Transformer - G-CLef @ CMU Anticipation and the Anticipatory Music Transformer Anticipatory Music Transformer - John Thickstun</a></li>

</ul>
</details>

**标签**: `#machine learning`, `#music AI`, `#transformers`, `#real-time systems`

---

<a id="item-tech-news-9"></a>
### [苹果启动健康 AI 使用研究，招募 20 万人](https://www.apple.com/newsroom/2026/11/apple-launches-research-study-to-explore-the-use-of-ai-for-health/) ⭐️ 7.0/10

苹果与 OpenEvidence 合作，在美国启动 Apple Health AI Usage Study，旨在研究用户如何与对话式健康 AI 互动，并评估用户对该类 AI 的信任和理解。该研究计划招募最多 20 万名年满 21 岁、使用支持 Apple Intelligence 的 iPhone 15 Pro 或更新机型、运行 iOS 26 及以上系统的美国居民。研究数据不会用于 AI 模型训练，且该应用不用于诊断或治疗疾病。

telegram · zaihuapd · 11月16日 05:01

**「背景信息」** 苹果公司与 OpenEvidence 合作，在美国推出了 Apple Health AI Usage Study，这是一项虚拟研究，旨在通过相关应用程序了解用户如何与健康领域的对话式 AI 互动。该研究主要关注用户对健康 AI 的信任和理解，而不是用于诊断或治疗。参与者需使用支持 Apple Intelligence 的 iPhone 15 Pro 或更新机型，并运行 iOS 26 及以上系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/11/apple-launches-research-study-to-explore-the-use-of-ai-for-health/">announced the launch of an Apple Health AI Usage Study</a></li>
<li><a href="https://www.livemint.com/technology/apps/apple-launches-ai-health-study-app-in-partnership-with-openevidence-who-can-participate-and-how-it-works-11794798693805.html">Apple launches AI health study app in partnership with ... - Mint</a></li>

</ul>
</details>

**标签**: `#healthcare AI`, `#industry initiative`, `#user study`, `#Apple`

---

<a id="item-tech-news-10"></a>
### [腾讯总办推动 AI 时代组织扁平化，减少管理岗位](https://weibo.com/1642634100/RrCqPwhiS) ⭐️ 7.0/10

腾讯总办近日发布内部讲话，号召公司核心业务团队在 AI 时代“再创业”，推动组织结构扁平化，并以小团队为基本作战单元。讲话明确提出未来不需要那么多管理岗位，强调要打破山头主义和地盘意识，管理和工作方式也需借助 AI 重新设计。这一举措反映出腾讯在 AI 浪潮下对内部管理体系和创新模式的重大调整。该政策目前针对公司内部，尚未披露具体实施细节。

telegram · zaihuapd · 11月16日 06:32

**「背景信息」** 近期，腾讯等中国大型科技公司正经历由 AI 驱动的组织结构调整。根据媒体报道，腾讯高层在公司 28 周年内部讲话中强调，AI 相关转型已从局部试点走向全面重组，要求各业务团队适应 AI 时代的创新和组织变革。这一趋势不仅体现在腾讯，也反映了整个行业对 AI 技术推动管理和业务流程再设计的重视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eu.36kr.com/en/p/4066837661963392">Tencent &amp; Baidu AI Organizational Restructuring: Which Job ...</a></li>

</ul>
</details>

**标签**: `#AI strategy`, `#organizational change`, `#technology industry`, `#management`

---

<a id="item-tech-news-11"></a>
### [腾讯混元发布 Hy4 flash，主打高性价比日常任务](https://mp.weixin.qq.com/s/5yBbf-ctYziM5r0i6Y17lA) ⭐️ 7.0/10

腾讯混元正式发布了 Hy4 flash 大模型，参数总量为 224B，激活参数为 12B，支持多模态和 100 万 Token 上下文窗口。该模型 API 价格相比 Hy4 大幅下降，单任务成本为 Hy4 preview 的 1/13、Hy4 的 1/20，综合效果略优于 Hy4 preview。Hy4 flash 已在腾讯云 TokenHub、WorkBuddy、元宝等平台上线，计划后续开源，并在 11 月 30 日前对 WorkBuddy 用户限时免费、API 五折优惠。API 定价为每百万 Token 输入 0.5 元、输出 2 元，命中缓存仅需 0.02 元。

telegram · zaihuapd · 11月16日 07:17

**「背景介绍」** 腾讯混元此前已推出 Hy4 模型，该模型为 7700 亿参数的 MoE（混合专家）大模型，支持 100 万上下文窗口，并已在腾讯云 TokenHub、WorkBuddy、元宝等平台上线。Hy4 以其大规模参数和多模态能力在国内大模型市场中具有一定影响力，但其 API 定价相对较高。Hy4 flash 的推出是在原有 Hy4 基础上，针对日常任务和成本优化需求的进一步细分。

**「影响」** 对于需要大模型日常任务的开发者和企业用户，Hy4 flash 显著降低了使用成本，并提升了多模态和长上下文处理能力，有助于推动大模型在实际业务场景中的普及和应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/tencent-hy4">Tencent Hunyuan Hy 4 : specs, benchmarks, and pricing... | eesel AI</a></li>
<li><a href="https://help.apiyi.com/en/hy4-vs-deepseek-v4-1-flash-comparison-en.html">Hy 4 vs. DeepSeek V4.1 Flash : 27 Wins in 34 Official... - Apiyi.com Blog</a></li>
<li><a href="https://www.binance.com/en/square/post/11-16-2026-tencent-hunyuan-launches-hy4-flash-with-224b-parameters-and-12b-active-388785367980171">Tencent Hunyuan Launches Hy 4 Flash With 224B Parameters and...</a></li>

</ul>
</details>

**标签**: `#large language models`, `#AI industry`, `#model deployment`, `#cost optimization`

---

<a id="item-tech-news-12"></a>
### [美等十国签署《旧金山宣言》共保 AI 供应链](https://www.state.gov/releases/office-of-the-spokesman/2026/11/the-san-francisco-declaration-on-the-secure-foundations-of-enduring-prosperity/) ⭐️ 7.0/10

美国与澳大利亚、印度、以色列、日本、韩国、卡塔尔、新加坡、阿联酋和英国于 11 月 15 日签署《旧金山宣言》，承诺共同保护支撑超级智能（SI）供应链的敏感技术与关键基础设施。宣言设立五个工作组，分别聚焦创新政策、SI 在关键领域的应用、全栈供应链协作、安全港与安全枢纽、以及 SI 的安全与韧性。该宣言为国际合作提供政策框架，但目前尚未公布具体技术措施或实施细节。此次签署主要为政策层面的联合声明，实际影响有待后续观察。

telegram · zaihuapd · 11月16日 10:40

**「背景介绍」** 《旧金山宣言》是在 2026 年 11 月 15 日由美国及九国共同签署，旨在通过建立合作机制，加强对超级智能（SI）相关敏感技术和关键基础设施的供应链安全保护。该宣言确立了共同的原则和行动路径，并设立五个工作组，分别聚焦创新政策、SI 应用、供应链协作、安全港与安全枢纽、以及 SI 安全与韧性。各国认为，单一国家无法独自保障 SI 时代的基础安全，必须通过国际合作来实现持久繁荣。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.state.gov/releases/office-of-the-spokesman/2026/11/the-san-francisco-declaration-on-the-secure-foundations-of-enduring-prosperity/">The San Francisco Declaration on the Secure Foundations of ...</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#supply chain`, `#international cooperation`, `#technology industry`

---

<a id="item-tech-news-13"></a>
### [亚马逊警告 AI 代理利用 Artex 框架窃取 API 密钥](https://cybernews.com/security/amazon-autonomous-cybercrime-artex-framework/) ⭐️ 7.0/10

亚马逊报告称，攻击者利用开源渗透测试框架 Artex 驱动 AI 代理，针对 LiteLLM、Dify 等公网暴露的 AI 应用窃取 API 密钥。被盗密钥经验证后汇入共享池，用于支付更多大模型调用，实现自我供血。该活动自 10 月 3 日开始，11 月 5 日被亚马逊的诱饵网络 MadPot 截获并阻断。亚马逊以中等信心将此次攻击归因于中国相关威胁组织，并已通知可能受影响的 AWS 客户。

telegram · zaihuapd · 11月16日 13:00

**「背景信息」** Artex 是一个开源的渗透测试框架，最初设计用于合法的安全测试，但近期被发现被攻击者利用以自动化网络攻击。FBI 和多家安全机构近期警告，Artex 及其 AI 代理已被用于全球范围内的攻击，包括针对企业云服务和 API 的入侵。由于其开源特性，即使原始仓库被下架，仍有多个副本在代码托管平台上流传，增加了滥用风险。

**「影响分析」** AI 应用开发者和云服务用户需警惕 API 密钥暴露风险，及时检查和加固相关安全措施，防止密钥被自动化工具批量窃取并滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/fbi-warns-artex-ai-hacking-tool-is-powering-global-cyberattacks/">FBI warns ARTEX AI hacking tool is powering global cyberattacks</a></li>
<li><a href="https://www.malwarebytes.com/blog/ai/2026/11/criminals-are-using-artex-ai-agents-to-speed-up-cyberattacks-fbi-warns">Criminals are using ARTEX AI agents to speed up cyberattacks , FBI...</a></li>
<li><a href="https://thehackernews.com/2026/11/backdoored-docker-image-for-artex-ai.html">CERT-In Flags AI -Driven Attacks as Backdoored ARTEX Exposes 62...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#API security`, `#cybersecurity`, `#cloud services`

---

<a id="item-tech-news-14"></a>
### [Apple 智能功能登陆国行 iPad 与 Mac，新增安全修复与使用上限](https://www.theverge.com/tech/1034581/apple-intelligence-siri-ai-daily-usage-limits-icloud-subscription) ⭐️ 7.0/10

Apple 智能（Apple Intelligence）现已通过 iPadOS 27.3 beta 2 和 macOS 27.3 beta 2 向中国大陆的 iPad 和 Mac 用户开放体验。此次更新还修复了所有 Apple 操作系统中的文件沙箱逃逸漏洞。此外，苹果在 iOS 27.3、iPadOS 27.3 和 macOS 27.3 beta 2 中测试了部分 Siri AI 与 Apple 智能功能的每日设备使用上限，基础 Siri 命令依然免费不限量，但云端进阶功能（如多步骤个人情境请求、图片生成与编辑）将受到限制。

telegram · zaihuapd · 11月16日 20:12

**「背景信息」** Apple Intelligence 最初在中国通过 iOS 27.3 beta 首次登陆 iPhone，如今随着 iPadOS 27.3 和 macOS 27.3 beta 2 的发布，支持范围扩展到了 iPad 和 Mac。此前，苹果已向中国监管机构注册相关功能，经历了较长等待期后才逐步开放至更多设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/11/16/ipad-mac-apple-intelligence-china/">iPad and Mac Get Apple Intelligence in China in 27.3 Betas</a></li>
<li><a href="https://appleinsider.com/articles/26/11/09/apple-intelligence-registered-for-ipad-mac-use-in-china">Apple Intelligence registered for iPad, Mac use in China</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#security`, `#operating systems`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [NVIDIA cuPotential 加速分子动力学模拟的实践与分析](https://developer.nvidia.com/blog/accelerate-molecular-dynamics-simulations-with-accurate-flexible-primitives-using-nvidia-cupotential/) ⭐️ 8.0/10

rss · NVIDIA CUDA Technical Blog · 11月16日 22:30

**「背景」** 分子动力学（MD）模拟广泛应用于物理、化学和生物等领域，但在 GPU 架构不断演进的今天，如何高效、准确地评估周期性边界下的长程相互作用（如静电和色散力）成为主要的计算与工程瓶颈。传统的 PME（Particle Mesh Ewald）方法虽为主流，但在兼容性、性能和易用性上对 MD 引擎开发者提出了更高要求。

**「方案」** 作者介绍了 NVIDIA cuPotential 库，它通过 C API 提供模块化的原语，允许开发者灵活替换和加速 MD 模拟中的关键计算环节。cuPotential 不仅支持直接空间和倒空间的高效计算，还为 OpenMM 等主流 MD 平台提供了插件，实现几乎无缝集成。文章详细讲解了在 Linux 环境下的构建、安装和验证流程，并通过 OpenMM 基准体系（如 DHFR、BACE、ApoA1 等）展示了准确性和性能测试方法。性能方面，cuPotential 在多种 NVIDIA GPU 上对 24,000 至 40 万原子的系统实现了 2-3 倍甚至更高的加速。核心技术突破在于与 D. E. Shaw Research 和 Flatiron Institute 合作开发的新型 C2 连续分割与扩散函数，这些方法在保持高精度的同时，允许缩小实空间截断和网格规模，显著降低能量漂移和误差。对于色散能，cuPotential 能将能量误差降低数千倍，且计算成本更低。文章还强调了能量漂移分析的重要性，cuPotential 在 10 ns 水体系模拟中表现出远优于传统 PME 的能量守恒性。

**「启示」** cuPotential 为分子动力学模拟提供了兼具高性能与高精度的 GPU 加速方案，尤其在长程相互作用和能量守恒方面实现了显著突破，极大简化了开发者的集成与优化工作。

**标签**: `#molecular-dynamics`, `#gpu-acceleration`, `#numerical-methods`, `#benchmarking`, `#simulation-software`

---

## 财经新闻

<a id="item-finance-news-1"></a>
### [中国 10 月经济数据全面低于预期，经济放缓加剧](https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html) ⭐️ 8.0/10

中国 10 月零售销售同比仅增长 0.4%，低于分析师预期的 0.8%，而工业产出同比增长 4.8%，也未达到 5.3%的预期，固定资产投资前十个月同比下降 8.1%，跌幅大于预期。分析师警告，经济对出口的依赖加大，使中国增长更易受外部冲击影响。

rss · CNBC Finance · 11月16日 03:53

**「背景」** 此前，2026 年 9 月中国工业产出同比增长 5.5%，为五个月来最高水平，而 10 月零售销售同比增长 1.1%，但 10 月两项数据均低于市场预期，显示经济复苏动能减弱。固定资产投资和消费持续疲软，反映出房地产市场低迷和内需不足对经济的持续压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html">China ’s slowdown deepens in October as key economic data ...</a></li>

</ul>
</details>

**标签**: `#China economy`, `#economic data`, `#retail sales`, `#industrial output`, `#trade`

---

<a id="item-finance-news-2"></a>
### [英特尔因股价暴跌遭股东集体诉讼](https://www.investing.com/news/stock-market-news/intel-sued-by-shareholders-following-29-stock-plunge-5028171) ⭐️ 8.0/10

英特尔及其 CEO 陈立武因被指隐瞒 PC 需求疲软和库存积压，遭股东集体诉讼，起因是公司 10 月 29 日发布的第四季度营收和利润预测低于预期，导致次日股价暴跌 28.6%。诉讼由密歇根州养老基金牵头，索赔对象为 2026 年 7 月 23 日至 10 月 29 日期间买入股票的投资者。

telegram · zaihuapd · 11月16日 11:10

**「背景」** 此前，英特尔因个人电脑（PC）需求疲软和库存积压导致季度盈利下滑，2026 年第三季度净利润同比下降 18%，并引发股价大幅下跌。该公司近期还加大了对人工智能相关制造的投资，但未能抵消 PC 业务的下行压力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wccftech.com/intel-ceo-lip-bu-tan-named-defendant-class-action-lawsuit-pc-sales-slowdown/">Intel CEO Lip-Bu Tan Named As Defendant In New Class-Action...</a></li>
<li><a href="https://www.kucoin.com/news/flash/intel-q3-net-profit-falls-18-amid-pc-demand-weakness-shares-drop-over-21-post-market">Intel &#x27;s Q3 net profit falls 18% amid weak PC demand , shares ... | KuCoin</a></li>

</ul>
</details>

**标签**: `#corporate litigation`, `#earnings`, `#technology sector`, `#stock market`, `#investor impact`

---

<a id="item-finance-news-3"></a>
### [伯克希尔哈撒韦三季度增持达美航空并减持美国银行](https://www.cnbc.com/2026/11/16/berkshire-hathaway-raised-its-stake-in-delta-air-in-the-third-quarter.html) ⭐️ 7.0/10

伯克希尔哈撒韦在 2026 年第三季度将其达美航空持股增加 12%，同时将美国银行持股减少近 6%。这反映了公司对航空和银行板块的最新投资调整。

rss · CNBC Finance · 11月16日 23:01

**「背景」** 伯克希尔哈撒韦是一家由格雷格·阿贝尔领导的大型投资公司，长期以来以其对主要上市公司的持股变动受到市场关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/16/berkshire-hathaway-raised-its-stake-in-delta-air-in-the-third-quarter.html">Berkshire Hathaway raised its stake in Delta in the third ...</a></li>

</ul>
</details>

**标签**: `#Berkshire Hathaway`, `#stock holdings`, `#Delta Air Lines`, `#Bank of America`, `#institutional investment`

---

<a id="item-finance-news-4"></a>
### [美国原油价格因中东出口恢复降至每桶 85 美元](https://www.cnbc.com/2026/11/16/us-crude-oil-declines-to-87-a-barrel-on-recovering-middle-east-exports.html) ⭐️ 7.0/10

受中东原油出口恢复影响，美国原油价格下跌至每桶 85 美元，为实际市场价格。国际能源署（IEA）预计 2026 年第四季度全球原油供应将每日超过需求 170 万桶，显示市场由短缺转为过剩。

rss · CNBC Finance · 11月16日 22:19

**「背景」** 此前，国际能源署（IEA）曾预计中东地区的石油供应要到 2027 年才能完全恢复，但最近数据显示中东原油出口已接近战前水平，推动全球供应增加。此前由于地区冲突，全球石油供应一度紧张，油价因此上涨。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iea.org/reports/oil-market-report-october-2026">Oil Market Report - October 2026 - IEA</a></li>
<li><a href="https://www.iea.org/reports/oil-market-report-september-2026">Oil Market Report - September 2026 - IEA</a></li>
<li><a href="https://www.worldoil.com/news/2026/9/11/iea-cuts-2026-oil-supply-outlook-as-gulf-recovery-slips-to-2027/">IEA cuts 2026 oil supply outlook as Gulf recovery slips to 2027</a></li>

</ul>
</details>

**标签**: `#oil prices`, `#energy markets`, `#Middle East exports`, `#IEA forecast`, `#commodities`

---

<a id="item-finance-news-5"></a>
### [英伟达高层动荡与国会政策或重塑 AI 板块格局](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 7.0/10

据 ETF 专家称，英伟达 CEO 黄仁勋辞职及其股价连续下跌，加上民主党控制的国会可能限制数据中心扩张，这些因素可能使竞争芯片厂商和大型科技公司受益。Yorkville Ives 将英伟达目标价从 300 美元下调至 225 美元，并预计国会新政策可能导致 10%至 20%的数据中心建设计划被取消。

rss · CNBC Finance · 11月16日 12:13

**「背景」** 英伟达（Nvidia）前首席执行官黄仁勋因被卷入与中国相关的间谍丑闻，于 2026 年 11 月辞职，引发国会对国家安全风险的关注，并导致对公司领导层的质疑和政策讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehill.com/homenews/senate/6217057-congress-jensen-huang-nvidia-national-security/">Jensen Huang resigns from Nvidia amid China spying scandal as ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI`, `#ETF`, `#Tech Stocks`, `#Policy`

---

<a id="item-finance-news-6"></a>
### [Cantor Fitzgerald 因与 Nvidia 关系及出口管制受审查](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 7.0/10

美国政府对 Cantor Fitzgerald 及其领导层与 Nvidia 的关系展开审查，因涉及对中国出口限制和潜在利益冲突，Cantor 在 2025 年 9 月至 2026 年 3 月间报告的 Nvidia 持股数量下降了 49%。

rss · CNBC Finance · 11月16日 12:14

**「背景」** 近期，Nvidia 首席执行官黄仁勋辞职后，美国商务部长霍华德·卢特尼克及其家族与该芯片制造商的财务关系受到重新关注。此前，卢特尼克因其部门未将涉嫌将 Nvidia AI 芯片转运至中国的 Megaspeed 公司列入黑名单而面临两党压力，并被批评对 Nvidia 采取较为宽松的监管立场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html">Howard Lutnick&#x27;s sons&#x27; Nvidia ties amid Jensen Huang China ...</a></li>
<li><a href="https://www.firstpost.com/explainers/nvidia-scandal-why-is-trump-commerce-secretary-howard-lutnick-under-fire-14060250.html">Nvidia scandal: Why is Trump’s Commerce Secretary Howard ...</a></li>
<li><a href="https://www.nytimes.com/2026/11/12/us/politics/lutnick-nvidia-commerce-china-chips.html">Howard Lutnick Took Softer Line on Nvidia as Calls for ...</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#Cantor Fitzgerald`, `#regulation`, `#conflict of interest`, `#technology`

---

<a id="item-finance-news-7"></a>
### [2026 年第三季度中国外资直接投资现净流出](https://cn.nikkei.com/china/ceconomy/64726-2026-11-16-09-03-25.html) ⭐️ 7.0/10

2026 年 7 月至 9 月，中国外商直接投资（FDI）出现 9 亿美元净流出，这是四个季度以来首次转为负值。该数据来自中国国家外汇管理局公布的国际收支统计。

telegram · zaihuapd · 11月16日 05:29

**「背景」** 此前连续四个季度中国吸引的外商直接投资（FDI）为净流入，显示外资持续进入中国市场。

**标签**: `#China`, `#foreign direct investment`, `#capital flows`, `#economic data`

---

<a id="item-finance-news-8"></a>
### [英伟达董事会未考虑让黄仁勋回归 CEO](https://www.cnbc.com/2026/11/16/nvidia-ceo-jensen-huang.html) ⭐️ 7.0/10

据 CNBC 援引知情人士消息，英伟达董事会目前未考虑让黄仁勋回归 CEO，并已聘请律师事务所调查其行为是否涉及国家安全和公司机密风险。

telegram · zaihuapd · 11月17日 01:39

**「背景」** 此前，英伟达董事会已聘请 Wachtell Lipton 律所调查黄仁勋的行为，重点关注其是否涉及危及公司机密或国家安全的问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/10/nvidia-wachtell-lipton-huang-affair.html">Nvidia hires law firm Wachtell Lipton to lead Jensen Huang ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/16/nvidia-ceo-jensen-huang.html">Nvidia board not considering bringing Huang back as CEO: Source</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#corporate governance`, `#executive leadership`, `#technology sector`

---