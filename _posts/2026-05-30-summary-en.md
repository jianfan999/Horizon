---
layout: default
title: "Horizon Summary: 2026-05-30 (EN)"
date: 2026-05-30
lang: en
---

> From 159 items, 29 important content pieces were selected

---

1. [Accenture acquires Ookla for $1.2B](#item-1) ⭐️ 8.0/10
2. [Zig ELF Linker Improvements Announced](#item-2) ⭐️ 8.0/10
3. [OpenRouter Raises $113M Series B for LLM Proxy Service](#item-3) ⭐️ 8.0/10
4. [Openrsync: OpenBSD's clean-room rsync implementation used in macOS 15.0](#item-4) ⭐️ 8.0/10
5. [SoftBank Plans €75B Investment in French Data Centers](#item-5) ⭐️ 8.0/10
6. [GitHub Copilot’s Token Billing Sparks Developer Outrage](#item-6) ⭐️ 8.0/10
7. [China's dexterous robotic hand startups set valuation records](#item-7) ⭐️ 8.0/10
8. [Chinese scientists create 'kill-them-all' drone swarm algorithm](#item-8) ⭐️ 8.0/10
9. [Huawei Tau Scaling Law: Breakthrough or Hype?](#item-9) ⭐️ 8.0/10
10. [Microsoft threatens legal action over vulnerability disclosure](#item-10) ⭐️ 8.0/10
11. [Domain expertise becomes the real moat in AI era](#item-11) ⭐️ 7.0/10
12. [Voxel Space: 1992 Heightmap Rendering Algorithm Demo](#item-12) ⭐️ 7.0/10
13. [AI Data Centers Stir Local Backlash](#item-13) ⭐️ 7.0/10
14. [China launches national AI evaluation framework](#item-14) ⭐️ 7.0/10
15. [17 Nations Form Pact to Protect Undersea Cables, US and China Absent](#item-15) ⭐️ 7.0/10
16. [Researchers Seek to Use Teacher-Worn Cameras for AI Training](#item-16) ⭐️ 7.0/10
17. [California's 300+ Data Centers Face Water Scarcity](#item-17) ⭐️ 7.0/10
18. [EU proposes Tech Sovereignty Package to override contracts](#item-18) ⭐️ 7.0/10
19. [Curated Pandoc Templates Collection Launched](#item-19) ⭐️ 6.0/10
20. [Haiguang Adapts Step 3.7 Flash on DTK Platform](#item-20) ⭐️ 6.0/10
21. [90s Tech Giants Resurge on AI Boom](#item-21) ⭐️ 6.0/10
22. [Google Gemini Spark review: useful but unnecessary as standalone product](#item-22) ⭐️ 6.0/10
23. [Alternative browsers challenge Chrome and Safari in 2026](#item-23) ⭐️ 6.0/10
24. [TikTok Reportedly Aims to Become a Super App](#item-24) ⭐️ 6.0/10
25. [Indian court ruling reignites Google ad business criticism](#item-25) ⭐️ 6.0/10
26. [DuckDuckGo 'No AI' Search Traffic Triples After Google Update](#item-26) ⭐️ 6.0/10
27. [Huawei Chairman Thanks US Export Curbs for Boosting China's Chips](#item-27) ⭐️ 6.0/10
28. [New US Bill Aims to Prepare Workers for AI Job Displacement](#item-28) ⭐️ 6.0/10
29. [Claim: New Device Boosts Processor Speed 1000x Without Extra Heat](#item-29) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Accenture acquires Ookla for $1.2B](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

Accenture has announced its acquisition of Ookla, the parent company of Speedtest and Downdetector, for $1.2 billion to enhance its network intelligence and data analytics capabilities for enterprises. This acquisition gives Accenture access to vast amounts of real-time network performance data from over 250 million monthly tests, enabling it to offer deeper insights to telecoms and enterprises, but also raises concerns about conflicts of interest as Accenture consults for many of the same companies whose outages Downdetector tracks. Ookla's data platform includes Speedtest, Downdetector, Ekahau, and RootMetrics, with telcos paying six-figure annual fees for this data. Accenture was already a competitor in this space through its earlier acquisition of Umlaut.

hackernews · Garbage · May 30, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48337987)

**Background**: Ookla is best known for Speedtest.net, a widely used tool for measuring internet connection performance, and Downdetector, which tracks real-time service outages. Beyond consumer tools, Ookla sells aggregated network data to telecom operators and other clients. Accenture is a global IT services and consulting firm that helps companies improve their operations, often in the telecom sector.

**Discussion**: Community comments highlight that the deal is primarily a data acquisition, with Ookla's real value lying in its telco data sales. Commenters express skepticism about Downdetector's neutrality under Accenture's ownership, given Accenture's consulting relationships with many of the same companies. Some note that Accenture's earlier acquisition of Umlaut already made it a competitor in network testing, reinforcing the data-driven motivation for this purchase.

**Tags**: `#acquisition`, `#network intelligence`, `#data analytics`, `#telecom`, `#AI`

---

<a id="item-2"></a>
## [Zig ELF Linker Improvements Announced](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

Zig's official devlog for May 30, 2026, details significant improvements to its ELF linker, enabling fast incremental linking that speeds up development iteration. These improvements bring Zig closer to being a viable C replacement, offering fast iteration speeds comparable to interpreted languages while maintaining C-level performance. This is critical for systems programming and for projects like a DAW that require uncompromising user experience. The linker improvements focus on incremental compilation, but this may be mutually exclusive with link-time optimization (LTO), meaning release builds would likely skip incremental linking. The devlog does not specify which targets are supported yet.

hackernews · kristoff_it · May 30, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48338673)

**Background**: Zig is a general-purpose systems programming language designed to be an improvement over C, emphasizing safety and performance. ELF (Executable and Linkable Format) is the standard binary format for executables on Linux and Unix-like systems. A linker is a tool that combines compiled object files into a single executable; incremental linking reuses previously linked results to reduce rebuild times.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://ziglang.org/">Home Zig Programming Language</a></li>

</ul>
</details>

**Discussion**: The community is highly enthusiastic, with one commenter stating that once incremental linking lands, Zig will become 'THE C replacement' enabling iteration speeds of JS/Python with C/Rust performance. Another developer building a memory-safe language that transpiles to Zig praised the build system design. A discussion also noted that incremental linking likely precludes LTO for release builds.

**Tags**: `#Zig`, `#linker`, `#systems programming`, `#compiler`, `#open source`

---

<a id="item-3"></a>
## [OpenRouter Raises $113M Series B for LLM Proxy Service](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter, a unified API platform providing access to over 400 AI models, announced a $113 million Series B funding round. This substantial investment signals strong market confidence in LLM proxy services as essential infrastructure for developers, enabling easier experimentation and cost management across multiple model providers. OpenRouter charges a 5% surcharge on API calls, and its features include billing caps, unified logging, and support for 400+ models from various providers.

hackernews · freeCandy · May 30, 17:27 · [Discussion](https://news.ycombinator.com/item?id=48338660)

**Background**: OpenRouter acts as a proxy between developers and LLM providers, offering a single API to access models from OpenAI, Anthropic, and others. This simplifies experimentation and provides features like cost tracking and spending limits that many individual providers lack. The service is popular among developers who want to quickly test new models without managing multiple API keys.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/about">About OpenRouter - The Unified Interface For LLMs | OpenRouter</a></li>
<li><a href="https://docs.litellm.ai/docs/simple_proxy">LiteLLM AI Gateway (LLM Proxy) | liteLLM</a></li>

</ul>
</details>

**Discussion**: Community comments were largely positive about OpenRouter's value for experimentation and billing caps, though some questioned the 5% surcharge for high-volume usage. Others noted that OpenRouter's utility might decrease as the LLM ecosystem consolidates around fewer dominant models.

**Tags**: `#AI`, `#LLM`, `#funding`, `#OpenRouter`, `#developer tools`

---

<a id="item-4"></a>
## [Openrsync: OpenBSD's clean-room rsync implementation used in macOS 15.0](https://github.com/kristapsdz/openrsync) ⭐️ 8.0/10

Openrsync, a BSD-licensed clean-room implementation of rsync developed by the OpenBSD team, has been adopted as the default rsync tool in macOS 15.0 (Sequoia) due to licensing conflicts with GPL-licensed rsync. This matters because Apple's switch highlights the growing importance of permissive licenses in mainstream operating systems and the security benefits of a clean-room reimplementation. It also gives users a modern, actively maintained alternative to the original rsync. Openrsync is licensed under the ISC license, a permissive BSD-style license, and is developed as part of an RPKI validator project. It currently does not support all features of the original rsync, such as the --rsync-path option reported by a user.

hackernews · sph · May 30, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48334854)

**Background**: rsync is a widely used file synchronization tool on Unix-like systems, traditionally licensed under the GPL. Due to licensing restrictions, Apple could not include newer GPLv3 versions in macOS, so it relied on the outdated GPLv2 rsync 2.6.9. Clean-room implementation means the Openrsync developers wrote the code independently based on the protocol specification, without copying any GPL-licensed rsync code, thus allowing a permissive license.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/kristapsdz/openrsync">GitHub - kristapsdz/openrsync: BSD-licensed implementation of rsync</a></li>
<li><a href="https://appleinsider.com/inside/macos-sequoia/tips/what-you-should-know-about-apples-switch-from-rsync-to-openrsync">rsync vs openrsync: Apple switch, Terminal commands</a></li>

</ul>
</details>

**Discussion**: User Panino reported that openrsync does not handle the --rsync-path option as expected, creating a directory instead of a file. Another commenter noted that a Go implementation by Michael Stapelberg exists. Thefilmore confirmed its use in macOS 15.0. Overall sentiment is positive, with interest in broader adoption and comparisons.

**Tags**: `#openrsync`, `#rsync`, `#OpenBSD`, `#filesync`, `#systems`

---

<a id="item-5"></a>
## [SoftBank Plans €75B Investment in French Data Centers](https://techcrunch.com/2026/05/30/softbank-says-it-will-invest-up-to-e75-billion-to-build-french-data-centers/) ⭐️ 8.0/10

SoftBank announced plans to invest up to €75 billion to build 5 GW of data center capacity in France, aiming to develop and operate the infrastructure. This massive investment signals a major push to expand European digital infrastructure, potentially boosting AI and cloud computing capabilities while strengthening France's position as a tech hub. The investment targets 5 gigawatts of additional data center capacity, though specific timelines and project locations have not been disclosed.

rss · TechCrunch · May 30, 21:45

**Background**: Data centers are critical for powering cloud services and AI workloads, requiring enormous amounts of electricity. France has been promoting itself as a green data center destination due to its low-carbon nuclear energy. SoftBank's investment could significantly boost the country's digital infrastructure.

**Tags**: `#SoftBank`, `#data centers`, `#investment`, `#France`, `#infrastructure`

---

<a id="item-6"></a>
## [GitHub Copilot’s Token Billing Sparks Developer Outrage](https://techcrunch.com/2026/05/30/what-a-joke-github-copilots-new-token-based-billing-spurs-consternation-among-devs/) ⭐️ 8.0/10

GitHub announced on May 30, 2026 that Copilot will switch from per-request to token-based billing starting June 1, 2026, drawing immediate backlash from developers. This billing change could significantly increase costs for heavy users, potentially reducing adoption of the widely used AI coding assistant and affecting developer tooling choices. Under the new model, users will be charged per token consumed in code completions and chat interactions, rather than paying a flat rate per request; exact token prices have not yet been disclosed.

rss · TechCrunch · May 30, 16:30

**Background**: GitHub Copilot is an AI-powered code completion tool launched in 2022, originally billed via monthly subscriptions based on the number of requests. The shift to token-based billing aligns with how large language model APIs typically charge, but represents a major departure from the simple per-request model that developers had become accustomed to.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.github.com/en/copilot/reference/copilot-billing">GitHub Copilot billing - GitHub Docs</a></li>
<li><a href="https://tech.xebia.ms/github-copilot/videos/github-copilot-token-based-billing?trk=public_post_comment-text">Token - based billing : from premium request units to AI... - Tech Hub</a></li>

</ul>
</details>

**Tags**: `#GitHub Copilot`, `#AI coding assistant`, `#pricing`, `#developer tools`, `#Microsoft`

---

<a id="item-7"></a>
## [China's dexterous robotic hand startups set valuation records](https://www.scmp.com/tech/article/3355365/unicorn-born-record-time-amid-arms-race-among-chinas-robotic-hand-developers?utm_source=rss_feed) ⭐️ 8.0/10

Venture capitalists in China, including Xiaomi and Li Auto, are heavily investing in dexterous robotic hand startups like Xynova, which recently completed a Series A round, creating unicorns in record time amid a global humanoid hardware arms race. Dexterous robotic hands are considered the toughest bottleneck in humanoid robotics. This investment surge could accelerate the development of humanoid robots for industrial and service applications, positioning China as a leader in this critical component. Xynova, a Hangzhou-based startup, announced its Series A funding from Xiaomi's and Li Auto's venture arms, though the exact amount was not disclosed. This reflects a broader trend of rapid valuations in this niche.

rss · SCMP · May 30, 06:00

**Background**: Dexterous robotic hands are advanced end-effectors designed to replicate the flexibility and sensitivity of human hands, enabling robots to perform delicate tasks. They are a critical bottleneck in humanoid robotics due to the challenges in achieving fine motor control and tactile sensing. The global race to develop humanoid robots has intensified investment in this component.

<details><summary>References</summary>
<ul>
<li><a href="https://shadowrobot.com/dexterous-hand-series/">Shadow Dexterous Hand Series - Research and Development Tool</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#humanoid`, `#venture capital`, `#AI hardware`, `#China`

---

<a id="item-8"></a>
## [Chinese scientists create 'kill-them-all' drone swarm algorithm](https://www.scmp.com/news/china/science/article/3355232/chinese-scientists-create-kill-them-all-algorithm-drone-warfare?utm_source=rss_feed) ⭐️ 8.0/10

Chinese researchers have developed HG-STR (Heterogeneous Graph Spatio-Temporal Reasoning), an algorithm that enables drone swarms to autonomously locate and destroy all enemy targets even under communication jamming and vision obstruction. This advancement significantly enhances autonomous drone swarm coordination and resilience in contested environments, potentially reshaping modern warfare by reducing reliance on human control and communication links. The algorithm is claimed to be the first capable of achieving 100% elimination of enemy targets in a battlefield scenario, using heterogeneous graph structures to model different drone and target types and spatio-temporal reasoning to predict movements.

rss · SCMP · May 30, 04:00

**Background**: Drone swarms typically rely on constant communication with a ground station or among themselves for coordination. HG-STR uses onboard spatio-temporal reasoning to maintain coordination even when communications are jammed, allowing autonomous decision-making without external input.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2408.10822">[2408.10822] Navigating Spatio-Temporal Heterogeneity: A Graph Transformer Approach for Traffic Forecasting</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2589004224014007">Deep transformer-based heterogeneous spatiotemporal graph learning for geographical traffic forecasting - ScienceDirect</a></li>

</ul>
</details>

**Tags**: `#drone swarms`, `#autonomous warfare`, `#AI`, `#algorithm`, `#military`

---

<a id="item-9"></a>
## [Huawei Tau Scaling Law: Breakthrough or Hype?](https://www.scmp.com/tech/tech-trends/article/3355314/huaweis-new-chip-scaling-law-true-breakthrough-or-mere-hype?utm_source=rss_feed) ⭐️ 8.0/10

Huawei introduced the Tau (τ) Scaling Law at the IEEE ISCAS conference, proposing a shift from transistor miniaturization to focusing on data movement speed to advance semiconductor performance. This law could redefine semiconductor progress, especially for companies like Huawei constrained by US export restrictions, potentially enabling advanced chip development without cutting-edge fabrication tools. Huawei claims it has already designed and mass-produced 381 chips based on the Tau law over six years, and targets 1.4 nm-equivalent chip density by 2031.

rss · SCMP · May 30, 03:00

**Background**: Traditional semiconductor scaling, known as Moore's Law, focuses on shrinking transistors to improve performance. However, as physical limits approach and data movement becomes a bottleneck, alternative approaches like Huawei's Tau law emphasize system-level optimization of data throughput, which is particularly relevant under US sanctions restricting access to advanced lithography equipment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in Transistor Density and System Performance - Huawei</a></li>
<li><a href="https://www.scmp.com/tech/article/3354710/huawei-unveils-new-scaling-law-and-tech-can-develop-14-nm-equivalent-chips-2031">Huawei unveils new scaling law and tech that narrows gap with TSMC, Samsung | South China Morning Post</a></li>
<li><a href="https://interestingengineering.com/energy/huawei-tau-scaling-law-1-4nm-chip-density-2031">Huawei targets 1.4 nm-class chips with new computing architecture</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#Huawei`, `#chip scaling law`, `#US-China tech war`, `#data movement`

---

<a id="item-10"></a>
## [Microsoft threatens legal action over vulnerability disclosure](https://www.reddit.com/r/technology/comments/1ts2sh9/microsoft_is_threatening_legal_action_for/) ⭐️ 8.0/10

Microsoft has threatened legal action against a security researcher for publicly posting exploits without prior coordination. The company is engaged in a dispute over the ethics and legality of full vulnerability disclosure. This case highlights the ongoing tension between security researchers who advocate for full disclosure and technology companies that prefer coordinated disclosure to protect users. It could set a precedent for legal boundaries in vulnerability research. The researcher reportedly posted working exploits for unpatched vulnerabilities, which Microsoft argues violates its terms of service and potentially laws against computer fraud. The specific vulnerabilities and researcher's identity have not been officially disclosed.

reddit · r/technology · /u/MarvelsGrantMan136 · May 30, 15:21

**Background**: Vulnerability disclosure is the practice of reporting security flaws to the affected vendor. Responsible disclosure involves giving the vendor time to patch before publicizing, while full disclosure releases details immediately. Legal threats by vendors against researchers can chill security research and reduce the number of vulnerabilities discovered and fixed, potentially leaving users less safe.

**Tags**: `#security`, `#vulnerability disclosure`, `#legal`, `#Microsoft`

---

<a id="item-11"></a>
## [Domain expertise becomes the real moat in AI era](https://www.brethorsting.com/blog/2026/05/domain-expertise-has-always-been-the-real-moat/) ⭐️ 7.0/10

A blog post argues that as AI automates coding tasks, domain expertise is now the key differentiator for software engineers, not just coding skill. This shift changes career advice for engineers, emphasizing deep industry knowledge over pure coding ability, and reshapes hiring criteria and team composition. The author contrasts the engineer's advantage (translating domain models into code) becoming cheap, while the domain expert's advantage (knowing what right looks like) remains valuable.

hackernews · aaronbrethorst · May 30, 20:40 · [Discussion](https://news.ycombinator.com/item?id=48340411)

**Background**: AI coding tools like GPT-4 and agentic assistants can now generate significant portions of code, reducing the barrier to implementation. This shifts the bottleneck from programming to understanding the problem domain, making domain expertise a critical skill for senior engineers.

**Discussion**: Comments include a finance developer agreeing that coding is the easiest part, skepticism about shifting AI narratives, and practical examples of AI still struggling with complex domains.

**Tags**: `#domain expertise`, `#AI`, `#software engineering`, `#career strategy`

---

<a id="item-12"></a>
## [Voxel Space: 1992 Heightmap Rendering Algorithm Demo](https://s-macke.github.io/VoxelSpace/) ⭐️ 7.0/10

A browser-based demo and explanation of the Voxel Space terrain rendering algorithm, originally used in the 1992 game Comanche, has been recreated and shared online. This nostalgic recreation highlights a historically significant algorithm that enabled efficient real-time terrain rendering in early 3D games, and the community discussion reveals technical insights and personal experiences with the technique. Technically, Voxel Space uses a heightmap (a 2D array of heights) rather than true volumetric voxels, rendering vertical columns based on the viewer's perspective.

hackernews · davikr · May 30, 14:25 · [Discussion](https://news.ycombinator.com/item?id=48336564)

**Background**: Voxel Space is a terrain rendering algorithm developed in 1992 for the video game Comanche. It renders a landscape by rasterizing a heightmap and color map, drawing vertical lines to create a 3D effect. Unlike true voxels which represent volumetric data, it uses a 2D heightmap, making it simpler and faster for its time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voxel">Voxel - Wikipedia</a></li>
<li><a href="https://github.com/jval1972/emupedia-demo-voxel-space">jval1972/emupedia-demo- voxel - space : Terrain rendering algorithm ...</a></li>

</ul>
</details>

**Discussion**: Comments highlight that the algorithm is technically a heightmap, not true voxels, and share nostalgic memories of playing Comanche on early PCs. One user describes a testing methodology inspired by the game's first mission, while others link to related projects like a C++ port and an AGS Engine adaptation.

**Tags**: `#voxel`, `#rendering`, `#game development`, `#height map`, `#retro gaming`

---

<a id="item-13"></a>
## [AI Data Centers Stir Local Backlash](https://www.bloomberg.com/news/videos/2026-05-30/can-ai-grow-without-hurting-local-communities-video) ⭐️ 7.0/10

A growing number of communities and officials are challenging the construction of AI data centers, citing concerns over electricity costs, water usage, noise, and lack of transparency, as highlighted by Michigan Attorney General Dana Nessel's legal challenge to a project near Ann Arbor. This tension illustrates a critical socio-technical issue: the rapid expansion of AI infrastructure may impose significant local costs, potentially slowing deployment and requiring new regulatory frameworks. DigitalBridge CEO Marc Ganzi acknowledged that the industry must work with local communities to demonstrate that benefits outweigh burdens, while the Michigan case focuses on ratepayer transparency and risk allocation.

rss · Bloomberg Markets · May 30, 14:03

**Background**: AI data centers house powerful computing hardware that requires massive amounts of electricity and water for cooling. Their rapid proliferation is driven by demand for large-scale AI model training and inference, but local communities often bear the environmental and economic externalities.

**Tags**: `#AI infrastructure`, `#data centers`, `#local communities`, `#regulation`

---

<a id="item-14"></a>
## [China launches national AI evaluation framework](https://www.scmp.com/economy/china-economy/article/3355324/china-launches-ai-framework-improve-black-box-transparency-and-raise-standards?utm_source=rss_feed) ⭐️ 7.0/10

China's central government released new guidelines to create a unified national yardstick for evaluating AI models, computing power, and data quality, aiming to improve transparency, accuracy, and reliability. This framework addresses the 'black box' problem in AI by standardizing assessments, which could boost trust in AI systems and shape global AI governance, especially as AI adoption accelerates across industries. The framework covers model performance, computing efficiency, and data quality under a common standard, but specific metrics and implementation timelines have not been disclosed yet.

rss · SCMP · May 30, 10:00

**Background**: AI systems often operate as 'black boxes,' making it difficult to understand their decision-making processes. China's move follows global efforts to regulate AI, such as the EU AI Act, and aims to set benchmarks for safety and transparency in domestic AI development.

**Tags**: `#AI governance`, `#China`, `#AI standards`, `#transparency`, `#regulation`

---

<a id="item-15"></a>
## [17 Nations Form Pact to Protect Undersea Cables, US and China Absent](https://www.scmp.com/week-asia/politics/article/3355411/17-nations-launch-pact-protect-vital-undersea-cables-amid-us-china-absence?utm_source=rss_feed) ⭐️ 7.0/10

On May 30, 2025, at the Shangri-La Dialogue in Singapore, 17 nations launched the Guiding Principles for Underwater Infrastructure Defence Exchanges (GUIDE), a framework to cooperate on protecting critical underwater infrastructure such as telecommunication cables. Notably, both the United States and China did not join the pact. Undersea cables carry over 95% of global internet traffic, making their security vital for the digital economy. The absence of major powers like the US and China could limit the pact's effectiveness and signal diverging approaches to maritime infrastructure governance. The GUIDE was initiated by Singapore and involves 17 countries from Europe and Asia, focusing on information sharing, joint exercises, and best practices for defending undersea assets. The framework is non-binding and aims to foster trust among like-minded nations.

rss · SCMP · May 30, 09:55

**Background**: Undersea cables are fiber-optic cables laid on the ocean floor that carry the vast majority of the world's data and communications. They are vulnerable to accidental damage from fishing or anchors, as well as intentional sabotage and espionage. Geopolitical tensions have heightened concerns about cable security, especially near strategic chokepoints. The absence of the US and China, two key stakeholders, highlights the challenge of achieving broad consensus on infrastructure protection in a polarized geopolitical environment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.channelnewsasia.com/singapore/critical-underwater-infrastructure-chan-chun-sing-shangri-la-dialogue-6151266">17 countries, including Singapore, launch framework to protect critical underwater infrastructure - CNA</a></li>
<li><a href="https://defencepioneer.sg/pioneer-articles/30may26_news1">17 countries launch new framework for cooperation on critical underwater infrastructure</a></li>
<li><a href="https://www.thestar.com.my/aseanplus/aseanplus-news/2026/05/30/singapore-16-other-countries-launch-effort-to-protect-critical-underwater-infrastructure-during-shangri-la-dialogue-event">Singapore, 16 other countries launch effort to protect critical underwater infrastructure during Shangri-La Dialogue event | The Star</a></li>

</ul>
</details>

**Tags**: `#undersea cables`, `#cybersecurity`, `#international policy`, `#infrastructure defense`

---

<a id="item-16"></a>
## [Researchers Seek to Use Teacher-Worn Cameras for AI Training](https://www.reddit.com/r/technology/comments/1tsd84s/researchers_wanted_preschool_teachers_to_wear/) ⭐️ 7.0/10

Researchers proposed that preschool teachers wear small cameras to capture first-person perspective footage for training AI systems, as described in a document given to parents requesting permission. This initiative raises significant privacy and ethical concerns about surveillance in early childhood education and the use of children's data for AI model training without explicit informed consent. The camera would capture the teacher's approximate first-person perspective, and a fixed video camera might also be placed in the classroom, according to the document given to parents.

reddit · r/technology · /u/ControlCAD · May 30, 22:16

**Background**: Collecting real-world video data from natural settings is valuable for training AI models that understand human activities and interactions. However, doing so in a preschool environment involves vulnerable subjects (children) and sensitive contexts, requiring strict ethical oversight and transparent consent processes. This proposal highlights the tension between advancing AI research and protecting privacy rights, especially for minors.

**Tags**: `#AI ethics`, `#privacy`, `#surveillance`, `#data collection`, `#education`

---

<a id="item-17"></a>
## [California's 300+ Data Centers Face Water Scarcity](https://www.reddit.com/r/technology/comments/1trw8ao/california_will_soon_have_more_than_300_data/) ⭐️ 7.0/10

California is on track to have more than 300 data centers, raising concerns about how these facilities will secure water in a drought-prone state. This highlights the growing tension between digital infrastructure expansion and environmental sustainability, especially in water-stressed regions like California, which is a global tech hub. Data centers use water primarily for cooling systems, and California's frequent droughts make water sourcing a critical issue. The article questions whether existing water supplies can support this growth.

reddit · r/technology · /u/WombatusMighty · May 30, 10:27

**Background**: Data centers require large amounts of electricity and water to operate, with cooling accounting for a significant portion of water use. California has experienced severe droughts in recent years, leading to strict water conservation measures. The state's tech industry drives demand for data centers, but environmental regulations and water availability pose challenges.

**Tags**: `#data centers`, `#California`, `#water usage`, `#sustainability`, `#environment`

---

<a id="item-18"></a>
## [EU proposes Tech Sovereignty Package to override contracts](https://www.reddit.com/r/geopolitics/comments/1try6co/brussels_just_gave_itself_the_power_to_override/) ⭐️ 7.0/10

The European Union has proposed a Tech Sovereignty Package that would allow authorities to override private contracts during emergencies, particularly in semiconductor supply and sensitive data storage. This could disrupt existing commercial agreements for major technology companies and cloud providers, enhancing EU control over critical supply chains and data sovereignty. The proposal targets semiconductor supply arrangements and imposes stricter requirements on where sensitive government data is stored and processed, affecting global tech firms and cloud providers.

reddit · r/geopolitics · /u/aymannasri_tcg · May 30, 12:06

**Background**: The EU has been pursuing greater technological independence to reduce reliance on foreign suppliers, especially amid geopolitical tensions. The Tech Sovereignty Package is part of this strategy, aiming to strengthen the region's resilience in critical technologies like semiconductors and cloud computing.

**Tags**: `#EU policy`, `#technology sovereignty`, `#semiconductors`, `#data privacy`, `#geopolitics`

---

<a id="item-19"></a>
## [Curated Pandoc Templates Collection Launched](https://pandoc-templates.org/) ⭐️ 6.0/10

A new website, pandoc-templates.org, offers a curated collection of templates for Pandoc, the universal document converter, enabling users to easily produce styled documents in multiple formats. This resource simplifies document formatting for Pandoc users, who previously had to create or find templates manually, potentially improving adoption and workflow efficiency in academic and publishing contexts. The templates support various output formats like HTML, PDF, and Word, and include visually appealing designs that go beyond basic formatting, as noted by community members who discovered the site.

hackernews · ankitg12 · May 30, 09:56 · [Discussion](https://news.ycombinator.com/item?id=48334515)

**Background**: Pandoc is a free and open-source document converter created by John MacFarlane, widely used by scholars and in publishing workflows. It converts between markup formats such as Markdown, LaTeX, and HTML. Templates allow users to control the output styling without writing complex commands.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pandoc">Pandoc</a></li>
<li><a href="https://grokipedia.com/page/Pandoc">Pandoc</a></li>

</ul>
</details>

**Discussion**: Commenters generally praised Pandoc and the new template gallery, with some sharing personal experiences using Pandoc for theses and novels. Several compared it to Quarto, noting Quarto's better user experience but acknowledging Pandoc's flexibility. One user reported difficulties with PDF generation, such as table layout issues and font fallback problems.

**Tags**: `#pandoc`, `#templates`, `#markdown`, `#document conversion`, `#open source`

---

<a id="item-20"></a>
## [Haiguang Adapts Step 3.7 Flash on DTK Platform](https://36kr.com/newsflashes/3831356538529409?f=rss) ⭐️ 6.0/10

On May 29, Stepfun released Step 3.7 Flash, and Haiguang Information completed full adaptation and deep optimization on its DTK heterogeneous computing platform the same day, enabling efficient deployment. This allows developers to run the multimodal model efficiently on Haiguang's platform, reducing integration costs for building multimodal agents, code assistants, and complex workflows. The adaptation leverages Haiguang's DTK heterogeneous computing platform and full software stack, achieving 'release-day adaptation and efficiency'. Step 3.7 Flash supports a 256K context window and selectable reasoning levels.

rss · 36氪 · May 30, 05:37

**Background**: Haiguang Information develops domestic GPU accelerators and software stacks for AI workloads. DTK (Deep Computing Toolkit) is a heterogeneous computing platform that allows efficient deployment of AI models across different processors. Step 3.7 Flash is a high-efficiency multimodal Mixture-of-Experts model by Stepfun (Jieyue Xingchen) with a 256K context window.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Heterogeneous_computing">Heterogeneous computing - Wikipedia</a></li>
<li><a href="https://static.stepfun.com/blog/step-3.7-flash/">Step 3 . 7 Flash — A high-efficiency Flash model for Real-World</a></li>
<li><a href="https://openrouter.ai/stepfun/step-3.7-flash">Step 3 . 7 Flash - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#AI model adaptation`, `#GPU computing`, `#multimodal AI`, `#software stack`, `#inference optimization`

---

<a id="item-21"></a>
## [90s Tech Giants Resurge on AI Boom](https://www.bloomberg.com/news/articles/2026-05-30/-dinosaur-tech-stocks-reborn-as-ai-fuels-1-7-trillion-rally) ⭐️ 6.0/10

Dell, Nokia, and Lenovo, which were stars of the dot-com era, are experiencing a resurgence driven by the massive spending on artificial intelligence infrastructure. This trend shows that legacy hardware and networking companies are benefiting from the AI boom, potentially reshaping market dynamics and investment strategies. The AI spending boom is fueling a $1.7 trillion rally in these so-called 'dinosaur' tech stocks, highlighting the shift in demand toward infrastructure providers.

rss · Bloomberg Markets · May 30, 13:00

**Background**: Dell, Nokia, and Lenovo were dominant in the dot-com era but faded as new tech darlings emerged. Now, the need for data centers, servers, and networking equipment for AI workloads is reviving their fortunes.

**Tags**: `#AI`, `#stock market`, `#legacy tech`, `#industry trends`

---

<a id="item-22"></a>
## [Google Gemini Spark review: useful but unnecessary as standalone product](https://techcrunch.com/2026/05/30/i-put-googles-24-7-ai-assistant-gemini-spark-to-work-and-its-actually-pretty-useful/) ⭐️ 6.0/10

A TechCrunch review of Google's Gemini Spark AI assistant found it helpful for automating daily tasks like inbox summaries and event planning, but questioned why it was released as a separate product rather than being integrated into existing Google services. The review highlights the ongoing competition among AI assistants (e.g., ChatGPT, Google Assistant) and raises strategic questions about product differentiation. If Gemini Spark is genuinely useful, its standalone status could fragment the user experience or confuse consumers. Gemini Spark operates as a 24/7 AI assistant, focusing on productivity and automation. The reviewer noted it can summarize emails, plan local events, and automate routine workflows, but the article did not specify pricing or availability details.

rss · TechCrunch · May 30, 15:30

**Background**: AI assistants like Google Assistant and Siri have long offered limited automation, but new generative AI tools (e.g., GPT-4) enable more complex task execution. Google's Gemini family includes multiple models; Spark appears to be a specialized assistant version aimed at proactive, always-on help. The separate product strategy may reflect Google's push to monetize AI capabilities beyond search.

**Tags**: `#AI assistant`, `#Google Gemini`, `#productivity`, `#automation`

---

<a id="item-23"></a>
## [Alternative browsers challenge Chrome and Safari in 2026](https://techcrunch.com/2026/05/30/as-the-browser-wars-heat-up-here-are-the-hottest-alternatives-to-chrome-and-safari-in-2026/) ⭐️ 6.0/10

TechCrunch published an overview of alternative browsers like Ladybird and Servo that are gaining traction against Chrome and Safari in 2026. These browsers emphasize privacy and independence from dominant browser engines, potentially diversifying the web ecosystem and reducing monopoly risks. Ladybird is building a new browser engine from scratch, while Servo leverages Rust for memory safety and concurrency; both are open-source and backed by non-profits.

rss · TechCrunch · May 30, 13:00

**Background**: Most current browsers rely on Blink (Chrome) or WebKit (Safari) engines, leading to limited diversity. Ladybird and Servo aim to create fully independent engines, promoting a more open web.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ladybird_(web_browser)">Ladybird ( web browser ) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Servo_(software)">Servo (software) - Wikipedia</a></li>
<li><a href="https://ladybird.org/">Ladybird is a truly independent web browser , backed by a non-profit.</a></li>

</ul>
</details>

**Tags**: `#browsers`, `#Chrome alternatives`, `#web browsers`, `#tech news`

---

<a id="item-24"></a>
## [TikTok Reportedly Aims to Become a Super App](https://techcrunch.com/2026/05/30/tiktoks-road-to-becoming-a-super-app/) ⭐️ 6.0/10

According to a TechCrunch report, TikTok is reportedly working to transform into a comprehensive super app that would handle a wide range of digital activities for users. If successful, TikTok could dominate the digital ecosystem by integrating social networking, e-commerce, payments, and more, similar to WeChat in China. This move would intensify competition among major tech platforms globally. No specific features or timeline have been confirmed, but the report suggests TikTok is exploring ways to add mini-apps and services beyond short videos. The super app model is well-established in Asia, with examples like WeChat, Grab, and Rappi.

rss · TechCrunch · May 30, 13:00

**Background**: A super app is a mobile application that provides a core set of features while also allowing access to independently developed mini-apps for various services like messaging, payments, e-commerce, and food delivery. Notable examples include WeChat in China, Grab in Southeast Asia, and Rappi in Latin America. TikTok, already a leading short-video platform, may leverage its massive user base to expand into adjacent services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Super-app">Super - app - Wikipedia</a></li>
<li><a href="https://www.techtarget.com/whatis/definition/super-app">What is a super app ?</a></li>
<li><a href="https://www.elluminatiinc.com/super-apps-examples/">Top 6 Successful Super Apps Examples in Market – 2026</a></li>

</ul>
</details>

**Tags**: `#TikTok`, `#super app`, `#social media`, `#digital platforms`

---

<a id="item-25"></a>
## [Indian court ruling reignites Google ad business criticism](https://techcrunch.com/2026/05/29/founders-seize-on-indian-court-ruling-to-revive-criticism-of-googles-ad-business/) ⭐️ 6.0/10

Following an Indian court ruling on trademarked keywords, founders have revived criticism of Google's ad business, arguing that the platform's practices unfairly exploit trademarked terms. This ruling could force ad platforms like Google to reassess how they handle trademarked keywords, potentially reshaping digital advertising practices and protecting brand owners' rights. Lawyers have noted that the decision may compel platforms to revisit their policies on trademarked keywords, though the specific technical or legal adjustments remain unclear.

rss · TechCrunch · May 30, 02:00

**Background**: Google's ad business allows advertisers to bid on keywords, including trademarked terms, to display ads in search results. This practice has long been controversial, as brand owners claim it can mislead consumers or dilute their trademarks. The Indian court ruling appears to address these concerns, potentially setting a precedent for other jurisdictions.

**Tags**: `#Google`, `#advertising`, `#trademark`, `#India`, `#legal`

---

<a id="item-26"></a>
## [DuckDuckGo 'No AI' Search Traffic Triples After Google Update](https://www.reddit.com/r/technology/comments/1tsbhq7/traffic_to_duckduckgos_proudly_no_ai_search_page/) ⭐️ 6.0/10

Traffic to DuckDuckGo's specialized 'No AI' search page has tripled following Google's latest AI-focused search update, as users seek alternatives without AI-generated answers. This surge indicates growing user resistance to AI integration in search, potentially reshaping the search engine market as privacy-conscious users demand AI-free options. The 'No AI' page lacks AI-assisted answers, chat interfaces, and surfaces fewer AI-generated images; however, it cannot be set as the default search engine on Apple devices directly.

reddit · r/technology · /u/MarvelsGrantMan136 · May 30, 21:05

**Background**: DuckDuckGo is a privacy-focused search engine that blocks third-party trackers. Its 'No AI' search page is an optional version that disables all AI features, including optional AI chatbot integration available on the main site. Google's latest search update heavily integrates AI-generated answers, prompting some users to seek alternatives.

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/05/29/duckduckgo-no-ai-search/">DuckDuckGo 's ' No AI ' Search Traffic Climbs as Users... - MacRumor...</a></li>
<li><a href="https://chromewebstore.google.com/detail/duckduckgo-no-ai-search/faoilnlkccdjdkpljainiiimmijofmpd">DuckDuckGo No - AI Search - Chrome Web Store</a></li>

</ul>
</details>

**Tags**: `#search`, `#AI`, `#privacy`, `#DuckDuckGo`, `#Google`

---

<a id="item-27"></a>
## [Huawei Chairman Thanks US Export Curbs for Boosting China's Chips](https://www.reddit.com/r/technology/comments/1ts0ekb/huawei_chairman_thanks_the_us_for_export/) ⭐️ 6.0/10

Huawei Chairman Liang Hua stated that US export restrictions on chips have inadvertently accelerated China's semiconductor R&D and self-reliance. He thanked Washington for pushing Chinese firms to invest in domestic technology. This statement highlights the geopolitical impact of US export controls on global semiconductor supply chains, potentially reshaping the industry's balance of power. It may influence future US trade policy and China's long-term tech independence. The remarks were made at a public event, though specific dates or figures on R&D investment were not detailed. Huawei has been under US sanctions since 2019, limiting its access to advanced chips and EDA tools.

reddit · r/technology · /u/LurkerFromTheVoid · May 30, 13:45

**Background**: Semiconductor manufacturing is a complex process involving photolithography, etching, and deposition to create integrated circuits. US export controls restrict sale of advanced chips and equipment to Chinese firms, aiming to curb China's technological rise. In response, China has increased domestic R&D efforts, seeking self-sufficiency in chip design and fabrication.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Semiconductor_manufacturing_process">Semiconductor manufacturing process</a></li>
<li><a href="https://en.wikipedia.org/wiki/350_nm_process">350 nm process - Wikipedia</a></li>
<li><a href="https://www.voxelmatters.com/where-am-fits-in-the-world-of-semiconductor-manufacturing/">Where AM fits in the world of semiconductor manufacturing</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#Huawei`, `#export controls`, `#China`, `#tech policy`

---

<a id="item-28"></a>
## [New US Bill Aims to Prepare Workers for AI Job Displacement](https://www.reddit.com/r/technology/comments/1tsbssa/ai_is_coming_for_truck_drivers_a_new_bill_is/) ⭐️ 6.0/10

A proposed bill in the US Congress seeks to establish programs to retrain and support workers, particularly truck drivers, whose jobs are threatened by the rise of AI and automation. This bill represents a proactive policy response to the accelerating impact of AI on the workforce, potentially setting a precedent for how governments address automation-driven job displacement. The legislation reportedly draws inspiration from existing programs like Trade Adjustment Assistance, and includes provisions for wage insurance and skill upgrading, targeting industries like trucking where autonomous vehicles are advancing.

reddit · r/technology · /u/Just-Grocery-2229 · May 30, 21:17

**Background**: Autonomous trucking technology has been rapidly developing, with companies like Applied Intuition and Kodiak AI working on driverless semis. Studies suggest AI-driven automation could lead to significant job displacement in logistics. While some argue AI will create new jobs, workers in manual roles like truck driving are particularly vulnerable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.appliedintuition.com/autonomous-trucking">Autonomous trucking & driverless trucks | Applied Intuition</a></li>
<li><a href="https://jacobin.com/2025/07/artificial-intelligence-worker-displacement-jobs">AI -Driven Worker Displacement Is a Serious Threat</a></li>
<li><a href="https://levelup.gitconnected.com/ai-is-displacing-workers-faster-than-we-can-retrain-them-a5fc0ed08a28">AI Is Displacing Workers Faster Than We Can... | Level Up Coding</a></li>

</ul>
</details>

**Tags**: `#AI impact`, `#automation`, `#labor policy`, `#self-driving trucks`

---

<a id="item-29"></a>
## [Claim: New Device Boosts Processor Speed 1000x Without Extra Heat](https://www.reddit.com/r/technology/comments/1ts70fc/new_device_could_make_processors_run_1000_times/) ⭐️ 6.0/10

A Reddit post claims a new device can make processors run 1,000 times faster without generating additional waste heat, potentially reducing data center energy demands. However, no article or technical details are provided to verify the claim. If true, this breakthrough could dramatically reduce energy consumption in data centers, which currently consume about 1-2% of global electricity. It would also enable much faster computing without thermal constraints, impacting AI, scientific simulations, and many other fields. The claim promises a 1,000x speedup without additional waste heat, which contradicts current physical understanding of computing efficiency. No specific device name, architecture, or experimental results were disclosed in the post.

reddit · r/technology · /u/Vailhem · May 30, 18:07

**Background**: Processor speed has historically been limited by heat dissipation, as faster switching generates more waste heat. This is why clock speeds stalled around 4-5 GHz in the mid-2000s, leading to multi-core architectures. A device that could run 1,000 times faster without extra heat would represent a revolutionary change in physics or materials, possibly based on new computing paradigms like reversible computing or topological states.

**Tags**: `#hardware`, `#processors`, `#energy efficiency`, `#data centers`, `#breakthrough`

---