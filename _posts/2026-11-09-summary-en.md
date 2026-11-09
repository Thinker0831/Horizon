---
layout: default
title: "Horizon Summary: 2026-11-09 (EN)"
date: 2026-11-09
lang: en
---

> From 32 items, 9 important content pieces were selected

---

**Technology News**
1. [KetchUp: Open-Source Rust/WebGPU 3D Modeler in Browser](#item-tech-news-1) ⭐️ 7.0/10
2. [Goldman Sachs Restricts Claude Code Use for Bankers and Traders](#item-tech-news-2) ⭐️ 7.0/10
3. [Llama-modchip Runs 284B DeepSeek Model on 64GB RAM, No GPU](#item-tech-news-3) ⭐️ 7.0/10
4. [Outlook.com Now Silently Rejects Email Without DMARC](#item-tech-news-4) ⭐️ 7.0/10
5. [Drex Max v1.1 Multimodal Decision Model Released with Open Weights](#item-tech-news-5) ⭐️ 7.0/10
6. [GRFNet: Open Source PyTorch Model for Multichannel Time-Series Classification](#item-tech-news-6) ⭐️ 7.0/10
7. [US Lawmaker Calls for Ban on AI Recursive Self-Improvement](#item-tech-news-7) ⭐️ 7.0/10
8. [Chinese AI Models Dominate Global Open-Source Enterprise Spending](#item-tech-news-8) ⭐️ 7.0/10

**Financial News**
1. [NVIDIA Board Investigates CEO Jensen Huang After Infidelity Admission](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [KetchUp: Open-Source Rust/WebGPU 3D Modeler in Browser](https://ketchup3d.github.io/app/) ⭐️ 7.0/10

KetchUp is a new open-source 3D modeling tool built with Rust and WebGPU, designed as a browser-based alternative to SketchUp. It aims to provide a performant, cross-platform modeling experience directly in the browser, leveraging modern technologies for both usability and extensibility. The project is accessible online and targets users seeking a free, open-source solution for 3D modeling tasks.

hackernews · dcoulmbe · Nov 8, 22:35 · [Discussion](https://news.ycombinator.com/item?id=50418176)

**「Background」** SketchUp is a widely used proprietary 3D modeling tool known for its accessibility and ease of use, especially among hobbyists and designers. Rust is a modern systems programming language valued for safety and performance, while WebGPU is a new web standard enabling high-performance graphics and computation in browsers. Combining Rust and WebGPU allows developers to build complex, performant browser-based applications, including 3D modeling tools, that can run cross-platform without native installation.

**「Impact」** Users and hobbyists who require simple 3D modeling tools, especially for tasks like 3D printing, now have a free, browser-based alternative to proprietary software like SketchUp. Developers interested in Rust and WebGPU can also study or contribute to a real-world application of these technologies.

**「Community Discussion」** Commenters praised the application&\#x27;s smooth Rust-based UI and browser performance, with some suggesting improvements such as curated example files and better default behaviors. Several users noted the tool&\#x27;s potential for customization and its appeal to those frustrated by the learning curve of existing 3D modeling software.

<details><summary>References</summary>
<ul>
<li><a href="https://pooya.ai/webgpu/">Rust WebGPU Examples &amp; Tutorials | wgpu &amp; WGSL</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#3d-modeling`, `#rust`, `#webgpu`, `#software-tools`

---

<a id="item-tech-news-2"></a>
### [Goldman Sachs Restricts Claude Code Use for Bankers and Traders](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

Goldman Sachs is withdrawing access to Claude Code, an AI coding agent, for its bankers and traders due to concerns over security, regulatory compliance, and operational costs. The restriction specifically targets finance staff whose workstations handle sensitive client, trading, and proprietary information. This move highlights the challenges of deploying AI tools in highly regulated and sensitive environments, where risks of data leakage and compliance violations are significant. The decision reflects both internal risk management priorities and broader industry hesitancy around enterprise AI adoption in critical sectors.

hackernews · TheWiggles · Nov 8, 18:16 · [Discussion](https://news.ycombinator.com/item?id=50415628)

**「Background」** Goldman Sachs had previously allowed traders, bankers, and other non-engineering staff to use AI coding tools like Anthropic&\#x27;s Claude Code and GitHub Copilot to assist with tasks such as monitoring customer flows, building trading models, and generating content reports. According to recent reports, the bank has now restricted access to these tools, limiting their use to software engineers after an internal evaluation of productivity and risk management. This marks a reversal of an earlier policy that permitted broader experimentation with AI assistants among finance professionals.

**「Impact」** Affected Goldman Sachs employees will lose access to Claude Code, potentially limiting their ability to automate coding tasks and requiring stricter adherence to manual processes for compliance and security. Organizations in similar sectors may reevaluate or restrict AI tool deployments, especially where sensitive data and regulatory obligations are involved.

**「Community Discussion」** Commenters note that running AI coding agents on primary finance workstations poses unacceptable risks of data leakage and compliance breaches. Others report similar restrictions in their organizations due to unpredictable billing and cost overruns, with some switching to alternatives like Gemini for more predictable pricing. There is also concern that AI-driven errors in regulated documentation could have severe legal consequences.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gate.com/news/detail/GS/goldman-sachs-restricts-claude-code-access-in-october-traders-can-no-longer-25394829">Goldman Sachs restricts Claude Code access in October ...</a></li>
<li><a href="https://www.siliconreport.com/goldman-sachs-cuts-off-most-staff-from-claude-code-and-github">Goldman Sachs cuts off most staff from Claude Code and GitHub</a></li>
<li><a href="https://explainx.ai/blog/goldman-sachs-restricts-traders-bankers-ai-coding-tools-claude-code-engineers-only-2026">Goldman Sachs Restricts AI Coding Tools: What We Know ...</a></li>

</ul>
</details>

**Tags**: `#AI adoption`, `#enterprise security`, `#finance industry`, `#regulatory compliance`

---

<a id="item-tech-news-3"></a>
### [Llama-modchip Runs 284B DeepSeek Model on 64GB RAM, No GPU](https://github.com/synchopate/llama-modchip) ⭐️ 7.0/10

The Llama-modchip project enables local inference of the 284B parameter DeepSeek language model on a machine with 64GB RAM and no GPU. This is achieved through aggressive model quantization, allowing such a large model to run on commodity hardware. The project is open source and has sparked technical discussion about quantization strategies and hardware trade-offs. Some users report that while the setup works, performance and quality depend heavily on quantization level and available RAM.

hackernews · joshcsimmons · Nov 8, 10:22 · [Discussion](https://news.ycombinator.com/item?id=50411961)

**「Background」** Running large language models \(LLMs\) like DeepSeek-V4-Flash with 284 billion parameters has traditionally required high-end hardware, especially powerful GPUs and large amounts of RAM. Llama-modchip is an open-source project that enables local inference of such massive models on systems with only 64GB of RAM and no GPU by using aggressive quantization techniques and CPU-based computation. This approach significantly lowers the hardware barrier for experimenting with and deploying large LLMs locally.

**「Impact」** Developers and researchers can now experiment with extremely large language models locally without requiring expensive GPUs, provided they have sufficient RAM and are willing to accept the trade-offs of aggressive quantization. This lowers the barrier to entry for running state-of-the-art models and may accelerate experimentation and accessibility in the AI community.

**「Community Discussion」** Commenters highlight that quantization is the key enabler but warn that reducing precision below 4-bit can cause significant performance and quality loss, especially for non-LLM modalities. Some users question the practical benefits over existing tools like llama.cpp, while others note that increasing RAM further improves speed, and that the documentation could better clarify quantization details.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/synchopate/llama-modchip">GitHub - synchopate/llama-modchip: Run 284B DeepSeek-V4 ...</a></li>
<li><a href="https://www.promptzone.com/mei_bui/llama-modchip-run-284b-deepseek-on-64gb-ram-no-gpu-required-3plk">Llama-modchip: Run 284B DeepSeek on 64GB RAM, No GPU Required</a></li>

</ul>
</details>

**Tags**: `#large language models`, `#model quantization`, `#local inference`, `#hardware requirements`, `#open source`

---

<a id="item-tech-news-4"></a>
### [Outlook.com Now Silently Rejects Email Without DMARC](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Outlook.com has implemented a policy to silently reject incoming email from domains that do not have a DMARC \(Domain-based Message Authentication, Reporting, and Conformance\) record. This change affects all senders attempting to deliver mail to Outlook.com users from domains lacking DMARC, regardless of other authentication mechanisms. The rejection is not accompanied by a bounce or notification, making it difficult for senders to detect delivery failures. This policy shift was not publicly announced and has been observed by administrators managing email infrastructure.

hackernews · xmddmx · Nov 8, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50416158)

**「Background」** DMARC \(Domain-based Message Authentication, Reporting, and Conformance\) is an email authentication protocol designed to help prevent email spoofing by allowing domain owners to specify how unauthenticated messages should be handled. Previously, Outlook.com accepted emails from domains without DMARC, but now it blocks such messages, enforcing stricter authentication requirements. This change builds on existing industry efforts to improve email security and reduce spam and phishing attacks.

**「Impact」** Email administrators and organizations without DMARC records will experience silent delivery failures when sending to Outlook.com, potentially leading to lost or delayed communications without clear error messages. To restore deliverability, affected domains must implement DMARC, and administrators should monitor outbound mail logs for undelivered messages.

**「Community Discussion」** Some administrators support the stricter DMARC enforcement as a positive security measure, while others criticize Outlook.com for silently discarding messages and using opaque blocklists, making troubleshooting difficult. Several commenters report longstanding frustration with Outlook.com&\#x27;s lack of transparency and inconsistent mail acceptance, even for properly configured domains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.factae.eu/en/article/outlook-com-quietly-rejects-emails-from-domains-without-dmarc-182744">Outlook . com quietly rejects emails from domains without DMARC</a></li>

</ul>
</details>

**Tags**: `#email`, `#security`, `#infrastructure`, `#policy`

---

<a id="item-tech-news-5"></a>
### [Drex Max v1.1 Multimodal Decision Model Released with Open Weights](https://www.reddit.com/r/MachineLearning/comments/1xr4hkm/artificial_analysis_multimodal_decision_model/) ⭐️ 7.0/10

Drex Max v1.1, an open-source multimodal decision model, has been released and claims to achieve state-of-the-art \(SOTA\) performance and Pareto frontier status for decision models. The model features a large context window of approximately 256,000 tokens, supports local inference \(including on Mac via the Kapitsa inference engine\), and is reported to be eight times cheaper than the next best model in its category according to the aa index. Open weights for v1 are available under the Open RAIL-M license, with v1.1 weights to follow, and a detailed training playbook is provided in an accompanying paper. These claims are based on a Reddit announcement with links to supporting resources, but independent verification and technical details remain limited.

reddit · r/MachineLearning · /u/m4rkGS · Nov 8, 17:54

**「Background」** Drex Max is a multimodal decision model developed by Nace.AI, designed to process and answer questions based on text, JSON, and images. The model is a dense 27-billion-parameter architecture with a 255-way readout head, and it is released under the Nace.AI Open RAIL-M license. Drex Max is intended for use in agents that interact with computers and browsers, and it supports local inference on various platforms, including Mac, with open weights and documentation available for reproducibility.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/nace-ai/drex-max-v1">nace-ai/drex-max-v1 · Hugging Face</a></li>
<li><a href="https://github.com/nace-ai/drex-decision-models/tree/main/models/drex-max-v1">drex-decision-models/models/drex-max-v1 at main · nace-ai ...</a></li>
<li><a href="https://www.nace.ai/drex">Drex Max, the decision model that sees | Nace.AI</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#open source`, `#decision models`, `#model release`

---

<a id="item-tech-news-6"></a>
### [GRFNet: Open Source PyTorch Model for Multichannel Time-Series Classification](https://www.reddit.com/r/MachineLearning/comments/1xqqj67/grfnet_pytorch_model_for_multichannel_timeseries/) ⭐️ 7.0/10

GRFNet is a newly released open source PyTorch model designed for multichannel time-series classification, with a particular focus on EEG and similar biosignal data. The architecture builds on the ROCKET approach by combining random, untrained convolutional kernels with learned spatial filters and sensor position-based initialization. The model is adaptable to any input length and sampling rate, and the default configuration supports 22 channels and 4 classes with 3,847 parameters. Benchmarking and subject-independent evaluation on the PhysioNet EEGMMIDB dataset are planned, but no comparative results are available yet.

reddit · r/MachineLearning · /u/joekrry · Nov 8, 05:13

**「Background」** Multichannel time-series classification, especially for biosignals like EEG, is challenging due to small datasets, high subject variability, and differences in signal acquisition. Existing approaches such as ROCKET use random convolutional kernels to extract features from time-series data, while models like EEGNet and ShallowConvNet are established baselines for EEG classification tasks. PyTorch is a widely used deep learning framework that supports flexible model development for such applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.youtube.com/watch?v=LyJtbe__2i0">PyTorch 101 Crash Course For Beginners in 2026 - YouTube</a></li>
<li><a href="https://www.udemy.com/course/pytorch-deep-learning/">PyTorch : Deep Learning and Artificial Intelligence</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#open source`, `#time-series`, `#PyTorch`

---

<a id="item-tech-news-7"></a>
### [US Lawmaker Calls for Ban on AI Recursive Self-Improvement](https://x.com/AlexBores/status/2118494668769878037) ⭐️ 7.0/10

U.S. Democratic Representative Alex Bores has publicly urged Congress to pass legislation this year banning recursive self-improvement \(RSI\) in artificial intelligence. RSI refers to AI systems that autonomously design and build more advanced versions of themselves. Bores cited forecasts from OpenAI and Anthropic, which predict significant automation of AI research and development by 2027–2028, and referenced a METR report as evidence that such advances are plausible and imminent. He argued that unchecked RSI could amplify existing AI errors or alignment issues across generations, increasing systemic risks.

telegram · zaihuapd · Nov 8, 01:30

**「Background」** Recursive self-improvement \(RSI\) in AI refers to systems that can autonomously enhance their own capabilities, potentially leading to rapid and unpredictable advances. Policymakers and experts have debated whether to regulate or ban RSI due to concerns about safety, alignment, and loss of human oversight. Recent discussions in U.S. policy circles and media have highlighted proposals to ban or restrict RSI as AI systems approach the ability to independently improve themselves without human intervention.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/10/26/magazine/ai-companies-law-regulations.html">What Should the Rules for A . I . Companies Actually Be?</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#AI safety`, `#regulation`, `#recursive self-improvement`

---

<a id="item-tech-news-8"></a>
### [Chinese AI Models Dominate Global Open-Source Enterprise Spending](http://z.ai/) ⭐️ 7.0/10

A new report from Menlo Ventures finds that Chinese AI models account for 89% of global enterprise spending on open-source models. Within this segment, Moonshot AI&\#x27;s Kimi leads with a 61% share, followed by DeepSeek at 15% and Z.ai&\#x27;s GLM series at 11%, while Meta&\#x27;s Llama holds 7%. However, open-source models represent only 4% of total enterprise model spending, with Anthropic and OpenAI together capturing 86% of the broader market via API-based offerings. The data is based on a September survey of nearly 400 U.S. enterprise decision-makers.

telegram · zaihuapd · Nov 8, 03:26

**「Background」** Enterprise adoption of AI models has rapidly increased, with spending shifting toward both frontier and open-source models in recent years. According to Menlo Ventures, from Q3 2025 to Q3 2026, the share of enterprise AI spending on frontier models rose significantly, reflecting a broader trend of organizations exploring alternatives to established closed-source providers. This context helps explain the significance of Chinese open-source models capturing a dominant share of global enterprise open-source model spending.

<details><summary>References</summary>
<ul>
<li><a href="https://menlovc.com/perspective/2026-the-state-of-enterprise-ai/">2026: The State of Enterprise AI | Menlo Ventures</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#open source`, `#enterprise adoption`, `#market analysis`

---

## Financial News

<a id="item-finance-news-1"></a>
### [NVIDIA Board Investigates CEO Jensen Huang After Infidelity Admission](https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity) ⭐️ 7.0/10

NVIDIA&\#x27;s board has launched an independent investigation, with external legal counsel, into whether CEO Jensen Huang was targeted by foreign intelligence operations after he admitted to infidelity and apologized to staff. Huang will remain CEO and cooperate fully with the probe until its results are released.

telegram · zaihuapd · Nov 8, 21:39

**「Background」** Nvidia&\#x27;s board began this investigation after reports suggested CEO Jensen Huang may have been targeted by foreign intelligence, following his public admission of infidelity and apology to staff and family.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity">Nvidia Board to Probe Spying Case After CEO Jensen Huang ...</a></li>
<li><a href="https://www.ft.com/content/1397e2f4-d7f5-4cbb-a4d9-04ecf661d1aa?syn-25a6b1a6=1">Nvidia’s Jensen Huang admits to affair after allegations of ...</a></li>
<li><a href="https://www.bbc.com/news/articles/c3dxw10rjn9no">Nvidia launches investigation into CEO&#x27;s affair with ... - BBC</a></li>

</ul>
</details>

**Tags**: `#corporate governance`, `#national security`, `#NVIDIA`, `#leadership`

---