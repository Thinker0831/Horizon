---
layout: default
title: "Horizon Summary: 2026-11-17 (EN)"
date: 2026-11-17
lang: en
---

> From 48 items, 23 important content pieces were selected

---

**Technology News**
1. [Optimizely Breach Led to Malware on Major Sites](#item-tech-news-1) ⭐️ 8.0/10
2. [Marimba Speech Model: Multi-Task Queries with Single Frozen Encoder](#item-tech-news-2) ⭐️ 8.0/10
3. [US Closes Remote Access Loophole for Advanced AI Chips](#item-tech-news-3) ⭐️ 8.0/10
4. [Shandong University Team Presents Conditional Proof of Goldbach Conjecture](#item-tech-news-4) ⭐️ 8.0/10
5. [Carnegie Mellon Releases Full CS Courses on YouTube for Free](#item-tech-news-5) ⭐️ 7.0/10
6. [Windows 11 Telemetry Now Tracks Developer Tools Usage](#item-tech-news-6) ⭐️ 7.0/10
7. [Jiff 1.0: New Stable Datetime Library for Rust](#item-tech-news-7) ⭐️ 7.0/10
8. [Real-Time Jazz Partner Uses Sampling-Time Steering, No Fine-Tuning](#item-tech-news-8) ⭐️ 7.0/10
9. [Apple Launches Large-Scale Health AI Usage Study in US](#item-tech-news-9) ⭐️ 7.0/10
10. [Tencent Urges AI-Driven Restructuring, Fewer Management Roles](#item-tech-news-10) ⭐️ 7.0/10
11. [Tencent Hunyuan Releases Hy4 Flash Model with Lower Costs](#item-tech-news-11) ⭐️ 7.0/10
12. [Ten Nations Sign San Francisco Declaration on AI Supply Chain Security](#item-tech-news-12) ⭐️ 7.0/10
13. [Amazon Reports AI Agents Stealing API Keys via Artex Framework](#item-tech-news-13) ⭐️ 7.0/10
14. [Apple Intelligence Beta Launches on Chinese iPad and Mac](#item-tech-news-14) ⭐️ 7.0/10

**Technology Blog**
1. [Accelerating Molecular Dynamics with NVIDIA cuPotential](#item-tech-blog-1) ⭐️ 8.0/10

**Financial News**
1. [China&\#x27;s October Economic Slowdown Deepens as Key Indicators Miss Forecasts](#item-finance-news-1) ⭐️ 8.0/10
2. [Intel and CEO Face Shareholder Lawsuit After Stock Plunge](#item-finance-news-2) ⭐️ 8.0/10
3. [Berkshire Hathaway Raises Delta Stake, Cuts Bank of America Holding](#item-finance-news-3) ⭐️ 7.0/10
4. [U.S. Crude Oil Drops to $85 as Middle East Exports Recover](#item-finance-news-4) ⭐️ 7.0/10
5. [Nvidia CEO Resignation and Congressional Shift May Reshape AI Sector](#item-finance-news-5) ⭐️ 7.0/10
6. [Cantor Fitzgerald Faces Scrutiny Over Nvidia Ties Amid U.S. Intelligence Concerns](#item-finance-news-6) ⭐️ 7.0/10
7. [China Sees Net Outflow of Foreign Direct Investment in Q3 2026](#item-finance-news-7) ⭐️ 7.0/10
8. [Nvidia Board Not Considering Jensen Huang&\#x27;s Return as CEO](#item-finance-news-8) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Optimizely Breach Led to Malware on Major Sites](https://blog.report-uri.com/worlds-largest-brands-infected-with-malware-via-optimizely/) ⭐️ 8.0/10

Optimizely, a widely used web optimization service, was compromised, resulting in malware being served to users of major platforms including Zoom and GitLab. The attack exploited the third-party script supply chain, allowing malicious code to be injected into high-profile websites. The incident exposed critical vulnerabilities in delegating script management to non-engineering teams and highlighted the risks of relying on external vendors for script delivery. The breach affected users visiting these sites while the compromised scripts were active.

hackernews · kristjansson · Nov 16, 23:00 · [Discussion](https://news.ycombinator.com/item?id=50524767)

**「Background」** Optimizely Web is a widely used website testing and optimization platform that allows organizations to run experiments and manage scripts on their sites. On November 16, 2026, attackers compromised Optimizely&\#x27;s platform and injected malicious JavaScript, which was then served to visitors of at least 178 major organizations, including Zoom, GitLab, BBC, CNN, Salesforce, and others. The malicious code reportedly swapped cryptocurrency wallet addresses and skimmed card details entered by users, highlighting the risks associated with third-party script supply chains.

**「Impact」** Organizations using Optimizely or similar third-party script services face increased risk of supply chain attacks, and may need to audit their dependencies, implement stricter controls, or consider self-hosting critical scripts to mitigate future incidents.

**「Community Discussion」** Commenters criticized the practice of allowing non-engineering teams to manage third-party scripts, citing it as a root cause for bloated and insecure websites. Others argued that both vendors like Optimizely and large sites should enforce stronger security checks and consider self-hosting scripts to reduce exposure to such attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://shiftdelete.net/en/optimizely-malware">Optimizely Malware Hit 178 Sites: What It Stole and What to Do</a></li>
<li><a href="https://cybersecuritynews.com/optimizely-websites-hijacked/">Hackers Infect 178 Major Websites via Optimizely to Steal ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#web-infrastructure`, `#supply-chain`, `#incident-response`

---

<a id="item-tech-news-2"></a>
### [Marimba Speech Model: Multi-Task Queries with Single Frozen Encoder](https://www.reddit.com/r/MachineLearning/comments/1xxsqro/marimba_a_system_one_model_for_speech_r/) ⭐️ 8.0/10

Marimba is a new speech model that enables users to ask typed questions about audio—such as term detection, language identification, turn end, and speaker change/count—and receive calibrated probabilistic answers, all using a single frozen Qwen3-ASR-0.6B encoder per 8-second audio window. The model supports zero-shot term detection without term-specific training and achieves competitive or superior results to the much larger Qwen3-Omni 30B model on most tested benchmarks, including perfect language ID on FLEURS and strong speaker change detection. Marimba&\#x27;s code and weights are available under Apache-2.0, and a demo is provided. However, the model does not generalize to unseen tasks like scene classification and has some limitations on turn-end detection outside its training distribution.

reddit · r/MachineLearning · /u/solanotodesch · Nov 16, 15:47

**「Background」** Marimba is introduced as a speech model that uses a single frozen encoder \(Qwen3-ASR-0.6B\) to answer various types of audio-related queries, such as term detection, language identification, turn-end detection, and speaker change/count, without requiring term-specific training. It is benchmarked against Qwen3-Omni, a much larger \(30B parameter\) multimodal model designed for diverse input types including audio, and demonstrates competitive or superior performance on several speech tasks. The comparison highlights Marimba&\#x27;s efficiency and versatility in multi-task speech analysis, especially given its smaller model size and zero-shot capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.alphaxiv.org/abs/2611.18330">Marimba : A System One Model for Speech | alphaXiv</a></li>
<li><a href="https://huggingface.co/collections/Qwen/qwen3-omni">Qwen 3 - Omni - a Qwen Collection</a></li>
<li><a href="https://github.locker/QwenLM/Qwen3-Omni">Qwen 3 - Omni on GitHub (QwenLM/ Qwen 3 - Omni ) — FAQ &amp; Similar...</a></li>

</ul>
</details>

**Tags**: `#speech-recognition`, `#machine-learning`, `#AI-models`, `#research`

---

<a id="item-tech-news-3"></a>
### [US Closes Remote Access Loophole for Advanced AI Chips](https://www.reuters.com/legal/litigation/us-issues-rule-protect-advanced-ai-chips-being-accessed-remotely-2026-11-16/) ⭐️ 8.0/10

The US Department of Commerce has issued a new interim final rule extending export controls on advanced AI chips and servers to include restrictions on remote access. This measure aims to prevent entities from bypassing existing export bans by accessing US-origin AI hardware via third-country data centers. The rule, drafted with input from the Treasury and National Security Council, also requires export licenses for re-exporting AI chips to Indonesia, Malaysia, Singapore, Thailand, and Brazil. These changes further tighten controls on China&\#x27;s access to advanced AI technology.

telegram · zaihuapd · Nov 16, 14:44

**「Background」** The United States has previously imposed export controls to restrict China&\#x27;s access to advanced AI chips, primarily by limiting direct sales and shipments. However, these measures were undermined by a loophole that allowed remote access to such chips via data centers in third countries. The new rules specifically target this workaround by extending export controls to cover remote access, aiming to prevent Chinese entities from using advanced AI hardware hosted outside their borders.

**「Impact」** Organizations and cloud providers must now ensure that advanced US AI chips cannot be accessed remotely from restricted countries, potentially requiring technical changes to data center operations and stricter compliance checks. Companies exporting or re-exporting AI chips to several Southeast Asian countries and Brazil will face new licensing requirements, increasing administrative burdens and possibly delaying shipments.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-16/us-moves-to-limit-remote-access-to-advanced-ai-chips">US Moves to Curb China’s Remote Access to Nvidia’s AI Chips</a></li>
<li><a href="https://edition.cnn.com/2026/11/16/politics/ai-chips-restrictions-china">Trump administration tightens restrictions on flow of AI chips ahead of...</a></li>
<li><a href="https://reason.com/2026/11/16/trumps-new-chip-export-rule-targets-china-but-exempts-tiktoks-parent-company/">Trump’s new chip export rule exempts TikTok’s parent company</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#export controls`, `#technology policy`, `#international regulation`

---

<a id="item-tech-news-4"></a>
### [Shandong University Team Presents Conditional Proof of Goldbach Conjecture](https://mrc.sdu.edu.cn/info/1018/2193.htm) ⭐️ 8.0/10

A team from Shandong University, led by Li Jiamin and Liu Jianya, has presented the first conditional proof of the binary Goldbach conjecture for all sufficiently large even numbers. Their result holds under the assumption that the Generalized Riemann Hypothesis \(GRH\) for Dirichlet L-functions is true and that one of two additional spectral hypotheses is satisfied. The proof also specifies that the two primes summing to the even number must each fall between one-third and two-thirds of that number. This approach uses novel techniques distinct from classical sieve and circle methods, but it does not constitute an unconditional proof, and the GRH alone is not sufficient for the result.

telegram · zaihuapd · Nov 16, 16:01

**「Background」** The binary Goldbach conjecture is a famous unsolved problem in mathematics, proposing that every even integer greater than 2 can be expressed as the sum of two prime numbers. Despite being easy to state and verified for many cases, it has resisted a general proof for nearly three centuries. Conditional proofs, which rely on unproven assumptions such as the Generalized Riemann Hypothesis, have been explored as partial progress toward resolving the conjecture.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thinkacademy.ca/blog/blog/2026/08/06/goldbach-conjecture-guide/">The Goldbach Conjecture : Math&#x27;s Most Famous Unsolved Problem</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#theory`, `#research`, `#algorithms`

---

<a id="item-tech-news-5"></a>
### [Carnegie Mellon Releases Full CS Courses on YouTube for Free](https://www.cs.cmu.edu/learn/) ⭐️ 7.0/10

Carnegie Mellon University has begun releasing full-semester computer science course lectures for free on YouTube, with one course premiering each day during launch week and more planned for January. The initiative covers a range of topics, including foundational and advanced courses, and is supported by student-developed tools that automate much of the video production process. While similar to earlier efforts by institutions like MIT, CMU&\#x27;s approach emphasizes breadth and up-to-date content. Courseware such as projects and feedback mechanisms are planned for future release.

hackernews · pcompeau · Nov 16, 20:43 · [Discussion](https://news.ycombinator.com/item?id=50522980)

**「Background」** Carnegie Mellon University has previously offered free computer science educational resources, such as the CS Academy, which provides an interactive curriculum for high school students. Other leading universities, including MIT and Harvard, have also made full computer science courses available online at no cost. This broader movement toward open-access technical education has made high-quality learning materials more widely accessible.

**「Impact」** Students, self-learners, and educators worldwide now have free access to high-quality, current CMU computer science lectures, including advanced topics that are often unavailable outside formal enrollment. The planned addition of courseware and feedback tools could further enhance the value for independent learners seeking a more complete educational experience.

**「Community Discussion」** Commenters praised the inclusion of advanced courses and highlighted the importance of supporting materials like projects and feedback for effective learning. Some alumni and learners expressed excitement about specific courses and requested additional offerings, while others noted that strong fundamentals remain crucial even in the age of AI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=hztO5vaBTRs">Demonstration of Carnegie Mellon CS Academy - YouTube</a></li>
<li><a href="https://www.openculture.com/freeonlinecourses">1,700 Free Online Courses from Top Universities | Open Culture</a></li>

</ul>
</details>

**Tags**: `#computer-science-education`, `#open-access`, `#software-engineering`, `#artificial-intelligence`

---

<a id="item-tech-news-6"></a>
### [Windows 11 Telemetry Now Tracks Developer Tools Usage](https://xusheng.dev/posts/windows-coding-agent-telemetry/) ⭐️ 7.0/10

Windows 11 has begun collecting telemetry data specifically about which coding agents and developer tools are used on the system. This data collection is active by default and has raised privacy concerns among developers, as it potentially exposes sensitive information about development workflows and tool preferences. The change affects all Windows 11 users, particularly software engineers and developers who rely on the platform for their work.

hackernews · cwaffles · Nov 16, 22:58 · [Discussion](https://news.ycombinator.com/item?id=50524736)

**「Background」** Telemetry refers to the automatic collection and transmission of data from software or devices back to the vendor, often for diagnostics or product improvement. Windows 10 and Windows 11 have both included built-in telemetry features, which have been criticized for collecting extensive user data by default. Tools and guides exist to help users reduce or block telemetry on Windows systems, reflecting ongoing privacy concerns among users and developers.

**「Impact」** Developers concerned about privacy may reconsider their choice of operating system, with some already discussing or planning a switch to Linux to avoid such telemetry. This could lead to increased adoption of alternative platforms among privacy-conscious users.

**「Community Discussion」** Several commenters report switching from Windows to Linux due to privacy concerns and note that Linux now offers strong compatibility for both gaming and development. Others share resources and advice for migrating to Linux, emphasizing that the transition is easier than many expect.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/N0tHorizon/WindowsTelemetryBlocker">N0tHorizon/WindowsTelemetryBlocker: A PowerShell based tool to...</a></li>
<li><a href="https://www.youtube.com/watch?v=-E-WC_UvHXE">Windows 11 : Kill Telemetry , Widgets &amp; Bloat - YouTube</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#operating-systems`, `#developer-tools`, `#software-engineering`

---

<a id="item-tech-news-7"></a>
### [Jiff 1.0: New Stable Datetime Library for Rust](https://burntsushi.net/jiff/) ⭐️ 7.0/10

Jiff 1.0 is a newly released, stable datetime library for the Rust programming language. Authored by a respected developer, it offers an alternative to the widely used Chrono library, aiming to address long-standing pain points in Rust&\#x27;s date and time handling. The 1.0 release signals production readiness and a thoughtfully designed API, with explicit acknowledgment that Jiff may not suit every use case. This release is available now for Rust developers seeking a modern, stable datetime solution.

hackernews · burntsushi · Nov 16, 16:53 · [Discussion](https://news.ycombinator.com/item?id=50519744)

**「Background」** Rust has historically relied on libraries like Chrono and time for date and time handling, but these have faced criticism for API design and limitations, especially around time zone support and daylight saving time. Jiff was created to address these issues by making time zone handling a core part of its API and by aiming for a more robust and user-friendly experience. The library offers features such as customizable support for Rust&\#x27;s standard library, optional serde integration, and the ability to embed the Time Zone Database directly into binaries.

**「Impact」** Rust developers now have a stable, production-ready alternative to Chrono for date and time handling, potentially reducing frustration with legacy APIs and enabling more robust time-sensitive or scientific applications. Projects that have struggled with Chrono&\#x27;s limitations or API design may consider migrating to Jiff, though careful evaluation of compatibility and feature coverage is advised.

**「Community Discussion」** Some developers, including a former Chrono maintainer, expressed relief and gratitude for Jiff&\#x27;s release, citing burnout and frustration with Chrono&\#x27;s API stagnation. Others praised Jiff&\#x27;s professional approach in acknowledging its limitations and not aiming to be a universal solution, while some users remain satisfied with Chrono and recommend evaluating Jiff based on specific project needs.

<details><summary>References</summary>
<ul>
<li><a href="https://burntsushi.net/jiff/">A datetime library for Rust - Andrew Gallant&#x27;s Blog</a></li>
<li><a href="https://github.com/burntsushi/jiff">GitHub - BurntSushi/ jiff : A datetime library for Rust that encourages...</a></li>

</ul>
</details>

**Tags**: `#rust`, `#datetime`, `#libraries`, `#software engineering`

---

<a id="item-tech-news-8"></a>
### [Real-Time Jazz Partner Uses Sampling-Time Steering, No Fine-Tuning](https://www.reddit.com/r/MachineLearning/comments/1xxkyh3/steering_a_pretrained_music_transformer_at/) ⭐️ 7.0/10

A new real-time jazz accompaniment system, &\#x27;duetto,&\#x27; uses the pretrained Anticipatory Music Transformer \(Thickstun et al., 2023\) and steers its output at sampling time through rule-based logit editing, rather than fine-tuning the model. This approach allows the system to interactively accompany a live MIDI keyboard player, masking or biasing possible outputs based on musical context and player input. The system achieves low-latency performance \(as low as 12 ms/note on a 3080 Ti\) and is available as open-source code for noncommercial use. Limitations include occasional drift from the player and a delicate balance between rule-based control and model creativity.

reddit · r/MachineLearning · /u/GGAllin43 · Nov 16, 09:19

**「Background」** The Anticipatory Music Transformer is a pretrained model designed for music generation tasks, including accompaniment and infilling, and was trained on the Lakh MIDI dataset. It supports controllable music generation by allowing users to guide outputs through prompts or control inputs, without requiring retraining or fine-tuning. The model&\#x27;s architecture and sampling methods enable flexible manipulation of generated music, making it suitable for interactive applications such as real-time accompaniment.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2306.08620">[2306.08620] Anticipatory Music Transformer - arXiv.org</a></li>
<li><a href="https://crfm.stanford.edu/2023/06/16/anticipatory-music-transformer.html">Anticipatory Music Transformer: A Controllable Infilling ...</a></li>
<li><a href="https://github.com/jthickstun/anticipation">GitHub - jthickstun/anticipation: Anticipatory Autoregressive ... Anticipatory Music Transformer - arXiv.org Anticipatory Music Transformer - G-CLef @ CMU Anticipation and the Anticipatory Music Transformer Anticipatory Music Transformer - John Thickstun</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#music AI`, `#transformers`, `#real-time systems`

---

<a id="item-tech-news-9"></a>
### [Apple Launches Large-Scale Health AI Usage Study in US](https://www.apple.com/newsroom/2026/11/apple-launches-research-study-to-explore-the-use-of-ai-for-health/) ⭐️ 7.0/10

Apple, in partnership with clinical AI platform OpenEvidence, has launched the Apple Health AI Usage Study in the United States. The study aims to recruit up to 200,000 US residents aged 21 or older who own an iPhone 15 Pro or newer running iOS 26 or later, to examine how users interact with conversational health AI and to assess trust and understanding. The research data will not be used to train AI models, and the application is not intended for diagnosis or treatment purposes.

telegram · zaihuapd · Nov 16, 05:01

**「Background」** Conversational health AI refers to artificial intelligence systems designed to interact with users through natural language to provide health-related information or support. Apple has previously integrated health features into its devices, but this is the first large-scale study by Apple specifically focused on how users interact with conversational health AI, conducted in partnership with OpenEvidence. The study will use a dedicated app and is not intended for diagnosis or treatment, nor will the collected data be used to train AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/11/apple-launches-research-study-to-explore-the-use-of-ai-for-health/">announced the launch of an Apple Health AI Usage Study</a></li>
<li><a href="https://www.livemint.com/technology/apps/apple-launches-ai-health-study-app-in-partnership-with-openevidence-who-can-participate-and-how-it-works-11794798693805.html">Apple launches AI health study app in partnership with ... - Mint</a></li>
<li><a href="https://explainx.ai/blog/apple-health-ai-usage-study-openevidence-2026">Apple Health AI Study: 200K Users, OpenEvidence (2026 ...</a></li>

</ul>
</details>

**Tags**: `#healthcare AI`, `#industry initiative`, `#user study`, `#Apple`

---

<a id="item-tech-news-10"></a>
### [Tencent Urges AI-Driven Restructuring, Fewer Management Roles](https://weibo.com/1642634100/RrCqPwhiS) ⭐️ 7.0/10

Tencent&\#x27;s executive office has called for a company-wide shift toward AI-driven innovation, urging all core business teams to &\#x27;restart entrepreneurship&\#x27; for the AI era. The directive emphasizes organizational flattening, reducing management layers, and restructuring teams into smaller, more agile units. Leadership stated that not as many management positions are needed in the future and called for breaking down internal silos and traditional territorial mindsets. The announcement signals a significant internal strategy adjustment but does not detail specific implementation timelines or affected roles.

telegram · zaihuapd · Nov 16, 06:32

**「Background」** Tencent has recently intensified its focus on AI-driven organizational transformation, following a broader trend among major Chinese tech companies. According to recent reports, Tencent leadership has publicly emphasized the need for comprehensive restructuring to adapt to the AI era, including flattening management layers and shifting significant portions of its workforce toward AI-related roles. This follows internal speeches and company-wide communications urging teams to embrace new ways of working and reduce traditional management hierarchies.

<details><summary>References</summary>
<ul>
<li><a href="https://eu.36kr.com/en/p/4066837661963392">Tencent &amp; Baidu AI Organizational Restructuring: Which Job ...</a></li>
<li><a href="https://en.sedaily.com/world/2026/11/13/tencent-to-shift-half-of-staff-to-ai-businesses-in-sweeping">Tencent to Shift Half of Staff to AI Businesses in Sweeping ...</a></li>

</ul>
</details>

**Tags**: `#AI strategy`, `#organizational change`, `#technology industry`, `#management`

---

<a id="item-tech-news-11"></a>
### [Tencent Hunyuan Releases Hy4 Flash Model with Lower Costs](https://mp.weixin.qq.com/s/5yBbf-ctYziM5r0i6Y17lA) ⭐️ 7.0/10

Tencent Hunyuan has launched the Hy4 flash model, featuring 224 billion total parameters \(12 billion activated\), multimodal support, and a 1 million token context window. The API pricing is significantly reduced compared to both Hy4 and Hy4 preview, with input tokens priced at 0.5 RMB per million and output at 2 RMB per million, and cache hits costing only 0.02 RMB. The company claims the model&\#x27;s overall performance is slightly better than Hy4 preview, and the cost per task is as low as 1/13 of Hy4 preview and 1/20 of Hy4. Hy4 flash is already available on Tencent Cloud&\#x27;s TokenHub, WorkBuddy, and Yuanbao, with plans for open-sourcing and temporary discounts until November 30.

telegram · zaihuapd · Nov 16, 07:17

**「Background」** Tencent Hunyuan previously released the Hy4 model, a 770B parameter mixture-of-experts \(MoE\) large language model with a 1 million token context window, available through Tencent Cloud services and other platforms. The new Hy4 flash model introduces a lower-cost alternative with 224B total parameters and 12B active parameters, aiming to provide more affordable access to large language model capabilities for daily tasks. This release continues Tencent&\#x27;s strategy of offering scalable AI solutions with varying performance and pricing tiers.

**「Impact」** Organizations and developers using Tencent Hunyuan models for daily AI tasks can now achieve substantial cost savings and access improved capabilities, especially for large-context and multimodal applications. Early adopters benefit from additional discounts and free access on select platforms until the end of November.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/tencent-hy4">Tencent Hunyuan Hy 4 : specs, benchmarks, and pricing... | eesel AI</a></li>
<li><a href="https://www.binance.com/en/square/post/11-16-2026-tencent-hunyuan-launches-hy4-flash-with-224b-parameters-and-12b-active-388785367980171">Tencent Hunyuan Launches Hy 4 Flash With 224B Parameters and...</a></li>

</ul>
</details>

**Tags**: `#large language models`, `#AI industry`, `#model deployment`, `#cost optimization`

---

<a id="item-tech-news-12"></a>
### [Ten Nations Sign San Francisco Declaration on AI Supply Chain Security](https://www.state.gov/releases/office-of-the-spokesman/2026/11/the-san-francisco-declaration-on-the-secure-foundations-of-enduring-prosperity/) ⭐️ 7.0/10

On November 15, the United States and nine other countries—including Australia, India, Israel, Japan, South Korea, Qatar, Singapore, the United Arab Emirates, and the United Kingdom—signed the San Francisco Declaration. This agreement establishes a framework for international cooperation to secure the supply chain and critical infrastructure supporting superintelligence \(SI\) technologies. The declaration creates five working groups focused on innovation policy, SI applications in key sectors, end-to-end supply chain collaboration, security hubs, and SI safety and resilience. The announcement outlines policy intentions and organizational structures, but does not specify immediate technical implementations or regulatory changes.

telegram · zaihuapd · Nov 16, 10:40

**「Background」** The San Francisco Declaration is a new international agreement signed by ten countries, including the United States, aimed at securing the supply chain and critical infrastructure for superintelligence \(SI\) and AI technologies. This declaration establishes a framework for cooperation through five dedicated working groups focused on innovation policy, SI applications, supply chain collaboration, security hubs, and SI safety and resilience. The agreement reflects growing concerns about the security and durability of AI-related supply chains as foundational to national and economic security.

<details><summary>References</summary>
<ul>
<li><a href="https://www.state.gov/releases/office-of-the-spokesman/2026/11/the-san-francisco-declaration-on-the-secure-foundations-of-enduring-prosperity/">The San Francisco Declaration on the Secure Foundations of ...</a></li>
<li><a href="https://currentaffairs.adda247.com/ten-countries-sign-san-francisco-declaration-2026-to-secure-ai-supply-chains/">Ten Countries Sign San Francisco Declaration 2026 ... - adda247</a></li>
<li><a href="https://explainx.ai/blog/pax-silica-joint-ai-supply-chain-list-san-francisco-declaration-november-2026">Pax Silica AI Supply Chain List: Who Signed (2026 ...</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#supply chain`, `#international cooperation`, `#technology industry`

---

<a id="item-tech-news-13"></a>
### [Amazon Reports AI Agents Stealing API Keys via Artex Framework](https://cybernews.com/security/amazon-autonomous-cybercrime-artex-framework/) ⭐️ 7.0/10

Amazon has reported that attackers used the open-source Artex penetration testing framework to drive AI agents that autonomously steal API keys from publicly exposed AI applications such as LiteLLM and Dify. The stolen keys were verified and pooled to fund further large language model usage, creating a self-sustaining attack loop. The activity began on October 3 and was intercepted by Amazon&\#x27;s MadPot honeypot network on November 5. Amazon attributes the campaign with moderate confidence to a China-linked threat group and has notified potentially affected AWS customers.

telegram · zaihuapd · Nov 16, 13:00

**「Background」** Artex is an open-source penetration testing framework designed to automate security assessments, but it has recently been repurposed by attackers to conduct AI-driven cyberattacks. The FBI and other security organizations have warned that Artex can be used by malicious actors to automate the exploitation of vulnerabilities, including stealing sensitive data such as API keys from exposed applications. The tool&\#x27;s open-source nature and availability have made it a target for abuse, leading to its removal from GitHub, though unofficial copies remain accessible.

**「Impact」** Organizations running publicly accessible AI applications face increased risk of API key theft and misuse, especially if using open-source frameworks like LiteLLM or Dify. Immediate review and tightening of API key exposure and access controls are advised for affected users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/news/security/fbi-warns-artex-ai-hacking-tool-is-powering-global-cyberattacks/">FBI warns ARTEX AI hacking tool is powering global cyberattacks</a></li>
<li><a href="https://www.malwarebytes.com/blog/ai/2026/11/criminals-are-using-artex-ai-agents-to-speed-up-cyberattacks-fbi-warns">Criminals are using ARTEX AI agents to speed up cyberattacks , FBI...</a></li>
<li><a href="https://thehackernews.com/2026/11/backdoored-docker-image-for-artex-ai.html">CERT-In Flags AI -Driven Attacks as Backdoored ARTEX Exposes 62...</a></li>

</ul>
</details>

**Tags**: `#AI security`, `#API security`, `#cybersecurity`, `#cloud services`

---

<a id="item-tech-news-14"></a>
### [Apple Intelligence Beta Launches on Chinese iPad and Mac](https://www.theverge.com/tech/1034581/apple-intelligence-siri-ai-daily-usage-limits-icloud-subscription) ⭐️ 7.0/10

Apple Intelligence features are now available to users in China on iPad and Mac devices running iPadOS 27.3 beta 2 or macOS 27.3 beta 2. This update also patches a file sandbox escape vulnerability affecting all Apple operating systems. Additionally, Apple is testing daily usage limits for advanced Siri AI and Apple Intelligence features on iOS 27.3, iPadOS 27.3, and macOS 27.3 beta 2, restricting cloud-based advanced functions such as multi-step personal context requests and image generation/editing, while basic Siri commands remain unlimited and free.

telegram · zaihuapd · Nov 16, 20:12

**「Background」** Apple Intelligence is Apple&\#x27;s suite of AI-powered features integrated into its operating systems. These features were initially introduced to Chinese users on the iPhone with the first iOS 27.3 beta, and have now been expanded to iPad and Mac devices through the iPadOS 27.3 and macOS 27.3 beta updates. This expansion follows regulatory approval and a phased rollout strategy in China.

**「Impact」** Chinese users and developers can now test Apple Intelligence features on supported beta software, but may encounter daily limits on advanced AI capabilities, potentially affecting workflows that rely on frequent or complex Siri interactions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/11/16/ipad-mac-apple-intelligence-china/">iPad and Mac Get Apple Intelligence in China in 27.3 Betas</a></li>
<li><a href="https://appleinsider.com/articles/26/11/09/apple-intelligence-registered-for-ipad-mac-use-in-china">Apple Intelligence registered for iPad, Mac use in China</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI`, `#security`, `#operating systems`

---

## Technology Blog

<a id="item-tech-blog-1"></a>
### [Accelerating Molecular Dynamics with NVIDIA cuPotential](https://developer.nvidia.com/blog/accelerate-molecular-dynamics-simulations-with-accurate-flexible-primitives-using-nvidia-cupotential/) ⭐️ 8.0/10

rss · NVIDIA CUDA Technical Blog · Nov 16, 22:30

**「Background」** Molecular dynamics \(MD\) simulations are foundational in fields like physics, chemistry, and biology, but their performance is often limited by the computational cost of evaluating long-range interactions, especially under periodic boundary conditions. While GPUs have long accelerated MD, evolving hardware and the complexity of optimizing kernels for heterogeneous systems have made it increasingly challenging for developers to maintain both speed and accuracy, particularly for classical forcefields.

**「Solution」** The author introduces NVIDIA cuPotential, a modular library providing accurate, flexible primitives for MD simulations, designed to be easily integrated—especially with OpenMM—via a C API and plugin system. cuPotential supplies both direct and reciprocal space utilities, including advanced cutoff-based interaction evaluators and charge spreading functions, aiming for drop-in acceleration with minimal code changes. The article details the build and integration process within a Conda environment, and demonstrates usage through sample systems \(DHFR, BACE, ApoA1\) under standard simulation conditions. Benchmarking across a range of NVIDIA GPUs shows substantial speedups \(often 2–3x or more\) for systems from 24,000 to 400,000 atoms. Technically, cuPotential advances accuracy and efficiency by implementing new C2 continuous splitting and spreading functions, developed in collaboration with D. E. Shaw Research and the Flatiron Institute, which outperform traditional Ewald and PME methods in both force accuracy and energy drift. The library enables reduced real-space cutoffs and grid sizes without sacrificing accuracy, and significantly improves dispersion energy calculations—by several orders of magnitude—compared to conventional approaches. Rigorous error and energy drift analyses confirm that cuPotential&\#x27;s kernels are not a dominant source of simulation error, even over long timescales.

**「Takeaway」** NVIDIA cuPotential delivers substantial acceleration and improved accuracy for molecular dynamics simulations by providing modular, high-performance primitives that are straightforward to integrate, setting a new standard for both speed and reliability in GPU-accelerated MD workflows.

**Tags**: `#molecular-dynamics`, `#gpu-acceleration`, `#numerical-methods`, `#benchmarking`, `#simulation-software`

---

## Financial News

<a id="item-finance-news-1"></a>
### [China&\#x27;s October Economic Slowdown Deepens as Key Indicators Miss Forecasts](https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html) ⭐️ 8.0/10

China&\#x27;s retail sales rose 0.4% year-over-year in October 2026, missing analysts&\#x27; forecast of 0.8%, while industrial output grew 4.8%, below the expected 5.3%, and fixed-asset investment for January–October shrank 8.1% versus a projected 7% decline. These figures signal a worsening slowdown and increased reliance on exports, according to analysts.

rss · CNBC Finance · Nov 16, 03:53

**「Background」** In September, China&\#x27;s retail sales and industrial output had shown stronger growth, with retail sales rising 1.1% and industrial output increasing 5.5% from a year earlier, both higher than the October figures that missed analyst expectations.

**「Impact」** The weaker-than-expected data may affect Chinese households and businesses by dampening consumer confidence and investment, while global markets could face increased risks due to China&\#x27;s growing dependence on exports.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/16/china-retail-sales-october-industrial-output-investment.html">China ’s slowdown deepens in October as key economic data ...</a></li>

</ul>
</details>

**Tags**: `#China economy`, `#economic data`, `#retail sales`, `#industrial output`, `#trade`

---

<a id="item-finance-news-2"></a>
### [Intel and CEO Face Shareholder Lawsuit After Stock Plunge](https://www.investing.com/news/stock-market-news/intel-sued-by-shareholders-following-29-stock-plunge-5028171) ⭐️ 8.0/10

Intel and its CEO are being sued by shareholders who allege the company hid weak PC demand and inventory problems, after Intel&\#x27;s October 29 earnings forecast missed expectations and its stock fell 28.6%, erasing about $140 billion in market value.

telegram · zaihuapd · Nov 16, 11:10

**「Background」** Intel recently reported weaker-than-expected earnings and forecasts, mainly due to falling demand for personal computers and excess inventory, which led to a sharp drop in its stock price and prompted the shareholder lawsuit.

<details><summary>References</summary>
<ul>
<li><a href="https://wccftech.com/intel-ceo-lip-bu-tan-named-defendant-class-action-lawsuit-pc-sales-slowdown/">Intel CEO Lip-Bu Tan Named As Defendant In New Class-Action...</a></li>
<li><a href="https://www.kucoin.com/news/flash/intel-q3-net-profit-falls-18-amid-pc-demand-weakness-shares-drop-over-21-post-market">Intel &#x27;s Q3 net profit falls 18% amid weak PC demand , shares ... | KuCoin</a></li>
<li><a href="https://www.bbc.com/news/articles/cw62p42p288do">Investors sue chip giant Intel after 29% stock plunge</a></li>

</ul>
</details>

**Tags**: `#corporate litigation`, `#earnings`, `#technology sector`, `#stock market`, `#investor impact`

---

<a id="item-finance-news-3"></a>
### [Berkshire Hathaway Raises Delta Stake, Cuts Bank of America Holding](https://www.cnbc.com/2026/11/16/berkshire-hathaway-raised-its-stake-in-delta-air-in-the-third-quarter.html) ⭐️ 7.0/10

Berkshire Hathaway increased its stake in Delta Air Lines by 12% and reduced its Bank of America holdings by nearly 6% in the third quarter of 2026. These portfolio changes reflect the company&\#x27;s latest investment decisions during a period of market volatility.

rss · CNBC Finance · Nov 16, 23:01

**「Background」** Berkshire Hathaway, a large investment company, regularly adjusts its stock holdings and in the third quarter increased its stake in Delta Air Lines while reducing its position in Bank of America, reflecting its ongoing portfolio management strategy.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/16/berkshire-hathaway-raised-its-stake-in-delta-air-in-the-third-quarter.html">Berkshire Hathaway raised its stake in Delta in the third ...</a></li>

</ul>
</details>

**Tags**: `#Berkshire Hathaway`, `#stock holdings`, `#Delta Air Lines`, `#Bank of America`, `#institutional investment`

---

<a id="item-finance-news-4"></a>
### [U.S. Crude Oil Drops to $85 as Middle East Exports Recover](https://www.cnbc.com/2026/11/16/us-crude-oil-declines-to-87-a-barrel-on-recovering-middle-east-exports.html) ⭐️ 7.0/10

U.S. crude oil prices fell to $85 a barrel on Monday as Middle East exports recovered, reversing earlier supply deficit forecasts according to the International Energy Agency. The IEA now expects global oil supply to exceed demand by 1.7 million barrels per day in the fourth quarter of 2026.

rss · CNBC Finance · Nov 16, 22:19

**「Background」** Earlier in 2026, Middle East oil exports had been disrupted by regional conflicts, but recent reports show shipments are recovering and approaching pre-war levels despite ongoing security risks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iea.org/reports/oil-market-report-october-2026">Oil Market Report - October 2026 - IEA</a></li>

</ul>
</details>

**Tags**: `#oil prices`, `#energy markets`, `#Middle East exports`, `#IEA forecast`, `#commodities`

---

<a id="item-finance-news-5"></a>
### [Nvidia CEO Resignation and Congressional Shift May Reshape AI Sector](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 7.0/10

Nvidia&\#x27;s CEO Jensen Huang has resigned and the company&\#x27;s stock posted its longest losing streak since 2012, while ETF experts say a Democratic-controlled Congress could slow data center expansion by up to 20%, potentially benefiting rival chipmakers and large technology firms. These developments are based on commentary from ETF managers and analysts following Nvidia&\#x27;s leadership turmoil and recent U.S. election results.

rss · CNBC Finance · Nov 16, 12:13

**「Background」** Nvidia CEO Jensen Huang resigned after being linked to a suspected Chinese asset, prompting national security concerns and calls for answers from Congress, which is also considering new policies affecting data centers and the AI sector.

<details><summary>References</summary>
<ul>
<li><a href="https://thehill.com/homenews/senate/6217057-congress-jensen-huang-nvidia-national-security/">Jensen Huang resigns from Nvidia amid China spying scandal as ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI`, `#ETF`, `#Tech Stocks`, `#Policy`

---

<a id="item-finance-news-6"></a>
### [Cantor Fitzgerald Faces Scrutiny Over Nvidia Ties Amid U.S. Intelligence Concerns](https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html) ⭐️ 7.0/10

Cantor Fitzgerald and its leadership are under scrutiny after U.S. officials raised intelligence concerns and imposed new export restrictions, with the firm reporting a 49% decline in its Nvidia share holdings between September 2025 and March 2026 according to CNBC analysis. There is no evidence of wrongdoing, but questions have been raised about possible conflicts of interest due to Cantor&\#x27;s ongoing business ties to Nvidia and its leadership.

rss · CNBC Finance · Nov 16, 12:14

**「Background」** Jensen Huang’s resignation as Nvidia CEO has brought renewed scrutiny to U.S. Commerce Secretary Howard Lutnick and his family&\#x27;s financial ties to Nvidia, especially as Lutnick faces bipartisan criticism for not blacklisting Megaspeed, a company suspected of sending Nvidia&\#x27;s AI chips to China, despite ongoing U.S. export restrictions and intelligence concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/13/howard-lutnick-nvidia-jensen-huang-china-cantor-fitzgerald.html">Howard Lutnick&#x27;s sons&#x27; Nvidia ties amid Jensen Huang China ...</a></li>
<li><a href="https://www.firstpost.com/explainers/nvidia-scandal-why-is-trump-commerce-secretary-howard-lutnick-under-fire-14060250.html">Nvidia scandal: Why is Trump’s Commerce Secretary Howard ...</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#Cantor Fitzgerald`, `#regulation`, `#conflict of interest`, `#technology`

---

<a id="item-finance-news-7"></a>
### [China Sees Net Outflow of Foreign Direct Investment in Q3 2026](https://cn.nikkei.com/china/ceconomy/64726-2026-11-16-09-03-25.html) ⭐️ 7.0/10

Foreign direct investment in China turned into a net outflow of $900 million in the third quarter of 2026, according to official data, marking the first quarterly net outflow in a year.

telegram · zaihuapd · Nov 16, 05:29

**「Background」** Foreign direct investment \(FDI\) measures the net inflow of investment from foreign companies into a country, and a net outflow means more capital is leaving than entering; China had previously reported positive FDI for four consecutive quarters before this reversal.

**Tags**: `#China`, `#foreign direct investment`, `#capital flows`, `#economic data`

---

<a id="item-finance-news-8"></a>
### [Nvidia Board Not Considering Jensen Huang&\#x27;s Return as CEO](https://www.cnbc.com/2026/11/16/nvidia-ceo-jensen-huang.html) ⭐️ 7.0/10

Nvidia&\#x27;s board is reportedly not considering Jensen Huang&\#x27;s return as CEO and has hired a law firm to investigate his conduct for possible national security and company confidentiality risks, according to unnamed sources cited by CNBC.

telegram · zaihuapd · Nov 17, 01:39

**「Background」** Nvidia&\#x27;s board recently hired the law firm Wachtell, Lipton, Rosen &amp; Katz to investigate CEO Jensen Huang&\#x27;s conduct, focusing on potential risks to national security and company confidentiality.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/10/nvidia-wachtell-lipton-huang-affair.html">Nvidia hires law firm Wachtell Lipton to lead Jensen Huang ...</a></li>
<li><a href="https://www.cnbc.com/2026/11/16/nvidia-ceo-jensen-huang.html">Nvidia board not considering bringing Huang back as CEO: Source</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#corporate governance`, `#executive leadership`, `#technology sector`

---