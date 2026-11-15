---
layout: default
title: "Horizon Summary: 2026-11-15 (EN)"
date: 2026-11-15
lang: en
---

> From 38 items, 15 important content pieces were selected

---

**Technology News**
1. [SpaceX Achieves First Starship Tower Catch on Flight 15](#item-tech-news-1) ⭐️ 9.0/10
2. [Lovable Apps Leak Passport Data and 200K+ Messages via Security Flaw](#item-tech-news-2) ⭐️ 8.0/10
3. [Cloudflare Open-Sources Kitesurf AI Agent Browser](#item-tech-news-3) ⭐️ 8.0/10
4. [Italy Fines Meta €805M for Facebook Album Access Violations](#item-tech-news-4) ⭐️ 8.0/10
5. [Google Antigravity /teamwork Enhances Collaborative AI Workflows](#item-tech-news-5) ⭐️ 7.0/10
6. [PyPI Launches Redesigned Project Pages with Enhanced Security Signals](#item-tech-news-6) ⭐️ 7.0/10
7. [Minimal DeepSeek V3 Model in Pure JAX Released](#item-tech-news-7) ⭐️ 7.0/10
8. [Project Zero to Shorten Vulnerability Disclosure Window](#item-tech-news-8) ⭐️ 7.0/10
9. [TimeCues Studio: Free Open-Source Music Annotation Tool Released](#item-tech-news-9) ⭐️ 7.0/10
10. [Debate on Baselines for Short-Horizon Price Forecasting Papers](#item-tech-news-10) ⭐️ 7.0/10
11. [OpenAI Disbands Robotics Team, Shifts to General AI Models for Robots](#item-tech-news-11) ⭐️ 7.0/10
12. [W5000 Unmanned Cargo Aircraft Completes Test Flight](#item-tech-news-12) ⭐️ 7.0/10
13. [Windows 11 Runs Natively on Foldable iPhone via Gemini and WindowsiOS](#item-tech-news-13) ⭐️ 7.0/10

**Financial News**
1. [Anthropic IPO Bars Mainland China and Hong Kong Investors](#item-finance-news-1) ⭐️ 8.0/10
2. [Nvidia CEO Resignation and Congressional Shift Affect AI Stocks and ETFs](#item-finance-news-2) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [SpaceX Achieves First Starship Tower Catch on Flight 15](https://www.spacex.com/launches/starship-flight-15) ⭐️ 9.0/10

SpaceX successfully caught its Starship vehicle using the launch tower&\#x27;s mechanical arms at the end of Flight 15, marking the first time a human-made orbital-class spacecraft has been recovered this way. The mission launched from Texas, completed approximately 14 orbits and 22.5 hours in space, and deployed 26 Starlink V3 satellites before returning to be caught by the tower. The Super Heavy booster, however, failed to return to the tower and was lost in a controlled splashdown. This achievement demonstrates a significant advance in large-scale spacecraft reusability, though full two-stage recovery was not accomplished.

hackernews · ls612 · Nov 14, 21:22 · [Discussion](https://news.ycombinator.com/item?id=50500963)

**「Background」** SpaceX&\#x27;s Starship program aims to develop a fully reusable, orbital-class launch system, with both the booster \(Super Heavy\) and the spacecraft \(Starship\) designed for recovery and reuse. Prior to Flight 15, SpaceX had attempted but not yet succeeded in catching either stage with the launch tower&\#x27;s mechanical arms, known as &quot;chopsticks.&quot; The successful catch of Starship itself during Flight 15 marks the first time this recovery method has been achieved, following earlier tests where the booster or ship either landed elsewhere or was lost.

**「Impact」** SpaceX&\#x27;s successful tower catch of Starship paves the way for rapid turnaround and potential cost reductions in orbital launches, as it eliminates the need for ocean landings or ground recovery for the upper stage. However, operational reliability and full two-stage reusability remain to be proven in future flights.

**「Community Discussion」** Commenters compared Starship&\#x27;s achievement to the Space Shuttle, noting improvements in safety and reusability, and highlighted the potential for dramatically lower launch costs if both stages can be reliably caught and reflown. Some expressed excitement about the engineering milestone, while others pointed out that further progress is needed to achieve full two-stage recovery and rapid reusability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=VEvzBhRyB94">SpaceX Catches Starship for the First Time Ending Flight Test 15</a></li>
<li><a href="https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-flight-15-chopsticks-double-catch-super-heavy-ship">SpaceX launches Starship on ambitious 22-hour Flight 15 ... | Space</a></li>

</ul>
</details>

**Tags**: `#spaceflight`, `#hardware`, `#systems engineering`, `#industry impact`

---

<a id="item-tech-news-2"></a>
### [Lovable Apps Leak Passport Data and 200K+ Messages via Security Flaw](https://www.crissyfield.de/research/lovable-en/) ⭐️ 8.0/10

A security vulnerability in Lovable apps exposed sensitive user data, including passport details and over 200,000 private messages, due to insufficient row-level security controls. The flaw was linked to default configurations in platforms like Supabase, which did not enforce strict access controls by default for existing projects. Lovable&\#x27;s Head of Security stated that their platform scans apps for such issues and offers automated fixes, but the incident highlights gaps in both platform defaults and developer practices. The issue has prompted discussion about the need for more secure defaults and automated security tooling in cloud-based and AI-generated applications.

hackernews · armcat · Nov 14, 17:43 · [Discussion](https://news.ycombinator.com/item?id=50499017)

**「Background」** Lovable is an AI-powered app development platform that enables users to quickly generate web applications, often using Supabase as a backend database. In November 2026, security researchers scanned over 159,000 Lovable-generated apps and discovered that many had databases left open without authentication, exposing sensitive data such as passport numbers, payment details, and private messages. The root cause was identified as missing or insufficient database access rules, rather than a direct hack of the Lovable platform itself.

**「Impact」** Users of Lovable apps had their sensitive information, including passport details and private messages, exposed to unauthorized access. Developers using platforms like Supabase should review and update their security configurations, especially row-level security settings, to prevent similar breaches.

**「Community Discussion」** Community members debated the responsibility between app developers and platform providers, with some attributing blame to Supabase&\#x27;s insecure defaults and others emphasizing the need for better developer awareness. The Lovable security lead highlighted their automated scanning and fix tools, while others called for stricter platform defaults and more robust automated security checks.

<details><summary>References</summary>
<ul>
<li><a href="https://cybernews.com/security/lovable-ai-apps-expose-personal-information/">Lovable AI apps exposed sensitive data in open databases ...</a></li>
<li><a href="https://dev.to/yashvikothari/lovable-data-leak-2026-24664-ai-apps-exposed-80000-user-records-via-supabase-2l7a">Lovable Data Leak 2026: 24,664 AI Apps Exposed 80,000+ User ...</a></li>
<li><a href="https://startupfortune.com/lovable-ai-apps-left-passport-and-payment-data-open-to-anyone/">Lovable AI Apps Left Passport and Payment Data Open to ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#data breach`, `#application development`, `#cloud platforms`

---

<a id="item-tech-news-3"></a>
### [Cloudflare Open-Sources Kitesurf AI Agent Browser](https://www.phoronix.com/news/Cloudflare-Kitesurf-Open-Source) ⭐️ 8.0/10

Cloudflare has released Kitesurf, an open-source, stateless browser designed specifically for AI agents, under the Apache 2.0 license. Built on Cloudflare Workers, Kitesurf can parse HTML, handle CSS, and execute JavaScript without requiring a traditional browser container. The project aims to provide a lightweight and efficient alternative to Chromium, using less CPU and memory, and is designed to scale on Cloudflare&\#x27;s global Workers network. The source code is now available on GitHub.

telegram · zaihuapd · Nov 14, 09:33

**「Background」** Traditional web browsers like Chromium are resource-intensive and not optimized for automated or AI-driven tasks. Cloudflare developed Kitesurf as a lightweight, stateless browser engine specifically designed for AI agents, allowing efficient web interaction without the overhead of a full browser. Built on Cloudflare Workers, Kitesurf can be deployed globally and is now open source under the Apache 2.0 license, enabling broader experimentation and adoption.

**「Impact」** Developers building AI agents that interact with the web can now leverage Kitesurf for more resource-efficient browsing tasks, potentially reducing infrastructure costs and improving scalability compared to using full browser engines like Chromium.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/kitesurf-open-source/">Kitesurf is now open source | Cloudflare Blog</a></li>
<li><a href="https://www.everydev.ai/tools/kitesurf">Kitesurf - Headless Browser for AI Agents | EveryDev. ai</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#AI agents`, `#web browsers`, `#cloud infrastructure`

---

<a id="item-tech-news-4"></a>
### [Italy Fines Meta €805M for Facebook Album Access Violations](https://www.garanteprivacy.it/home/docweb/-/docweb-display/docweb/10321080) ⭐️ 8.0/10

The Italian privacy regulator has fined Meta €805 million for Facebook&\#x27;s Android app accessing approximately 20 million Italian users&\#x27; photo albums, videos, and metadata without explicit consent. The violation centers on a photo album recommendation feature introduced in 2023, which was enabled by default and used a vague authorization prompt. Meta is required to change the feature to be opt-in, with explicit user consent, within 60 days or face a ban on the feature for users who have not provided valid authorization.

telegram · zaihuapd · Nov 14, 14:37

**「Background」** The Italian Data Protection Authority fined Meta for a feature in the Facebook Android app that accessed users&\#x27; photo and video galleries without obtaining specific consent. This feature, introduced in 2023, was enabled by default and provided only a general authorization prompt, rather than clear, explicit consent for accessing personal media. The regulatory action addresses concerns over privacy and user consent in mobile app design, particularly regarding access to sensitive personal data such as photos and videos.

**「Impact」** Facebook Android users in Italy will see the album recommendation feature disabled by default, and Meta must obtain clear, separate consent before enabling it for any user. Developers and privacy teams at Meta will need to update consent flows and default settings to comply with the regulator&\#x27;s order.

<details><summary>References</summary>
<ul>
<li><a href="https://apnews.com/article/italy-meta-android-facebook-feature-9b3073c52464d5cd0e8facbc57285194">Italy fines Meta $887M over access to users&#x27; photos | AP News</a></li>
<li><a href="https://abcnews.com/Technology/wireStory/meta-fined-887-million-italy-android-gallery-photos-138145127">Meta fined $887M in Italy over Android gallery photos, videos ...</a></li>
<li><a href="https://www.politico.eu/article/italy-hits-meta-with-e805m-fine-over-privacy-law-violation/">Italy hits Meta with €805m fine over privacy law violation</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#regulation`, `#mobile development`, `#technology industry`

---

<a id="item-tech-news-5"></a>
### [Google Antigravity /teamwork Enhances Collaborative AI Workflows](https://research.google/blog/advancing-science-engineering-with-antigravitys-teamwork-feature/) ⭐️ 7.0/10

Google has introduced advances to the Antigravity /teamwork feature, which enables collaborative, multi-agent AI workflows for science and engineering tasks. The update showcases examples in mathematics, science, coding, and engineering, but represents incremental progress rather than a major shift. The feature is available to external users, with ongoing improvements and plans for more dynamic agent team-building. Some community members note that the current capabilities lag behind competing tools and lack certain automation features.

hackernews · acossta · Nov 14, 13:20 · [Discussion](https://news.ycombinator.com/item?id=50496811)

**「Background」** Google Antigravity is a software development platform where AI agents autonomously write, run, and test code. The /teamwork feature in Antigravity enables the deployment of collaborative multi-agent teams to handle large projects, complex research, and multi-file code refactoring. This framework, first announced at Google I/O and updated in August 2026, allows agents to propose, critique, and refine each other&\#x27;s work over extended periods, leveraging Google&\#x27;s advanced Gemini 3.7 Flash model.

**「Impact」** Researchers and engineers using Antigravity can now experiment with more collaborative, agent-based workflows, but may encounter limitations compared to other platforms, such as missing automation modes and less mature dynamic workflow features.

**「Community Discussion」** Some users are optimistic about the potential for AI-driven teamwork to accelerate research and development, while others express frustration over unclear usage instructions and the feature&\#x27;s lag behind alternatives like Claude dynamic workflows. There is also discussion about the need for more detailed documentation and automation capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Antigravity">Google Antigravity - Wikipedia</a></li>
<li><a href="https://antigravity.google/docs/teamwork/">Teamwork agent teams (/teamwork) | Google Antigravity Docs</a></li>
<li><a href="https://antigravity.google/blog/teamwork-when-ai-becomes-a-research-partner">Teamwork: when AI becomes a research partner - antigravity.google</a></li>

</ul>
</details>

**Tags**: `#AI systems`, `#collaborative workflows`, `#software engineering`, `#multi-agent systems`

---

<a id="item-tech-news-6"></a>
### [PyPI Launches Redesigned Project Pages with Enhanced Security Signals](https://blog.pypi.org/posts/2026-11-06-ui-updates-complete/) ⭐️ 7.0/10

PyPI has released redesigned project pages that now display clearer security and provenance signals for Python packages. These updates are live and aim to improve package trust and supply chain transparency by making it easier for users to assess the authenticity and security of packages. The new interface highlights provenance information, such as whether a package was published using trusted workflows or includes cryptographic signatures. This change is intended for all PyPI users, including developers and organizations relying on open-source Python packages.

hackernews · rbanffy · Nov 14, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50497892)

**「Background」** PyPI \(Python Package Index\) is the primary repository for Python packages, and provenance refers to verifiable information about the origin and build process of a package release. According to PyPI&\#x27;s documentation, provenance is shared via attestations, which provide a record of how and where a release file was built or published. The recent redesign of PyPI project pages now includes a dedicated Security tab that displays provenance confirmations for each release file, with a &\#x27;Full provenance&\#x27; label shown when all files have attestations.

**「Impact」** Developers and organizations can now more easily evaluate the trustworthiness of Python packages on PyPI, potentially reducing the risk of supply chain attacks. However, some users may need to adapt their publishing workflows to take full advantage of the new provenance and security features.

**「Community Discussion」** Some community members praised the move toward clearer provenance and keyless signing, hoping for broader support across CI/CD providers. Others expressed concern that the emphasis on centralized trust and reliance on major cloud providers could lead to lock-in and reduce the openness of the Python ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.pypi.org/using-pypi/package-security/provenance/">Checking Provenance (package origin) - PyPI User Documentation</a></li>
<li><a href="https://habr.com/ru/companies/codescoring/articles/1107380/">[46. 2026 ] Обзор новых правил безопасности в пакетных... / Хабр</a></li>

</ul>
</details>

**Tags**: `#python`, `#security`, `#open-source`, `#software-supply-chain`

---

<a id="item-tech-news-7"></a>
### [Minimal DeepSeek V3 Model in Pure JAX Released](https://github.com/Vaibhaav-Tiwari/deepseek-v3-jax) ⭐️ 7.0/10

A new open-source project provides a minimal implementation of the DeepSeek V3 deep learning model in approximately 200 lines of pure JAX code. This concise version is designed for accessibility, enabling users to study, experiment with, and adapt the model without the overhead of large frameworks or complex dependencies. The project is particularly notable for its compatibility with ROCm, allowing users with AMD GPUs to run and train the model locally. This release is aimed at learners, researchers, and practitioners interested in understanding modern deep learning architectures from first principles.

hackernews · VaibhaavTiwari · Nov 14, 15:04 · [Discussion](https://news.ycombinator.com/item?id=50497589)

**「Background」** DeepSeek V3 is a large-scale Mixture-of-Experts \(MoE\) language model featuring 671 billion total parameters, with only 37 billion activated per token for efficiency. It introduces architectural innovations such as Multi-head Latent Attention \(MLA\) and the DeepSeekMoE framework, aiming for faster inference and cost-effective training. The model and its technical details are fully open-sourced, enabling the community to study and experiment with its design.

**「Impact」** Users with AMD GPUs and ROCm support can now run and experiment with a modern deep learning model using JAX, which previously posed compatibility challenges. The minimal codebase also serves as an educational resource for those seeking to understand or extend DeepSeek V3 without navigating large, complex repositories.

**「Community Discussion」** Commenters praised the project for its educational value and simplicity, with one user highlighting successful end-to-end training on an AMD RX 7600 XT using ROCm and JAX. Others expressed appreciation for the opportunity to learn from a first-principles implementation and discussed the benefits of visual and interactive model representations.

<details><summary>References</summary>
<ul>
<li><a href="https://deepwiki.com/deepseek-ai/DeepSeek-V3/1.2-model-architecture-overview">Model Architecture Overview | deepseek-ai/DeepSeek-V3 | DeepWiki</a></li>
<li><a href="https://www.deepseek.com/en/news/deepseek-v3/">Introducing DeepSeek-V3</a></li>
<li><a href="https://arxiv.org/abs/2412.19437">[2412.19437] DeepSeek-V3 Technical Report - arXiv.org DeepSeek-V3 Technical Report - arXiv.org deepseek-ai/DeepSeek-V3 · Hugging Face DeepSeek-V3 - Hugging Face GitHub - deepseek-ai/DeepSeek-V3 · GitHub</a></li>

</ul>
</details>

**Tags**: `#machine-learning`, `#jax`, `#open-source`, `#deep-learning`

---

<a id="item-tech-news-8"></a>
### [Project Zero to Shorten Vulnerability Disclosure Window](https://projectzero.google/2026/11/disclosure-policy.html) ⭐️ 7.0/10

Google Project Zero has announced a phased reduction in its vulnerability disclosure window: starting immediately, vulnerabilities will be disclosed 90 days after reporting to vendors, moving to 60 days on February 2, 2027, and then to 30 days on January 3, 2028. This policy applies to all vulnerabilities reported by Project Zero and is intended to accelerate the patching and public awareness of security issues. The change affects both open source and commercial software vendors, who will have less time to address reported vulnerabilities before public disclosure.

hackernews · hacb · Nov 14, 11:13 · [Discussion](https://news.ycombinator.com/item?id=50496051)

**「Background」** Since 2021, Google Project Zero has operated under a &quot;90 + 30&quot; vulnerability disclosure policy, giving vendors 90 days to fix reported vulnerabilities and an additional 30 days for patch rollout before public disclosure. This policy aimed to balance encouraging faster patching with allowing vendors sufficient time to protect users. The evolving threat landscape, particularly with AI-assisted vulnerability discovery and exploitation, has prompted Project Zero to reconsider these timelines.

**「Impact」** Software vendors will need to accelerate their vulnerability response and patch development processes to meet the shorter disclosure timelines, or risk having unpatched vulnerabilities publicly disclosed. Organizations relying on affected software may face increased exposure if vendors cannot meet the new deadlines.

**「Community Discussion」** Some commenters argue that immediate disclosure would be more effective in compelling vendors to fix vulnerabilities, while others express concern that certain projects, such as Ubuntu, may struggle to meet the shortened timelines. There is also discussion about whether companies discovering vulnerabilities should provide vendors with the same tools or access used in their research.

<details><summary>References</summary>
<ul>
<li><a href="https://projectzero.google/2026/11/disclosure-policy.html">Policy and Disclosure: 2026 Edition - Project Zero</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability-disclosure`, `#software-industry`, `#policy`

---

<a id="item-tech-news-9"></a>
### [TimeCues Studio: Free Open-Source Music Annotation Tool Released](https://www.reddit.com/r/MachineLearning/comments/1xwh3mw/acm_multimedia_2026_timecues_studio_a_free/) ⭐️ 7.0/10

TimeCues Studio is a newly released, free, open-source web application for annotating music structure on a beat-locked timeline. It supports collaborative annotation, algorithm comparison \(including built-in detectors like allin1 and MSAF\), and export to formats such as Audacity labels, MIDI, and JSON. The tool provides visualizations including separated stems, spectrograms, and color-coded waveforms, and is available under the MIT license. Users can run it locally with Docker Compose or try a demo version without registration.

reddit · r/MachineLearning · /u/SapirCa · Nov 14, 23:59

**「Background」** Music structure annotation is a key task in music information retrieval and machine learning, involving the labeling of sections, cues, and other features within audio tracks. Existing tools often lack integrated support for collaborative annotation, algorithm comparison, and export to multiple formats. TimeCues Studio was developed to address these needs, providing a web-based, open-source workspace where users can annotate music, evaluate detection algorithms, and prototype new methods within a unified environment.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.10338">[2609.10338] TimeCues Studio : A Workspace for Music Annotation ...</a></li>
<li><a href="https://github.com/sapirca/timecues-studio">GitHub - sapirca/ timecues - studio · GitHub</a></li>

</ul>
</details>

**Tags**: `#open source`, `#music information retrieval`, `#machine learning tools`, `#data annotation`

---

<a id="item-tech-news-10"></a>
### [Debate on Baselines for Short-Horizon Price Forecasting Papers](https://www.reddit.com/r/MachineLearning/comments/1xw6fk9/should_shorthorizon_price_forecasting_papers/) ⭐️ 7.0/10

A discussion post questions the common practice in short-horizon price forecasting research of benchmarking models only against naive baselines such as ARIMA or random walk. The author suggests that papers should also compare their models to market-implied forecasts, such as those derived from options-implied volatility or crowd-sourced prediction markets, which incorporate more public information. The post also critiques the focus on point forecast metrics like RMSE, arguing that interval coverage is more informative for assets like Bitcoin. No new research or policy change is announced; the post highlights a methodological gap in current evaluation standards.

reddit · r/MachineLearning · /u/happypeanut-t · Nov 14, 16:23

**「Background」** In financial forecasting, especially for assets like cryptocurrencies and commodities, researchers often use simple statistical models or naive approaches as baselines to evaluate new machine learning models. Market-implied forecasts, such as those inferred from options prices, reflect the collective expectations and information of market participants, potentially providing a more challenging and realistic benchmark.

**Tags**: `#machine learning`, `#finance`, `#forecasting`, `#research methodology`

---

<a id="item-tech-news-11"></a>
### [OpenAI Disbands Robotics Team, Shifts to General AI Models for Robots](https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/) ⭐️ 7.0/10

OpenAI has dissolved its dedicated robotics team and reassigned its researchers to broader AI research groups. The company stated that its latest general-purpose AI models, such as GPT-6 Astra, are now capable of directly controlling robots, eliminating the need for a specialized robotics team. OpenAI maintains that robotics remains central to its long-term vision and continues to develop humanoid robots internally, with a public demonstration targeted for 2027. This move follows the termination of OpenAI&\#x27;s partnership with Figure in February 2025 and marks a strategic shift toward leveraging advanced general AI for embodied tasks.

telegram · zaihuapd · Nov 14, 04:00

**「Background」** OpenAI previously maintained a dedicated robotics team focused on developing specialized AI for robotic control. According to recent reports, the company has now reassigned these researchers to broader AI research groups, citing advancements in general-purpose AI models that can directly operate robots. This shift follows earlier cycles of forming and dissolving robotics teams at OpenAI, as well as collaborations with external robotics firms.

<details><summary>References</summary>
<ul>
<li><a href="https://casrai.org/news/openai-disbands-robotics-team-2026">OpenAI Disbands Its Robotics Team: What It Means — CASRAI</a></li>
<li><a href="https://tech.yahoo.com/ai/articles/exclusive-openai-disbands-stand-alone-170530559.html">Exclusive: OpenAI disbands its stand-alone robotics team as ...</a></li>
<li><a href="https://fortune.com/2026/11/13/openai-disbands-robotics-team-as-its-general-models-start-running-robots/">Exclusive: OpenAI disbands stand-alone robotics team as ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#robotics`, `#AI models`, `#industry news`

---

<a id="item-tech-news-12"></a>
### [W5000 Unmanned Cargo Aircraft Completes Test Flight](https://www.ithome.com/1/027/068.htm) ⭐️ 7.0/10

The W5000, described as the world&\#x27;s largest unmanned cargo aircraft, has successfully completed a technical verification test flight in Inner Mongolia. The aircraft features a maximum takeoff weight of 10.8 tons, a payload capacity of 5 tons, and a range of 2,600 kilometers. It uses turboprop power and operates autonomously with ground-based monitoring, allowing one crew to supervise 6–7 aircraft simultaneously. The manufacturer expects to obtain airworthiness certification in the first half of 2027.

telegram · zaihuapd · Nov 14, 05:00

**「Background」** The W5000 is an unmanned cargo aircraft developed by Air White Whale \(Beijing\) Technology, designed as a twin-turboprop drone with a maximum takeoff weight of 10.8 tons and a payload capacity of 5 tons. It features an upper monoplane design, a rectangular fuselage, and a low horizontal tailplane, with an internal cargo space exceeding 65 cubic meters. The aircraft is intended to serve as an efficient, low-cost platform for air logistics, aiming to set new standards in unmanned cargo transport.

**「Impact」** Organizations in logistics and freight transport could benefit from the W5000&\#x27;s ability to autonomously deliver medium truck-sized loads over long distances, potentially reducing labor costs and increasing operational flexibility once certified.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chinadaily.com.cn/a/202410/22/WS6717074aa310f1265a1c8dd2.html">Firm unveils unmanned cargo drone - Chinadaily.com.cn</a></li>
<li><a href="https://interestingengineering.com/innovation/china-worlds-largest-cargo-drone">World’s largest cargo drone with 5-ton payload capacity unveiled</a></li>

</ul>
</details>

**Tags**: `#autonomous systems`, `#hardware`, `#aviation`, `#AI applications`

---

<a id="item-tech-news-13"></a>
### [Windows 11 Runs Natively on Foldable iPhone via Gemini and WindowsiOS](https://www.windowslatest.com/2026/11/14/windows-11-can-run-on-apples-foldable-iphone-and-googles-ai-boss-proved-it-using-gemini-years-after-microsoft-gave-up-on-windows-phones/) ⭐️ 7.0/10

Ammaar Reshi, Google AI Studio&\#x27;s product design lead, demonstrated Windows 11 24H2 running natively on Apple&\#x27;s foldable iPhone Duo using Gemini 4 Carbon and the open source WindowsiOS project. This setup does not require jailbreaking and uses JIT translation to run ARM64 code, with partial support for legacy Windows applications via Microsoft&\#x27;s Prism. The Windows 11 image is approximately 12 GB and requires an Apple Silicon Mac and development tools for installation. This demonstration was shared publicly through an operational video.

telegram · zaihuapd · Nov 14, 06:52

**「Background」** Running Windows on non-Microsoft hardware has long been a technical challenge, especially on Apple&\#x27;s iOS devices due to their locked-down environment and ARM architecture. The open source WindowsiOS project enables Windows 11 ARM64 to run at near-native speed on modern, non-jailbroken iOS devices by using just-in-time \(JIT\) code translation, without relying on Apple&\#x27;s Hypervisor.framework. This approach builds on recent advances in ARM64 compatibility and cross-platform virtualization, making it possible to run full Windows environments on devices like the foldable iPhone Duo.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ammaarreshi/WindowsiOS">GitHub - ammaarreshi/ WindowsiOS : Native Windows 11 ARM64 on...</a></li>

</ul>
</details>

**Tags**: `#cross-platform`, `#operating systems`, `#AI tools`, `#hardware`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Anthropic IPO Bars Mainland China and Hong Kong Investors](https://m.economictimes.com/markets/us-stocks/news/anthropic-ipo-share-orders-from-china-are-said-to-be-rebuffed/articleshow/135809948.cms) ⭐️ 8.0/10

Anthropic will not accept IPO share orders from investors in mainland China or Hong Kong, citing export control regulations, as it seeks to raise up to $90.4 billion at a $1.4 trillion valuation according to sources.

telegram · zaihuapd · Nov 14, 10:18

**「Background」** Anthropic is a U.S.-based artificial intelligence company, and its IPO is reportedly excluding investors from mainland China and Hong Kong due to U.S. export control regulations known as ITAR, which restrict certain technology-related investments from these regions.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/markets/stocks/articles/anthropic-ipo-reportedly-closed-china-174510000.html?fr=sycsrp_catchall">Anthropic IPO Reportedly Closed To China, Hong Kong Buyers ...</a></li>
<li><a href="https://the-decoder.com/banks-bar-chinese-and-hong-kong-investors-from-anthropic-ipo-over-us-export-controls/">Banks bar Chinese and Hong Kong investors from Anthropic IPO ...</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-13/anthropic-ipo-share-orders-from-china-are-said-to-be-rebuffed">Anthropic IPO Share Orders From China Are Said to Be Rebuffed</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#regulation`, `#technology`, `#capital markets`, `#geopolitics`

---

<a id="item-finance-news-2"></a>
### [Nvidia CEO Resignation and Congressional Shift Affect AI Stocks and ETFs](https://www.cnbc.com/2026/11/14/nvidia-ai-trade-data-centers-congress.html) ⭐️ 7.0/10

Nvidia&\#x27;s CEO Jensen Huang has resigned and ETF experts say a Democratic-controlled Congress could slow data center expansion, with Yorkville Ives estimating that 10% to 20% of planned data centers may not be built. Nvidia shares ended the week at $162.85, their longest losing streak since 2012, while AMD and Broadcom gained nearly 13% each.

rss · CNBC Finance · Nov 14, 15:50

**「Background」** Nvidia&\#x27;s founder and CEO Jensen Huang resigned on November 12, 2026, and the company&\#x27;s chief financial officer Colette Kress was appointed interim CEO, amid increased political attention on technology regulation and data centers in the U.S. Congress.

<details><summary>References</summary>
<ul>
<li><a href="https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Announces-CEO-Transition/">NVIDIA Corporation - NVIDIA Announces CEO Transition</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI`, `#ETFs`, `#Tech Regulation`, `#Market Reaction`

---