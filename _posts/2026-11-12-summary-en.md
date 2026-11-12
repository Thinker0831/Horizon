---
layout: default
title: "Horizon Summary: 2026-11-12 (EN)"
date: 2026-11-12
lang: en
---

> From 48 items, 21 important content pieces were selected

---

**Technology News**
1. [Nvidia Reportedly Preparing to Replace CEO Jensen Huang](#item-tech-news-1) ⭐️ 9.0/10
2. [AWS Releases Official Local Emulator for Cloud Services](#item-tech-news-2) ⭐️ 9.0/10
3. [Google Launches Gemini Decisions API for Multimodal Decision Tasks](#item-tech-news-3) ⭐️ 8.0/10
4. [AMD Uses AI to Swap Cold DRAM Pages to Flash, Claims 83% Server Cost Savings](#item-tech-news-4) ⭐️ 8.0/10
5. [Tim Peters, Author of &\#x27;The Zen of Python,&\#x27; Has Died](#item-tech-news-5) ⭐️ 7.0/10
6. [Guidance on Locking GitHub Actions Dependencies](#item-tech-news-6) ⭐️ 7.0/10
7. [Apple Researches Faster Retrieval for RAG Systems](#item-tech-news-7) ⭐️ 7.0/10
8. [AI Agents Used to Identify Previously Documented Maya Site](#item-tech-news-8) ⭐️ 7.0/10
9. [Emacs, AI Code, and Software Freedom Debated](#item-tech-news-9) ⭐️ 7.0/10
10. [United Airlines Bans AI Agents from Booking Flights](#item-tech-news-10) ⭐️ 7.0/10
11. [Anthropic Reveals Multi-Chip AI Strategy in IPO Roadshow](#item-tech-news-11) ⭐️ 7.0/10
12. [Explorer Indexes 2,100+ CoRL Robotics Papers with Summaries and Code Links](#item-tech-news-12) ⭐️ 7.0/10
13. [WorkflowArena: Strongest Model Not Always Best Coordinator](#item-tech-news-13) ⭐️ 7.0/10
14. [Microsoft Patents Distributed AI Training Using Idle Devices](#item-tech-news-14) ⭐️ 7.0/10
15. [ByteDance Plans Muse-like AI Agent, Targets OpenAI Parity by 2030](#item-tech-news-15) ⭐️ 7.0/10

**Financial News**
1. [Fed&\#x27;s Goolsbee calls inflation report &\#x27;borderline disturbing&\#x27; as central bank weighs more hikes](#item-finance-news-1) ⭐️ 8.0/10
2. [China Ends Offshore Trust Tax Transition, Reports Over 1600 Billion Yuan Declared](#item-finance-news-2) ⭐️ 8.0/10
3. [Report Alleges 240,000 Nvidia AI Chips Worth $7.5 Billion Illegally Imported to China](#item-finance-news-3) ⭐️ 8.0/10
4. [Senators Question Prediction Markets on Drug Trials](#item-finance-news-4) ⭐️ 7.0/10
5. [Alibaba Plans Hong Kong Listing for Chip Unit T-Head](#item-finance-news-5) ⭐️ 7.0/10
6. [Nvidia Board Reportedly Preparing to Remove CEO Jensen Huang](#item-finance-news-6) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Nvidia Reportedly Preparing to Replace CEO Jensen Huang](https://www.wsj.com/business/nvidia-is-preparing-to-oust-nvidia-ceo-jensen-huang-30f421ad) ⭐️ 9.0/10

Nvidia is reportedly preparing to replace its founder and CEO, Jensen Huang, according to a Wall Street Journal article. This would mark a significant leadership change at one of the most influential companies in AI and hardware. The report does not specify a timeline or a successor, and there is no confirmation from Nvidia at this time. The move, if confirmed, could have major implications for Nvidia&\#x27;s strategic direction and the broader technology sector.

hackernews · jbredeche · Nov 11, 22:31 · [Discussion](https://news.ycombinator.com/item?id=50459703)

**「Background」** Jensen Huang has served as Nvidia&\#x27;s CEO and co-founder for over 30 years, playing a central role in the company&\#x27;s rise as a leader in AI and hardware. Recent reports indicate that Huang is under investigation for personal conduct, specifically an alleged affair with an individual suspected of being a Chinese spy. This situation has led to increased scrutiny of Nvidia&\#x27;s leadership and raised questions about the company&\#x27;s future direction and governance.

**「Community Discussion」** Commenters note that Nvidia&\#x27;s leadership is seen as a critical asset for U.S. economic and national security interests, and that founder-led companies often have structures making such oustings rare. Some express concern about the loss of Huang&\#x27;s unique technical vision, while others speculate that a new CEO may prioritize financial performance over technological innovation. There is also discussion about the potential for Huang to remain influential within Nvidia even if he steps down as CEO.

<details><summary>References</summary>
<ul>
<li><a href="https://www.businessinsider.com/jensen-huang-resign-nvidia-ceo-future-debate-2026-11">Will Nvidia CEO Jensen Huang Resign? Leaders Weigh in ...</a></li>
<li><a href="https://techcrunch.com/2026/11/10/nvidia-ceo-jensen-huangs-affair-with-alleged-chinese-spy-a-timeline/">Nvidia CEO Jensen Huang&#x27;s affair with alleged Chinese spy: a ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/nov/09/jensen-huang-image-nvidia">Jensen Huang’s image has been shattered. Could he be pushed ...</a></li>

</ul>
</details>

**Tags**: `#leadership`, `#AI industry`, `#hardware`, `#technology business`

---

<a id="item-tech-news-2"></a>
### [AWS Releases Official Local Emulator for Cloud Services](https://simonwillison.net/2026/Nov/11/aws-emulator/) ⭐️ 9.0/10

AWS has released an official emulator, aws-emulator, allowing developers to locally test a wide range of AWS services without needing paid API keys. The emulator is written in Rust and currently requires Docker to run on macOS or Windows. This tool was developed with significant contributions from autonomous AI agents, as detailed in a guest post by Swaminathan Sivasubramanian. However, the emulator has notable limitations: it should not be used to test IAM policies, resource-based policies, KMS key policies, cross-account or cross-region access, or other security controls, as its policy evaluation does not fully match AWS&\#x27;s production environment.

rss · Simon Willison · Nov 11, 21:18

**「Background」** AWS Emulator is a newly released tool that allows developers to locally emulate over 200 AWS services using API models published by AWS. The emulator&\#x27;s codebase was generated and tested entirely by autonomous AI agents, marking a novel approach to large-scale software development. This tool is intended to provide a high-fidelity local testing environment that closely mirrors AWS service behavior, with updates synchronized to AWS API changes.

**「Impact」** Developers can now perform local integration testing of AWS services more easily and cost-effectively, but must avoid relying on the emulator for security-related testing due to its incomplete policy enforcement. Teams using macOS or Windows must also have Docker installed, and those seeking a standalone binary or broader platform support will need to wait for future updates.

**「Community Discussion」** Some users are skeptical about the emulator&\#x27;s long-term support and maintenance, comparing it to existing tools like Floci and Testcontainers, which already offer multi-cloud emulation. Others highlight the limitations around security testing and note the unprecedented scale of AI agent involvement in the project&\#x27;s development, expressing both surprise and concern about the use of Rust and agentic engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/about-aws/whats-new/2026/11/aws-emulator-now-available/">AWS Emulator is now available for building and testing AWS ...</a></li>
<li><a href="https://www.unite.ai/aws-releases-local-emulator-written-entirely-by-autonomous-ai-agents/">AWS Releases Local Emulator Written Entirely by Autonomous AI ...</a></li>
<li><a href="https://www.aboutamazon.com/news/aws/how-autonomous-ai-agents-built-aws-emulator">AWS Emulator: a local emulator built 100% by autonomous AI agents</a></li>

</ul>
</details>

**Tags**: `#cloud`, `#developer-tools`, `#aws`, `#emulation`, `#infrastructure`

---

<a id="item-tech-news-3"></a>
### [Google Launches Gemini Decisions API for Multimodal Decision Tasks](https://blog.google/innovation-and-ai/technology/developers-tools/gemini-decisions-api/) ⭐️ 8.0/10

Google has released the Gemini Decisions API, powered by the new Gemini Decision 1 model, which enables automated decision-making across text, images, audio, video, and PDF inputs. The API supports yes/no, choice, and rubric-scoring questions, returning probabilities and confidence scores for up to 1,000 questions per request, with an end-to-end latency of 150–250 ms. Pricing is $0.10 per million input tokens \(output tokens are free\), making it about five times cheaper than Gemini 3.5 Flash-Lite and comparable to OpenAI&\#x27;s GPT-6 Luna decision model, though Jev remains less expensive. The API is now available in Google AI Studio.

hackernews · iamdelirium · Nov 11, 18:32 · [Discussion](https://news.ycombinator.com/item?id=50456791)

**「Background」** Decision models like Jev and OpenAI&\#x27;s offerings have recently established a category of APIs that provide structured, probabilistic answers to specific types of questions, such as yes/no, multiple choice, and rubric scoring. Jev, for example, is text-only and introduced the &\#x27;Noul&\#x27; term for yes/no queries, while OpenAI&\#x27;s model added image support. Google&\#x27;s Gemini Decisions API builds on this trend by introducing full multimodal support, allowing inputs from text, images, audio, video, and PDFs, and is based on the new Gemini Decision 1 model.

**「Impact」** Developers can now integrate multimodal decision-making into their applications at a lower cost, especially for use cases requiring analysis of audio and video, which competing models like Jev and OpenAI&\#x27;s decision models do not fully support. This broadens the range of automated evaluation and routing tasks that can be handled programmatically.

**「Community Discussion」** Commenters note that while Gemini Decisions is more expensive than some alternatives, its ability to process audio and video inputs is a significant advantage for certain applications. There is also discussion about the practical uses of decision models and curiosity about how these models calculate probabilities, with some expressing optimism based on positive experiences with related models.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Nov/11/gemini-decisions-api/">Gemini Decisions API - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#AI APIs`, `#multimodal AI`, `#decision models`, `#software engineering`

---

<a id="item-tech-news-4"></a>
### [AMD Uses AI to Swap Cold DRAM Pages to Flash, Claims 83% Server Cost Savings](https://www.theregister.com/systems/2026/11/11/amd-where-were-going-we-dont-need-as-much-dram/5308953) ⭐️ 8.0/10

AMD has integrated AI-driven memory management, based on its acquired Mext technology, into its server offerings. This software uses AI models to proactively swap cold memory pages from DRAM to less expensive NVMe flash storage before the operating system or applications detect the need. AMD claims that replacing half of the DRAM with flash can retain up to 99% of server performance and potentially reduce enterprise server costs by as much as 83%. The solution requires purchasing a Mext license alongside AMD Epyc servers.

telegram · zaihuapd · Nov 11, 11:15

**「Background」** Traditional server architectures rely heavily on DRAM for memory, which is fast but expensive and volatile. AMD&\#x27;s MEXT technology, originally founded in 2022, uses AI-based page prediction to extend server memory by swapping less frequently used \(&\#x27;cold&\#x27;\) memory pages from DRAM to lower-cost NVMe flash storage. This approach aims to reduce reliance on DRAM by making flash storage behave more like main memory, with AI algorithms managing which pages are kept in DRAM for performance and which are offloaded to flash to optimize cost and capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guru3d.com/story/amd-mext-uses-flash-to-expand-server-memory-capacity/">AMD MEXT Uses Flash to Expand Server Memory Capacity</a></li>
<li><a href="https://www.amd.com/en/products/software/mext.html">AMD MEXT Predictive Memory Software</a></li>
<li><a href="https://wccftech.com/amd-mext-memory-solution-flash-repaces-dram-same-performance/">AMD Unveils MEXT Memory Solution: Leverages Flash To Mitigate...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#AI systems`, `#server architecture`, `#memory management`

---

<a id="item-tech-news-5"></a>
### [Tim Peters, Author of &\#x27;The Zen of Python,&\#x27; Has Died](https://discuss.python.org/t/in-memoriam-tim-peters-1952-2026/110028) ⭐️ 7.0/10

Tim Peters, a foundational contributor to the Python programming language and author of &\#x27;The Zen of Python,&\#x27; has died. Peters was also known for his work on the SpamBayes project and contributions to the Python Cookbook. His influence shaped Python&\#x27;s design philosophy and community culture. The news was shared on Python community forums and widely acknowledged by developers.

hackernews · ayhanfuat · Nov 11, 07:03 · [Discussion](https://news.ycombinator.com/item?id=50450488)

**「Background」** Tim Peters was a highly influential software engineer in the Python community, best known for authoring &\#x27;The Zen of Python,&\#x27; a set of guiding principles for Python&\#x27;s design and philosophy, first posted in 1999. He contributed significantly to Python&\#x27;s core development, including technical work on modules such as timsort, doctest, and timeit, and played a key role in shaping Python&\#x27;s usability and culture. Peters also contributed to the Python Cookbook and was instrumental in projects like SpamBayes.

**「Impact」** Python users and developers are reflecting on Peters&\#x27; legacy, particularly his articulation of Python&\#x27;s guiding principles, which continue to influence code style and community discussions. His passing is prompting tributes and remembrances across the programming community.

**「Community Discussion」** Commenters highlighted Peters&\#x27; role in shaping Python&\#x27;s philosophy and his technical contributions, such as SpamBayes and the Python Cookbook. Many shared personal anecdotes about his generosity, humor, and impact on their understanding of programming.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zen_of_Python">Zen of Python - Wikipedia</a></li>
<li><a href="https://discuss.python.org/t/in-memoriam-tim-peters-1952-2026/110028">In Memoriam: Tim Peters 1952–2026 - Core Development...</a></li>
<li><a href="https://lunduke.locals.com/post/5985667/python-bans-prominent-dev-for-enjoying-the-wrong-old-snl-sketch">Python Bans Prominent Dev for Enjoying the Wrong Old SNL Sketch</a></li>

</ul>
</details>

**Tags**: `#python`, `#community`, `#software-engineering`, `#history`

---

<a id="item-tech-news-6"></a>
### [Guidance on Locking GitHub Actions Dependencies](https://hugovk.dev/blog/2026/lock-github-actions/) ⭐️ 7.0/10

A new guide outlines how to securely lock dependencies in GitHub Actions workflows to reduce supply chain risks. The article explains that while lockfiles can pin normal action calls, they do not automatically cover reusable workflows or composite actions, which require manual intervention. Community discussion highlights additional security pitfalls in GitHub Actions defaults, such as broad permissions and lack of timeouts, and notes that trust in commit hashes is not a complete safeguard. The guidance is aimed at developers and DevOps practitioners managing CI/CD pipelines on GitHub.

hackernews · gslin · Nov 11, 22:16 · [Discussion](https://news.ycombinator.com/item?id=50459485)

**「Background」** GitHub Actions is a popular CI/CD platform that automates software workflows using third-party and custom actions. To address supply chain security risks, GitHub introduced workflow dependency lockfiles, which pin each action used in a workflow to a specific commit hash, ensuring that only reviewed code is executed. This mechanism helps prevent unauthorized or malicious changes in dependencies from affecting workflow runs.

**「Community Discussion」** Commenters note that current lockfile solutions only partially address the problem, as reusable workflows and composite actions are not fully covered. Others point out broader security issues with GitHub Actions, such as default permissions and the risk of running compromised actions, and suggest that platform-level improvements are needed for comprehensive protection.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.github.com/en/actions/concepts/security/workflow-dependency-lockfiles">Workflow dependency lockfiles - GitHub Docs</a></li>

</ul>
</details>

**Tags**: `#security`, `#devops`, `#github-actions`, `#supply-chain`

---

<a id="item-tech-news-7"></a>
### [Apple Researches Faster Retrieval for RAG Systems](https://machinelearning.apple.com/research/faster-retrieval) ⭐️ 7.0/10

Apple has published research on more efficient retrieval methods for Retrieval-Augmented Generation \(RAG\) systems, focusing on improving scalability and performance for large-scale AI applications. The work explores learned retrieval techniques, which use machine learning models to select relevant information more quickly and accurately than traditional methods. This research is particularly relevant for organizations handling massive datasets, where retrieval speed and quality directly impact the effectiveness of AI-generated outputs.

hackernews · zerop · Nov 11, 16:57 · [Discussion](https://news.ycombinator.com/item?id=50455633)

**「Background」** Retrieval-Augmented Generation \(RAG\) is a technique that enhances large language models by allowing them to retrieve and incorporate information from external data sources, improving the accuracy and reliability of generated outputs. This approach is particularly valuable for AI applications that require up-to-date or domain-specific knowledge beyond the model&\#x27;s training data. Apple&\#x27;s research focuses on making this retrieval process faster and more efficient, which is crucial for scaling RAG systems to handle large datasets and real-time demands.

**「Community Discussion」** Practitioners debated the trade-offs between learned retrieval systems and traditional approaches like grep, with some arguing that current embedding models may not outperform simple heuristics for certain tasks. Others noted that learned retrieval methods are most beneficial at hyperscale, while concerns were raised about potential biases and quality trade-offs introduced by retrieval mechanisms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval - augmented generation - Wikipedia</a></li>
<li><a href="https://blogs.nvidia.com/blog/what-is-retrieval-augmented-generation/">What Is Retrieval - Augmented Generation aka RAG | NVIDIA Blogs</a></li>

</ul>
</details>

**Tags**: `#retrieval-augmented-generation`, `#machine-learning`, `#ai-systems`, `#scalability`

---

<a id="item-tech-news-8"></a>
### [AI Agents Used to Identify Previously Documented Maya Site](https://pietromiotti.com/latest/maya-site) ⭐️ 7.0/10

AI agents were employed to analyze remote sensing data and identified a Maya archaeological site that was believed to be unmapped. However, subsequent updates from the author and community members revealed that the site had already been documented in a 2025 academic paper. This case highlights both the potential and the current limitations of using AI for archaeological discovery, particularly the importance of expert validation and thorough literature review.

hackernews · eyvindn · Nov 11, 12:05 · [Discussion](https://news.ycombinator.com/item?id=50452455)

**「Background」** The use of lidar \(Light Detection and Ranging\) data has become a powerful tool in archaeology, enabling researchers to identify ancient structures hidden beneath dense vegetation. In this case, independent researcher Pietro Miotti deployed 48 AI agents across multiple platforms to analyze 1,200 km² of NASA lidar data from the Maya jungle. While the AI agents flagged a significant Classic-period Maya site, it was later clarified that the site had already been documented in a 2025 academic paper, though it was not listed in Mexico&\#x27;s official INAH register.

**「Impact」** Researchers and AI practitioners are reminded that while AI can accelerate the identification of potential archaeological sites, expert review and cross-referencing with existing records remain essential to avoid redundant claims and ensure scientific accuracy.

**「Community Discussion」** Commenters noted that the site had been previously found and documented, questioning the novelty of the AI discovery. Others emphasized the need for archaeological verification and cautioned against overhyping AI findings without expert confirmation.

<details><summary>References</summary>
<ul>
<li><a href="https://emergent.sh/news/48-ai-agents-rediscover-mapped-maya-site-nasa">48 AI Agents Rediscover Mapped Maya Site from NASA Lidar</a></li>
<li><a href="https://www.winzheng.com/en/article/ai-agents-maya-lidar-discovery-72-hours">48 AI Agents Flag a Maya Site in 72 Hours—but Miss a Key Paper</a></li>

</ul>
</details>

**Tags**: `#AI applications`, `#remote sensing`, `#archaeology`, `#machine learning`

---

<a id="item-tech-news-9"></a>
### [Emacs, AI Code, and Software Freedom Debated](https://commandlinesystems.com/magic.txt) ⭐️ 7.0/10

A reflective analysis discusses the implications of AI-generated code contributions on open source projects like Emacs, focusing on concerns about software freedom, code provenance, and the evolving role of traditional development tools. The article highlights debates within the Emacs community about whether to accept or reject code written by large language models \(LLMs\), and how this may affect the project&\#x27;s alignment with GNU policies. No new technical features or releases are announced; the discussion centers on ethical and philosophical challenges posed by AI in software development.

hackernews · ggcr · Nov 11, 20:26 · [Discussion](https://news.ycombinator.com/item?id=50458208)

**「Background」** Emacs is a long-standing open source text editor maintained by the GNU Project. Recently, concerns have arisen within the Emacs community about the use of code generated by large language models \(LLMs\), leading to the formation of the Human Emacs initiative, which opposes LLM-generated contributions on ethical and legal grounds. This follows GNU Emacs&\#x27;s temporary ban on LLM-generated code, implemented to address legal uncertainties regarding copyright and code provenance.

**「Impact」** Developers and maintainers of Emacs and similar open source projects may face decisions about whether to accept AI-generated code, potentially leading to forks or alternative versions that explicitly exclude LLM contributions. This could affect project governance, contributor guidelines, and the definition of software freedom within these communities.

**「Community Discussion」** Some community members advocate for maintaining an LLM-free version of Emacs regardless of official GNU policy, citing concerns about code provenance and software freedom. Others argue that AI-generated code changes the nature of development and may render traditional tools less relevant, while some stress the need for modularity and clear boundaries to manage maintainability in the age of AI-assisted coding.

<details><summary>References</summary>
<ul>
<li><a href="https://freenode.net/article/emacs-group-vows-fork-if-project-accepts-llm-generated-code">Emacs group vows fork if project accepts LLM-generated code</a></li>
<li><a href="https://emergent.sh/news/human-emacs-fork-proposal-bans-all-llm">Human Emacs Fork Proposal Bans All LLM Contributions</a></li>
<li><a href="https://lists.gnu.org/archive/html/emacs-devel/2026-10/msg00508.html">Human Emacs - lists.gnu.org</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI ethics`, `#software engineering`, `#developer tools`

---

<a id="item-tech-news-10"></a>
### [United Airlines Bans AI Agents from Booking Flights](https://www.cbsnews.com/news/united-airlines-bans-ai-agents-booking-flights/) ⭐️ 7.0/10

United Airlines has implemented a policy that prohibits AI agents from booking flights on behalf of travelers. This ban targets automated tools and services that act as intermediaries between customers and the airline&\#x27;s booking system. The policy is intended to restrict the use of automation in the flight booking process, though the technical means of enforcement and specific exceptions, if any, are not detailed in the available information.

hackernews · herpderperator · Nov 11, 21:24 · [Discussion](https://news.ycombinator.com/item?id=50458900)

**「Background」** United Airlines&\#x27; decision to ban AI agents from booking flights is based on concerns about customer privacy, unauthorized transactions, and compliance with federal aviation regulations. The airline cited security risks associated with allowing artificial intelligence agents to make reservations on behalf of travelers. This move comes as AI-powered personal agents have become increasingly capable of automating online tasks, including purchasing airline tickets.

**「Impact」** Travelers and developers who rely on AI-powered booking assistants will need to revert to manual booking or use approved third-party agencies, as automated agents may now be blocked or result in canceled reservations. This could complicate workflows for users who have integrated AI tools into their travel planning.

**「Community Discussion」** Commenters questioned the practicality of enforcing the ban, noting that users could disguise AI agent activity as normal browser traffic. Some argued that flight booking is already streamlined and that users prefer direct control over such transactions, while others speculated that airlines aim to prevent certain customers from gaining an advantage through automation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbsnews.com/news/united-airlines-bans-ai-agents-booking-flights/">United Airlines bans AI agents from booking flights on behalf ...</a></li>
<li><a href="https://www.newsmax.com/newsfront/united-airlines-ai-agents-booking-flights/2026/11/11/id/1275977/">United Airlines Bans AI Agents From Booking Flights</a></li>
<li><a href="https://www.usatoday.com/story/travel/airline-news/2026/11/11/united-ai-travel-agents-booking/92728156007/">United Airlines bans personal AI agents from booking flights</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#automation`, `#consumer technology`, `#industry policy`

---

<a id="item-tech-news-11"></a>
### [Anthropic Reveals Multi-Chip AI Strategy in IPO Roadshow](https://simonwillison.net/2026/Nov/11/anthropic-ipo-roadshow/) ⭐️ 7.0/10

Anthropic&\#x27;s IPO roadshow video discloses that the company now trains and serves its Claude AI models across AWS Trainium, Google TPUs, NVIDIA GPUs, and AMD GPUs. This multi-chip approach, previously considered unconventional, is enabled by Anthropic&\#x27;s investment in tailored software and inference stacks for each hardware platform. Notably, the company claims that its Mythos system enabled Claude to run on AMD GPUs in just three days with minimal human intervention. The video also highlights Anthropic&\#x27;s focus on discovering &\#x27;compute multipliers&\#x27;—techniques that increase effective compute capacity—and suggests that future recursive self-improvement could accelerate these gains.

rss · Simon Willison · Nov 11, 15:11

**「Background」** Anthropic is an AI company known for developing the Claude language model. Their IPO roadshow video, released as part of their initial public offering process, disclosed for the first time that Claude is trained and served across four major chip families: AWS Trainium, Google TPUs, NVIDIA GPUs, and AMD GPUs. This multi-chip strategy, described by co-founder Tom Brown as unconventional, allows Anthropic to onboard new hardware platforms much faster than before, leveraging internal tools like Mythos to automate much of the adaptation process.

<details><summary>References</summary>
<ul>
<li><a href="https://todayforai.com/en/items/art-5672236b-42d">Anthropic IPO Roadshow Reveals Four-Chip Training Strategy</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#IPO`, `#industry news`, `#hardware`

---

<a id="item-tech-news-12"></a>
### [Explorer Indexes 2,100+ CoRL Robotics Papers with Summaries and Code Links](https://www.reddit.com/r/MachineLearning/comments/1xtul3j/i_built_an_explorer_of_2100_robotics_papers/) ⭐️ 7.0/10

A new open-source tool has been released that indexes over 2,100 robotics papers from the past 10 years of the Conference on Robot Learning \(CoRL\), covering 2017–2026. The explorer provides TLDR summaries, links to code repositories, project pages, arXiv entries, task tags, summary statistics, and research trend visualizations. The resource is designed to improve accessibility and discovery of robotics research for the community, and contributions are encouraged via GitHub. The tool is available at https://corl.operatic.ai/explore.

reddit · r/MachineLearning · /u/promptdom · Nov 11, 21:42

**「Background」** The Conference on Robot Learning \(CoRL\) is an annual international event that brings together researchers from robotics and machine learning to discuss advances at their intersection. CoRL has become a key venue for presenting research on learning-based approaches in robotics, with proceedings and papers published each year since its inception in 2017.

<details><summary>References</summary>
<ul>
<li><a href="https://www.corl.org/contributions">CoRL 2026 - Contributions</a></li>
<li><a href="https://www.corl2023.org/">CoRL 2023</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#research tools`, `#open source`, `#machine learning`

---

<a id="item-tech-news-13"></a>
### [WorkflowArena: Strongest Model Not Always Best Coordinator](https://www.reddit.com/r/MachineLearning/comments/1xt9hbe/would_you_pick_your_strongest_model_to_coordinate/) ⭐️ 7.0/10

Experimental results from the new WorkflowArena benchmark show that the highest-performing model is not always the most effective coordinator in multi-agent workflows. In tests with Opus 5.5 and GPT-6 Astra, Opus&\#x27;s workflows improved the performance of four executor models, while Astra&\#x27;s workflows actually reduced their scores, despite Astra being the stronger model in solo benchmarks. WorkflowArena evaluates coordination across 145 tasks in eight domains, focusing on how well a coordinator&\#x27;s workflow helps other models complete tasks. This challenges the common assumption that the strongest model should always lead in multi-agent setups.

reddit · r/MachineLearning · /u/OliviaYii · Nov 11, 05:25

**「Background」** WorkflowArena is a recently introduced benchmark designed to evaluate how language models coordinate multi-agent workflows on 145 long-horizon tasks across eight professional domains. Unlike previous benchmarks that use fixed coordination protocols or assign tasks independently, WorkflowArena allows models to design their own division of labor and workflow structure. This setup enables researchers to assess not just individual model performance, but also how effectively a model can orchestrate and delegate tasks among other agents.

<details><summary>References</summary>
<ul>
<li><a href="https://lab.einsia.ai/workflowarena/home.html">WorkflowArena · Executable Workflow Orchestration</a></li>
<li><a href="https://arxiv.org/pdf/2611.12856">WorkflowArena: Benchmarking Executable Workflow Orchestration ...</a></li>

</ul>
</details>

**Tags**: `#multi-agent systems`, `#coordination`, `#benchmarks`, `#machine learning`

---

<a id="item-tech-news-14"></a>
### [Microsoft Patents Distributed AI Training Using Idle Devices](https://www.techspot.com/news/114499-microsoft-patent-describes-paying-you-train-ai-idle.html) ⭐️ 7.0/10

Microsoft has filed a patent for a system that monitors user devices for idle resources and assigns them AI training tasks when underutilized. Participants would be compensated with cash, app store credits, or early access to AI models, depending on their contribution. The patent describes monitoring CPU, GPU, memory, temperature, and power usage to determine device suitability, and splitting training tasks accordingly. It is not yet clear if or when this system will be implemented.

telegram · zaihuapd · Nov 11, 04:45

**「Background」** Distributed computing projects, such as SETI@home and Folding@home, have previously used idle computing resources from volunteers&\#x27; devices to process scientific workloads. Microsoft&\#x27;s patent extends this concept to AI training, proposing a system that monitors device resource usage and allocates AI training tasks during periods of low activity. The patent suggests compensation for participants, which could include cash, credits, or early access to AI models, and envisions using a range of devices including servers, desktops, and smartphones.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techspot.com/news/114499-microsoft-patent-describes-paying-you-train-ai-idle.html">Microsoft patent describes paying you to train AI on your ...</a></li>
<li><a href="https://cryptobriefing.com/microsoft-patent-idle-computing-power-ai/">Microsoft patent filing describes paying users for idle ...</a></li>
<li><a href="https://tbreak.com/microsoft-idle-gpu-patent-ai-training/">Microsoft idle GPU patent pays PC owners to train AI</a></li>

</ul>
</details>

**Tags**: `#distributed-computing`, `#AI-infrastructure`, `#patents`, `#industry-trends`

---

<a id="item-tech-news-15"></a>
### [ByteDance Plans Muse-like AI Agent, Targets OpenAI Parity by 2030](https://www.bloomberg.com/news/articles/2026-11-11/bytedance-prepares-muse-like-agent-in-push-to-close-ai-gap) ⭐️ 7.0/10

ByteDance has announced plans to launch an AI assistant similar to Meta&\#x27;s Muse in the coming weeks, aiming to strengthen its position in AI video technology. The company intends to invest up to $70 billion in its Seedance video AI platform and has set a goal to reach parity with leading AI labs such as OpenAI and Anthropic by 2029 or 2030. The initiative, outlined by co-founder Zhang Yiming, explicitly avoids reliance on model distillation. This announcement is a forward-looking strategy and does not include the release of any immediate technical breakthroughs or products.

telegram · zaihuapd · Nov 11, 12:31

**「Background」** Meta&\#x27;s Muse is an artificial intelligence agent announced in September 2026, designed to perform long-running tasks for users rather than just responding to single queries like traditional chatbots. Muse can be integrated into devices such as AI glasses, allowing users to delegate tasks hands-free and interact with their environment through the agent. ByteDance&\#x27;s planned AI assistant is described as &\#x27;Muse-like,&\#x27; indicating a focus on persistent, proactive AI capabilities similar to those introduced by Meta.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_%28AI_agent%29">Muse (AI agent) - Wikipedia</a></li>
<li><a href="https://www.meta.com/help/ai-glasses/1391796469223757/">How to use Muse on your AI glasses (Beta) | AI Glasses Help ...</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#strategic investment`, `#AI assistants`, `#video AI`

---

## Financial News

<a id="item-finance-news-1"></a>
### [Fed&\#x27;s Goolsbee calls inflation report &\#x27;borderline disturbing&\#x27; as central bank weighs more hikes](https://www.cnbc.com/2026/11/11/goolsbee-october-inflation-fed-rates-disturbing-distressing.html) ⭐️ 8.0/10

Fed officials signal heightened concern over persistent inflation after a higher-than-expected CPI report, raising the odds of further and possibly larger interest rate hikes.

rss · CNBC Finance · Nov 11, 16:49

**Tags**: `#Federal Reserve`, `#inflation`, `#interest rates`, `#monetary policy`, `#economic data`

---

<a id="item-finance-news-2"></a>
### [China Ends Offshore Trust Tax Transition, Reports Over 1600 Billion Yuan Declared](https://www.news.cn/20261111/9bcce99c779b4a6197ff45bbbc3e4c50/c.html) ⭐️ 8.0/10

China&\#x27;s 90-day transition period for taxing offshore trust income has ended, with over 1600 billion yuan in personal income tax declared and a nearly 90% year-on-year increase in national personal income tax revenue for October, according to the State Taxation Administration.

telegram · zaihuapd · Nov 11, 10:35

**「Background」** In July 2026, China introduced new rules requiring resident individuals to pay individual income tax on gains from transferring property into offshore trusts, with a 90-day transition period for compliance before penalties would apply.

**「Impact」** High-net-worth individuals with offshore trusts face stricter enforcement and potential penalties if they fail to comply with the new tax rules.

<details><summary>References</summary>
<ul>
<li><a href="https://www.morganlewis.com/pubs/2026/07/china-establishes-new-individual-income-tax-rules-for-offshore-trusts">China Establishes New Individual Income Tax Rules for ...</a></li>

</ul>
</details>

**Tags**: `#tax policy`, `#offshore trusts`, `#China`, `#personal income tax`, `#regulation`

---

<a id="item-finance-news-3"></a>
### [Report Alleges 240,000 Nvidia AI Chips Worth $7.5 Billion Illegally Imported to China](https://www.tomshardware.com/tech-industry/policy/alice-huang-reportedly-instrumental-in-securing-over-usd7-5-billion-of-nvidia-ai-gpu-imports-during-three-year-relationship-with-jensen-huang-helped-move-240-000-banned-chips-into-china-mostly-h100-and-h200) ⭐️ 8.0/10

A report from The Information alleges Alice Huang helped facilitate the import of about 240,000 restricted Nvidia AI chips, valued at $7.5 billion, into China despite export controls.

telegram · zaihuapd · Nov 11, 14:41

**「Background」** U.S. export controls restrict the sale of advanced Nvidia AI chips to China, and recent reports allege that Alice Huang used a network of companies in China and Singapore, including Shanghai Century Litong and Megaspeed, to help import these restricted chips despite the ban.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theinformation.com/articles/jensen-huangs-yearslong-ties-alice-huang-enabled-nvidia-chip-sales-china">How Jensen Huang’s Yearslong Ties to Alice Huang Enabled $7 ...</a></li>
<li><a href="https://www.theinformation.com/briefings/nvidia-ceo-reportedly-targeted-suspected-chinese-informant">Nvidia CEO Reportedly Targeted By Suspected Chinese Informant</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#export controls`, `#Nvidia`, `#China`, `#trade policy`

---

<a id="item-finance-news-4"></a>
### [Senators Question Prediction Markets on Drug Trials](https://www.cnbc.com/2026/11/11/kalsi-polymarket-prediction-market-senators-hhs-drug-approval.html) ⭐️ 7.0/10

Two U.S. senators have asked the Department of Health and Human Services what steps it is taking to address risks from prediction markets tied to clinical trials and drug approvals, signaling possible regulatory scrutiny but no immediate policy change.

rss · CNBC Finance · Nov 11, 19:16

**「Background」** Prediction market platforms like Kalshi and Polymarket began allowing bets on the outcomes of clinical drug trials and FDA regulatory decisions in mid-2026, raising concerns among some researchers and policymakers about potential ethical and insider trading risks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/07/28/business/kalshi-polymarket-prediction-market-drugs.html">Prediction Market Betting on Drug Trials and Approvals Sparks ...</a></li>
<li><a href="https://www.npr.org/2026/08/07/nx-s1-5922530/patients-betting-kalshi-polymarket-clinical-trials">Kalshi, Polymarket offer bets on clinical trials and FDA ...</a></li>
<li><a href="https://www.reuters.com/legal/litigation/kalshi-allow-bets-clinical-trials-fda-decisions-2026-07-16/">Kalshi to allow bets on clinical trials, FDA decisions</a></li>

</ul>
</details>

**Tags**: `#regulation`, `#prediction markets`, `#healthcare policy`, `#biotechnology`, `#insider trading`

---

<a id="item-finance-news-5"></a>
### [Alibaba Plans Hong Kong Listing for Chip Unit T-Head](https://www.cnbc.com/2026/11/11/alibaba-pr.html) ⭐️ 7.0/10

Alibaba announced plans to spin off and publicly list its semiconductor subsidiary T-Head on the Hong Kong Stock Exchange, pending regulatory approval; the company did not disclose the expected date or size of the offering.

rss · CNBC Finance · Nov 11, 07:47

**「Background」** T-Head is Alibaba&\#x27;s semiconductor design unit that mainly develops chips for use within Alibaba&\#x27;s own cloud computing services, rather than selling them widely to other companies. Alibaba has recently increased investment in T-Head as part of a broader push to strengthen China&\#x27;s domestic chip industry amid global supply concerns and technology restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/tech/big-tech/article/3358032/alibaba-chip-unit-t-head-triples-capital-amid-ai-hardware-bet">Alibaba chip unit T-Head triples capital amid AI hardware bet</a></li>
<li><a href="https://chips.techbuzzchina.com/companies/alibaba-t-head">Alibaba T-Head | China Chip Stack</a></li>

</ul>
</details>

**Tags**: `#Alibaba`, `#semiconductors`, `#IPO`, `#China tech`, `#regulation`

---

<a id="item-finance-news-6"></a>
### [Nvidia Board Reportedly Preparing to Remove CEO Jensen Huang](https://www.wsj.com/business/nvidia-is-preparing-to-oust-nvidia-ceo-jensen-huang-30f421ad?mod=tech_lead_pos2) ⭐️ 7.0/10

Nvidia&\#x27;s board is reportedly preparing to remove CEO Jensen Huang following allegations of personal scandals, with the company&\#x27;s stock falling about 8% after hours according to the report. Nvidia has not officially responded to these claims.

telegram · zaihuapd · Nov 11, 23:39

**「Background」** Nvidia&\#x27;s board began an independent investigation after CEO Jensen Huang admitted to extramarital affairs, including one with a person suspected of ties to Chinese intelligence and another with a company executive.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wsj.com/business/nvidia-is-preparing-to-oust-nvidia-ceo-jensen-huang-30f421ad">Exclusive | Nvidia Is Preparing to Oust CEO Jensen Huang</a></li>
<li><a href="https://www.wsj.com/cfo-journal/jensen-huang-investigation-rocks-nvidia-as-board-investigates-a0581595">Jensen Huang Investigation Rocks Nvidia as Board Investigates</a></li>
<li><a href="https://www.reuters.com/world/china/view-nvidia-is-preparing-oust-ceo-jensen-huang-wsj-reports-2026-11-11/">VIEW Nvidia is preparing to oust CEO Jensen Huang, WSJ ...</a></li>

</ul>
</details>

**Tags**: `#corporate governance`, `#executive changes`, `#technology`, `#stock movement`

---