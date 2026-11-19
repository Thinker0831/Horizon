---
layout: default
title: "Horizon Summary: 2026-11-19 (EN)"
date: 2026-11-19
lang: en
---

> From 42 items, 19 important content pieces were selected

---

**Technology News**
1. [Critical Unauthenticated RCE in Nginx HTTP/2 Fixed](#item-tech-news-1) ⭐️ 9.0/10
2. [Critical &\#x27;Java4Shell&\#x27; RCE Vulnerability in Java on Modern x86-64 Servers](#item-tech-news-2) ⭐️ 9.0/10
3. [OpenAI Applies AI Models to Chip Design Workflows](#item-tech-news-3) ⭐️ 8.0/10
4. [Google Introduces Gemini 4 Neon AI Model](#item-tech-news-4) ⭐️ 7.0/10
5. [AI Agents Outperform KPMG Accountants in Audit Questioning Trial](#item-tech-news-5) ⭐️ 7.0/10
6. [ExitPath Lists Open-Source Alternatives to Major SaaS Suites](#item-tech-news-6) ⭐️ 7.0/10
7. [Deutsche Bank Investigation Uses Open Source Data Tools](#item-tech-news-7) ⭐️ 7.0/10
8. [Microsoft Announces Seven New AI Models with Claimed Opus-Level Performance](#item-tech-news-8) ⭐️ 7.0/10
9. [Quad9 Withdraws from France Over DNS Blocking Mandate](#item-tech-news-9) ⭐️ 7.0/10
10. [KVM x86 MMU Context Reset Vulnerability \(CVE-2026-99312\)](#item-tech-news-10) ⭐️ 7.0/10
11. [DaisyRose-27B Open-Source 27B Parameter LLM Released](#item-tech-news-11) ⭐️ 7.0/10
12. [Xiaomi Considers Spinning Off MiMo Large Model Team](#item-tech-news-12) ⭐️ 7.0/10

**Financial News**
1. [Fed Minutes Signal Possible Rate Hikes and AI-Driven Inflation Risks](#item-finance-news-1) ⭐️ 8.0/10
2. [Fed Governor Waller Signals Possible Half-Point Rate Hike to Fight Inflation](#item-finance-news-2) ⭐️ 8.0/10
3. [Trump, Xi, and Putin Meet at APEC Summit Amid Trade and Tech Tensions](#item-finance-news-3) ⭐️ 8.0/10
4. [UK House of Commons Passes Immigration and Asylum Bill](#item-finance-news-4) ⭐️ 8.0/10
5. [China and South Korea Conclude FTA Talks on Services and Investment](#item-finance-news-5) ⭐️ 8.0/10
6. [US Chip Rules Halt $480 Million ByteDance GPU Loan](#item-finance-news-6) ⭐️ 7.0/10
7. [Tencent Q3 Revenue Misses Expectations as AI Spending Surges](#item-finance-news-7) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Critical Unauthenticated RCE in Nginx HTTP/2 Fixed](https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities) ⭐️ 9.0/10

Multiple critical unauthenticated remote code execution \(RCE\) vulnerabilities affecting Nginx&\#x27;s HTTP/2 implementation \(notably CVE-2026-123007\) have been disclosed, allowing attackers to execute arbitrary commands in the Nginx worker process without authentication. These issues were fixed in Nginx versions 1.30.7 and 1.31.9, released on November 18, 2026, which addressed a total of 10 CVEs. Proof-of-concept exploits are publicly available, but there are no reports of active exploitation yet. Servers unable to upgrade are advised to disable HTTP/2 as a mitigation.

hackernews · speedping · Nov 18, 15:19 · [Discussion](https://news.ycombinator.com/item?id=50547374)

**「Background」** Nginx is a widely used open-source web server and reverse proxy. The reported vulnerabilities, CVE-2026-123633 and CVE-2026-123007, affect the HTTP/2 implementation in Nginx and have existed since version 1.9.5, the first to support HTTP/2. These flaws allow unauthenticated remote code execution and were fixed in versions 1.30.7 and 1.31.9 released on November 18, 2026.

**「Impact」** Administrators running Nginx with HTTP/2 enabled must urgently upgrade to the patched versions or disable HTTP/2 to prevent unauthenticated attackers from gaining code execution, potentially leading to full server compromise.

**「Community Discussion」** Commenters noted that the vulnerability was fixed in the open source repository before the official advisory, raising concerns about the window for silent exploitation. Others pointed out that HTTP/2 is not enabled by default in Nginx, but even a minority of affected servers represents a significant risk at internet scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wiz.io/blog/nginx-http2-rce-vulnerabilities">Unauthenticated Remote Code Execution in NGINX ... | Wiz Blog</a></li>
<li><a href="https://xint.io/blog/nginx2root-remote-code-execution">NGINX 2 Root: New Remote Code Execution Vulnerabilities in nginx ...</a></li>
<li><a href="https://nginx2shell.com/">Remote code execution in NGINX HTTP / 2 ( CVE - 2026 - 123633 ...)</a></li>

</ul>
</details>

**Tags**: `#security`, `#web servers`, `#nginx`, `#vulnerabilities`, `#infrastructure`

---

<a id="item-tech-news-2"></a>
### [Critical &\#x27;Java4Shell&\#x27; RCE Vulnerability in Java on Modern x86-64 Servers](https://censys.com/advisory/cve-2026-114938/) ⭐️ 9.0/10

A critical remote code execution vulnerability \(CVE-2026-114938, &\#x27;Java4Shell&\#x27;\) has been disclosed in Java versions 17 \(from 17.0.6 onward\), 21, 25, and 27, with a CVSS 4.0 score of 9.2. The flaw only affects systems running on x86-64 server CPUs with the AVX-512 VBMI instruction set—specifically, Intel Xeon processors from Ice Lake \(2021+\) and newer, and AMD EPYC/Ryzen processors from Zen 4 \(2022+\) and newer. Standard Java 8 and 11 are generally not affected, except for Oracle Java 8 Performance Pack. ARM64 systems are not impacted.

telegram · zaihuapd · Nov 18, 03:55

**「Background」** CVE-2026-114938, also known as &\#x27;Java4Shell,&\#x27; is a critical remote code execution vulnerability in OpenJDK that was publicly disclosed on November 17, 2026. The flaw affects Java versions 17 \(from 17.0.6 onward\), 21, 25, and 27, and is notable for its high CVSS 4.0 score of 9.2. The vulnerability specifically impacts systems running on x86-64 server CPUs with AVX-512 VBMI instruction sets, such as Intel Ice Lake and newer Xeon processors \(2021+\) and AMD Zen 4 and newer EPYC/Ryzen processors \(2022+\), while ARM64 architectures are not affected.

**「Impact」** Organizations running affected Java versions on recent Intel or AMD server hardware are at high risk of unauthenticated remote code execution and should prioritize patching or mitigation. Users of ARM64 servers or standard Java 8/11 \(excluding Oracle Java 8 Performance Pack\) are not exposed to this vulnerability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wiz.io/blog/cve-2026-114938-rce-java4shell-openjdk">CVE - 2026 - 114938 OpenJDK RCE ( Java 4 Shell ): Everything... | Wiz Blog</a></li>
<li><a href="https://www.aikido.dev/blog/java-17-rce-vulnerability-cve-2026-114938">Java 4 Shell Java RCE: Fix &amp; Versions ( CVE - 2026 - 114938 )</a></li>
<li><a href="https://techcommunity.microsoft.com/blog/azurenetworksecurityblog/addressing-java4shell-cve-2026-114938-upgrade-guidance-and-azure-waf-mitigations/4574305">Addressing Java 4 Shell CVE - 2026 - 114938 : upgrade guidance and...</a></li>

</ul>
</details>

**Tags**: `#security`, `#Java`, `#vulnerability`, `#software engineering`, `#hardware`

---

<a id="item-tech-news-3"></a>
### [OpenAI Applies AI Models to Chip Design Workflows](https://openai.com/index/advancing-chip-design-with-our-models/) ⭐️ 8.0/10

OpenAI is applying its AI models to advance chip design, focusing on automating and optimizing electronic design automation \(EDA\) workflows. The initiative includes using AI agents to generate circuits, automate simulation runs, and potentially streamline both digital and analog design processes. While the announcement highlights novel approaches, there is no indication that OpenAI is releasing specific chip designs or tools to the public at this stage.

hackernews · vighneshiyer · Nov 18, 17:45 · [Discussion](https://news.ycombinator.com/item?id=50549493)

**「Background」** OpenAI has been applying its advanced AI models, such as GPT-6 Astra, to optimize circuit designs and improve RISC-V core architectures, as demonstrated in their Jalapeño silicon project. This approach leverages AI to automate and enhance electronic design automation \(EDA\) workflows, aiming to streamline and innovate the chip design process. The Jalapeño chip serves as a concrete example of AI-assisted hardware development, reflecting OpenAI&\#x27;s broader strategy to reduce reliance on traditional chip suppliers and advance custom silicon tailored for AI workloads.

**「Impact」** Developers and hardware engineers may see increased automation in chip design tasks, potentially reducing manual effort in simulation and EDA flows. However, the lack of public release for specific designs or tools means that direct benefits are currently limited to OpenAI&\#x27;s internal projects or select partners.

**「Community Discussion」** Commenters note concerns about AI companies competing with their own customers by withholding models and designs, and question whether OpenAI is sharing its RISC-V designs. Others share practical experiences using AI agents to automate parts of the chip design process, especially for analog circuits and EDA workflow management.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/advancing-chip-design-with-our-models/">Advancing chip design with OpenAI models | OpenAI</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/openai-jalapeno-design-interview-transcript-hardware-vp-richard-ho-explains-how-ai-assisted-design-may-shape-the-future-of-inference-asics">OpenAI Jalapeño design interview transcript... | Tom&#x27;s Hardware</a></li>
<li><a href="https://www.nytimes.com/2026/06/24/technology/openai-broadcom-chip-jalapeno.html">OpenAI and Broadcom Unveil Custom A . I . Chip Design</a></li>

</ul>
</details>

**Tags**: `#AI applications`, `#chip design`, `#EDA`, `#hardware`

---

<a id="item-tech-news-4"></a>
### [Google Introduces Gemini 4 Neon AI Model](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/) ⭐️ 7.0/10

Google has announced Gemini 4 Neon, a new variant in its Gemini AI model lineup. While specific technical details and availability are not provided in the source, community discussion suggests Neon is positioned as more intelligent overall than Gemini Carbon, but with different strengths in research-scale reasoning tasks. The announcement adds to Google&\#x27;s growing portfolio of named AI models, each targeting distinct use cases or performance profiles. This release appears to be an incremental update rather than a major paradigm shift.

hackernews · yigitdemirag · Nov 18, 21:34 · [Discussion](https://news.ycombinator.com/item?id=50552424)

**「Background」** Gemini 4 Neon is a new AI model from Google, positioned within the Gemini 4 lineup to address complex coding, analytical reasoning, and enterprise workflows. It is designed to balance depth and efficiency, distinguishing itself from other Gemini variants like Carbon, which focuses on long-horizon projects, and Hydrogen, which is optimized for fast, everyday tasks. According to Google&\#x27;s model card and announcement, Neon aims to deliver advanced reasoning capabilities at a lower cost compared to other frontier models.

**「Impact」** Users and developers may need to evaluate Gemini 4 Neon against other Gemini variants to determine which model best fits their needs, as the proliferation of model names and capabilities can complicate selection and integration decisions.

**「Community Discussion」** Commenters express fatigue with the proliferation of model names and confusion about mapping them to practical use cases. Some users report that Neon offers a noticeable improvement in usability and task execution over previous models, while others debate the comparative intelligence and specialization of different AI models from Google and competitors.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-4-neon/">Gemini 4 Neon - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/">Introducing Gemini 4 Neon</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#Google`, `#machine learning`, `#industry developments`

---

<a id="item-tech-news-5"></a>
### [AI Agents Outperform KPMG Accountants in Audit Questioning Trial](https://europeanbusinessmagazine.com/ai-agents-better-questions-kpmg/) ⭐️ 7.0/10

In a recent audit trial conducted by KPMG, AI agents demonstrated superior ability to ask relevant audit questions compared to KPMG&\#x27;s own accountants. The trial suggests that AI can effectively handle the detail-oriented and exhaustive questioning required in auditing, a field traditionally dominated by human professionals. While the article does not specify the technical details of the AI agents or the scope of the trial, it highlights a concrete application of AI in professional services. This result is based on a controlled experiment and does not yet indicate industry-wide adoption.

hackernews · Betelbuddy · Nov 18, 15:49 · [Discussion](https://news.ycombinator.com/item?id=50547777)

**「Background」** KPMG recently conducted its first AI-based audit of a UK-listed company, where AI agents were tasked with reviewing financial information and asking questions about the client&\#x27;s finances. According to reports, the AI technology was able to ask more probing and relevant questions than KPMG&\#x27;s own accountants, sometimes digging deeper into specific issues. This trial reflects ongoing efforts by major accounting firms to explore the use of AI in automating and enhancing traditionally human-driven audit processes.

**「Impact」** Organizations considering automation in auditing may find AI agents increasingly viable for tasks involving comprehensive data review and question generation. However, the evidence is limited to a specific trial and does not guarantee similar performance across all audit scenarios or firms.

**「Community Discussion」** Commenters note that AI&\#x27;s strength in detail retention and exhaustive coverage makes it well-suited for auditing, especially compared to inexperienced or overworked human accountants. Some argue that while AI can ask more questions, experienced auditors add value by discerning which issues are truly significant, suggesting that AI may complement rather than fully replace human judgment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ft.com/content/5168b3e9-75d0-4be0-9ccd-d327d6b16c05?syn-25a6b1a6=1">AI asked ‘better questions’ than KPMG accountants in pilot audit</a></li>

</ul>
</details>

**Tags**: `#artificial-intelligence`, `#automation`, `#professional-services`, `#audit`

---

<a id="item-tech-news-6"></a>
### [ExitPath Lists Open-Source Alternatives to Major SaaS Suites](https://exitpath-ruddy.vercel.app/) ⭐️ 7.0/10

ExitPath is a curated online resource that aggregates open-source alternatives to proprietary productivity platforms such as Slack, Notion, and Microsoft 365. The site is aimed at organizations and individuals seeking to migrate away from closed SaaS ecosystems, providing a centralized list of options for communication, collaboration, and office software. While ExitPath itself is not a software package, it serves as a discovery and comparison tool for those interested in open-source adoption.

hackernews · zerocool0101 · Nov 18, 16:04 · [Discussion](https://news.ycombinator.com/item?id=50547980)

**「Background」** ExitPath is an open-source project that compiles migration routes from major proprietary productivity platforms such as Slack, Notion, Microsoft 365, Google Workspace, Dropbox, and GitHub to open-source alternatives like Mattermost, AppFlowy, Nextcloud, and Forgejo. The project provides practical guidance by grading the difficulty of each migration path, helping users assess the effort required to switch. This resource addresses the common challenge of vendor lock-in and the complexities organizations face when considering open-source replacements.

**「Impact」** IT decision-makers and software engineers now have a single reference point to evaluate open-source replacements for widely used SaaS tools, potentially lowering costs and increasing control over data and infrastructure. However, users should be aware that many open-source alternatives may lack feature parity, especially in areas like calendaring and single sign-on \(SSO\), and may require more effort to deploy and maintain.

**「Community Discussion」** Commenters highlighted persistent challenges with open-source alternatives, including complex setup, weaker user experience, and missing features such as robust calendaring and SSO. Some users noted that these gaps often outweigh the benefits for organizations accustomed to the seamless integration and management offered by proprietary suites.

<details><summary>References</summary>
<ul>
<li><a href="https://exitpath-ruddy.vercel.app/">ExitPath — find your way out of big-platform lock-in</a></li>
<li><a href="https://numootech.com/en/article/tl-mwmbf8su-8arf2">ExitPath — Open-source alternatives to Slack, Notion, and ...</a></li>
<li><a href="https://zeli.app/story/50547980">ExitPath - Open-source migration routes · Hacker News | Zeli</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#productivity`, `#software-engineering`, `#tools`

---

<a id="item-tech-news-7"></a>
### [Deutsche Bank Investigation Uses Open Source Data Tools](https://www.inside-db.com/) ⭐️ 7.0/10

An investigative journalism project examining Deutsche Bank utilized open source tools such as OpenAleph, which is built on ElasticSearch and uses the FollowTheMoney schema, to process and analyze approximately 15 million documents, primarily Outlook mailbox exports. These tools enabled consortium partners to manage, search, and structure large-scale financial data for reporting purposes. The project highlights the application of open source data engineering solutions in investigative workflows, though the raw data will not be published publicly.

hackernews · gyre007 · Nov 18, 15:38 · [Discussion](https://news.ycombinator.com/item?id=50547620)

**「Technical Foundations of the Investigation」** The investigative project on Deutsche Bank relied on processing over 15 million documents, primarily Outlook mailbox exports. The team used OpenAleph, an open source platform designed for investigative journalism and research, which is built on ElasticSearch and utilizes the FollowTheMoney schema for structuring financial data. OpenAleph enables journalists to efficiently search, organize, and analyze large volumes of unstructured and structured data, supporting collaborative investigations into complex financial activities.

**「Impact」** Journalists and data engineers working on large-scale investigations can reference this project as a model for handling and analyzing massive document troves using open source tools tailored for investigative needs. However, the decision not to release the raw data may limit independent verification or broader public analysis.

**「Community Discussion」** Commenters noted the technical stack&\#x27;s relevance for investigative journalism and expressed concerns about the lack of raw data publication, arguing that selective reporting could shape public perception. Others suggested that a higher-level summary would help readers grasp the investigation&\#x27;s key findings more efficiently.

<details><summary>References</summary>
<ul>
<li><a href="https://openaleph.org/">Welcome - OpenAleph</a></li>
<li><a href="https://github.com/openaleph/openaleph">GitHub - openaleph / openaleph : The open source platform that...</a></li>
<li><a href="https://www.inside-db.com/">Inside Deutsche Bank</a></li>

</ul>
</details>

**Tags**: `#data engineering`, `#open source`, `#investigative journalism`, `#information retrieval`

---

<a id="item-tech-news-8"></a>
### [Microsoft Announces Seven New AI Models with Claimed Opus-Level Performance](https://microsoft.ai/news/microsoft-ignite-2026/) ⭐️ 7.0/10

Microsoft has announced seven new AI models, claiming competitive price-performance and parity with leading models such as Anthropic&\#x27;s Opus and OpenAI&\#x27;s Sol. The announcement was made at Microsoft Ignite 2026, but no detailed technical specifications or independent benchmarks were provided in the available information. The models are positioned as scalable solutions for practitioners and businesses, but the extent of their availability and licensing terms remains unclear.

hackernews · gmays · Nov 18, 16:08 · [Discussion](https://news.ycombinator.com/item?id=50548021)

**「Background」** Microsoft announced the release of seven new AI models at its Ignite 2026 event, emphasizing exceptional price-performance. Among these, the MAI Cyber 2 Flash model is highlighted for surpassing GPT-6 Astra&\#x27;s quality at less than 2% of the cost per task on the CyberGymE2E benchmark. This launch is positioned as a direct response to recent advancements from competitors and aims to offer practitioners and businesses more cost-effective AI options.

**「Impact」** Practitioners and organizations evaluating AI model providers may now consider Microsoft&\#x27;s offerings as potential alternatives to Anthropic and OpenAI, especially if the claimed performance and pricing are substantiated. However, the lack of open-source availability or published benchmarks may limit immediate adoption or trust among developers seeking transparency.

**「Community Discussion」** Some users report positive experiences with specific Microsoft models like MAI Code 2, noting performance comparable to Opus or Sol, while others express skepticism about Microsoft&\#x27;s innovation and call for open-sourcing models to gain market share. There is also broader concern about industry reliance on large language models and the impact on developer autonomy.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/microsoft-ignite-2026/">Seven new world class models at scalable... | Microsoft AI</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#Microsoft`, `#machine learning`, `#industry news`

---

<a id="item-tech-news-9"></a>
### [Quad9 Withdraws from France Over DNS Blocking Mandate](https://techstackups.com/articles/quad9-leaves-france-dns-blocking/) ⭐️ 7.0/10

Quad9, a global DNS resolver, has withdrawn its services from France following a court order requiring DNS-based blocking of certain domains to combat piracy. This move highlights the ongoing debate over whether DNS infrastructure should be used as a tool for content regulation and anti-piracy enforcement. The withdrawal means French users will no longer be able to use Quad9&\#x27;s DNS services, and it underscores the technical and ethical limitations of using DNS blocking as a regulatory mechanism.

hackernews · ritzaco · Nov 18, 13:18 · [Discussion](https://news.ycombinator.com/item?id=50545958)

**「Background」** Quad9 is a nonprofit DNS resolver that provides both general DNS resolution and cybersecurity filtering services. In October 2026, a French court ordered Quad9 to block access to domains accused of distributing unauthorized sports broadcasts, following a lawsuit by beIN Sports. As a result, Quad9 announced it would withdraw its services from France effective November 24, 2026, making it the second DNS resolver to leave the country due to similar court orders.

**「Impact」** French internet users who relied on Quad9 for DNS resolution will need to switch to alternative providers, potentially reducing their options for privacy-focused DNS services. The decision also sets a precedent that may influence other DNS providers&\#x27; willingness to operate in jurisdictions with similar regulatory requirements.

**「Community Discussion」** Commenters debated the effectiveness and ethics of DNS-based anti-piracy measures, with some arguing that such approaches are ineffective and risk broader censorship. Others questioned whether the fault lies with the courts for enforcing the law or with lawmakers for creating problematic legislation.

<details><summary>References</summary>
<ul>
<li><a href="https://cyberinsider.com/quad9-to-leave-france/">Quad9 to leave France after court orders piracy-related DNS ...</a></li>
<li><a href="https://thecybersecguru.com/online-privacy/quad9-leaves-france-bein-sports-dns-blocking/">Quad9 Exits France: Why the beIN Sports DNS Ruling Matters ...</a></li>
<li><a href="https://torrentfreak.com/dns-resolver-quad9-will-leave-france-after-court-orders-piracy-blocking-penalty/">DNS Resolver Quad9 Will Leave France After Court Orders ...</a></li>

</ul>
</details>

**Tags**: `#internet infrastructure`, `#policy`, `#censorship`, `#DNS`

---

<a id="item-tech-news-10"></a>
### [KVM x86 MMU Context Reset Vulnerability \(CVE-2026-99312\)](https://www.cve.org/CVERecord?id=CVE-2026-99312) ⭐️ 7.0/10

A security vulnerability identified as CVE-2026-99312 affects the KVM \(Kernel-based Virtual Machine\) hypervisor&\#x27;s x86 MMU \(Memory Management Unit\) context handling. The issue involves the unconditional reset of the MMU context when emulating the INIT signal, which could potentially be exploited in virtualized environments. Technical details are limited due to the unavailability of the primary CVE record, but the vulnerability is relevant for administrators and developers managing Linux-based virtualization infrastructure.

hackernews · Kozmik1 · Nov 18, 16:06 · [Discussion](https://news.ycombinator.com/item?id=50548004)

**「Background」** KVM \(Kernel-based Virtual Machine\) is a Linux kernel module that enables hardware-assisted virtualization for x86 systems. The MMU \(Memory Management Unit\) context is critical for managing virtual memory in guest virtual machines. This vulnerability \(CVE-2026-99312\) relates to how KVM handles resetting the MMU context when emulating the INIT signal, which is part of the x86 CPU initialization process; improper handling could potentially expose security risks in virtualized environments.

**「Community Discussion」** Commenters question the severity and technical nature of the vulnerability, with some speculating it may involve a dangling pointer bug. There is also skepticism about the proliferation of CVEs for kernel issues and concerns about the reliability of AI-generated articles on the topic.

<details><summary>References</summary>
<ul>
<li><a href="https://app.opencve.io/cve/CVE-2026-99312">CVE-2026-99312 - Vulnerability Details - OpenCVE</a></li>

</ul>
</details>

**Tags**: `#security`, `#virtualization`, `#linux`, `#kernel`

---

<a id="item-tech-news-11"></a>
### [DaisyRose-27B Open-Source 27B Parameter LLM Released](https://www.radixark.com/blog/daisyrose-27b) ⭐️ 7.0/10

DaisyRose-27B is a newly released open-source large language model with 27 billion parameters. The model was trained using significant hardware resources \(reportedly 18 days on 144 H200 GPUs\) and is available for download, including on Hugging Face. Technical discussion centers on its training methods, evaluation benchmarks, and comparisons to similar models such as Sabi-noema. The release adds another high-capacity option to the open-source LLM ecosystem.

hackernews · de\_sty · Nov 18, 19:39 · [Discussion](https://news.ycombinator.com/item?id=50551046)

**「Background」** DaisyRose-27B is an open-source large language model developed by RadixArk as a derivative of Qwen3.8-27B. The model was trained using reinforcement learning with RadixArk&\#x27;s Miles framework, focusing on 1,200 curated long-horizon agent tasks. Training was conducted over 18 days on 144 H200 GPUs, aiming to improve agent task performance as measured by benchmarks such as Terminal-Bench 4.1.

**「Impact」** Developers and researchers now have access to a new, large-scale open-source language model, potentially enabling more experimentation and applications without proprietary restrictions. However, some users note the absence of a GGUF format download at launch, which may delay adoption for certain workflows.

**「Community Discussion」** Commenters debated the reliance on evaluation datasets, with some expressing skepticism about benchmark-driven claims and the risk of overfitting to specific metrics. Others highlighted the substantial hardware investment required for training and compared DaisyRose-27B to competing models, while some requested additional model formats for easier testing.

<details><summary>References</summary>
<ul>
<li><a href="https://todayforai.com/en/items/art-d6667117-06c">RadixArk Open-Sources DaisyRose-27B Agent Model Trained in 18 ...</a></li>
<li><a href="https://www.aigpu.cloud/en/blog/radixark-daisyrose-27b-rl-post-training">RadixArk&#x27;s DaisyRose-27B Doubles Agent Benchmark Scores with ...</a></li>
<li><a href="https://daily.dev/posts/daisyrose-27b-1-200-task-rl-took-qwen3-8-from-5-6-to-12-on-terminal-bench-4-1-m8yz1a39l">DaisyRose-27B: 1,200-task RL took Qwen3.8 from 5.6% to...</a></li>

</ul>
</details>

**Tags**: `#large-language-models`, `#open-source`, `#machine-learning`, `#model-training`

---

<a id="item-tech-news-12"></a>
### [Xiaomi Considers Spinning Off MiMo Large Model Team](https://mp.weixin.qq.com/s/7LwGupEtmtLzWKQM1-vEfQ) ⭐️ 7.0/10

Xiaomi is reportedly at a critical decision point regarding the potential spin-off of its MiMo large model \(AI\) business. While several venture capital and corporate venture capital firms have made preliminary contact, Xiaomi has not finalized a spin-off or financing plan. There are internal disagreements, particularly between Xiaomi&\#x27;s Lei Jun and MiMo head Luo Fuli, whose future with the company is uncertain. The MiMo team, with over 100 members and a trillion-parameter V2-Pro model ranked fifth globally by Artificial Analysis, is seen as having potential synergies with Xiaomi&\#x27;s smart home and smart cockpit ecosystems.

telegram · zaihuapd · Nov 18, 04:11

**「Background」** Xiaomi&\#x27;s MiMo is its in-house large language model \(LLM\) initiative, reportedly led by Luo Fuli, who joined Xiaomi in late 2025 after experience at Alibaba DAMO Academy and as a key developer of DeepSeek-V2. Recent reports indicate that Xiaomi is considering spinning off the MiMo business for independent financing, with preliminary contacts made with several venture capital and corporate investment firms. However, Xiaomi Group has not yet finalized or announced a clear plan for the spinoff, and there are internal disagreements between Luo Fuli and Xiaomi&\#x27;s leadership regarding the move.

**「Impact」** If the spin-off proceeds, MiMo could gain more operational independence and potentially attract external investment, but leadership uncertainty and unclear market positioning may affect team stability and investor interest. Xiaomi&\#x27;s broader AI ecosystem, especially in smart home and automotive applications, could be influenced by the outcome.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chaincatcher.com/en/article/2305793">Xiaomi was reported to be discussing...</a></li>
<li><a href="https://www.lookonchain.com/feeds/82786">Xiaomi&#x27;s MiMo is reportedly planning a separate financing ...</a></li>
<li><a href="https://news.qq.com/rain/a/20261118A0DPRD00">罗福莉想带MiMo分拆融资，雷军还没松口_腾讯新闻</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#corporate strategy`, `#large language models`, `#China tech`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed Minutes Signal Possible Rate Hikes and AI-Driven Inflation Risks](https://www.cnbc.com/2026/11/18/fed-minutes-october-2026.html) ⭐️ 8.0/10

Federal Reserve officials expect further interest rate hikes may be needed to control inflation, with most seeing a higher federal funds rate as likely appropriate under current forecasts, according to October meeting minutes. The minutes also highlight growing concern that artificial intelligence could become a significant source of inflation and financial instability.

rss · CNBC Finance · Nov 18, 19:41

**「Background」** The Federal Reserve sets U.S. interest rates to control inflation and support economic stability, and recent increases in AI-related business activity have contributed to higher prices, especially in sectors like technology and data centers, raising new concerns for policymakers about inflation and financial risks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.richmondfed.org/research/national_economy/macro_minute/2026/ai_imprint_on_prices_and_inflation">AI&#x27;s Imprint on Prices and Inflation | Richmond Fed</a></li>
<li><a href="https://en.cryptonomist.ch/2026/07/09/federal-reserve-inflation-concerns-ai/">Federal Reserve Inflation Concerns Over AI-Driven Chipflation</a></li>
<li><a href="https://www.federalreserve.gov/newsevents/speech/cook20260928a.htm">An Update on AI and the Economy - Federal Reserve Board</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#Interest Rates`, `#Inflation`, `#Artificial Intelligence`, `#Monetary Policy`

---

<a id="item-finance-news-2"></a>
### [Fed Governor Waller Signals Possible Half-Point Rate Hike to Fight Inflation](https://www.cnbc.com/2026/11/18/federal-reserve-governor-christopher-waller.html) ⭐️ 8.0/10

Federal Reserve Governor Christopher Waller said the central bank may need to raise its benchmark interest rate by half a percentage point at the December 8-9 meeting to address persistent inflation, a move larger than the quarter-point hike currently expected by markets. Waller stated this action could be necessary to reverse last year&\#x27;s rate cuts and more aggressively curb inflation that remains above the Fed&\#x27;s 2% target.

rss · CNBC Finance · Nov 18, 15:13

**「Background」** Christopher Waller is a member of the Federal Reserve Board of Governors, which sets U.S. interest rate policy to manage inflation and employment, and he has served in this role since 2020.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Christopher_Waller">Christopher Waller - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Federal Reserve`, `#interest rates`, `#inflation`, `#monetary policy`, `#economic outlook`

---

<a id="item-finance-news-3"></a>
### [Trump, Xi, and Putin Meet at APEC Summit Amid Trade and Tech Tensions](https://www.cnbc.com/2026/11/18/apec-trump-xi-putin-shenzhen.html) ⭐️ 8.0/10

Leaders of the U.S., China, and Russia are meeting at the APEC summit in Shenzhen to discuss trade, technology, and geopolitical issues, with the U.S. and China focusing on implementing a trade agreement that includes lowering tariffs on $30 billion of goods from each country, according to official statements. Expectations for major breakthroughs are low, but the summit could influence future global economic policy and market stability.

rss · CNBC Finance · Nov 18, 06:04

**「Background」** The Asia-Pacific Economic Cooperation \(APEC\) summit is an annual meeting where leaders from major economies in the Asia-Pacific region, including the U.S., China, and Russia, discuss trade, technology, and geopolitical issues; this year&\#x27;s summit in Shenzhen follows a period of heightened U.S.-China tensions and ongoing global conflicts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/18/apec-trump-xi-putin-shenzhen.html">Three things to watch as Trump , Xi and Putin meet in China</a></li>

</ul>
</details>

**Tags**: `#geopolitics`, `#trade policy`, `#APEC`, `#US-China relations`, `#technology regulation`

---

<a id="item-finance-news-4"></a>
### [UK House of Commons Passes Immigration and Asylum Bill](https://www.bloomberg.com/news/articles/2026-11-17/uk-s-house-of-commons-passes-controversial-immigration-bill) ⭐️ 8.0/10

The UK House of Commons has passed the Immigration and Asylum Bill, which extends the standard residency requirement for most immigrants to apply for permanent settlement from 5 to 10 years, with some healthcare and social care workers still eligible after 5 years if they earn at least £25,000; the bill now moves to the House of Lords for further review.

telegram · zaihuapd · Nov 18, 05:51

**「Background」** The UK Immigration and Asylum Bill proposes stricter rules for residency and asylum, and must pass both the House of Commons and the House of Lords before becoming law.

<details><summary>References</summary>
<ul>
<li><a href="https://www.naijaukhub.com/news/immigration-asylum-bill-second-reading">Immigration and Asylum Bill Second Reading Debate... | NaijaUKHub</a></li>

</ul>
</details>

**Tags**: `#immigration policy`, `#UK legislation`, `#labor market`, `#public policy`

---

<a id="item-finance-news-5"></a>
### [China and South Korea Conclude FTA Talks on Services and Investment](https://x.com/Jaemyung_Lee/status/2122988472994791476) ⭐️ 8.0/10

China and South Korea announced the substantive conclusion of negotiations to expand their free trade agreement to cover services and investment, with China pledging most-favored-nation treatment for South Korea in sectors such as film, games, tourism, legal, construction, and finance as of November 18, 2026.

telegram · zaihuapd · Nov 18, 10:02

**「Background」** Negotiations to expand the China-South Korea Free Trade Agreement to include services and investment began in March 2018 and lasted over eight years, aiming to increase market access and economic cooperation between the two countries.

<details><summary>References</summary>
<ul>
<li><a href="https://biz.chosun.com/en/en-policy/2026/11/18/3HXWCB2DJJGY5JHJZMFZGGB3CQ/">South Korea and China reach deal on services and investment ...</a></li>

</ul>
</details>

**Tags**: `#trade agreement`, `#China`, `#South Korea`, `#services sector`, `#investment`

---

<a id="item-finance-news-6"></a>
### [US Chip Rules Halt $480 Million ByteDance GPU Loan](https://www.bloomberg.com/news/articles/2026-11-17/banks-pause-480-million-chip-loan-tied-to-china-s-bytedance) ⭐️ 7.0/10

Five banks have paused a $480 million loan for ByteDance&\#x27;s planned purchase of advanced Nvidia GPUs after new US AI chip export regulations, according to Bloomberg. The financing was intended for a data center project in Malaysia.

telegram · zaihuapd · Nov 18, 05:11

**「Background」** The US recently tightened export controls on advanced AI chips, which led banks to pause a $480 million loan intended for ByteDance&\#x27;s purchase of Nvidia GPUs for a Malaysian data center.

**「Impact」** The suspension directly affects ByteDance&\#x27;s ability to expand its data center capacity and highlights how US chip export rules can disrupt financing for Chinese technology companies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-17/banks-pause-480-million-chip-loan-tied-to-china-s-bytedance">Banks Pause $480 Million Chip Loan Tied to China’s ByteDance</a></li>
<li><a href="https://www.gate.com/news/detail/NVDA/bytedance-480m-loan-stalled-after-us-tightens-ai-chip-export-rules-25700410">ByteDance $480M Loan Stalled After US Tightens AI Chip Export ...</a></li>

</ul>
</details>

**Tags**: `#US-China relations`, `#semiconductors`, `#regulation`, `#corporate finance`, `#technology sector`

---

<a id="item-finance-news-7"></a>
### [Tencent Q3 Revenue Misses Expectations as AI Spending Surges](https://api3.cls.cn/share/article/2537922?os=android&amp;amp;sv=8.8.5&amp;amp;app=cailianpress&amp;amp;selected=) ⭐️ 7.0/10

Tencent reported third-quarter 2026 revenue of RMB 207.3 billion, up 8% from a year earlier but below market expectations, while capital expenditure jumped to RMB 81.4 billion, far above the estimated RMB 55.4 billion, resulting in negative free cash flow of RMB 69.1 billion.

telegram · zaihuapd · Nov 18, 09:20

**「Background」** Tencent is a major Chinese technology company that regularly reports quarterly financial results, with market expectations often influencing investor reactions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tencent.com/wp-content/uploads/2026/11/Tencent-Announces-2026-Third-Quarter-Results.pdf">For Immediate Release - Tencent</a></li>

</ul>
</details>

**Tags**: `#earnings`, `#capital expenditure`, `#AI`, `#China`, `#technology`

---