---
layout: default
title: "Horizon Summary: 2026-11-14 (EN)"
date: 2026-11-14
lang: en
---

> From 45 items, 19 important content pieces were selected

---

**Technology News**
1. [FAA Orders Nationwide Ground Stop Amid Telecom and AI System Issues](#item-tech-news-1) ⭐️ 8.0/10
2. [Scaling a 1T-Parameter MoE Model on TorchTitan with GH200 GPUs](#item-tech-news-2) ⭐️ 8.0/10
3. [Frontier AI Models Nearly Perfect Materials Science Benchmark](#item-tech-news-3) ⭐️ 8.0/10
4. [Shanghai Jiao Tong Gene Editing Case: Investigation Results Announced](#item-tech-news-4) ⭐️ 8.0/10
5. [Python Contributor Tim Peters Passes Away at 74](#item-tech-news-5) ⭐️ 8.0/10
6. [Microsoft Outlook, Teams, Copilot Suffer 12+ Hour Global Outage](#item-tech-news-6) ⭐️ 8.0/10
7. [Community Debates Haskell&\#x27;s Technical Vision and Ecosystem Challenges](#item-tech-news-7) ⭐️ 7.0/10
8. [Granzyme K Identified as Tissue Aging Driver Without Inflammation](#item-tech-news-8) ⭐️ 7.0/10
9. [ICML 2027 Overhauls Review and Authorship Rules](#item-tech-news-9) ⭐️ 7.0/10
10. [Open-Source Legal Conflict Detector Uses NLI and Encoder Models](#item-tech-news-10) ⭐️ 7.0/10
11. [ParaTrace v8 Open Weights Released, 5th on RAID Leaderboard](#item-tech-news-11) ⭐️ 7.0/10
12. [tamserve: Open-Source Real-Time Video Tracking Cuts Costs](#item-tech-news-12) ⭐️ 7.0/10
13. [SpaceX Disbands Most of Grok Imagine Team](#item-tech-news-13) ⭐️ 7.0/10
14. [OpenAI Launches ChatGPT Wallet for Secure AI Payments](#item-tech-news-14) ⭐️ 7.0/10

**Technology Blog**
1. [GPU-Accelerated Black Hole Interferometry with NVIDIA cuPhoton.xBeam](#item-tech-blog-1) ⭐️ 8.0/10
2. [Native DLA Inference in Python on Jetson AGX Orin with cuDLA](#item-tech-blog-2) ⭐️ 7.0/10

**Financial News**
1. [Nvidia CEO Resignation Sparks U.S.-China Tension and Export Control Debate](#item-finance-news-1) ⭐️ 8.0/10
2. [Lutnick faces questions over Nvidia spy scandal. His sons&\#x27; firm has deep ties to the chipmaker](#item-finance-news-2) ⭐️ 7.0/10
3. [Chicago Fed President Signals More Action Needed on Inflation](#item-finance-news-3) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [FAA Orders Nationwide Ground Stop Amid Telecom and AI System Issues](https://www.nbcnews.com/news/us-news/faa-orders-nationwide-ground-stop-departing-flights-reasons-safety-rcna609247) ⭐️ 8.0/10

On November 13, 2026, the FAA issued a nationwide ground stop for all departing flights in the United States. The incident is reportedly linked to an outage in a telecommunications network managed by L3Harris Technologies, which supports critical air traffic control communications. There is also speculation that a recent nationwide rollout of the FAA&\#x27;s SMART AI-based air traffic control system may have contributed, as the system was expanded to all 22 airspace centers following a D.C. test. The outage has caused widespread flight delays and cancellations, with officials warning that the disruption may be prolonged.

hackernews · zulln · Nov 13, 21:05 · [Discussion](https://news.ycombinator.com/item?id=50489641)

**「Background」** A nationwide ground stop is an extremely rare event in U.S. aviation, typically reserved for severe technical failures or safety threats. On November 13, 2026, the FAA halted all departing flights across the country due to a major outage affecting its air traffic control system, specifically impacting communications at multiple Air Route Traffic Control Centers. FAA technicians are actively investigating the cause of the disruption.

**「Impact」** Airlines, passengers, and airport operations across the U.S. are experiencing significant disruptions, with departures halted and uncertainty about when normal service will resume. Organizations relying on air travel and logistics should prepare for extended delays and monitor official FAA updates for restoration timelines.

**「Community Discussion」** Commenters are debating whether the outage was primarily caused by the telecom network failure or by issues with the newly deployed AI air traffic control system, with some pointing to a recent system update and others highlighting the lack of clear information from authorities. There is widespread frustration over the scarcity of official details and concern about the reliability of critical infrastructure when integrating new technologies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/live/2026/11/13/us/ground-stop-nationwide-flights-faa">Live Updates: FAA Declares Rare Nationwide Ground Stop of Flights</a></li>
<li><a href="https://www.axios.com/2026/11/13/faa-nationwide-ground-stop">FAA issues nationwide ground stop due to &quot;extraordinary...&quot;</a></li>
<li><a href="https://www.dailymail.com/news/article-16291587/FAA-groundstop-live.html">New AI traffic control system is may be possible cause of groundstop</a></li>

</ul>
</details>

**Tags**: `#infrastructure`, `#AI systems`, `#aviation`, `#incident response`

---

<a id="item-tech-news-2"></a>
### [Scaling a 1T-Parameter MoE Model on TorchTitan with GH200 GPUs](https://www.reddit.com/r/MachineLearning/comments/1xvce5h/scaling_to_1t_moe_on_torchtitan_p/) ⭐️ 8.0/10

Researchers successfully trained a 1 trillion parameter Mixture-of-Experts \(MoE\) model on TorchTitan using 384 NVIDIA GH200 GPUs, achieving approximately 1,300 tokens per second per GPU. The team used Fully Sharded Data Parallel \(FSDP\) and Expert Parallelism \(EP\), optimizing communication and memory usage to overcome bottlenecks such as limited InfiniBand bandwidth and memory allocation inefficiencies. Key technical improvements included activation checkpointing, optimizer offloading, smarter sharding with FlexShard, and custom communication strategies \(e.g., FP8 all-gather, node-local resharding\). These optimizations resulted in a 14-fold throughput increase from their initial baseline.

reddit · r/MachineLearning · /u/f14-bertolotti · Nov 13, 16:28

**「Background」** Mixture-of-Experts \(MoE\) models are a type of neural network architecture that scales to very large parameter counts by activating only a subset of model parameters \(experts\) for each input, making them more efficient for large-scale tasks. Training trillion-parameter MoE models requires advanced parallelization strategies and high-performance hardware, such as NVIDIA GH200 GPUs and specialized interconnects like NVLink and InfiniBand. TorchTitan is a machine learning infrastructure platform designed to support large-scale distributed training, and the JUPITER supercomputer is one of the environments where such experiments are conducted.

**「Impact」** Practitioners aiming to train extremely large models on shared supercomputing resources can now reference concrete strategies and performance data for overcoming communication and memory bottlenecks, particularly when using GH200 GPUs and TorchTitan. The lessons and code contributions described may directly benefit users of PyTorch and similar large-scale training frameworks.

**Tags**: `#large-scale-models`, `#machine-learning-infrastructure`, `#deep-learning`, `#hardware`

---

<a id="item-tech-news-3"></a>
### [Frontier AI Models Nearly Perfect Materials Science Benchmark](https://www.reddit.com/r/MachineLearning/comments/1xvgf6h/four_frontier_models_scored_978100_on_a_7part/) ⭐️ 8.0/10

Four leading AI models—Gemini 4 Carbon, Gemini 4 Hydrogen \(Antigravity\), Claude Opus 5.5, and Claude Fable 5.2—achieved mean scores between 98.5 and 100 on a comprehensive seven-part materials science research test. The benchmark included tasks such as data reduction, physics calculations, manuscript critique, and experimental design, with all models performing at a level that matched or exceeded an estimated PhD student baseline. The evaluation used synthetic data, code-verified answer keys, and allowed web search and code execution, with each model tested in three fresh runs. The results highlight that current benchmarks for bounded, procedural scientific work are nearly saturated by top models, raising questions about how to evaluate long-horizon, open-ended agentic tasks going forward.

reddit · r/MachineLearning · /u/v\_aravind · Nov 13, 18:58

**「Benchmarking AI in Materials Science」** Recent advances in AI have led to the development of sophisticated benchmarks to evaluate model performance on domain-specific tasks. In materials science, such benchmarks now include multi-part tests that simulate real research workflows, covering data analysis, physics calculations, manuscript critique, and experimental design. These tests are designed to be realistic, use synthetic data with code-verified answers, and aim to measure how well AI models can perform tasks typically handled by human researchers.

**Tags**: `#AI evaluation`, `#benchmarks`, `#materials science`, `#frontier models`

---

<a id="item-tech-news-4"></a>
### [Shanghai Jiao Tong Gene Editing Case: Investigation Results Announced](https://mp.weixin.qq.com/s/p0iC3tcI1yr10EBl2NjUvg) ⭐️ 8.0/10

Shanghai authorities have released the results of an official investigation into a gene editing case at Shanghai Jiao Tong University Medical School. The investigation found significant ethical and procedural failures, including inadequate preclinical research, flawed ethical review, and insufficient informed consent. Two key personnel, Qiu and Yang, were expelled and banned from practice for five years, and related institutions received administrative penalties and were ordered to rectify. The case involved a rare disease patient who died after receiving a custom gene editing therapy, and the incident was later published in Nature in February 2026.

telegram · zaihuapd · Nov 13, 09:24

**「Background」** Gene editing in humans is subject to strict ethical and regulatory oversight in China and internationally, especially following previous controversies involving unapproved clinical applications. Shanghai Jiao Tong University Medical School is a leading institution in biomedical research, making incidents there particularly significant for the field. The case involved a rare genetic disorder and experimental therapy, highlighting ongoing challenges in balancing innovation with patient safety and ethical standards.

**「Impact」** Researchers and institutions involved in gene editing in China face increased scrutiny and stricter enforcement of ethical and procedural standards, with concrete disciplinary actions and administrative penalties now demonstrated in high-profile cases.

**Tags**: `#gene editing`, `#bioethics`, `#regulation`, `#technology policy`

---

<a id="item-tech-news-5"></a>
### [Python Contributor Tim Peters Passes Away at 74](https://x.com/Itsfoss/status/2120957452937998716) ⭐️ 8.0/10

Tim Peters, a foundational contributor to Python, has passed away at the age of 74. Peters was the author of the Timsort sorting algorithm, creator of &\#x27;The Zen of Python&\#x27; \(PEP 20\), and served on the Python Software Foundation board for 13 years. His work has had a lasting impact on Python&\#x27;s design, culture, and technical capabilities. The announcement was made by Python creator Guido van Rossum.

telegram · zaihuapd · Nov 13, 09:55

**「Background」** Tim Peters was a highly influential software engineer in the Python community. He authored &\#x27;The Zen of Python&\#x27; \(PEP 20\), a set of guiding principles for Python&\#x27;s design, and created the Timsort sorting algorithm, which is used in Python and other programming languages. Peters was also an early adopter of Python and served on the Python Software Foundation board for 13 years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zen_of_Python">Zen of Python - Wikipedia</a></li>
<li><a href="https://discuss.python.org/t/in-memoriam-tim-peters-1952-2026/110028">In Memoriam: Tim Peters 1952–2026 - Core Development...</a></li>

</ul>
</details>

**Tags**: `#python`, `#open-source`, `#community`, `#software-engineering`

---

<a id="item-tech-news-6"></a>
### [Microsoft Outlook, Teams, Copilot Suffer 12+ Hour Global Outage](https://www.reuters.com/technology/microsoft-365-outlook-down-thousands-us-users-downdetector-shows-2026-11-12/) ⭐️ 8.0/10

Microsoft Outlook, Teams, and Copilot experienced a global outage lasting over 12 hours, affecting enterprise and government communications worldwide. Microsoft attributed the disruption to server issues, stated there was no evidence of malicious activity, and reported that recovery efforts were underway with some stabilization observed. The outage impacted government agencies in Australia, Japan, and the US, as well as financial institutions and organizations such as Euronext in Europe. This marks the second major Microsoft 365 service interruption reported this year.

telegram · zaihuapd · Nov 13, 12:21

**「Background」** Microsoft 365 is a suite of cloud-based productivity and collaboration tools, including Outlook, Teams, and Copilot, widely used by enterprises and government agencies globally. Outages of these services can have significant operational impacts due to their central role in business communications. Previous incidents have shown that technical failures, such as server configuration issues, can disrupt access to these platforms for extended periods.

**「Impact」** Organizations relying on Microsoft 365 services faced significant operational disruptions, with some financial institutions resorting to fax for transaction confirmations and government agencies experiencing communication breakdowns. Users may need to review contingency plans for critical communications during future outages.

<details><summary>References</summary>
<ul>
<li><a href="https://gulfbusiness.com/en/2026/tech/microsoft-outage-cause-outlook-teams-restoration-november-2026/">Microsoft outage : What went wrong and when will Outlook , Teams ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/13/microsoft-outage-outlook-teams-word-excel-reports">Microsoft scrambles to fix global outage affecting Teams and Outlook</a></li>

</ul>
</details>

**Tags**: `#outage`, `#cloud services`, `#enterprise IT`, `#incident response`, `#reliability`

---

<a id="item-tech-news-7"></a>
### [Community Debates Haskell&\#x27;s Technical Vision and Ecosystem Challenges](https://discourse.haskell.org/t/a-technical-vision-for-the-haskell-ecosystem/15078) ⭐️ 7.0/10

A community-driven technical vision for the Haskell ecosystem has been published, prompting extensive discussion about Haskell&\#x27;s current capabilities, adoption barriers, and future direction. The conversation highlights Haskell&\#x27;s strengths in safety and terseness, but also its limitations in cross-platform development and mainstream adoption compared to languages like Rust and JavaScript. The vision is not a formal roadmap or release, but rather a catalyst for community input on Haskell&\#x27;s evolution and relevance in areas such as AI and modern software engineering.

hackernews · cosmic\_quanta · Nov 13, 14:43 · [Discussion](https://news.ycombinator.com/item?id=50484235)

**「Background」** Haskell is a statically typed, purely functional programming language known for its expressive type system and emphasis on correctness. The Haskell ecosystem has historically faced challenges with adoption, tooling, and cross-platform support compared to more mainstream languages like JavaScript, Rust, or C\#. Community-driven technical visions aim to address these issues and guide the language&\#x27;s evolution to better meet modern software engineering needs.

**「Community Discussion」** Commenters debated why Haskell is not more widely used in AI, despite its expressive and safe features, and compared its ecosystem limitations to the universality of languages like JavaScript and Rust. Some praised recent technical achievements in Haskell, such as improved debugging tools and performance in specific domains, while others pointed to the JVM ecosystem as a model for long-term stability and innovation.

**Tags**: `#programming languages`, `#Haskell`, `#ecosystem`, `#community debate`

---

<a id="item-tech-news-8"></a>
### [Granzyme K Identified as Tissue Aging Driver Without Inflammation](https://www.nature.com/articles/d41586-026-03638-3) ⭐️ 7.0/10

Researchers have identified Granzyme K \(GzmK\) as a protein that promotes tissue aging independently of inflammation, based on studies in animal models. The findings, published in a peer-reviewed journal, show that mice lacking GzmK experienced reduced organ aging despite persistent immune aging phenotypes, effectively separating tissue aging from immune system aging and systemic inflammation. This discovery advances the understanding of aging mechanisms but is currently limited to preclinical \(animal\) research.

hackernews · gumby · Nov 13, 19:25 · [Discussion](https://news.ycombinator.com/item?id=50488470)

**「Background」** Aging research has long focused on the role of inflammation and immune system changes in driving tissue degeneration and age-related diseases. Traditionally, proteins that accelerate aging have been linked to inflammatory processes, making it difficult to separate the effects of tissue aging from immune system aging. The identification of a protein that promotes tissue aging independently of inflammation provides a new perspective on the mechanisms underlying aging.

**「Impact」** For researchers and biotechnologists, this finding suggests a new potential target for interventions aimed at slowing tissue aging without affecting immune function or triggering inflammation, though any therapeutic applications remain speculative until validated in humans.

**「Community Discussion」** Commenters highlight that the results are currently limited to mice, cautioning against overgeneralization to humans. Some users note the nuance in the research, emphasizing that GzmK deficiency uncouples tissue aging from immune aging and inflammaging, while others express skepticism or humor about the practical implications.

**Tags**: `#aging`, `#biotechnology`, `#research`, `#biology`

---

<a id="item-tech-news-9"></a>
### [ICML 2027 Overhauls Review and Authorship Rules](https://www.reddit.com/r/MachineLearning/comments/1xvkxbj/icml_2027_changes_d/) ⭐️ 7.0/10

ICML 2027 will implement a two-stage review process: area chairs will decide if submissions proceed to full review, with senior area chair confirmation required for first-stage rejections. New authorship and reviewing rules include a cap of 20 submissions per person, a reciprocal reviewer requirement \(max 6 papers per reviewer\), and mandatory program committee service for anyone with 3 or more submissions. Each author can only be on one paper without an eligible reciprocal reviewer, and non-compliant papers risk desk rejection. These changes aim to address reviewer overload and tie authorship volume to reviewing responsibilities.

reddit · r/MachineLearning · /u/Gravitist · Nov 13, 21:53

**「Background」** The International Conference on Machine Learning \(ICML\) is a leading annual conference in the field of machine learning, attracting thousands of research paper submissions each year. In recent years, the rapid growth in submissions has led to concerns about reviewer overload and the sustainability of the peer review process. The 2027 changes are a response to these challenges, aiming to balance submission volume with reviewer capacity and maintain review quality.

**「Impact」** Researchers submitting to ICML 2027 will need to carefully manage coauthorship and reviewer commitments, as exceeding submission or reviewer limits may result in desk rejection. The new process may reduce reviewer burden but could also increase the risk of early-stage rejections for some papers.

<details><summary>References</summary>
<ul>
<li><a href="https://icml.cc/">2027 Conference - ICML 2027</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#conference policy`, `#peer review`, `#research community`

---

<a id="item-tech-news-10"></a>
### [Open-Source Legal Conflict Detector Uses NLI and Encoder Models](https://www.reddit.com/r/MachineLearning/comments/1xuzv6d/how_to_make_a_legorastyle_legal_conflict_detector/) ⭐️ 7.0/10

An open-source legal conflict detector tool has been released that identifies deviations and gaps between pairs of legal documents using only encoder models and natural language inference \(NLI\), without relying on generative models. The pipeline processes documents by enriching, embedding, filtering, shortlisting, scoring, and sorting clauses, enabling efficient clause-level pairwise comparison. The tool is MIT-licensed, supports model customization, and demonstrates significant speed and cost advantages over generative or agentic approaches, with a full pipeline run on long document pairs completing in under 20 seconds. Optional generative steps, such as summarization, are only applied after conflicts are detected, reducing the risk of hallucinated results.

reddit · r/MachineLearning · /u/ladyofcode · Nov 13, 05:48

**「Background」** Legora is an AI-powered legal tool designed to help lawyers review, research, and draft documents more efficiently by leveraging machine learning for document analysis and collaboration. Traditional legal conflict detection tools often rely on large generative models, which can be slow and costly for clause-level pairwise comparisons. The approach described in the post uses only encoder models and natural language inference \(NLI\), offering a more scalable and cost-effective alternative for legal document conflict detection.

**「Impact」** Legal professionals and developers can now use or adapt this open-source tool to efficiently detect conflicts in legal documents at scale, avoiding the high costs and slower performance associated with generative models. The MIT license allows for both personal and commercial use, and the modular design supports integration with custom models or workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://legora.com/product/aos">Legora</a></li>
<li><a href="https://www.youtube.com/watch?v=H4iOV0yEV_I">LTH Product Briefing - Legora - YouTube</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#natural language processing`, `#legal tech`, `#open source`

---

<a id="item-tech-news-11"></a>
### [ParaTrace v8 Open Weights Released, 5th on RAID Leaderboard](https://www.reddit.com/r/MachineLearning/comments/1xv4ldx/open_weights_paratrace_v8_raidtuned_5th_on_the/) ⭐️ 7.0/10

The open weights for ParaTrace v8, a RAID-tuned AI-generated text detector based on the Ettin-1B encoder \(ModernBERT architecture\), have been released under a CC BY-NC-SA 4.0 license. The model achieved 5th place on the RAID leaderboard, with a true positive rate \(TPR\) of 99.20% at 1% false positive rate \(FPR\) on the RAID hidden test set. ParaTrace v8 was fine-tuned specifically on RAID&\#x27;s training split and further refined with hard examples, but its model card cautions that it is not reliable for general text detection outside the RAID benchmark. The release includes code to reproduce leaderboard results, but the model is intended for research use only due to its tuning specificity and generalizability limitations.

reddit · r/MachineLearning · /u/AltruisticCouple3491 · Nov 13, 10:39

**「Background」** ParaTrace is an AI-generated text detector that uses the Ettin-1B encoder based on the ModernBERT architecture. The RAID benchmark is a widely used evaluation suite for AI text detection models, measuring their ability to distinguish between human and machine-generated text under various conditions, including adversarial attacks. Open-weight releases like this allow researchers to inspect, reproduce, and build upon the model&\#x27;s performance, but tuning for a specific benchmark \(such as RAID\) can limit generalizability to other real-world scenarios.

**Tags**: `#AI Detection`, `#NLP`, `#Open Source`, `#Machine Learning`

---

<a id="item-tech-news-12"></a>
### [tamserve: Open-Source Real-Time Video Tracking Cuts Costs](https://www.reddit.com/r/MachineLearning/comments/1xuvxke/i_built_tamserve_to_make_realtime_video_tracking/) ⭐️ 7.0/10

tamserve is a newly released open-source system for real-time video tracking that enables advanced segmentation models \(like SAM 2.1 and EdgeTAM\) to run up to 3.8 times faster and at less than half the cost per camera compared to Meta&\#x27;s reference code. It achieves this by sharing a single model instance across multiple cameras and maintaining constant memory usage, allowing for indefinite operation without running out of GPU memory. Benchmarks on an RTX 4090 show tamserve costs $1.07 per camera per day at 30 fps, compared to $2.40 with Meta&\#x27;s code, with similar savings at lower frame rates. The system supports dynamic object tracking, automatic camera reconnection, and multi-GPU scaling.

reddit · r/MachineLearning · /u/Chunkymunkey642069 · Nov 13, 02:23

**「Background」** Real-time video tracking involves identifying and following objects across frames in live video streams, often using segmentation models for precise outlines. Recent trackers like SAM 2.1 and EdgeTAM offer high accuracy but are resource-intensive, especially when handling multiple camera feeds, leading to high GPU memory usage and operational costs. Open-source solutions for video tracking exist, but many struggle with scalability and efficiency when deployed at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sci-hub.ru/10.1186/s13104-020-4916-6">Sci-Hub | An open - source video tracking system for mouse...</a></li>

</ul>
</details>

**Tags**: `#computer vision`, `#open source`, `#video tracking`, `#machine learning tools`

---

<a id="item-tech-news-13"></a>
### [SpaceX Disbands Most of Grok Imagine Team](https://weibo.com/1642634100/RreMyi69Y) ⭐️ 7.0/10

SpaceX has reportedly laid off about 60 members of its Grok Imagine team, leaving only a small group to maintain the video and image generation tool. The product remains operational, but its future is uncertain following the dissolution of the dedicated team. This move follows SpaceX&\#x27;s $250 billion stock acquisition of xAI in February and its $60 billion purchase of AI code startup Cursor in August, signaling a shift in focus toward AI code tools and intelligent agents.

telegram · zaihuapd · Nov 13, 15:00

**「Background」** SpaceX, founded by Elon Musk in 2002, is primarily known for its work in rocket and spacecraft development. In recent years, the company has expanded its focus to include artificial intelligence initiatives, such as the Grok Imagine video and image generation tool. The reported layoffs follow SpaceX&\#x27;s major acquisitions in the AI sector, including the purchase of xAI and Cursor, indicating a shift in strategic priorities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SpaceX">SpaceX - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#corporate strategy`, `#machine learning`, `#technology business`

---

<a id="item-tech-news-14"></a>
### [OpenAI Launches ChatGPT Wallet for Secure AI Payments](https://openai.com/index/introducing-chatgpt-wallet/) ⭐️ 7.0/10

OpenAI has launched ChatGPT Wallet, a payment solution that allows AI agents to make purchases without exposing users&\#x27; real card numbers. The service is available starting today in the US for ChatGPT Pro subscribers aged 18 and over, using US-issued cards, and is integrated with American Express, Mastercard, and Visa. Each transaction requires user verification via Face ID or fingerprint, and payment networks issue a tokenized card number for each purchase. This approach aims to enhance payment security and privacy by leveraging AI and tokenization.

telegram · zaihuapd · Nov 13, 15:43

**「Background」** Digital wallets are applications that allow users to make electronic payments without directly exposing their credit card numbers, often using tokenization and biometric authentication for added security. OpenAI&\#x27;s ChatGPT Wallet builds on this concept by integrating AI agents to assist with purchases, and it launches in partnership with major payment networks American Express, Mastercard, and Visa. The service is initially available to ChatGPT Pro subscribers in the US, requiring a US-issued card and biometric confirmation for each transaction.

**「Impact」** ChatGPT Pro users in the US can now make more secure online payments through AI agents, reducing the risk of card number exposure and unauthorized transactions. Developers and merchants may need to adapt to tokenized payment flows and new user authentication requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-chatgpt-wallet/">Introducing ChatGPT Wallet | OpenAI</a></li>
<li><a href="https://www.cnbc.com/2026/11/13/openai-chatgpt-wallet-dot-purchases.html">OpenAI &#x27;s ChatGPT Wallet allows &#x27;dots&#x27; AI agents to make purchases</a></li>
<li><a href="https://vc.ru/chatgpt/3254374-openai-zapuskayut-chatgpt-wallet-dlya-bezopasnykh-pokupok-v-ssha">OpenAI представила ChatGPT Wallet , чтобы... — ChatGPT на vc.ru</a></li>

</ul>
</details>

**Tags**: `#AI applications`, `#fintech`, `#security`, `#OpenAI`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [GPU-Accelerated Black Hole Interferometry with NVIDIA cuPhoton.xBeam](https://developer.nvidia.com/blog/run-gpu-powered-black-hole-interferometry-with-nvidia-cuphoton/) ⭐️ 8.0/10

rss · NVIDIA CUDA Technical Blog · Nov 13, 21:17

**「Background」** Imaging black holes like M87\* is exceptionally difficult due to their tiny apparent size and the fact that they emit no light directly; instead, telescopes must capture faint radio emissions from gas swirling near the event horizon. The Event Horizon Telescope \(EHT\) tackles this by linking radio observatories worldwide using very-long-baseline interferometry \(VLBI\), generating petabytes of high-speed voltage data that must be correlated and processed to reconstruct images. Traditional CPU-based workflows for this FX correlation step are slow and struggle to keep up with the growing data volumes and the need for rapid, iterative analysis.

**「Solution」** The author details how NVIDIA&\#x27;s cuPhoton.xBeam leverages GPUs to accelerate the core interferometric correlation workflow, dramatically reducing processing times for VLBI data. cuPhoton.xBeam ingests telescope recordings, organizes them for parallel access, and performs the FX correlation—Fourier-transforming each station&\#x27;s voltage data and cross-multiplying all pairs—entirely on GPUs. It uses a sidecar index \(.vdix\) to enable efficient, non-redundant data access, and supports both standard POSIX and GPUDirect Storage \(GDS\) for high-throughput disk-to-GPU transfers. Delay and fringe corrections are applied based on job-supplied models, but xBeam does not compute geometric delays from station positions or model light paths around black holes. The tool scales across multiple GPUs and nodes by sharding the time axis, with each GPU processing a segment and results merged afterward. On an NVIDIA Vera Rubin NVL72 system with 64 GPUs, xBeam processed a 10 TB dataset in just 70 seconds—about 460 times faster than a CPU baseline. The workflow is accessible via both command-line and Python APIs, and the toolkit is designed to integrate with downstream calibration and imaging tools. While xBeam focuses on correlation, the broader cuPhoton suite extends GPU-first processing to other scientific domains, and the author notes the potential for AI agents to automate and orchestrate these complex pipelines.

**「Takeaway」** NVIDIA cuPhoton.xBeam demonstrates that GPU acceleration can transform the speed and scalability of radio astronomy data processing, making previously prohibitive VLBI workflows practical for next-generation black hole imaging. While domain-specific and not a full imaging solution, its architecture and performance gains offer a compelling model for other large-scale, parallel scientific data challenges.

**Tags**: `#GPU computing`, `#radio astronomy`, `#interferometry`, `#scientific data processing`, `#parallel computing`

---

<a id="item-tech-blog-2"></a>
### [Native DLA Inference in Python on Jetson AGX Orin with cuDLA](https://developer.nvidia.com/blog/run-native-dla-inference-in-python-on-nvidia-jetson-agx-orin-using-cudla/) ⭐️ 7.0/10

rss · NVIDIA CUDA Technical Blog · Nov 13, 18:57

**「Background」** Edge AI applications often need to run multiple neural networks efficiently within tight compute and power constraints. NVIDIA&\#x27;s Deep Learning Accelerator \(DLA\) hardware on Jetson AGX Orin enables offloading inference from the GPU, improving power efficiency and freeing GPU resources for other tasks. However, integrating DLA inference into Python applications previously required complex C++ code or lacked direct Python support, making rapid prototyping and flexible orchestration challenging.

**「Solution」** The author details how the cuda.bindings.cudla Python module, introduced in cuda-bindings 13.3.0, exposes the cuDLA C++ API directly to Python, allowing developers to manage DLA devices, load compiled models, allocate and register memory, and submit inference tasks—all from Python. The workflow begins with compiling a neural network into a DLA loadable using TensorRT&\#x27;s trtexec tool, ensuring the model is compatible with DLA&\#x27;s supported layers. In Python, developers initialize CUDA, create a DLA device in hybrid mode \(enabling seamless GPU-DLA pipelines\), and load the compiled model as raw bytes. The API allows introspection of model input/output tensor descriptors, making the workflow model-agnostic and eliminating hardcoded buffer sizes. GPU memory is allocated and registered with the DLA device, and input data is preprocessed and transferred to the GPU. Inference tasks are submitted via a CUDA stream, enabling coordination with other GPU operations. After synchronizing the stream, output is retrieved as a NumPy array for standard Python postprocessing. The API uses Python exceptions for error handling, integrating naturally with Python&\#x27;s resource management patterns. The approach is portable to both Jetson and RTX Spark platforms, and the author provides practical code snippets and emphasizes that only minimal model-specific code is needed for preprocessing and postprocessing.

**「Takeaway」** The cuda.bindings.cudla module enables efficient, model-agnostic DLA inference workflows directly in Python on Jetson AGX Orin, streamlining development and orchestration without C++ boilerplate. This approach brings native DLA acceleration to Python-centric edge AI pipelines, making advanced hardware features accessible and flexible for rapid prototyping and deployment.

**Tags**: `#NVIDIA Jetson`, `#DLA`, `#Python bindings`, `#Edge AI`, `#Inference workflow`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Nvidia CEO Resignation Sparks U.S.-China Tension and Export Control Debate](https://www.cnbc.com/2026/11/13/jensen-huang-nvidia-us-china-relations.html) ⭐️ 8.0/10

Nvidia CEO Jensen Huang resigned after admitting to an affair with a woman alleged by U.S. intelligence to be a Chinese spy, prompting Congressional scrutiny and raising the likelihood of stricter U.S. technology export controls on China before year-end, according to analysts. China&\#x27;s Foreign Ministry has denied the espionage allegations.

rss · CNBC Finance · Nov 13, 02:56

**「Background」** Jensen Huang co-founded Nvidia and served as its CEO from 1993 until his resignation in November 2026, leading the company to become a major player in the global technology and semiconductor industry.

**「Impact」** Tighter U.S. export controls could limit American technology sales to China and disrupt the global semiconductor industry.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jensen_Huang">Jensen Huang - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#US-China relations`, `#semiconductors`, `#corporate governance`, `#export controls`, `#policy risk`

---

<a id="item-finance-news-2"></a>
### [Lutnick faces questions over Nvidia spy scandal. His sons&\#x27; firm has deep ties to the chipmaker](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 7.0/10

Cantor Fitzgerald and its leadership face scrutiny over their ties to Nvidia amid U.S. government concerns about AI chip exports to China and potential conflicts of interest.

rss · CNBC Finance · Nov 13, 23:42

**Tags**: `#Nvidia`, `#Cantor Fitzgerald`, `#US-China relations`, `#regulation`, `#technology`

---

<a id="item-finance-news-3"></a>
### [Chicago Fed President Signals More Action Needed on Inflation](https://www.cnbc.com/2026/11/13/chicago-feds-goolsbee-says-central-bank-has-definitely-got-work-to-do-on-inflation.html) ⭐️ 7.0/10

Chicago Federal Reserve President Austan Goolsbee said the central bank &\#x27;has definitely got work to do&\#x27; on inflation, following October&\#x27;s producer price index showing a 6.5% annual gain—the highest since November 2022. Markets now expect a possible interest rate hike at the next Federal Open Market Committee meeting in December.

rss · CNBC Finance · Nov 13, 14:22

**「Background」** The Federal Reserve sets U.S. interest rates to control inflation, with a long-term target of 2% annual inflation; recent data shows inflation has remained above this target for nearly six years.

**Tags**: `#Federal Reserve`, `#inflation`, `#monetary policy`, `#interest rates`, `#economic data`

---