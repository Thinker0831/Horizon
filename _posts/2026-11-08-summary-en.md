---
layout: default
title: "Horizon Summary: 2026-11-08 (EN)"
date: 2026-11-08
lang: en
---

> From 39 items, 17 important content pieces were selected

---

**Technology News**
1. [Ant Ling Releases Ling-3.2-flash: 560B Multimodal MoE Model](#item-tech-news-1) ⭐️ 9.0/10
2. [MaxxBench Critiques DeepSWE LLM Benchmark Reliability](#item-tech-news-2) ⭐️ 8.0/10
3. [Apple Reveals HALO Humanoid Robot System Using Qwen Models](#item-tech-news-3) ⭐️ 8.0/10
4. [GitHub Unveils New Git Storage Architecture Supporting 7200 Pushes/sec](#item-tech-news-4) ⭐️ 8.0/10
5. [Microsoft Research Disbands AI Frontiers Group](#item-tech-news-5) ⭐️ 7.0/10
6. [Coldframe Honeypot Emulates Supermarket Fridge Controllers](#item-tech-news-6) ⭐️ 7.0/10
7. [Undocumented Mac Daemons Build Personal Knowledge Graphs](#item-tech-news-7) ⭐️ 7.0/10
8. [Claude Code &\#x27;Don&\#x27;t Ask Again&\#x27; Led to Password Leaks on GitHub](#item-tech-news-8) ⭐️ 7.0/10
9. [Pointer Networks for Combinatorial Optimization: Benchmarks and Limitations](#item-tech-news-9) ⭐️ 7.0/10
10. [Microsoft Phases Out Oracle AI Compute Rental Deal](#item-tech-news-10) ⭐️ 7.0/10
11. [Claude Code May Leak User Emails During Web Search](#item-tech-news-11) ⭐️ 7.0/10
12. [OnlyFake AI Fake ID Platform Founder Convicted and Deported](#item-tech-news-12) ⭐️ 7.0/10
13. [Anthropic Must Face Lawsuit Over Claude Max Usage Claims](#item-tech-news-13) ⭐️ 7.0/10
14. [US Lawmaker Urges Ban on AI Recursive Self-Improvement](#item-tech-news-14) ⭐️ 7.0/10

**Financial News**
1. [China Launches Financial Audit of Over 33,500 Temples](#item-finance-news-1) ⭐️ 8.0/10
2. [Berkshire Hathaway Doubles Share Buybacks as Earnings Fall in Q3 2026](#item-finance-news-2) ⭐️ 7.0/10
3. [SoftBank and ABB Consider China Carve-Out to Save $5.4 Billion Robotics Deal](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Ant Ling Releases Ling-3.2-flash: 560B Multimodal MoE Model](https://www.reddit.com/r/MachineLearning/comments/1xpye7g/ant_ling_introduces_ling32flash_560b25b_native/) ⭐️ 9.0/10

Ant Ling has released Ling-3.2-flash, a native multimodal Mixture-of-Experts \(MoE\) model with 560 billion total parameters and 25 billion activated parameters per inference. The model supports a 1 million token context window and accepts text, image, and video inputs. Benchmark results show strong performance across diverse tasks, including math, vision, medical, and document understanding, with notable scores such as 96.80 on MathVision and 89.52% comprehensiveness on AntBench-Medical. Ling-3.2-flash offers both OpenAI-compatible and Anthropic-compatible API access, and demonstrates capabilities like PDF-to-code, GUI operation, 3D reconstruction, and multi-agent collaboration.

reddit · r/MachineLearning · /u/the-hollow-soul · Nov 7, 05:21

**「Background」** Mixture-of-Experts \(MoE\) architectures are a type of neural network design that selectively activates subsets of model parameters for each input, enabling very large models to be trained and used efficiently. Multimodal models are capable of processing and understanding multiple types of input data, such as text, images, and video, within a single architecture. Recent advances in large language models have focused on expanding context windows and supporting broader input modalities, but context windows of 1 million tokens and native multimodal support at this scale remain rare.

**Tags**: `#multimodal`, `#large language models`, `#AI research`, `#MoE`, `#benchmarking`

---

<a id="item-tech-news-2"></a>
### [MaxxBench Critiques DeepSWE LLM Benchmark Reliability](https://maxxbench.unlap.ai/research/why-maxxbench/) ⭐️ 8.0/10

A technical analysis by MaxxBench questions the reliability of DeepSWE benchmark scores for large language models \(LLMs\), highlighting methodological flaws and the presence of bugs in the benchmark itself. The article demonstrates that varying task specifications can reveal weaknesses in model generalization and exposes how some models, especially smaller ones, are prone to score collapses under such variations. The discussion also notes that some models may overfit to specific benchmark tasks, and that the &\#x27;max mode&\#x27; evaluation approach can be misleading. These findings suggest that current LLM benchmarks like DeepSWE may not provide robust or generalizable measures of model capability.

hackernews · antiuniverse · Nov 7, 17:19 · [Discussion](https://news.ycombinator.com/item?id=50406222)

**「Background」** DeepSWE is a software engineering benchmark designed to evaluate large language models \(LLMs\) on complex, long-horizon coding tasks. Compared to earlier benchmarks like SWE-bench Pro, DeepSWE features prompts that are shorter but require solutions with significantly more code and output tokens, aiming to better reflect real-world software engineering challenges. The benchmark also attempts to reduce issues like benchmark leakage, which previously gave certain models an artificial advantage.

**「Impact」** Practitioners and researchers relying on DeepSWE or similar benchmarks should be cautious, as the reported scores may not accurately reflect real-world model performance or generalization. The analysis encourages the adoption of more rigorous and varied evaluation methods to avoid overfitting and to better assess LLM capabilities.

**「Community Discussion」** Commenters generally agree that the article exposes important flaws in current LLM benchmarking practices, with several expressing increased skepticism about benchmark reliability. Some highlight the tendency of smaller models to perform poorly under varied task specifications, while others point out the need for more robust and diverse evaluation environments to prevent overfitting and misleading results.

<details><summary>References</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://deepswe.net/">DeepSWE Benchmark : GPT vs Claude for Agentic Coding</a></li>

</ul>
</details>

**Tags**: `#AI evaluation`, `#benchmarks`, `#large language models`, `#software engineering`

---

<a id="item-tech-news-3"></a>
### [Apple Reveals HALO Humanoid Robot System Using Qwen Models](https://weibo.com/1642634100/RqjjGllvw) ⭐️ 8.0/10

Apple has disclosed its HALO humanoid robot control system, which uses two Qwen models for hierarchical control. The system employs Qwen3.6-35B-A3B at the top layer for task planning and Qwen3.5-2B at the middle layer for action generation, with a reinforcement learning-trained tracker at the bottom. HALO has been validated on the Unitree G1 robot, successfully transferring skills learned in simulation to execution in unfamiliar real-world environments. Apple has open-sourced the code for data generation, model training, and deployment.

telegram · zaihuapd · Nov 7, 13:35

**「Background」** Qwen is a family of large language models developed by Alibaba Cloud, offering capabilities in language understanding, multimodal processing, and agentic system integration. These models have been used in various AI and robotics applications, including navigation and task planning. The HALO system leverages two different Qwen models for hierarchical control in humanoid robotics, building on Qwen&\#x27;s established use in agentic and robotic contexts.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen">Org profile for Qwen on Hugging Face, the AI community building the...</a></li>
<li><a href="https://github.com/QwenLM/Qwen-RobotNav">GitHub - QwenLM/ Qwen -RobotNav: Official Repo for Qwen -RobotNav</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#AI systems`, `#machine learning`, `#open source`

---

<a id="item-tech-news-4"></a>
### [GitHub Unveils New Git Storage Architecture Supporting 7200 Pushes/sec](https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/) ⭐️ 8.0/10

GitHub has introduced a new Git storage architecture, codenamed Rubicon, designed to support high-concurrency operations such as those generated by AI agents. In internal testing, Rubicon handled 5000 AI agents collaborating on a single repository, achieving up to 7200 pushes per second while maintaining low read latency. The architecture stores Git objects in Azure Blob Storage, manages reference states with Ref-CAS, and uses virtual replicas for read/write operations and background data compression. Rubicon is currently in limited private preview and will be gradually rolled out to more users.

telegram · zaihuapd · Nov 7, 14:12

**「Background」** GitHub&\#x27;s new storage architecture, codenamed Rubicon, was developed in response to the increasing demands of agentic \(AI-driven\) development, where automated agents perform high-frequency operations on repositories. Over the past year, the rise of such agents has significantly changed the workload patterns on GitHub, necessitating a more scalable and concurrent storage solution. The new system was built while maintaining GitHub&\#x27;s ongoing operations, aiming to support hundreds of millions of developers and their automated workflows.

**「Impact」** Organizations and developers with large-scale, automated, or AI-driven workflows will benefit from significantly improved scalability and concurrency in GitHub repositories. Early access is limited, so most users will need to wait for broader availability before leveraging these enhancements.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/engineering/architecture-optimization/inside-githubs-new-git-storage-architecture/">Inside GitHub &#x27;s new Git storage architecture - The GitHub Blog</a></li>

</ul>
</details>

**Tags**: `#infrastructure`, `#version-control`, `#scalability`, `#AI-workflows`

---

<a id="item-tech-news-5"></a>
### [Microsoft Research Disbands AI Frontiers Group](https://hunch.net/?p=13764006) ⭐️ 7.0/10

Microsoft Research has closed its AI Frontiers group, which was dedicated to fundamental advances in artificial intelligence. This move reflects a shift in Microsoft&\#x27;s research priorities away from exploratory AI research and toward scaling established transformer-based models. The change aligns with a broader industry trend where companies prioritize scaling and iteration of current AI architectures over riskier, foundational research. The closure affects researchers focused on novel AI methods within Microsoft.

hackernews · srean · Nov 7, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50406563)

**「Background」** Microsoft Research has historically maintained specialized groups focused on fundamental advances in artificial intelligence, such as the AI Frontiers group. These groups have contributed to early-stage, exploratory research distinct from the product-driven development of established AI models. The closure of such a group reflects a shift in research priorities within large technology companies, where resources are increasingly allocated to scaling and refining existing transformer-based AI models rather than pursuing alternative or foundational approaches.

**「Impact」** Researchers at Microsoft who were engaged in fundamental AI exploration may need to shift their focus to scaling existing models or seek opportunities elsewhere for foundational research. This could reduce the diversity of AI research directions within the company and potentially slow progress on alternative approaches to AI beyond transformers.

**「Community Discussion」** Commenters express concern that the closure signals a narrowing of research priorities, with companies discouraging exploration of alternative AI methods in favor of scaling transformer models. Some lament the loss of a culture that valued fundamental research, warning that this focus on predictability and scale could stifle innovation and risk missing out on potentially superior approaches.

**Tags**: `#AI research`, `#industry trends`, `#Microsoft`, `#transformer models`

---

<a id="item-tech-news-6"></a>
### [Coldframe Honeypot Emulates Supermarket Fridge Controllers](https://github.com/hedgerow-dev/coldframe) ⭐️ 7.0/10

Coldframe is a new honeypot project that convincingly mimics supermarket refrigeration controllers, specifically emulating the Danfoss AK-SM 800A and Dixell XWEB interfaces. Written in Python using only the standard library, it closely matches real device behaviors such as HTTP headers, page sizes, and TLS versions, making it difficult to distinguish from actual devices on platforms like Shodan. The honeypot recognizes and logs attempts to exploit known vulnerabilities, including CVE-2025-41450 and several other Danfoss and Dixell issues, and provides a fake dashboard to observe attacker behavior beyond initial access. Coldframe is available as open source and has been deployed in the wild, though so far it has only attracted generic scanners and Shodan crawlers.

hackernews · hedgerow-dev · Nov 7, 17:27 · [Discussion](https://news.ycombinator.com/item?id=50406292)

**「Background」** Honeypots are decoy systems designed to attract and study attackers by mimicking real devices or services, often used in cybersecurity research to understand attack methods and vulnerabilities. Industrial control systems, such as supermarket refrigeration controllers, have become targets for cyberattacks due to their increasing connectivity and often limited security measures. Recent public research and incidents involving attacks on these types of devices have highlighted the need for realistic honeypots to better assess threats and inform defensive strategies.

**「Impact」** Security researchers and defenders can use Coldframe to study real-world attack techniques targeting industrial refrigeration systems, potentially improving detection and mitigation strategies for operational technology environments. Its high fidelity may also help identify new attack patterns or vulnerabilities that are actively being exploited.

**「Community Discussion」** Commenters debated the reliability of using Shodan data to model honeypots, with some warning that many devices found online are themselves honeypots or already compromised. Others highlighted the broader issue of poor security practices in industrial environments, noting that patching and secure configuration are often neglected due to lack of dedicated security teams in settings like supermarkets.

**Tags**: `#honeypots`, `#industrial-security`, `#IoT`, `#cybersecurity`

---

<a id="item-tech-news-7"></a>
### [Undocumented Mac Daemons Build Personal Knowledge Graphs](https://8rank.ai/game/apple-intelligence-personal-knowledge-graph) ⭐️ 7.0/10

Recent research claims that every Mac since 2022 ships with undocumented background daemons that construct a detailed personal and social knowledge graph about the user and their contacts. These daemons reportedly track relationships, communication patterns, locations, and activities, but their existence and operation are not disclosed to users. This has sparked significant debate about privacy, transparency, and user consent, as the functionality is neither opt-in nor clearly documented.

hackernews · infwhispers · Nov 7, 09:46 · [Discussion](https://news.ycombinator.com/item?id=50403097)

**「Background」** Apple&\#x27;s macOS reportedly includes two undocumented daemons that build a personal knowledge graph about users and their social connections. According to technical analysis, these daemons store their data in the ~/Library/IntelligencePlatform directory, using a set of fifty-one plaintext SQLite databases protected by TCC Full Disk Access. This system is not publicly documented by Apple, raising questions about transparency and user awareness.

**「Impact」** Mac users may have their personal and social data processed and analyzed without explicit awareness or consent, raising potential privacy risks and concerns about data transparency. Developers and privacy advocates may need to reassess trust in macOS system processes and push for clearer documentation and user controls.

**「Community Discussion」** Some commenters argue that such data collection could be useful for features like personalized assistants, but express discomfort with the lack of transparency and opt-in controls. Others note that while similar data is already used by apps like Photos and Calendar, the undocumented nature of these daemons undermines user trust and contradicts Apple&\#x27;s stated privacy principles.

<details><summary>References</summary>
<ul>
<li><a href="https://8rank.ai/game/apple-intelligence-personal-knowledge-graph">Anatomy of Apple&#x27;s Personal Knowledge Graph — Eighth Rank</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#macOS`, `#system internals`, `#personal data`

---

<a id="item-tech-news-8"></a>
### [Claude Code &\#x27;Don&\#x27;t Ask Again&\#x27; Led to Password Leaks on GitHub](https://apiiro.com/blog/coding-agents-leaking-secrets-github-dont-ask-again) ⭐️ 7.0/10

A security incident involving Claude Code&\#x27;s &\#x27;Don&\#x27;t Ask Again&\#x27; feature resulted in passwords being exposed in 1,122 public GitHub files. The issue arose when users committed their local .claude/settings.local.json files—which can contain approved commands with embedded secrets—to public repositories, despite these files being intended for local use and automatically gitignored by Claude when created through its interface. Claude Code does not perform automated secret scrubbing, and the exposure was due to manual user actions rather than an automatic process.

hackernews · shmulc · Nov 7, 20:45 · [Discussion](https://news.ycombinator.com/item?id=50407882)

**「Background」** Claude Code is an AI-powered coding assistant that operates in the terminal and can automate coding tasks, manage git workflows, and interact with codebases using natural language commands. The tool creates a local configuration file, .claude/settings.local.json, which is intended to remain on the user&\#x27;s machine and is automatically added to .gitignore when generated by Claude. However, if users manually create or modify this file and commit it to a public repository, sensitive information such as passwords or API keys can be inadvertently exposed.

**「Impact」** Developers using Claude Code should review their repositories to ensure that sensitive local configuration files, especially those containing secrets, are not committed to source control. Organizations may need to update internal guidelines and consider additional secret scanning tools to mitigate similar risks.

**「Community Discussion」** Claude Code team members clarified that the exposed files were manually committed and that the tool&\#x27;s default behavior is to gitignore sensitive local settings. Commenters debated the responsibility of secret management, with some advocating for stricter operational security and others sharing strategies like using password managers or isolated environments to limit AI agent access to credentials.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/anthropics/claude-code/issues">Issues · anthropics/ claude - code · GitHub</a></li>
<li><a href="https://support.claude.com/">Home | Claude Help Center</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI tools`, `#software engineering`, `#source control`

---

<a id="item-tech-news-9"></a>
### [Pointer Networks for Combinatorial Optimization: Benchmarks and Limitations](https://www.reddit.com/r/MachineLearning/comments/1xqgg4v/combinatorial_optimization_with_pointer_networks/) ⭐️ 7.0/10

A technical analysis evaluates classical Pointer Network architectures, trained with REINFORCE, for solving the 2D Euclidean Travelling Salesman Problem \(TSP\). The study benchmarks these neural models against Google OR-Tools \(Guided Local Search, 10s timeout\) across problem sizes from N=20 to N=200. Results show that Pointer Networks generate solutions almost instantly, but solution quality degrades significantly as problem size increases. The analysis attributes this limitation to the LSTM encoder&\#x27;s artificial sequential ordering and recency bias, which conflicts with the permutation-invariant nature of geometric graphs.

reddit · r/MachineLearning · /u/an2ancan · Nov 7, 20:44

**「Background」** Pointer Networks are a neural network architecture introduced to address combinatorial optimization problems, such as the Travelling Salesman Problem \(TSP\), by learning to output sequences that represent solutions. Unlike classical solvers, Pointer Networks use attention mechanisms to select elements from an input set, making them suitable for problems where the output is a permutation of the input. Traditional approaches to TSP, like Google OR-Tools, rely on algorithmic heuristics rather than learned models.

**Tags**: `#machine learning`, `#combinatorial optimization`, `#pointer networks`, `#benchmarking`

---

<a id="item-tech-news-10"></a>
### [Microsoft Phases Out Oracle AI Compute Rental Deal](https://www.bloomberg.com/news/articles/2026-11-06/microsoft-is-winding-down-oracle-deal-to-rent-ai-cloud-capacity) ⭐️ 7.0/10

Microsoft is gradually ending its agreement to rent AI compute capacity from Oracle, having not renewed contracts in recent months. The decision is attributed to Oracle&\#x27;s use of older-generation NVIDIA chips, which no longer meet Microsoft&\#x27;s technical requirements. The original deal, announced in 2023, supported AI features in Bing search. Oracle stated that demand for its AI infrastructure remains strong and noted a recent GPU contract renewal at a 20% price increase, while Microsoft declined to comment.

telegram · zaihuapd · Nov 7, 02:00

**「Background」** Microsoft and Oracle announced their AI compute rental agreement in 2023, with Microsoft renting Oracle&\#x27;s servers to support the AI-powered version of Bing. At the time, this arrangement was seen as evidence of a global shortage of high-performance compute resources, prompting even direct competitors to collaborate. The deal specifically addressed the need for large-scale AI infrastructure during a period of intense demand for advanced hardware.

**「Impact」** Organizations relying on Oracle&\#x27;s AI cloud offerings may face increased scrutiny over hardware currency and competitiveness, while Microsoft will likely shift its AI workloads to alternative providers or its own infrastructure to meet performance needs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.zerohedge.com/markets/microsoft-pulls-plug-oracle-ai-rental-post-election-data-center-fallout-spreads">Microsoft Pulls The Plug On Oracle AI Rental As... | ZeroHedge</a></li>

</ul>
</details>

**Tags**: `#cloud infrastructure`, `#AI hardware`, `#industry news`, `#enterprise agreements`

---

<a id="item-tech-news-11"></a>
### [Claude Code May Leak User Emails During Web Search](https://github.com/anthropics/claude-code/issues/107757) ⭐️ 7.0/10

Developers have reported that Claude Code, an AI coding tool, may leak users&\#x27; login email addresses during web search requests, resulting in increased spam and exposure to third parties. Anthropic engineers acknowledged that the email was added to the model context to address an earlier issue with author name attribution, but this led to emails being sent to sites like Wikipedia and the U.S. Securities and Exchange Commission. Version 2.1.317 introduced a partial fix by blocking the email, but this can be bypassed with Python scripts. Anthropic plans to remove the login email from the model context entirely in the next release.

telegram · zaihuapd · Nov 7, 08:09

**「Background」** Claude Code is an AI-powered coding assistant developed by Anthropic, designed to help developers write and analyze code. It is part of the broader Claude suite of AI tools, which are used for various problem-solving and productivity tasks. The tool integrates with online resources to assist users, which can involve sending requests to external websites.

**「Impact」** Developers using Claude Code may have their email addresses unintentionally exposed to external websites during web searches, increasing their risk of receiving spam or being targeted by malicious actors. Users should be cautious and monitor for updates addressing this privacy issue.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_%28AI%29">Claude (AI) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#privacy`, `#AI tools`, `#software engineering`

---

<a id="item-tech-news-12"></a>
### [OnlyFake AI Fake ID Platform Founder Convicted and Deported](https://www.404media.co/an-ai-fraud-kingpins-confessions/) ⭐️ 7.0/10

The founder of OnlyFake, an AI-powered fake ID platform, was convicted in the United States and subsequently deported after automating document forgery using generative AI. OnlyFake enabled users to generate fake IDs—including U.S. driver’s licenses, passports, and documents from over 56 countries—for as little as $15. The platform evolved from manual Photoshop forgery to a fully automated service leveraging generative AI. The founder, Nazarenko, received a sentence equivalent to time served \(about one year\), was ordered deported, detained by ICE for several months, and is now permanently barred from re-entering the U.S.

telegram · zaihuapd · Nov 7, 10:54

**「Background」** OnlyFake was an online platform operated by Yurii Nazarenko from 2021 to 2024 that used generative AI to automate the creation of fake digital identification documents. The service enabled customers to generate counterfeit U.S. driver&\#x27;s licenses, passports, and IDs from over 50 countries, reportedly producing at least 10,000 fake IDs and earning hundreds of thousands of dollars. This case is notable as one of the first involving criminal charges for the use of AI-powered digital fake IDs.

**「Impact」** This case demonstrates the real-world legal consequences for operators of AI-driven forgery services and highlights the growing regulatory and law enforcement attention on generative AI misuse in security-sensitive areas. Users and developers of similar platforms face increased risk of prosecution and international scrutiny.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/ukrainian-man-pleads-guilty-to-running-ai-powered-fake-id-site/">Ukrainian man pleads guilty to running AI -powered fake ID site</a></li>
<li><a href="https://me.pcmag.com/en/ai/35593/us-nabs-man-behind-onlyfake-which-trafficked-in-ai-powered-digital-fake-ids">US Nabs Man Behind OnlyFake , Which Trafficked in AI -Powered...</a></li>
<li><a href="https://securityaffairs.com/188734/cyber-crime/ukrainian-hacker-pleads-guilty-to-running-onlyfake-ai-id-scam-site.html">Ukrainian hacker pleads guilty to running OnlyFake AI ID scam site</a></li>

</ul>
</details>

**Tags**: `#AI misuse`, `#cybersecurity`, `#generative AI`, `#legal issues`

---

<a id="item-tech-news-13"></a>
### [Anthropic Must Face Lawsuit Over Claude Max Usage Claims](https://thenextweb.com/news/anthropic-claude-max-lawsuit-ruling-usage-claims) ⭐️ 7.0/10

A US federal court has ruled that Anthropic must respond to allegations of misleading advertising regarding the usage tiers of its Claude Max subscription plans. The lawsuit claims that the $100 and $200 tiers were advertised as offering 5x and 20x more usage than the Pro plan, but in practice, users received only about 3.5x and 6x more usage per week. The court found that key details about usage calculations were hidden behind hyperlinks and that monthly subscribers could reasonably expect monthly calculations. Claims of negligent misrepresentation and breach of contract will proceed, while claims under California&\#x27;s unfair competition and false advertising laws were dismissed.

telegram · zaihuapd · Nov 7, 12:44

**「Background」** Anthropic is an American artificial intelligence company known for developing the Claude series of large language models. The company was founded in 2021 by former OpenAI members and focuses on AI safety and transparency. Claude Max is one of its subscription offerings, with different usage tiers marketed to customers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#legal`, `#Anthropic`, `#transparency`

---

<a id="item-tech-news-14"></a>
### [US Lawmaker Urges Ban on AI Recursive Self-Improvement](https://x.com/AlexBores/status/2118494668769878037) ⭐️ 7.0/10

US Democratic lawmaker Alex Bores has called on Congress to pass legislation in 2024 banning recursive self-improvement \(RSI\) in artificial intelligence, which would prohibit AI systems from autonomously developing more advanced versions of themselves. Bores cited industry forecasts from OpenAI and Anthropic, as well as research from METR, suggesting that AI could soon automate most advanced model development. He argued that current alignment and error issues in AI could be amplified with each generation, making urgent regulation necessary.

telegram · zaihuapd · Nov 8, 01:30

**「Background」** Recursive self-improvement \(RSI\) in AI refers to the process where an AI system is capable of autonomously improving its own architecture or creating more advanced versions of itself. This concept is considered significant because it could accelerate AI development beyond human oversight, raising concerns about safety and control. Industry research, including from Anthropic, has highlighted that full RSI could increase the risk of humans losing control over advanced AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/institute/recursive-self-improvement">Our progress toward recursive self - improvement , and its implications.</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#AI safety`, `#regulation`, `#industry trends`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China Launches Financial Audit of Over 33,500 Temples](https://www.163.com/dy/article/LB2VSRQD0556HNS1.html) ⭐️ 8.0/10

China has begun a nationwide financial audit of more than 33,500 temples and 9,000 Taoist sites, requiring third-party audits for venues with significant income and imposing strict controls on commercial activities and financial transparency.

telegram · zaihuapd · Nov 7, 15:02

**「Background」** China previously allowed temples and Taoist sites to engage in some commercial activities, but concerns about financial transparency and commercialization have led to increased regulatory scrutiny.

**Tags**: `#regulation`, `#policy`, `#religious organizations`, `#China`, `#financial audit`

---

<a id="item-finance-news-2"></a>
### [Berkshire Hathaway Doubles Share Buybacks as Earnings Fall in Q3 2026](https://www.cnbc.com/2026/11/07/berkshire-hathaway-q3-2026-earnings-buybacks.html) ⭐️ 7.0/10

Berkshire Hathaway more than doubled its share buybacks to $9.6 billion in the third quarter of 2026, while overall earnings fell 28% year over year to $22.1 billion. The company reported that operating profits and insurance business earnings also declined compared to the same period last year.

rss · CNBC Finance · Nov 7, 15:23

**「Background」** Berkshire Hathaway is a large American conglomerate holding company based in Omaha, Nebraska, known for its diverse business interests and significant stock market investments.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Berkshire_Hathaway">Berkshire Hathaway - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#earnings`, `#buybacks`, `#conglomerates`, `#investment`, `#stock performance`

---

<a id="item-finance-news-3"></a>
### [SoftBank and ABB Consider China Carve-Out to Save $5.4 Billion Robotics Deal](https://www.bloomberg.com/news/articles/2026-11-07/softbank-abb-weigh-china-carve-out-to-salvage-robotics-deal) ⭐️ 7.0/10

SoftBank and ABB are considering splitting off ABB&\#x27;s China robotics business to rescue a $5.4 billion acquisition that was blocked by Chinese regulators this week. The plan would create a separate entity for the China business with different ownership, according to sources.

telegram · zaihuapd · Nov 7, 11:24

**「Background」** Chinese regulators recently blocked SoftBank&\#x27;s planned $5.4 billion acquisition of ABB&\#x27;s robotics business, prompting both companies to consider restructuring the deal by separating the China operations into a distinct entity.

**Tags**: `#M&amp;A`, `#robotics`, `#regulation`, `#China`, `#technology`

---