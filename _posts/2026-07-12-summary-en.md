---
layout: default
title: "Horizon Summary: 2026-07-12 (EN)"
date: 2026-07-12
lang: en
---

> From 121 items, 20 important content pieces were selected

---

1. [Math.tanh in Chromium 148 enables OS fingerprinting](#item-1) ⭐️ 8.0/10
2. [Claude Code vs OpenCode: Token Overhead Comparison](#item-2) ⭐️ 8.0/10
3. [GPT-5.6 Migration Boosts AI Agent Speed 2.2x, Cuts Costs 27%](#item-3) ⭐️ 8.0/10
4. [Terry Tao explores LLM coding agents for research apps](#item-4) ⭐️ 8.0/10
5. [Meta faces $1.4 trillion fines for harming minors with algorithms](#item-5) ⭐️ 8.0/10
6. [Irish datacenters now consume 23% of national electricity](#item-6) ⭐️ 7.0/10
7. [Tencent-backed DPU startup Cloud Leopard files for ChiNext IPO](#item-7) ⭐️ 7.0/10
8. [China's Cloud & Semiconductor Equipment Exports Surge Over 90% in Early 2025](#item-8) ⭐️ 7.0/10
9. [Japan's Hayabusa2 Successfully Flies By Asteroid Torifune](#item-9) ⭐️ 7.0/10
10. [Tiny Emulators: Cycle-Accurate 8-bit Emulation in JavaScript](#item-10) ⭐️ 6.0/10
11. [Anthropic Clarifies Claude Code: Model Upgrade Isn't Always the Fix](#item-11) ⭐️ 6.0/10
12. [Embodied Data Industry: 97 Players, $6.2B Funding, Who Profits?](#item-12) ⭐️ 6.0/10
13. [Focus on Domestic AI Computing Amid Overseas Tech Volatility](#item-13) ⭐️ 6.0/10
14. [CITIC: AI Hardware Stays Hot, Software Shows Early Recovery](#item-14) ⭐️ 6.0/10
15. [AI Boom Drives Gas Turbine Prices Up 300% in 3 Years](#item-15) ⭐️ 6.0/10
16. [CXMT Set for Largest A-Share IPO of the Year on STAR Market](#item-16) ⭐️ 6.0/10
17. [Phoebe Gates' Startup Phia Accused of Cookie Overwriting](#item-17) ⭐️ 6.0/10
18. [AI Trio Dominates Emerging Markets, Worrying Investors](#item-18) ⭐️ 6.0/10
19. [Robotaxi Ultimatum: Regulatory Pressure Mounts](#item-19) ⭐️ 6.0/10
20. [Memory Chip Prices Triple in Shenzhen's Electronics Hub](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Math.tanh in Chromium 148 enables OS fingerprinting](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 8.0/10

Scrapfly researchers discovered that Chromium 148's Math.tanh function returns OS-dependent numerical values, enabling fingerprinting of the underlying operating system through a single function call. This technique poses a privacy risk as it can reveal the real OS even if the User-Agent header is spoofed, and it may be used by anti-bot systems to detect inconsistencies for user tracking or blocking. The fingerprinting works because Math.tanh, along with CSS trigonometric functions and the Web Audio compressor, routes through the host's libm library, whose floating-point rounding behavior varies by OS and hardware platform.

hackernews · joahnn_s · Jul 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=48884853)

**Background**: Floating-point arithmetic is not standardized across platforms, leading to small but detectable differences in results for certain operations. Chromium 148's use of the host system's math library (libm) for Math.tanh exposes these platform-specific rounding behaviors, which can be exploited for fingerprinting.

<details><summary>References</summary>
<ul>
<li><a href="https://scrapfly.dev/posts/browser-math-os-fingerprint/">Your Browser Does Math Differently on Every OS , and Anti-Bot...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48884853">Since Chronium 148, Math . tanh is now fingerprintable... | Hacker News</a></li>

</ul>
</details>

**Discussion**: Hacker News comments were mixed: some noted the technique is not entirely new and is limited, while others criticized the article's promotional nature. Some users expressed hope that this will push for correctly rounded transcendental functions to mitigate such fingerprinting.

**Tags**: `#fingerprinting`, `#security`, `#privacy`, `#chromium`, `#javascript`

---

<a id="item-2"></a>
## [Claude Code vs OpenCode: Token Overhead Comparison](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

A comparative study found that Claude Code uses 33,000 tokens before processing a user prompt, while OpenCode uses only 7,000 tokens, due to inefficient caching and harness token usage. Token efficiency directly affects user costs, and this overhead makes Claude Code significantly more expensive than OpenCode for similar tasks. It highlights the need for more efficient agent design and may influence user adoption. The study logged all requests between the coding agents and Anthropic's endpoint, capturing usage blocks. A caveat is that the results may not generalize to all tasks; the authors plan to include more in-depth tasks and qualitative comparisons.

hackernews · systima · Jul 12, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48883275)

**Background**: Token overhead in coding agents refers to tokens consumed by system prompts, harness logic, and tool definitions before the actual user request is processed. Claude Code and OpenCode are AI-powered coding assistants that use large language models to generate code. Harness tokens are part of the agent orchestration framework that manages tool calls and sub-agents.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/costs">Manage costs effectively - Claude Code Docs</a></li>
<li><a href="https://prowe214.medium.com/agentic-coding-harnesses-a-comparison-4db34b87fd5c">Agentic Coding Harnesses: A Comparison | by Paul Cullen Rowe | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters noted that sub-agents are a major source of token bloat, with one user reporting 7 sub-agents spawned for a single task. Others speculated that Anthropic may intentionally inflate token usage to drive subscriptions, while some argued that prompt minimalism and tooling quality matter more than raw prompt size.

**Tags**: `#coding agents`, `#token efficiency`, `#Claude Code`, `#OpenCode`, `#AI tools`

---

<a id="item-3"></a>
## [GPT-5.6 Migration Boosts AI Agent Speed 2.2x, Cuts Costs 27%](https://ploy.ai/blog/migrating-a-production-ai-agent-to-gpt-5-6) ⭐️ 8.0/10

Ploy's blog documents migrating their production AI agent from older GPT-5.4 models to GPT-5.6, achieving a 2.2x speedup and 27% cost reduction in real-world marketing website building workflows. This real-world case provides concrete evidence that upgrading to newer models like GPT-5.6 can yield significant performance and cost benefits, encouraging other companies to consider similar migrations. It also shows that for many workflows, the upgrade is a simple one-line change. The migration was applied to Ploy's agent which builds and edits marketing websites, including planning, code reading, component writing, image generation, and self-screening. The improvements held across varied tiny workflows, with some cases of improved classification accuracy.

hackernews · brryant · Jul 12, 17:13 · [Discussion](https://news.ycombinator.com/item?id=48882716)

**Background**: GPT-5.6 is a large language model released by OpenAI in July 2026, with variants including Sol for complex tasks, Luna for cost-effective runs, and Terra. AI model migration involves switching from one model to another while preserving prompts and workflow quality, often requiring evaluation and prompt optimization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT‑5.6 Sol: a next-generation model - OpenAI</a></li>
<li><a href="https://theaitrack.com/ai-model-migration/">AI Model Migration: Switch Without Losing Workflow</a></li>

</ul>
</details>

**Discussion**: Community comments generally validated the reported improvements, with one user noting similar gains across varied workflows and calling the upgrade a one-liner. Another discussed the cost-performance trade-off between Sol and Luna, while a third praised even cheaper alternatives like Reasonix with Deepseek. Some criticism targeted the article's writing style.

**Tags**: `#AI`, `#GPT-5.6`, `#model migration`, `#performance`, `#cost efficiency`

---

<a id="item-4"></a>
## [Terry Tao explores LLM coding agents for research apps](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

Fields Medalist Terry Tao published a blog post detailing his experience using LLM-based coding agents to build interactive visualizations for mathematical research. He highlights both the surprising effectiveness and the limitations of these tools. Tao's perspective brings mainstream credibility to AI-assisted programming, especially for niche scientific applications. It signals that even top-tier researchers can benefit from LLM agents, potentially accelerating discovery and lowering barriers to creating specialized software. Tao notes that while LLM-generated code is often imperfect and requires careful supervision, the speed of prototyping is unmatched. He emphasizes that such visualizations are not mission-critical to his papers, so the risk is acceptable.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: LLM agents are AI systems that use large language models combined with planning, memory, and tool use to execute complex tasks. Coding agents specifically leverage LLMs to generate, debug, and refine code. Terry Tao is a renowned mathematician and Fields Medalist who often experiments with new computational tools.

<details><summary>References</summary>
<ul>
<li><a href="https://www.promptingguide.ai/research/llm-agents">LLM Agents | Prompt Engineering Guide</a></li>
<li><a href="https://www.superannotate.com/blog/llm-agents">LLM agents: The ultimate guide 2026 | SuperAnnotate</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, with many sharing similar experiences of productivity boosts from LLM coding agents. Some comments draw humorous analogies, like comparing Tao's excitement to a chef discovering microwave dinners, while others caution that LLM-generated code should not be fully trusted without human oversight.

**Tags**: `#LLM`, `#coding agents`, `#AI-assisted programming`, `#software development`, `#Terry Tao`

---

<a id="item-5"></a>
## [Meta faces $1.4 trillion fines for harming minors with algorithms](https://36kr.com/newsflashes/3892793713670919?f=rss) ⭐️ 8.0/10

Meta is being sued by 29 US states and faces EU penalties for using addictive algorithms that harm minors, with total potential fines up to $1.4 trillion. The EU's Digital Services Act preliminary report demands changes to features like autoplay and infinite scroll. This case could set a precedent for regulating algorithmic design across the tech industry, especially regarding child safety. It highlights the growing global consensus that social media platforms must be held accountable for mental health impacts. The EU's DSA requires Very Large Online Platforms to conduct risk assessments and mitigate systemic risks, including addictive design. Meta denies the allegations and plans to contest the actions.

rss · 36氪 · Jul 12, 23:13

**Background**: Addictive algorithms are designed to maximize user engagement by triggering dopamine-driven reward cycles, potentially leading to compulsive use, especially in teens. The EU's Digital Services Act (DSA), effective from 2022, imposes strict obligations on large platforms to protect users, including minors, from harmful design practices.

<details><summary>References</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11804976/">Social Media Algorithms and Teen Addiction: Neurophysiological Impact and Ethical Considerations - PMC</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#algorithm regulation`, `#Digital Services Act`, `#minors protection`, `#tech regulation`

---

<a id="item-6"></a>
## [Irish datacenters now consume 23% of national electricity](https://www.theregister.com/on-prem/2026/07/11/irish-datacenters-now-guzzle-23-of-the-countrys-electricity/5270013) ⭐️ 7.0/10

According to a report covered by The Register, Irish data centers now consume 23% of the country's total electricity, a significant increase from previous years. This high consumption rate raises concerns about Ireland's energy capacity and the economic trade-offs of hosting large-scale data centers, especially as the AI boom drives further demand. The 23% figure is based on data from Ireland's national grid; community commenters noted that California's data center energy use per capita is similar but Ireland's smaller population makes the share appear larger.

hackernews · Bender · Jul 12, 20:16 · [Discussion](https://news.ycombinator.com/item?id=48884322)

**Background**: Data centers are facilities that house computing equipment for processing, storing, and transmitting digital information. Their energy use includes both IT equipment and supporting infrastructure like cooling, measured by Power Usage Effectiveness (PUE). The rapid growth of cloud computing and AI has led to a surge in data center construction and energy demand worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Power_usage_effectiveness">Power usage effectiveness - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hyperscale_data_center">Hyperscale data center</a></li>

</ul>
</details>

**Discussion**: Commenters offered diverse perspectives: some argued the energy consumption reflects economic value and job creation, while others highlighted rising electricity prices and broadband costs in Ireland. One commenter compared the situation to other resource allocation issues, and another suggested nuclear power as a solution.

**Tags**: `#data centers`, `#energy consumption`, `#Ireland`, `#sustainability`, `#infrastructure`

---

<a id="item-7"></a>
## [Tencent-backed DPU startup Cloud Leopard files for ChiNext IPO](https://36kr.com/p/3892352153942530?f=rss) ⭐️ 7.0/10

Cloud Leopard Intelligent, a DPU chip company heavily invested by Tencent, has submitted its IPO application to the ChiNext board of the Shenzhen Stock Exchange, aiming to become the first publicly traded DPU company in China. This IPO represents a milestone for China's domestic DPU industry, highlighting the push for homegrown alternatives in data center infrastructure chips. It also underscores Tencent's strategic bet on foundational semiconductor technology. Cloud Leopard's DPU SoC achieves 400Gbps network bandwidth, offering 4x performance improvement and over 50% power reduction compared to traditional solutions. Despite rapid revenue growth (from 17万元 in 2023 to 3.7亿元 in 2025), the company remains unprofitable.

rss · 36氪 · Jul 12, 07:59

**Background**: A DPU (Data Processing Unit) is a specialized processor that offloads networking, storage, and security tasks from the CPU, improving efficiency in data centers. NVIDIA first popularized the 'CPU+DPU+GPU' architecture in 2020. Cloud Leopard was founded by Stanford PhD Xiao Qiyang in 2020, and Tencent became its largest shareholder before the IPO.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data_processing_unit">Data processing unit - Wikipedia</a></li>
<li><a href="https://blogs.nvidia.com/blog/whats-a-dpu-data-processing-unit/">What Is a DPU? - NVIDIA Blog</a></li>

</ul>
</details>

**Tags**: `#DPU`, `#半导体`, `#IPO`, `#腾讯投资`, `#国产替代`

---

<a id="item-8"></a>
## [China's Cloud & Semiconductor Equipment Exports Surge Over 90% in Early 2025](https://36kr.com/newsflashes/3892797787208449?f=rss) ⭐️ 7.0/10

In the first five months of 2025, China's exports of cloud computing equipment and semiconductor equipment surged by 114.4% and 91.5% year-over-year, respectively, driven by strong AI demand. This significant growth highlights the booming AI industry's impact on upstream manufacturing and global supply chains, and underscores China's strengthening role as a key supplier of critical AI infrastructure components. The surge is linked to the rapid iteration of AI terminal products, where timeliness equates to market share and profits. Air freight routes from China to Europe and America have remained strong despite the typical July lull, buoyed by structural demand for high-tech electronics and semiconductors.

rss · 36氪 · Jul 12, 23:23

**Background**: Artificial intelligence development is accelerating globally, driving demand for computing power from data centers to edge devices. Cloud computing equipment includes servers and networking hardware for AI training and inference, while semiconductor equipment refers to machinery used to manufacture chips. China is a major producer of both types of equipment, and the export growth reflects strong international demand for AI infrastructure.

**Tags**: `#AI`, `#Semiconductors`, `#Cloud Computing`, `#Trade`

---

<a id="item-9"></a>
## [Japan's Hayabusa2 Successfully Flies By Asteroid Torifune](https://www.scmp.com/week-asia/politics/article/3360222/nasa-knows-how-deflect-asteroid-can-japans-hayabusa2-pull-it?utm_source=rss_feed) ⭐️ 7.0/10

Japan's Hayabusa2 probe successfully flew within 800 meters of asteroid Torifune on July 5, 2025, demonstrating precise navigation and operational capabilities for asteroid deflection. This flyby advances planetary defense by showcasing Japan's ability to perform close-proximity operations around asteroids, a key step for future deflection missions. Hayabusa2 performed as expected and responded to all commands from ground control, according to JAXA. The probe had previously returned samples from asteroid Ryugu in 2020.

rss · SCMP · Jul 12, 04:00

**Background**: Asteroid deflection is a key strategy for planetary defense, aiming to alter the trajectory of a potentially hazardous object. The NASA DART mission in 2022 demonstrated a kinetic impact technique. JAXA's Hayabusa2, originally a sample-return mission, is now being used to test precision flyby techniques that could inform future deflection methods.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hayabusa_1_mission">Hayabusa 1 mission</a></li>

</ul>
</details>

**Tags**: `#space exploration`, `#asteroid defense`, `#Hayabusa2`, `#JAXA`, `#planetary protection`

---

<a id="item-10"></a>
## [Tiny Emulators: Cycle-Accurate 8-bit Emulation in JavaScript](https://floooh.github.io/tiny8bit-preview/index.html) ⭐️ 6.0/10

A collection of small, cycle-accurate emulators for classic 8-bit computers and consoles has been re-released as a web demo, implemented entirely in JavaScript. This project demonstrates that pin-level emulation of vintage hardware is feasible in a modern web browser, potentially lowering the barrier for retrocomputing enthusiasts to experiment with low-level emulation. The emulators are cycle-accurate, meaning they replicate the exact timing of the original hardware's machine cycles. The project is at least 8 years old but remains a technical showcase for modular, interface-driven emulation.

hackernews · naves · Jul 12, 20:23 · [Discussion](https://news.ycombinator.com/item?id=48884395)

**Background**: Cycle-accurate emulation is a technique where the emulator replicates the behavior of the original hardware on a per-clock-cycle basis, ensuring precise timing and compatibility. Pin-level emulation takes this further by modeling each physical pin of a chip, allowing highly modular and interchangeable components. The Tiny Emulators project uses this approach to emulate chips like the 6502 CPU and other 8-bit components in JavaScript.

<details><summary>References</summary>
<ul>
<li><a href="https://floooh.github.io/tiny8bit/">Tiny Emulators</a></li>
<li><a href="https://news.ycombinator.com/item?id=43815511">Tiny Emulators | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Higan_(emulator)">higan (emulator) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised the pin-level emulation model for its modularity and flexibility. One user noted the project is over 8 years old, while another warned that some demos have unexpectedly loud volume.

**Tags**: `#emulation`, `#retrocomputing`, `#javascript`, `#8-bit`, `#cycle-accurate`

---

<a id="item-11"></a>
## [Anthropic Clarifies Claude Code: Model Upgrade Isn't Always the Fix](https://36kr.com/p/3892222176574211?f=rss) ⭐️ 6.0/10

Anthropic published an article explaining that upgrading to a larger Claude Code model (like Fable) does not guarantee better results; the Effort setting, which controls how thoroughly the model works, is often the real factor. This clarification helps developers avoid wasting money on unnecessary model upgrades and instead optimize Claude Code's performance by adjusting the Effort setting, which can be more effective and cost-efficient. The Effort setting was silently lowered from high to medium in March 2026 to reduce latency, leading users to believe the model was getting dumber; Anthropic reverted it in April and reset usage quotas. A high Effort setting can produce up to 7x more tokens than low Effort, translating to more thorough file reading, testing, and verification.

rss · 36氪 · Jul 12, 05:47

**Background**: Claude Code is an AI coding agent that operates in the terminal. Its Model setting determines the underlying AI weights (e.g., Claude Fable), which are frozen after training and cannot be changed by user input. The Effort setting dictates how much work the model puts into a task, such as reading multiple files or running tests, independent of the model's inherent capability.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>
<li><a href="https://dev.to/ayyazzafar/claude-code-just-got-smarter-the-effort-parameter-explained-4jlc">Claude Code Just Got Smarter — The Effort ... - DEV Community</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>

</ul>
</details>

**Discussion**: AMD's AI lead Stella Laurenzo analyzed 6,852 session logs and found Claude's thinking tokens dropped 67% after the change, stating it was no longer trustworthy for complex engineering. The community widely criticized the silent change, and Anthropic's response was seen as belated but informative.

**Tags**: `#Claude`, `#AI tools`, `#machine learning`, `#best practices`

---

<a id="item-12"></a>
## [Embodied Data Industry: 97 Players, $6.2B Funding, Who Profits?](https://36kr.com/p/3892027841362694?f=rss) ⭐️ 6.0/10

A 36Kr survey reveals that nearly 100 companies have entered the embodied data industry, with 15 independent data service providers raising a total of 44.7 billion yuan ($6.2 billion) in the past year. The industry has split into four main technical routes: real-robot teleoperation, no-robot collection, simulation synthesis, and internet video distillation. Embodied data is a critical bottleneck for training general-purpose robots, and the emergence of an independent data service sector signals the maturation of the embodied AI ecosystem. With 44.7 billion yuan flowing into pure data players, the race is on to determine which data collection method can achieve the scale and quality needed for real-world deployment. The survey identifies 97 players: 70 in data collection and 27 in data infrastructure. Among collection companies, 31% focus exclusively on real-robot teleoperation, while 43% adopt multiple routes. Notably, 67% of all players are 'embodied-native' startups, whereas infrastructure companies are mostly cross-industry converts from AI data annotation and autonomous driving.

rss · 36氪 · Jul 12, 02:16

**Background**: Embodied data refers to the sensorimotor data (e.g., joint angles, tactile feedback, camera views) required to train robots to perform physical tasks. Current collection methods range from humans teleoperating real robots to using VR setups or extracting motion cues from internet videos. The industry is still early, and no single method has proven sufficient, leading to a fragmented landscape with multiple approaches vying for dominance.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260630A09N6500">《2026中国具身智能数据采集与数据产业发展展望》解读文章-产业链结构...</a></li>
<li><a href="https://developer.nvidia.cn/blog/pico-4-ultra-isaac-teleop-open-robotics/">PICO 展示PICO 4 Ultra支持 NVIDIA Isaac Teleop，共同推进标准化的开...</a></li>
<li><a href="https://www.bilibili.com/video/BV1mkE76GE7u/">从遥操作到数据采集，VR正在成为具身智能训练入口_哔哩哔哩_bilibili TWIST2——全身VR遥操控制：采集人形全身数据后，可训练视觉base的自主... MIT韩松团队突破机器人训练瓶颈：用人类第一视角视频教会机器人「心灵... 基于宇树 G1 的 VR 遥操作与模仿学习开发指南 | 极客日志 MotionTrans：人体VR数据助力机器人操作策略的运动-级学习_机器人数据...</a></li>

</ul>
</details>

**Tags**: `#embodied AI`, `#data collection`, `#robotics`, `#industry analysis`

---

<a id="item-13"></a>
## [Focus on Domestic AI Computing Amid Overseas Tech Volatility](https://36kr.com/newsflashes/3892799853410823?f=rss) ⭐️ 6.0/10

China Merchants Securities released a strategy report recommending focus on domestic AI computing opportunities, citing the upcoming debut of Huawei's Atlas 950 SuperPoD at the World AI Conference. The report notes that recent A-share volatility is partly a reflection of high volatility in overseas tech markets. This signals a shift in investment focus toward domestic AI infrastructure as overseas tech uncertainty rises, potentially boosting Chinese AI hardware stocks. It underscores the strategic importance of self-sufficient AI computing in China's tech ecosystem. Huawei's Atlas 950 SuperPoD, integrated with 64 NPUs per cabinet and capable of scaling to 8,192 NPUs, will be shown as a true machine at the conference. The report also highlights that Hong Kong stock market rebound may be limited without further earnings upgrades or increased AI revenue share from major tech firms.

rss · 36氪 · Jul 12, 23:31

**Background**: SuperPoD (Super Node) is a system-level AI computing architecture that tightly interconnects dozens to hundreds of GPUs via high-bandwidth, low-latency networks to form a 'supercomputer' for large model training. Huawei's Atlas 950 SuperPoD, powered by Ascend chips and UnifiedBus interconnect, is positioned as a competitor to Nvidia's GPU clusters. The World AI Conference (WAIC) is a major event for AI industry showcases in China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/3/mwc-superpod-ai">Huawei Unveiled the Latest SuperPoD, Making an AI Infrastructure New Option to the World - Huawei</a></li>
<li><a href="https://www.techradar.com/pro/huawei-debuts-its-atlas-950-ai-superpod-at-mwc-2026-taking-the-ai-data-center-fight-to-nvidia-and-amd">Huawei debuts its Atlas 950 AI SuperPoD at MWC 2026, taking the AI data center fight to Nvidia and AMD</a></li>
<li><a href="https://news.qq.com/rain/a/20260708A066A900">华为Atlas 950超节点真机亮相WAIC，国产算力从芯片到系统级能力跃升</a></li>

</ul>
</details>

**Tags**: `#finance`, `#AI infrastructure`, `#Chinese tech stocks`, `#investment strategy`, `#Huawei`

---

<a id="item-14"></a>
## [CITIC: AI Hardware Stays Hot, Software Shows Early Recovery](https://36kr.com/newsflashes/3892794471643912?f=rss) ⭐️ 6.0/10

CITIC Securities report finds that A-share computer sector half-year previews, together with overseas model iterations, confirm sustained AI industry chain prosperity, with AI servers and intelligent computing infrastructure showing strong hardware performance, while software and AI application firms begin to see operational recovery and revenue realization. This signals that AI investment is shifting from pure infrastructure to application monetization, impacting investors and tech strategists. The sustained high demand for AI computing hardware validates the ongoing AI arms race, while early software recovery suggests a maturing ecosystem. Overseas models from OpenAI, xAI, and Meta are intensifying focus on agents, coding, multimodality, and office entry points, moving competition from capability verification to high-frequency scenario deployment. This creates resonance for inference-side computing power consumption, infrastructure investment, and AI application commercialization.

rss · 36氪 · Jul 12, 23:16

**Background**: AI agents are software programs powered by large language models that can autonomously pursue goals, use tools, and take actions. Intelligent computing infrastructure (智算基础设施) refers to integrated hardware and software systems encompassing computing, networking, and storage to support AI training and inference. Inference-side computing power consumption is the compute and energy required when a trained model generates outputs, distinct from training.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="http://www.caict.ac.cn/kxyj/qwfb/ztbg/202409/P020241105565523891417.pdf">智算基础设施发展研究报告</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#computing hardware`, `#industry analysis`, `#AI applications`, `#Chinese tech`

---

<a id="item-15"></a>
## [AI Boom Drives Gas Turbine Prices Up 300% in 3 Years](https://36kr.com/newsflashes/3892556678543880?f=rss) ⭐️ 6.0/10

Microsoft recently purchased seven large gas turbines from GE Vernova to power its Texas data center, and according to Melius Research, gas turbine prices have risen by approximately 300% over the past three years. This surge highlights how AI infrastructure's enormous energy demands are driving up costs for traditional power equipment, which could affect data center economics and accelerate the search for alternative power solutions. Each gas turbine costs over $250 million, and GE Vernova's stock has risen more than 70% in the past six months, while competitors like Caterpillar and Siemens also see strong growth.

rss · 36氪 · Jul 12, 11:37

**Background**: Gas turbines are widely used for power generation in industrial settings, including data centers that require reliable, around-the-clock electricity. The AI boom has led to rapid construction of large-scale data centers, sharply increasing demand for gas turbines. However, these complex machines face supply constraints due to long manufacturing lead times and specialized components.

<details><summary>References</summary>
<ul>
<li><a href="https://gasturbineworld.com/behind-the-meter-data-centers/">Data Center developers bypassing grid to obtain... - Gas Turbine World</a></li>
<li><a href="https://en.wikipedia.org/wiki/GE_Vernova">GE Vernova - Wikipedia</a></li>
<li><a href="https://rocketreach.co/melius-research-profile_b44d3570fd2ee3da">Melius Research Information</a></li>

</ul>
</details>

**Tags**: `#AI`, `#data centers`, `#energy`, `#gas turbines`

---

<a id="item-16"></a>
## [CXMT Set for Largest A-Share IPO of the Year on STAR Market](https://36kr.com/newsflashes/3892554879515140?f=rss) ⭐️ 6.0/10

ChangXin Memory Technologies (CXMT) will launch its IPO subscription on the Shanghai Stock Exchange STAR Market on July 16, 2026, aiming to raise 29.5 billion yuan. This IPO will be the largest in the A-share market this year and the second-largest in STAR Market history, underscoring China's push for semiconductor self-sufficiency and providing capital for domestic DRAM production. CXMT is issuing the highest number of shares of any new stock this year, with a subscription cap of 1.672 million shares and a required market value of 16.72 million yuan for maximum allocation.

rss · 36氪 · Jul 12, 11:18

**Background**: The STAR Market, launched in July 2019, is Shanghai's science and technology-focused board, designed to support innovative companies. CXMT is a leading Chinese DRAM manufacturer headquartered in Hefei, specializing in memory chip design and production.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Shanghai_Stock_Exchange_STAR_Market">Shanghai Stock Exchange STAR Market - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#semiconductor`, `#memory chip`, `#A-share market`, `#长鑫科技`

---

<a id="item-17"></a>
## [Phoebe Gates' Startup Phia Accused of Cookie Overwriting](https://www.bloomberg.com/news/videos/2026-07-12/phoebe-gates-startup-draws-tracking-scrutiny-video) ⭐️ 6.0/10

Phoebe Gates' shopping startup Phia was found to overwrite affiliate tracking cookies, potentially redirecting sales commissions from publishers and influencers to itself without user consent. Bloomberg reported the issue, and Phia acknowledged and fixed it, but questions remain about intent and legal consequences. This incident highlights ethical and legal risks in affiliate marketing, where cookie manipulation can undermine trust and damage partnerships. It also draws scrutiny to startups founded by high-profile individuals, raising questions about oversight and business practices. Phia's browser extension reportedly overwrote affiliate tracking cookies during checkout, a practice known as 'cookie stuffing,' which could earn commissions fraudulently. Partners including Impact.com suspended Phia's account after the Bloomberg investigation.

rss · Bloomberg Markets · Jul 12, 14:32

**Background**: Affiliate tracking cookies are small text files stored on a user's browser that record which affiliate (e.g., blogger or influencer) referred a sale. When a purchase occurs within the cookie's validity period, the affiliate earns a commission. Overwriting such cookies, or 'cookie stuffing,' can fraudulently redirect commissions to a different entity, harming legitimate affiliates and merchants.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postaffiliatepro.com/blog/cookie-tracking-affiliate-marketing/">Cookie Tracking in Affiliate Marketing: Complete Guide | Post Affiliate Pro</a></li>
<li><a href="https://mezha.net/eng/bukvy/6aee934a_phia_manipulated_affiliate/">Phia manipulated affiliate cookies, Impact.com suspended the ...</a></li>

</ul>
</details>

**Tags**: `#affiliate marketing`, `#tracking`, `#startup ethics`, `#web cookies`

---

<a id="item-18"></a>
## [AI Trio Dominates Emerging Markets, Worrying Investors](https://www.bloomberg.com/news/articles/2026-07-12/funds-fret-over-4-4-trillion-ai-trio-s-grip-on-emerging-markets) ⭐️ 6.0/10

Investors are rotating away from just three AI technology stocks that, with a combined market capitalization of $4.4 trillion, are driving an outsized share of returns in emerging markets. This concentration highlights the risk of overexposure to a few AI giants in emerging market portfolios, potentially leading to heightened volatility and undermining diversification strategies. The three unnamed stocks collectively worth $4.4 trillion account for a disproportionate share of emerging market returns, prompting fund managers to seek broader exposure beyond AI winners.

rss · Bloomberg Markets · Jul 12, 12:30

**Background**: Concentration risk occurs when a portfolio is heavily weighted in a small number of assets, increasing vulnerability to losses if those assets underperform. Emerging markets are economies of developing countries that often offer high growth but also higher risk. AI stocks have surged recently, making them a dominant force in certain indices.

**Tags**: `#finance`, `#emerging markets`, `#AI stocks`, `#market concentration`, `#investment`

---

<a id="item-19"></a>
## [Robotaxi Ultimatum: Regulatory Pressure Mounts](https://techcrunch.com/2026/07/12/techcrunch-mobility-a-robotaxi-ultimatum/) ⭐️ 6.0/10

TechCrunch Mobility reports on a robotaxi ultimatum, likely involving regulators demanding compliance or industry players facing deadlines. This ultimatum could accelerate regulatory frameworks for autonomous vehicles, impacting companies like Waymo and Cruise, and reshaping urban mobility. The specific details of the ultimatum are not disclosed, but it signals increasing government scrutiny and urgency in the robotaxi sector.

rss · TechCrunch · Jul 12, 16:07

**Background**: Robotaxis are self-driving taxis that operate without human drivers. They are being developed by companies like Waymo and Cruise, but face regulatory hurdles and safety concerns. An ultimatum likely refers to a deadline set by authorities for these companies to meet safety standards or cease operations.

**Tags**: `#robotaxi`, `#AI`, `#autonomous vehicles`, `#transportation`, `#mobility`

---

<a id="item-20"></a>
## [Memory Chip Prices Triple in Shenzhen's Electronics Hub](https://www.scmp.com/tech/tech-trends/article/3360212/chinas-electronics-hub-memory-chip-crisis-hitting-consumers-hard?utm_source=rss_feed) ⭐️ 6.0/10

Memory product prices in Shenzhen's Huaqiangbei electronics hub have tripled over the past year, driven by surging demand from the global AI boom. This price spike is significantly increasing costs for computer builders and consumers in the world's largest wholesale electronics market. This price surge shows how AI-driven demand for memory chips, especially High Bandwidth Memory (HBM) used in AI accelerators, is spilling over into consumer memory markets. It directly impacts DIY PC builders and small electronics businesses, highlighting supply chain pressures from the AI boom. The price increase affects both DRAM and NAND flash memory, with SSDs also becoming major cost drivers in PC builds. Huaqiangbei is a key bellwether for global electronics pricing, making this trend significant for worldwide markets.

rss · SCMP · Jul 12, 05:00

**Background**: Memory chips are essential components in computers, with DRAM used for temporary data storage and NAND flash for persistent storage like SSDs. The AI boom has driven huge demand for High Bandwidth Memory (HBM), a specialized 3D-stacked DRAM used in NVIDIA's AI accelerators, which has tightened overall DRAM supply and raised prices. NAND flash prices have also risen due to increased data center demand for AI training.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@loomy.sjyoo/bandwidth-is-not-coordination-why-hbm-still-isnt-a-brain-87371964be99">Bandwidth Is Not Coordination: Why HBM Still Isn’t a Brain | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/NAND_flash">NAND flash</a></li>
<li><a href="https://grokipedia.com/page/2024_DRAM_and_NAND_flash_price_increases">2024 DRAM and NAND flash price increases</a></li>

</ul>
</details>

**Tags**: `#memory chips`, `#AI boom`, `#hardware pricing`, `#electronics market`, `#supply chain`

---