---
layout: default
title: "Horizon Summary: 2026-11-09 (EN)"
date: 2026-11-09
lang: en
---

> From 33 items, 11 important content pieces were selected

---

**Technology News**
1. [Drex Max v1.1 Multimodal Decision Model Released with Open Weights](#item-tech-news-1) ⭐️ 8.0/10
2. [KetchUp: Open-Source SketchUp Alternative in Rust/WebGPU](#item-tech-news-2) ⭐️ 7.0/10
3. [Llama-modchip Runs 284B DeepSeek LLM on 64GB RAM, No GPU](#item-tech-news-3) ⭐️ 7.0/10
4. [Shift from Claude to Pi Harnesses for LLM Interfaces](#item-tech-news-4) ⭐️ 7.0/10
5. [Goldman Sachs Restricts Claude Code for Bankers and Traders](#item-tech-news-5) ⭐️ 7.0/10
6. [Outlook.com Now Rejects Email from Domains Without DMARC](#item-tech-news-6) ⭐️ 7.0/10
7. [GRFNet: Open Source PyTorch Model for Multichannel Time-Series Classification](#item-tech-news-7) ⭐️ 7.0/10
8. [Playable Diffusion World Model and Agent Harness for Pokémon Red](#item-tech-news-8) ⭐️ 7.0/10
9. [Chinese Models Dominate Global Open-Source AI Enterprise Spending](#item-tech-news-9) ⭐️ 7.0/10
10. [Anthropic Report: Scientists Use Claude Mainly for Data Analysis and Writing](#item-tech-news-10) ⭐️ 7.0/10

**Financial News**
1. [NVIDIA Board Launches Independent Probe After CEO Jensen Huang Admits Infidelity](#item-finance-news-1) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Drex Max v1.1 Multimodal Decision Model Released with Open Weights](https://www.reddit.com/r/MachineLearning/comments/1xr4hkm/artificial_analysis_multimodal_decision_model/) ⭐️ 8.0/10

Drex Max v1.1, a multimodal decision model from Nace, has been released with claims of achieving state-of-the-art \(SOTA\) performance and reaching the Pareto frontier for decision models. The model offers open weights \(with v1.1 weights to follow\), a full training playbook, and supports local inference, including on Mac devices via the Kapitsa inference engine. Drex Max features a large context window of approximately 256,000 tokens, surpassing models like Glide1.2 \(64k\) and Mammoth \(16k\), and is reported to be eight times cheaper than the next best model in its category according to the aa index. The model is released under the Open RAIL-M license, with documentation and previous versions available on Hugging Face.

reddit · r/MachineLearning · /u/m4rkGS · Nov 8, 17:54

**「Background」** Drex Max is a multimodal decision model developed by Nace.AI, designed to answer typed questions about a given context using text, JSON, and images. It is the successor to Drex v2.0 and supports large context windows, with self-reported benchmark results published by Nace.AI. The model is available with open weights and supports local inference, making it accessible for a wide range of AI practitioners.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/11/01/nace-ai-open-sources-drex-max-v1-local-inference/">Nace AI Open-Sources Drex Max v 1 : A 27B Decision Model That...</a></li>
<li><a href="https://openrouter.ai/nace-ai/drex-max">Drex Max - API Pricing &amp; Providers | OpenRouter</a></li>
<li><a href="https://huggingface.co/nace-ai/drex-max-v1">nace-ai/ drex - max - v 1 · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#AI models`, `#open source`, `#multimodal`

---

<a id="item-tech-news-2"></a>
### [KetchUp: Open-Source SketchUp Alternative in Rust/WebGPU](https://ketchup3d.github.io/app/) ⭐️ 7.0/10

KetchUp is a newly released open-source 3D modeling tool designed as a modern alternative to SketchUp. It is built using Rust and WebGPU, enabling browser-based 3D modeling with a focus on performance and cross-platform compatibility. The project aims to fill the gap left by SketchUp&\#x27;s move away from free and open development, offering a free tool for hobbyists and professionals alike. KetchUp is accessible via its web app and is positioned to appeal to users seeking a lightweight, modern, and open 3D modeling solution.

hackernews · dcoulmbe · Nov 8, 22:35 · [Discussion](https://news.ycombinator.com/item?id=50418176)

**「Background」** SketchUp is a widely used 3D modeling tool that was originally free but has become less accessible over time, prompting demand for open-source alternatives. KetchUp is built using Rust, a modern systems programming language, and WebGPU, a web standard for high-performance graphics. The Rust library &\#x27;wgpu&\#x27; provides a safe, cross-platform implementation of the WebGPU API, enabling advanced graphics capabilities directly in the browser.

**「Impact」** Users who previously relied on SketchUp, especially those frustrated by its reduced free offerings and lack of updates, now have a viable open-source alternative that runs in the browser. Developers interested in Rust and WebGPU can also study KetchUp as a reference for building performant, cross-platform graphical applications.

**「Community Discussion」** Several users expressed enthusiasm for KetchUp as a spiritual successor to SketchUp, lamenting SketchUp&\#x27;s decline in openness and usability. Others praised the technical achievement of delivering a responsive Rust-based UI in the browser, though some noted minor usability quirks, such as being prompted to name objects too frequently.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/gfx-rs/wgpu">GitHub - gfx-rs/wgpu: A cross-platform, safe, pure- Rust graphics API.</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#3d-modeling`, `#rust`, `#webgpu`, `#software-tools`

---

<a id="item-tech-news-3"></a>
### [Llama-modchip Runs 284B DeepSeek LLM on 64GB RAM, No GPU](https://github.com/synchopate/llama-modchip) ⭐️ 7.0/10

Llama-modchip is an open-source project that enables local inference of the 284-billion parameter DeepSeek large language model \(LLM\) on a CPU with just 64GB of RAM and no GPU. This is achieved through advanced model quantization techniques, making it possible to run extremely large models on relatively modest hardware. The project is available on GitHub and targets users interested in running state-of-the-art LLMs without access to high-end GPUs. However, practical performance and quality may vary depending on quantization settings and hardware specifics.

hackernews · joshcsimmons · Nov 8, 10:22 · [Discussion](https://news.ycombinator.com/item?id=50411961)

**「Background」** Llama-modchip is an open-source project that allows users to run the 284B parameter DeepSeek-V4-Flash large language model locally on a CPU with as little as 64GB of RAM and no GPU. This is achieved through advanced model quantization, custom compression, and memory tiling techniques, enabling inference of extremely large models on commodity hardware. Previous approaches to running such large models typically required much more memory and powerful GPUs, making local inference inaccessible to most users.

**「Impact」** Developers and AI practitioners can now experiment with very large LLMs like DeepSeek locally, even on workstations without powerful GPUs, potentially lowering the barrier to entry for advanced AI research and applications. Users should be aware that aggressive quantization may impact model quality and performance, and optimal results may require more RAM or careful tuning.

**「Community Discussion」** Commenters note that while the ability to run large models locally is impressive, quantization trade-offs can significantly affect output quality, especially below 4-bit precision. Some users report that performance is comparable to existing tools like llama.cpp, with prefill speeds being notably faster, but practical usability depends on hardware and quantization choices.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/synchopate/llama-modchip">GitHub - synchopate/llama-modchip: Run 284B DeepSeek-V4 ...</a></li>
<li><a href="https://www.inferwire.com/en/posts/llama-modchip-runs-284b-deepseek-model-on-64gb-ram-cpus">Llama-modchip Runs 284B DeepSeek Model on 64GB RAM CPUs</a></li>
<li><a href="https://braindetox.kr/en/posts/llama_modchip_deepseek_284b_cpu_64gb.html">llama-modchip 284B: DeepSeek-V4-Flash on 64GB RAM, No GPU</a></li>

</ul>
</details>

**Tags**: `#large language models`, `#model quantization`, `#AI infrastructure`, `#open source`

---

<a id="item-tech-news-4"></a>
### [Shift from Claude to Pi Harnesses for LLM Interfaces](https://caleb.software/posts/claude-to-pi.html) ⭐️ 7.0/10

Advanced users are increasingly migrating from mainstream large language model \(LLM\) interfaces like Claude and ChatGPT to alternative harnesses such as Pi. This shift is driven by the need for more flexible, customizable, and efficient workflows, especially for software engineering and AI development tasks. The discussion highlights technical trade-offs, including API compatibility, interface design, and the risks associated with using third-party wrappers for proprietary models. Users report both improved productivity and new complexities in managing AI toolchains.

hackernews · karagenit · Nov 8, 03:11 · [Discussion](https://news.ycombinator.com/item?id=50410107)

**「Background」** Agent harnesses are software frameworks that provide interfaces and orchestration for interacting with large language models \(LLMs\), often enabling local or customized workflows. In 2026, open-source harnesses such as Pi, OpenCode, and others have gained popularity among developers seeking more control and flexibility compared to mainstream LLM interfaces like Claude or ChatGPT. These harnesses can facilitate local LLM deployment, integration with developer tools, and advanced automation, but may introduce compatibility and support considerations when used with proprietary models.

**「Impact」** Developers adopting alternative harnesses like Pi may gain greater workflow flexibility and integration options, but face potential issues with model compatibility, API stability, and possible violations of terms of service when using proprietary models in non-native environments.

**「Community Discussion」** Commenters note that while Pi offers significant flexibility and integration benefits, using it with proprietary models like Anthropic&\#x27;s can risk bans and unpredictable behavior due to undocumented API features. Others highlight that much of the efficiency and complexity now lies in the harness itself, and that open-weight models combined with Pi provide a satisfying, customizable experience.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/09/18/best-open-source-agent-harnesses-for-local-llms-in-2026/">Best Open-Source Agent Harnesses for Local LLMs in 2026</a></li>

</ul>
</details>

**Tags**: `#large-language-models`, `#developer-tools`, `#ai-interfaces`, `#software-engineering`

---

<a id="item-tech-news-5"></a>
### [Goldman Sachs Restricts Claude Code for Bankers and Traders](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

Goldman Sachs is withdrawing access to Claude Code, an AI coding agent, from its bankers and traders due to concerns over security, regulatory compliance, and cost management. The decision highlights the challenges of deploying generative AI tools in highly regulated financial environments, where sensitive data and strict oversight are paramount. The move reportedly stems from risks related to data privacy, potential information leaks, and unpredictable billing associated with usage-based pricing models.

hackernews · TheWiggles · Nov 8, 18:16 · [Discussion](https://news.ycombinator.com/item?id=50415628)

**「Background」** Goldman Sachs had previously allowed traders and bankers to use AI coding tools such as Anthropic&\#x27;s Claude Code and GitHub Copilot to assist with tasks like building market models and monitoring client flows. In October 2026, the company updated its internal guidelines to restrict access to these tools, limiting their use primarily to engineers. This change followed a period of experimentation and was motivated by concerns over security, compliance, and operational risks associated with running AI agents on machines that handle sensitive financial data.

**「Impact」** Affected Goldman Sachs employees will lose access to Claude Code, potentially limiting their ability to leverage AI-assisted coding and automation in daily workflows. Organizations in similar sectors may reevaluate or restrict AI tool deployments, especially where compliance and cost predictability are critical.

**「Community Discussion」** Commenters note that running AI agents on machines with access to sensitive financial data poses unacceptable security and compliance risks. Others report similar restrictions at their organizations due to unpredictable billing, with some switching to alternatives offering flat-rate pricing and stricter access controls.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gate.com/news/detail/GS/goldman-sachs-restricts-claude-code-access-in-october-traders-can-no-longer-25394829">Goldman Sachs restricts Claude Code access in October ...</a></li>
<li><a href="https://aigovernance.com/news/goldmans-claude-code-ban-exposes-ai-coding-tool-governance-gap">Goldman&#x27;s Claude Code Ban Exposes AI Coding Tool Governance…</a></li>
<li><a href="https://explainx.ai/blog/goldman-sachs-restricts-traders-bankers-ai-coding-tools-claude-code-engineers-only-2026">Goldman Sachs Restricts AI Coding Tools: What We Know ...</a></li>

</ul>
</details>

**Tags**: `#enterprise-ai`, `#security`, `#finance`, `#regulation`, `#llm`

---

<a id="item-tech-news-6"></a>
### [Outlook.com Now Rejects Email from Domains Without DMARC](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Outlook.com has begun rejecting incoming emails from domains that do not have a DMARC \(Domain-based Message Authentication, Reporting, and Conformance\) policy in place. This change affects any sender whose domain lacks DMARC, regardless of other authentication measures like SPF or DKIM. The enforcement appears to be active now, with affected senders receiving permanent delivery failures \(5xx errors\). The policy shift was not widely announced, leading to unexpected deliverability issues for some users.

hackernews · xmddmx · Nov 8, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50416158)

**「Background」** DMARC \(Domain-based Message Authentication, Reporting, and Conformance\) is an email authentication protocol that helps prevent email spoofing by allowing domain owners to specify how unauthenticated messages should be handled. Prior to this change, many major email providers accepted messages from domains without DMARC records, though some encouraged its adoption for improved security. Outlook.com and related Microsoft email services began rejecting emails from domains lacking DMARC records starting November 5, 2026, affecting both large and small senders.

**「Impact」** Email administrators, self-hosters, and organizations without DMARC configured on their domains will see their messages to Outlook.com users rejected outright. To restore deliverability, affected senders must implement a valid DMARC policy on their domains.

**「Community Discussion」** Some administrators support the move, arguing that DMARC should already be standard practice, while others express frustration at the lack of transparency and the broader challenges of delivering mail to Outlook.com. Several users note that Outlook.com has a history of quietly dropping or blocking emails for reasons unrelated to DMARC, making troubleshooting difficult.

<details><summary>References</summary>
<ul>
<li><a href="https://mailroute.net/blog/outlook-rejecting-email-without-dmarc">Outlook.com Is Quietly Rejecting Email From Domains Without DMARC</a></li>
<li><a href="https://tosend.com/articles/outlook-rejects-email-without-dmarc/">Outlook.com now rejects email from domains without DMARC</a></li>
<li><a href="https://news.lavx.hu/article/outlook-com-rejects-some-email-from-domains-without-dmarc-records">Outlook.com Rejects Some Email From Domains Without DMARC ...</a></li>

</ul>
</details>

**Tags**: `#email-security`, `#infrastructure`, `#policy-change`, `#software-engineering`

---

<a id="item-tech-news-7"></a>
### [GRFNet: Open Source PyTorch Model for Multichannel Time-Series Classification](https://www.reddit.com/r/MachineLearning/comments/1xqqj67/grfnet_pytorch_model_for_multichannel_timeseries/) ⭐️ 7.0/10

GRFNet is a newly released open source PyTorch model designed for multichannel time-series classification, with a focus on EEG and similar biomedical data. The architecture combines random, untrained convolutional kernels \(inspired by ROCKET\) with learned spatial filters that can be initialized using sensor positions, and a mix of random and learnable dilated convolutions. The model is lightweight \(3,847 parameters for a 22-channel, 4-class setup\), accepts variable input lengths and sampling rates, and is being evaluated on the PhysioNet EEGMMIDB dataset. Benchmarking against EEGNet and ShallowConvNet is planned, but no comparative results are available yet.

reddit · r/MachineLearning · /u/joekrry · Nov 8, 05:13

**「Background」** Multichannel time-series classification, such as EEG signal analysis, often faces challenges due to small dataset sizes and high variability between subjects. The ROCKET architecture, which uses random convolutional kernels for feature extraction, has been influential in this domain. GRFNet builds on ROCKET by introducing learnable spatial filters and a hybrid of random and learnable convolutions, aiming to better adapt to the unique characteristics of EEG data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kongchang.com/en/articles/grfnet-a-lightweight-pytorch-model-designed-for-multichannel-time-series-classification">GRFNet: A Lightweight PyTorch Model Designed for Multichannel ...</a></li>

</ul>
</details>

**Tags**: `#time-series`, `#deep learning`, `#open source`, `#PyTorch`, `#EEG`

---

<a id="item-tech-news-8"></a>
### [Playable Diffusion World Model and Agent Harness for Pokémon Red](https://www.reddit.com/r/MachineLearning/comments/1xqt0pk/i_trained_a_playable_diffusion_world_model_of/) ⭐️ 7.0/10

A diffusion-based world model of Pokémon Red has been trained to generate game frames based on the last four screens and a button press, using a 16.7M parameter DIAMOND-style EDM U-Net. This model is paired with a System 1/2 agent harness, inspired by Krafton&\#x27;s PUBG Ally, where System 2 \(planner\) uses game RAM and external lookups to set goals, and System 1 \(executor\) consists of small policies trained entirely within the world model. The system can play through the first gym badge in the real game with high reliability, though battle sequences remain scripted due to model limitations. Additional upscaler and colorizer networks enhance the visual output, and the entire project was trained in 50 GPU-hours on a single RTX 4090.

reddit · r/MachineLearning · /u/priyanshu123sah · Nov 8, 07:48

**「Background」** Diffusion models are a class of generative neural networks originally popularized for image synthesis, now being adapted for sequential data such as video game frames. The System 1/2 agent split, inspired by cognitive science, separates fast, reactive behaviors \(System 1\) from slower, deliberative planning \(System 2\). Krafton&\#x27;s PUBG Ally, referenced here, is an AI system for PUBG that uses a similar architecture to enable co-playable AI agents, blending rapid execution with higher-level goal planning.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ajupress.com/view/20260616153131697">Krafton unveils &#x27; PUBG Ally &#x27; AI mode in two -week beta | Aju Press</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#world models`, `#diffusion models`, `#game AI`, `#agent architectures`

---

<a id="item-tech-news-9"></a>
### [Chinese Models Dominate Global Open-Source AI Enterprise Spending](http://z.ai/) ⭐️ 7.0/10

A new report from Menlo Ventures finds that Chinese AI models account for 89% of global enterprise spending on open-source models. Within this segment, Moonshot AI&\#x27;s Kimi leads with a 61% share, followed by DeepSeek at 15% and Z.ai&\#x27;s GLM series at 11%, while Meta&\#x27;s Llama holds only 7%. However, open-source models represent just 4% of total enterprise AI model spending, with Anthropic and OpenAI together capturing 86% of the overall market via API-based offerings. The data is based on a September survey of nearly 400 U.S. enterprise decision-makers.

telegram · zaihuapd · Nov 8, 03:26

**「Background」** Open-source AI models are alternatives to proprietary models, allowing enterprises to deploy and customize AI solutions without relying on closed platforms. Menlo Ventures, a venture capital firm focused on technology sectors, has tracked the rapid growth of enterprise AI spending, which surged from $33 billion to $177 billion in a single year. Their recent reports analyze how enterprises allocate budgets between open-source and proprietary AI models, providing context for the current market share figures.

**「Impact」** Enterprises relying on open-source AI models are overwhelmingly choosing Chinese-developed options, but the vast majority of enterprise AI spending still goes to proprietary API-based models from Anthropic and OpenAI. Organizations considering open-source adoption should note the limited overall market share and the dominance of a few Chinese providers in this space.

<details><summary>References</summary>
<ul>
<li><a href="https://menlovc.com/">Menlo Ventures | Early-Stage Venture Capital Firm</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#open source`, `#enterprise adoption`, `#market analysis`

---

<a id="item-tech-news-10"></a>
### [Anthropic Report: Scientists Use Claude Mainly for Data Analysis and Writing](https://www.anthropic.com/research/how-researchers-use-claude) ⭐️ 7.0/10

Anthropic has released a report analyzing 207,000 scientific conversations with its Claude AI model from August to September 2026. The report finds that data analysis accounts for 33.7% of Claude usage and 48.1% of Claude Code usage, while writing tasks make up 32% of Claude usage. Formal sciences such as computer science and mathematics show higher per-capita usage compared to experimental sciences like chemistry and medicine. The report estimates that widespread adoption of current AI capabilities could double research output in some fields, and if AI were to handle all non-physical tasks, output in fields like computer science could increase up to 15-fold.

telegram · zaihuapd · Nov 9, 01:29

**「Background」** Anthropic is an AI company that develops Claude, a large language model used for various tasks including writing, data analysis, and coding. AI companies like Anthropic and OpenAI periodically release usage reports to illustrate how their models are adopted in real-world scenarios, though these reports typically present selected data. Claude is accessible as an AI assistant for researchers and professionals, supporting tasks such as data analysis and scientific writing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.technologyreview.com/2026/08/18/1142226/how-people-use-ai/480/">We still don’t know how people are really using AI</a></li>
<li><a href="https://claude.ai/">Sign in or create an account | Claude .ai</a></li>

</ul>
</details>

**Tags**: `#AI applications`, `#research productivity`, `#data analysis`, `#scientific writing`

---

## Financial News

<a id="item-finance-news-1"></a>
### [NVIDIA Board Launches Independent Probe After CEO Jensen Huang Admits Infidelity](https://www.bloomberg.com/news/articles/2026-11-08/nvidia-board-to-probe-spying-case-after-ceo-jensen-huang-admits-infidelity) ⭐️ 7.0/10

NVIDIA&\#x27;s board has started an independent investigation, with external legal counsel, into whether CEO Jensen Huang was targeted by foreign intelligence operations after he admitted to infidelity and apologized to his family and staff. Huang will remain CEO during the investigation and has pledged full cooperation.

telegram · zaihuapd · Nov 8, 21:39

**「Background」** NVIDIA&\#x27;s board began an independent investigation after CEO Jensen Huang admitted to an affair and reports surfaced alleging the woman involved may be linked to foreign intelligence, specifically concerns about a possible Chinese spy connection.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/08/nvidia-jensen-huang-investigation-china-spy.html">Nvidia investigates CEO Jensen Huang&#x27;s relationship with ...</a></li>
<li><a href="https://www.nytimes.com/2026/11/08/technology/nvidia-investigation-jensen-huang-china.html">Nvidia Opens Investigation Into Jensen Huang’s Relationship ...</a></li>
<li><a href="https://sfstandard.com/2026/11/08/nvidia-jensen-huang-affair-board-investigation-chinese-spy/">Nvidia launches probe as Jensen Huang admits affair with ...</a></li>

</ul>
</details>

**Tags**: `#corporate governance`, `#national security`, `#NVIDIA`, `#executive leadership`, `#investigation`

---