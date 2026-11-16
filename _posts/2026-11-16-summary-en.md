---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 37 items, 16 important content pieces were selected

---

**Technology News**
1. [Meta FAIR &amp; NYU: Vision Encoder Pretraining Optional in MLLMs](#item-tech-news-1) ⭐️ 8.0/10
2. [Multiplayer Game Uses Local World Models for Real-Time Rendering](#item-tech-news-2) ⭐️ 8.0/10
3. [Meituan Open-Sources LongCat-2.5, Trained Without Nvidia GPUs](#item-tech-news-3) ⭐️ 8.0/10
4. [Old Bitly Links Vulnerable to Hijacking](#item-tech-news-4) ⭐️ 7.0/10
5. [Protomaps Simplifies and Lowers Cost of Self-Hosting Map Tiles](#item-tech-news-5) ⭐️ 7.0/10
6. [MacBook Pro OLED Displays and PWM Flicker Concerns](#item-tech-news-6) ⭐️ 7.0/10
7. [Microsoft 365 Outage Linked to Chlorine Gas Incident at Hotel](#item-tech-news-7) ⭐️ 7.0/10
8. [Tool Achieves 5x Faster cudaMemcpy on B300 GPUs](#item-tech-news-8) ⭐️ 7.0/10
9. [Training-Free Early Exit for Reasoning Models via Output Layer Edit](#item-tech-news-9) ⭐️ 7.0/10
10. [Marimba: Lightweight Open-Source Speech Model Released](#item-tech-news-10) ⭐️ 7.0/10
11. [Hackathon Tool Aligns Wikipedia Sentences Across Languages and Time](#item-tech-news-11) ⭐️ 7.0/10
12. [Tesla Cybercab Requires $299/Month Subscription to Operate](#item-tech-news-12) ⭐️ 7.0/10
13. [Allegations of Anthropic, Rubio Role in Jensen Huang Ouster](#item-tech-news-13) ⭐️ 7.0/10
14. [Huawei Cloud Releases openPangu-2.1-Pro Open-Source Model](#item-tech-news-14) ⭐️ 7.0/10

**Financial News**
1. [Cantor Fitzgerald&\#x27;s Nvidia Ties Face Scrutiny Amid U.S. Export Crackdown](#item-finance-news-1) ⭐️ 8.0/10
2. [U.S. Judge Allows DRAM Price-Fixing Lawsuit Against Chipmakers to Proceed](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Meta FAIR &amp; NYU: Vision Encoder Pretraining Optional in MLLMs](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Meta FAIR and NYU conducted a large-scale study training over 200 multimodal large language models \(MLLMs\) to systematically test the necessity of vision encoder pretraining and architecture choices. Their results show that separate pretraining of the vision encoder is optional: models with encoders trained from scratch alongside the LLM perform as well as those with extensive pretraining, even when pretraining is &\#x27;free&\#x27; or much longer. However, having vision-only parameters \(distinct from text\) is essential for strong visual question answering \(VQA\) performance, regardless of whether these parameters are in a separate encoder or fused into the LLM&\#x27;s early layers. The study also finds that the placement of vision processing \(before or within the LLM\) is flexible, but omitting vision-only parameters leads to much worse results.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**「Background」** Multimodal large language models \(MLLMs\) combine vision and language processing, and there has been ongoing debate about the necessity and design of vision encoders within these systems. Previous research from Meta FAIR and NYU has explored unified architectures and the impact of pretraining strategies, with some studies suggesting that training vision and language together from scratch can outperform approaches that bolt on vision encoders after language model pretraining. These discussions have highlighted the complexity of balancing compute budgets, data requirements, and architectural choices in developing effective multimodal models.

**「Impact」** Developers of multimodal LLMs can simplify model design by skipping separate vision encoder pretraining, focusing instead on ensuring vision-only parameters are present somewhere in the architecture. This could reduce training complexity and resource requirements for new multimodal models.

<details><summary>References</summary>
<ul>
<li><a href="https://aigazine.net/industry/meta-fair-and-nyu-present-advances-in-multimodal-ai-pretraining-with-moe-architecture--s">Meta FAIR and NYU Present Advances in Multimodal AI Pretraining ...</a></li>
<li><a href="https://toknow.ai/posts/meta-fair-beyond-language-modeling-multimodal-pretraining/">Meta FAIR Finds That Training Vision and Language Together From...</a></li>

</ul>
</details>

**Tags**: `#multimodal models`, `#vision encoders`, `#machine learning research`, `#model architecture`

---

<a id="item-tech-news-2"></a>
### [Multiplayer Game Uses Local World Models for Real-Time Rendering](https://www.reddit.com/r/MachineLearning/comments/1xx4ta3/we_made_a_multiplayer_game_where_each_players/) ⭐️ 8.0/10

A new multiplayer game prototype generates each player&\#x27;s view in real time using a world model and diffusion transformers running locally on their GPU. The system synchronizes game state via a lightweight server, but all rendering is performed client-side based on player actions and previous frames. The model was trained on an open dataset of 3,958 hours of 10-player CS:GO bot matches, and the beta is now open and free to play for users with an RTX 3080 or better \(with an experimental Mac build also available\). The current implementation is limited to a single small map and pistols, with visual fidelity still below the original game.

reddit · r/MachineLearning · /u/bengal7ion · Nov 15, 19:46

**「Background」** Traditional multiplayer games rely on a central server to synchronize game state and a local game engine to render each player&\#x27;s view. In contrast, this project uses a machine learning world model—specifically, diffusion transformers—trained on a large dataset of CS:GO bot matches to generate each player&\#x27;s visual experience in real time on their own GPU. This approach eliminates the need for a conventional rendering engine, instead leveraging generative AI to synthesize game visuals based on synchronized game state and player inputs.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/v0rt3ch/status/2122031717712085388">vor.tech on X: &quot;1/ We made a playable multiplayer game using ...</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#world models`, `#diffusion transformers`, `#multiplayer systems`, `#open dataset`

---

<a id="item-tech-news-3"></a>
### [Meituan Open-Sources LongCat-2.5, Trained Without Nvidia GPUs](https://the-decoder.com/meituan-releases-a-1-6-trillion-parameter-agent-model-that-never-touched-an-nvidia-gpu/) ⭐️ 8.0/10

Meituan has released the weights for LongCat-2.5, a large multimodal agent model designed for complex, multi-step tasks such as programming. The model was trained entirely on Chinese hardware \(Huawei Ascend accelerators\) and did not use Nvidia GPUs at any stage. LongCat-2.5 supports text, image, and video inputs, activates approximately 48 billion parameters per token, and is available under the commercial-friendly MIT license. On the Terminal Bench v2.1 benchmark, it scored 88.4, slightly below Claude Opus 5&\#x27;s 89.1.

telegram · zaihuapd · Nov 15, 11:08

**「Background」** LongCat-2.5 is a large language model developed by Meituan, notable for its multimodal capabilities and a context window of up to 1 million tokens. The model was released in November 2026 and is available via API with commercial pricing, as well as a temporary free trial on some platforms. Its release follows a trend of increasingly large and capable AI models, but LongCat-2.5 distinguishes itself by being trained entirely on Chinese hardware, specifically Huawei Ascend accelerators, rather than Nvidia GPUs.

**「Impact」** Developers and organizations seeking alternatives to Nvidia-based AI infrastructure can now access a high-performing, open-source model trained entirely on Chinese hardware, potentially reducing reliance on US technology and easing compliance with export restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/models/longcat-2.5">LongCat - 2 . 5 Benchmarks, Pricing &amp; Context Window</a></li>
<li><a href="https://teamorouter.com/blogs/longcat-2-5-api">LongCat - 2 . 5 API: Price, Specs and How to Call Meituan &#x27;s New Model ...</a></li>
<li><a href="https://www.youtube.com/watch?v=xYo_lFvVKpY">LongCat 2 . 5 Is Now FREE on OpenCode?! - YouTube</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI models`, `#hardware`, `#machine learning`

---

<a id="item-tech-news-4"></a>
### [Old Bitly Links Vulnerable to Hijacking](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 7.0/10

Old Bitly links are reportedly being hijacked, raising concerns about the security and reliability of using third-party URL shorteners. This issue affects any web content or service that relies on persistent access to resources via Bitly links, especially those created years ago. The report highlights the risk that abandoned or unmaintained short links can be repurposed for malicious or unintended uses, undermining trust in shared URLs.

hackernews · hspeiser · Nov 15, 22:11 · [Discussion](https://news.ycombinator.com/item?id=50511395)

**「Background」** Bitly is a popular URL shortening service that allows users to create compact links that redirect to longer web addresses. Broken link hijacking is a known security risk where attackers take control of expired or abandoned links, often by registering lapsed domains or reclaiming unused short links, and redirect them to malicious or unintended destinations. This vulnerability is particularly concerning for organizations and individuals who have widely shared short links, as these can be repurposed if not properly maintained or if the associated accounts lapse.

**「Impact」** Organizations and individuals who have used Bitly or similar URL shorteners for important or long-lived content may find their links redirecting to unintended or malicious destinations if those links are hijacked. This can damage reputations, disrupt user access, and potentially expose users to security threats, making regular auditing or archiving of critical links advisable.

**「Community Discussion」** Commenters argue that relying on outsourced link shorteners increases the risk of broken or hijacked links over time, and some advocate for in-house solutions or archiving as safer alternatives. Others note the broader problem of abandoned web resources and the challenges of maintaining link integrity across the internet.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=grLWfIbXAys">How I was found broken link hijacking less than 2 minutes... - YouTube</a></li>
<li><a href="https://www.drlinkcheck.com/blog/broken-link-hijacking">Broken Link Hijacking : How Broken Links Can Be a Security Risk</a></li>

</ul>
</details>

**Tags**: `#security`, `#web infrastructure`, `#url shorteners`, `#internet hygiene`

---

<a id="item-tech-news-5"></a>
### [Protomaps Simplifies and Lowers Cost of Self-Hosting Map Tiles](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

Protomaps now enables developers to self-host map tiles more affordably and with less complexity, providing a viable alternative to commercial mapping APIs. This approach allows for greater privacy, control, and cost savings, especially for projects with high map usage or specific customization needs. The tool is positioned as easy to deploy and maintain, making it accessible even for smaller teams or individual developers. However, high-resolution satellite imagery at large scales remains costly and storage-intensive.

hackernews · bcye · Nov 15, 19:26 · [Discussion](https://news.ycombinator.com/item?id=50509837)

**「Background」** Protomaps is an open-source mapping solution that allows developers to self-host vector map tiles as a single file, eliminating the need for a dedicated tile server. Unlike commercial providers such as Mapbox or Google Maps, which require API keys and charge based on usage, Protomaps enables unmetered access with costs limited to storage and bandwidth. The system uses HTTP range requests to efficiently serve map data, and its basemaps are derived from OpenStreetMap data.

**「Impact」** Developers and organizations can reduce or eliminate recurring costs from commercial map providers by switching to Protomaps, while gaining more control over data privacy and customization. This is particularly beneficial for projects with high map traffic or those requiring offline access, though storage requirements for high-resolution or global coverage may still pose challenges.

**「Community Discussion」** Users report positive experiences with Protomaps, citing significant cost savings and ease of use compared to commercial services like Google Maps and Maptiler. Some highlight technical limitations with large or high-resolution datasets, while others mention alternative open-source projects and practical deployment tips.

<details><summary>References</summary>
<ul>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>
<li><a href="https://protomaps.com/about">Protomaps - The open source map in a file</a></li>
<li><a href="https://docs.protomaps.com/">Protomaps Documentation | Protomaps Docs</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#mapping`, `#web-development`, `#tools`

---

<a id="item-tech-news-6"></a>
### [MacBook Pro OLED Displays and PWM Flicker Concerns](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

A technical analysis highlights that recent MacBook Pro models with OLED displays use Pulse Width Modulation \(PWM\) for brightness control, which can introduce flicker at certain frequencies. The article discusses measurements suggesting PWM frequencies around 480Hz to 960Hz, depending on display configuration, and notes that this flicker may cause discomfort or health issues for users sensitive to such effects. The issue is particularly relevant for those with flicker sensitivity, migraines, or neurological conditions. The analysis also points out that while OLED offers superior image quality, its PWM implementation can make the display less usable for some users.

hackernews · MacAnorak · Nov 15, 13:15 · [Discussion](https://news.ycombinator.com/item?id=50506719)

**「Background」** Pulse Width Modulation \(PWM\) is a common method used in OLED displays to control brightness by rapidly switching the display on and off. Recent lab tests, such as those by Notebookcheck, have measured the new 14-inch MacBook Pro&\#x27;s OLED display using PWM at 240 Hz for brightness settings below 100%, which is significantly lower than the 14,880 Hz measured on previous Mini-LED models. Lower PWM frequencies like 240 Hz are more likely to cause visible flicker, which can lead to eye strain, headaches, or nausea in users sensitive to flicker.

**「Impact」** Users who are sensitive to screen flicker, such as those with migraines or certain neurological conditions, may experience discomfort or adverse effects when using MacBook Pro OLED displays due to their PWM-based brightness control. Developers and organizations concerned with accessibility should be aware of these limitations when recommending or deploying these devices.

**「Community Discussion」** Commenters debated the technical specifics of the PWM frequency, with some suggesting the effective frequency could be as high as 960Hz due to the tandem OLED design. Others shared personal experiences with flicker sensitivity, noting that even high-frequency PWM can cause significant discomfort for some individuals, and highlighted the broader impact of display technologies on users with specific health conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.appleheadlines.com/macbook-pro-oled-eye-strain-pwm-flicker/">MacBook Pro OLED Eye Strain &amp; PWM Flicker: 7 Moves - AH</a></li>
<li><a href="https://daily.dev/posts/the-macbook-pro-s-oled-pwm-problem-when-a-better-display-becomes-worse-to-use-bxu5e2tu9">The MacBook Pro&#x27;s OLED PWM Problem: When a &#x27;Better&#x27;...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#display technology`, `#user experience`, `#accessibility`

---

<a id="item-tech-news-7"></a>
### [Microsoft 365 Outage Linked to Chlorine Gas Incident at Hotel](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

A Microsoft 365 outage reportedly prevented email alerts from reaching hotel staff, resulting in a chlorine dosing system over-dispensing chlorine and causing gas poisoning for 15 guests at a hotel in Germany. The hotel&\#x27;s automated safety system relied on email notifications to warn staff of dangerous chlorine levels, but these alerts were not received due to the cloud service disruption. This incident highlights a critical failure in the design of safety-critical automation systems that depend solely on cloud-based communication channels.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**「Background」** The incident occurred when a Microsoft 365 \(Outlook\) outage prevented automated safety alert emails from reaching staff at Hotel Ling Bao in Germany&\#x27;s Phantasialand theme park. The hotel&\#x27;s pool area had an automated dosing system that malfunctioned and dispensed excessive chlorine, but the maintenance safety system&\#x27;s warning was only sent via email, which was blocked by the cloud outage. As a result, staff were unaware of the chemical hazard until guests were already exposed and injured.

**「Impact」** Organizations operating safety-critical systems that depend on cloud-based alerting should urgently review their failover and redundancy strategies, as reliance on a single communication channel can lead to severe real-world consequences if disrupted.

**「Community Discussion」** Commenters overwhelmingly argue that the fault lies with the hotel&\#x27;s system design, not Microsoft, emphasizing that safety-critical alerts should never depend solely on cloud email. Several note that proper redundancy and local fail-safes are essential, and that this incident demonstrates a dangerous lack of operational risk planning.

<details><summary>References</summary>
<ul>
<li><a href="https://timesofindia.indiatimes.com/technology/tech-news/a-hotel-in-germany-reports-chlorine-gas-poisoning-after-email-warning-system-fails-due-to-microsoft-365-outage-guests-taken-to-hospital/articleshow/135864509.cms">A hotel in Germany reports Chlorine gas poisoning after email ...</a></li>
<li><a href="https://windowsforum.com/news/outlook-outage-blocked-phantasialand-pool-alerts-before-chlorine-incident-injured-15.452435/">Outlook Outage Blocked Phantasialand Pool Alerts Before ...</a></li>
<li><a href="https://www.yahoo.com/news/world/articles/microsoft-365-outage-leads-chlorine-154113086.html?fr=sycsrp_catchall">Microsoft 365 outage leads to chlorine gas poisoning of 15 ...</a></li>

</ul>
</details>

**Tags**: `#cloud-dependency`, `#system-design`, `#automation`, `#safety-critical`

---

<a id="item-tech-news-8"></a>
### [Tool Achieves 5x Faster cudaMemcpy on B300 GPUs](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

A new tool has been released that accelerates cudaMemcpy pageable memory transfers on B300 GPUs, achieving up to a 5x speedup in benchmarked scenarios. In a practical test copying a 1 GB tensor between CPU and GPU, transfer speeds increased from 10.2 GB/s to 51.5 GB/s when using the tool. The tool is available on GitHub and is aimed at users seeking to optimize data movement in machine learning and high-performance computing workflows. No deep technical details or broad compatibility information are provided in the announcement.

reddit · r/MachineLearning · /u/makneeee · Nov 15, 18:20

**「Background」** cudaMemcpy is a CUDA API function used to transfer data between CPU \(host\) and GPU \(device\) memory. Transfers from pageable \(regular\) host memory are typically slower than those from pinned \(page-locked\) memory, which is often used to maximize transfer speeds. The new cudamemcpy-tuner tool specifically targets pageable memory transfers on Nvidia B300 GPUs, where such transfers have historically been a bottleneck in machine learning and high-performance computing workflows.

**「Impact」** Users working with B300 GPUs can potentially reduce data transfer bottlenecks in their machine learning pipelines by adopting this tool, leading to faster training and inference times when large tensors are involved.

<details><summary>References</summary>
<ul>
<li><a href="https://agihunt.info/en/p/1a1e07bf9febb7c90bad763fb45">cudamemcpy-tuner speeds up pageable cudaMemcpy… · AGI Hunt</a></li>
<li><a href="https://stackoverflow.com/questions/19268428/pinned-memory-in-cuda-and-cudamemcpy">gpu - Pinned memory in CUDA and cudamemcpy () - Stack Overflow</a></li>

</ul>
</details>

**Tags**: `#GPU`, `#performance`, `#machine learning`, `#tools`

---

<a id="item-tech-news-9"></a>
### [Training-Free Early Exit for Reasoning Models via Output Layer Edit](https://www.reddit.com/r/MachineLearning/comments/1xx1xdm/trainingfree_early_exit_for_reasoning_models_a/) ⭐️ 7.0/10

A Reddit post introduces a training-free method to enable early exit in reasoning models by modifying a single row in the output layer weights, specifically the row corresponding to the &lt;/think&gt; token. This approach uses a linear probe derived from hidden states to adjust the model so it halts computation once an answer is reached, without requiring retraining or inference-time code changes. Preliminary results on models like Qwen3.5-4B and DeepSeek V4.1 Flash show significant reductions in token usage \(up to 84% less &\#x27;thinking&\#x27;\) with no loss in accuracy on small math and coding tasks. The method&\#x27;s limitations include small sample sizes and fitting the probe only on math problems, so broader applicability remains unproven.

reddit · r/MachineLearning · /u/Good-Presentation-23 · Nov 15, 17:52

**「Background」** Early exit techniques in reasoning models aim to reduce unnecessary computation by halting inference once the model has likely reached a correct answer. Traditional approaches often require additional training, external probes, or inference-time code changes to detect when reasoning is complete. Recent research has explored training-free methods, but these typically involve external probes or heuristics rather than directly modifying the model&\#x27;s output layer weights.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2602.02010v1">NEAT: Neuron-Based Early Exit for Large Reasoning Models</a></li>
<li><a href="https://aiweekly.co/alerts/paper-injected-think-doesnt-cleanly-halt-lrm-reasoning">Paper: Injected Doesn&#x27;t Cleanly Halt LRM Reasoning</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#language models`, `#model efficiency`, `#reasoning`

---

<a id="item-tech-news-10"></a>
### [Marimba: Lightweight Open-Source Speech Model Released](https://www.reddit.com/r/MachineLearning/comments/1xwzsm4/marimba_a_system_one_model_for_speech_r/) ⭐️ 7.0/10

Marimba is a newly released open-source speech model designed for fast, lightweight, and typed decision-making on audio data. Built on a frozen Qwen3-ASR-0.6B backbone, it supports multiple speech-related tasks such as voice activity detection, turn endings, speaker changes, and speaker count, using zero-shot scores and calibration for word and language queries. The release includes open weights under the Apache-2.0 license, installation via pip, code, benchmarks, and a forthcoming arXiv paper. Marimba is intended for practitioners and researchers seeking efficient, multi-task speech processing tools.

reddit · r/MachineLearning · /u/solanotodesch · Nov 15, 16:30

**「Background」** Marimba is built on top of the Qwen3-ASR-0.6B model, which is an open-weight, compact speech recognition model designed for efficient speech-to-text tasks. Qwen3-ASR-0.6B is part of the Qwen3-ASR family and is known for its lightweight architecture and open-source availability, making it suitable for integration into new speech processing systems.

<details><summary>References</summary>
<ul>
<li><a href="https://benchlm.ai/models/qwen3-asr-0-6b">Qwen 3 - ASR 0 . 6 B Context, Specs &amp; Sources (September 2026)</a></li>

</ul>
</details>

**Tags**: `#speech-recognition`, `#open-source`, `#machine-learning`, `#audio-processing`

---

<a id="item-tech-news-11"></a>
### [Hackathon Tool Aligns Wikipedia Sentences Across Languages and Time](https://www.reddit.com/r/MachineLearning/comments/1xwttxo/hackathon_project_for_mariadbs_wikipedia_through/) ⭐️ 7.0/10

A hackathon project called Parallax enables users to align and compare Wikipedia articles across Finnish, Swedish, German, English, Russian, Estonian, and Ukrainian editions at any historical revision. The system uses MariaDB&\#x27;s system-versioned tables to track sentence-level changes over time, sentence embeddings \(bge-m3, 1024 dimensions\) for cross-lingual matching, and Gemini 3.8 Flash to judge semantic similarity. The tool can identify where editions differ at any past date, with retrieval and matching performance metrics provided. Limitations include reliance on a small hand-checked set for evaluating the LLM-based judge&\#x27;s accuracy.

reddit · r/MachineLearning · /u/Loxbey · Nov 15, 12:03

**「Background」** MariaDB is an open-source relational database system that supports advanced features such as system-versioned tables, which allow tracking changes to data over time. The MariaDB Foundation organizes hackathons to promote innovative uses of its database technology, including challenges like &\#x27;Wikipedia Through Time&\#x27; that encourage participants to explore historical and multilingual data analysis. Previous hackathons have focused on leveraging MariaDB&\#x27;s capabilities for time-based and vector search applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MariaDB">MariaDB - Wikipedia</a></li>
<li><a href="https://github.com/danielbacsur/junction-x-wikipedia-hackathon">GitHub - danielbacsur/junction-x-wikipedia-hackathon: A time ...</a></li>
<li><a href="https://mariadb.org/projects/hackathons/">MariaDB Hackathons - MariaDB.org</a></li>

</ul>
</details>

**Tags**: `#natural-language-processing`, `#multilingual`, `#databases`, `#hackathon`

---

<a id="item-tech-news-12"></a>
### [Tesla Cybercab Requires $299/Month Subscription to Operate](https://www.tesla.com/configurator/api/v4/terms?category=autonomy_subs&amp;amp;locale=en_US&amp;amp;model=cc&amp;amp;saleType=Sale) ⭐️ 7.0/10

Tesla has released the subscription terms for its Cybercab autonomous vehicle: buyers pay $29,990 for the car and must maintain a $299 monthly subscription for autonomous operation, or the vehicle will not function. Tesla reserves the right to change the subscription price with one month&\#x27;s notice and can suspend or cancel service for non-payment or policy violations, including a one-week autonomous driving suspension after three warnings. The Cybercab is restricted to designated areas and cannot be used on ride-hailing, delivery, or rental platforms without authorization. The vehicle uses the same AI4 hardware and autonomous software as the Robotaxi Model Y, but unlike the consumer Full Self-Driving \(FSD\) package, it does not require human supervision.

telegram · zaihuapd · Nov 15, 01:10

**「Background」** Tesla&\#x27;s Cybercab is a new autonomous vehicle designed for both personal and fleet use, requiring no steering wheel or pedals. The vehicle operates under a subscription model, where users must pay a monthly fee for autonomous driving capabilities. This approach builds on Tesla&\#x27;s previous autonomous driving offerings, but Cybercab specifically enforces operational restrictions and subscription compliance to enable or disable vehicle functionality.

**「Impact」** Buyers of the Tesla Cybercab must budget for ongoing subscription fees in addition to the purchase price, and risk losing vehicle functionality if payments lapse or terms are violated. This model shifts vehicle ownership toward a software-as-a-service approach, with strict operational and usage controls enforced remotely by Tesla.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tesla.com/support/robotaxi/cybercab">Cybercab Frequently Asked Questions | Tesla Support</a></li>
<li><a href="https://www.zerohedge.com/technology/tesla-opens-cybercab-orders-select-customers-personal-use">Tesla Opens Cybercab Orders To &quot;Select Customers...&quot; | ZeroHedge</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#software licensing`, `#AI hardware`, `#technology industry`

---

<a id="item-tech-news-13"></a>
### [Allegations of Anthropic, Rubio Role in Jensen Huang Ouster](https://www.washingtonpost.com/technology/2026/11/13/behind-jensen-huangs-spy-scandal-shadow-war-trumps-ear-china/) ⭐️ 7.0/10

A Washington Post report alleges that Nvidia CEO Jensen Huang&\#x27;s departure was influenced by a coordinated effort involving US Senator Marco Rubio, US intelligence officials, and possibly Anthropic executives. The report claims Huang&\#x27;s lobbying to ease US chip export restrictions to China angered national security officials and &\#x27;China hawks,&\#x27; leading to pressure for his removal. Anthropic is suspected of tipping off journalists about a related investigation, due to its lobbying for stricter export controls and technical restrictions on AI chips. These developments coincide with new legislative efforts to further tighten US controls on AI chip exports and require anti-smuggling technology in hardware.

telegram · zaihuapd · Nov 15, 08:08

**「Background」** Jensen Huang, the CEO of Nvidia, recently resigned following media reports about his personal life and alleged lobbying activities related to US-China chip export policy. The Washington Post and other outlets have reported that US officials, including Senator Marco Rubio, played a role in escalating pressure on Huang, with Rubio reportedly drafting a strong memo based on CIA intelligence. There is also speculation that Anthropic, an AI company with interests in stricter export controls, may have influenced media investigations, though neither journalists nor Anthropic have confirmed this involvement.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=7UX_h-DVUuc">Who Took Down Jensen Huang , and Why? - YouTube</a></li>
<li><a href="https://www.zerohedge.com/ai/was-jensen-taken-out-over-open-source-sacks-says-anthropics-safetyist-allies-want-all-models-and">Was Jensen Taken Out Over Open Source? Sacks Says... | ZeroHedge</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/14/jensen-huang-affair-nvidia-nightmare">‘ Jensen Huang lost his mind’: how AI ’s smartest man... | The Guardian</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#hardware`, `#technology industry`, `#geopolitics`

---

<a id="item-tech-news-14"></a>
### [Huawei Cloud Releases openPangu-2.1-Pro Open-Source Model](https://mp.weixin.qq.com/s/8JfFmscBTDl_mPQMycD8Nw) ⭐️ 7.0/10

Huawei Cloud has launched the open-source Pangu-2.1-Pro model on its MaaS \(Model-as-a-Service\) platform. This release focuses on enhanced capabilities for agent development, AI coding, and inference optimization, with over 100,000 specialized data samples used to improve skill triggering and tool invocation. The model is specifically adapted for HarmonyOS ArkTS development, Ascend hardware operator generation, and integration with Huawei products such as AgentArts, CodeArts, and OfficeAce. Pricing for inference is set at 0.8 RMB per million input tokens, 3.2 RMB per million output tokens, and 0.016 RMB per million input tokens for cache hits.

telegram · zaihuapd · Nov 15, 16:03

**「Background」** Huawei&\#x27;s Pangu series are large language models developed for enterprise and industry applications, with previous versions such as PanGu 3.0 introduced in 2023 and tailored for sectors like government and manufacturing. The openPangu-2.1-Pro model is part of Huawei Cloud&\#x27;s Model as a Service \(MaaS\) platform, and this release focuses on enhancing capabilities for the HarmonyOS ecosystem and low-level operator development on Ascend hardware. The Pangu models use a layered architecture to support both general and scenario-specific AI tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Huawei_PanGu">Huawei PanGu - Wikipedia</a></li>
<li><a href="https://baike.baidu.com/en/item/openPangu-2.1-Pro/7509035">openPangu-2.1-Pro（Huawei Cloud Pangu Series Large Language ...</a></li>
<li><a href="https://www.huaweicloud.com/intl/en-us/product/pangu.html">PanguLM_Large Models-HUAWEI CLOUD</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI models`, `#cloud platforms`, `#software engineering`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Cantor Fitzgerald&\#x27;s Nvidia Ties Face Scrutiny Amid U.S. Export Crackdown](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 8.0/10

Cantor Fitzgerald, led by the sons of Commerce Secretary Howard Lutnick, reduced its reported Nvidia shareholdings by nearly 50% between September 2025 and March 2026, as U.S. officials increased scrutiny of Nvidia&\#x27;s links to China and imposed new export restrictions. There is no evidence of wrongdoing, but ethics experts and government officials have raised concerns about potential conflicts of interest and the firm&\#x27;s ongoing business ties to Nvidia.

rss · CNBC Finance · Nov 15, 19:58

**「Background」** Howard Lutnick, now U.S. Commerce Secretary, previously led Cantor Fitzgerald, a financial firm that held significant Nvidia shares and maintained business ties with the chipmaker while Lutnick faced government pressure to restrict technology exports to China due to national security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/lutnick-nvidia-ai-chips-china/">Lutnick should have prevented the diversion of sensitive ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/13/nvidia-scandal-sparks-us-national-security-concerns-china">Nvidia scandal: Howard Lutnick under pressure over alleged ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Cantor Fitzgerald`, `#export controls`, `#conflict of interest`, `#technology sector`

---

<a id="item-finance-news-2"></a>
### [U.S. Judge Allows DRAM Price-Fixing Lawsuit Against Chipmakers to Proceed](https://www.tomshardware.com/tech-industry/big-tech/judge-denies-motion-to-dismiss-dram-price-fixing-lawsuit-against-micron-samsung-and-sk-hynix-says-chipmakers-acted-like-hawks-flying-in-formation-finds-evidence-of-dram-collusion-plausible-after-500-percent-price-surge) ⭐️ 7.0/10

A U.S. judge denied Micron, Samsung, and SK Hynix&\#x27;s request to dismiss a class-action lawsuit alleging DRAM price-fixing, citing plausible evidence of collusion after prices reportedly surged up to 500% in one year.

telegram · zaihuapd · Nov 15, 16:39

**「Background」** A group of individuals and small businesses filed a class-action lawsuit in the U.S. alleging that Micron, Samsung, and SK Hynix coordinated to restrict DRAM \(computer memory chip\) supply and drive up prices, leading to a reported surge of up to 500%.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/articles/judge-denies-motion-dismiss-dram-152445837.html?fr=sycsrp_catchall">Judge denies motion to dismiss DRAM price-fixing lawsuit ...</a></li>
<li><a href="https://wccftech.com/federal-judge-rejects-memory-makers-defense-samsung-micron-sk-hynix-dram-shortage-lawsuit/">Federal Judge Rejects Memory Makers’ Defense To ... - Wccftech</a></li>
<li><a href="https://www.techpowerup.com/354863/samsung-sk-hynix-and-micron-fail-to-get-dram-antitrust-suit-dismissed">Samsung, SK hynix, and Micron Fail to Get DRAM Antitrust Suit ...</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#semiconductors`, `#legal`, `#market regulation`

---