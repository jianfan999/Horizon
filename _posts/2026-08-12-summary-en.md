---
layout: default
title: "Horizon Summary: 2026-08-12 (EN)"
date: 2026-08-12
lang: en
---

> From 113 items, 26 important content pieces were selected

---

1. [Qwen Releases 2.4T-Parameter MoE Model with Frontier-Level Performance](#item-1) ⭐️ 9.0/10
2. [xAI Releases Grok 4.6, a New Frontier AI Model](#item-2) ⭐️ 9.0/10
3. [Researcher publishes Windows zero-day after Microsoft legal threats](#item-3) ⭐️ 9.0/10
4. [DeepSeek V4 Pro 0813 Released, Sparking Community Testing and Debate](#item-4) ⭐️ 8.0/10
5. [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL Bug](#item-5) ⭐️ 8.0/10
6. [Why Tiny JPEGs Render Differently in Chrome](#item-6) ⭐️ 8.0/10
7. [uBlock Origin Gives Up on Blocking Facebook Ads](#item-7) ⭐️ 8.0/10
8. [Northrop's robot space mechanic makes first satellite thruster attachment attempt](#item-8) ⭐️ 8.0/10
9. [AI Pioneers Defend Open Source Amid Safety and China Competition Debate](#item-9) ⭐️ 8.0/10
10. [Lovable raises $400M at $13.3B valuation on $500M ARR](#item-10) ⭐️ 8.0/10
11. [Zed introduces Delta, a real-time multiplayer environment for agentic coding](#item-11) ⭐️ 7.0/10
12. [Tim King, AmigaDOS Developer and UK Online Founder, Dies](#item-12) ⭐️ 7.0/10
13. [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](#item-13) ⭐️ 7.0/10
14. [Discovered Materials (YC P26) Uses AI Agents to Discover New Chip Materials](#item-14) ⭐️ 7.0/10
15. [Amazon to Train AI on Twitch Streams by Default Unless Opt-Out](#item-15) ⭐️ 7.0/10
16. [AI coding startup Cognition reportedly in talks for $40B valuation](#item-16) ⭐️ 7.0/10
17. [OpenAI-backed Thrive Holdings Raises $2B for Enterprise AI](#item-17) ⭐️ 7.0/10
18. [Form Energy raises $750M to scale 100-hour iron-air batteries](#item-18) ⭐️ 7.0/10
19. [Opaque AI Systems Are the Real Threat to Elections](#item-19) ⭐️ 7.0/10
20. [US-China Science Rift Opens Doors for Singapore, South Korea](#item-20) ⭐️ 7.0/10
21. [YMTC-backed fund invests in SOI Micro to advance FD-SOI chipmaking](#item-21) ⭐️ 7.0/10
22. [2026 Eclipse Webcam Aggregator Gains Traction on Hacker News](#item-22) ⭐️ 6.0/10
23. [Uber Freight Probes Claimed Data Breach by Extortion Gang](#item-23) ⭐️ 6.0/10
24. [Tesla Plans $10B Solar Factory in Texas, Seeks State Incentives](#item-24) ⭐️ 6.0/10
25. [VideoVerse's $250M Acquisition Collapses Amid Fraud Allegations](#item-25) ⭐️ 6.0/10
26. [Tech innovator uses AI to rebuild David Webb’s Hong Kong database](#item-26) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Qwen Releases 2.4T-Parameter MoE Model with Frontier-Level Performance](https://huggingface.co/Qwen/Qwen3.8-2.4T-A95B) ⭐️ 9.0/10

Qwen released Qwen3.8-2.4T-A95B, a Mixture-of-Experts language model with 2.4 trillion total parameters and 95 billion active parameters, available in BF16 and FP8 formats. The model card claims performance competitive with frontier models such as Opus 4.8 and Fable 5. This release significantly pushes the frontier of open-weight MoE models, offering a huge parameter count while keeping inference costs reasonable through sparse activation. The availability of a 1-bit quantized version at roughly 397GB means performance near frontier models could run on a single workstation, attracting broad community interest. The BF16 version is about 4.9TB, while an FP8 version is also provided; an Unsloth 1-bit quantized build is approximately 397GB with 95B active parameters. The open-weight model lacks the vision input, 1M context, and built-in tools of the official Qwen3.8-Max, and its license has revenue-based restrictions similar to Kimi k3.

hackernews · Philpax · Aug 12, 15:01 · [Discussion](https://news.ycombinator.com/item?id=49273478)

**Background**: Mixture-of-Experts (MoE) is a neural network architecture that increases total parameter count while activating only a small subset of expert sub-networks per token, keeping inference costs low. FP8 is an 8-bit floating-point format that reduces memory usage and boosts throughput on modern GPUs like NVIDIA H100 and Blackwell. Quantization to 1-bit can shrink models dramatically, at some quality cost, enabling local deployment on high-end consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@kittikawin_ball/you-dont-need-a-phd-to-understand-mixture-of-experts-here-s-the-intuition-in-plain-english-8972d6e7ad51">You Don’t Need a PhD to Understand Mixture of Experts ... | Medium</a></li>
<li><a href="https://www.emergentmind.com/topics/mixtures-of-experts-moe">Mixtures of Experts ( MoE ) in Neural Models</a></li>
<li><a href="https://medium.com/@StackGpu/fp8-bf16-and-int8-how-low-precision-formats-are-revolutionizing-deep-learning-throughput-e6c1f3adabc2">FP8, BF16, and INT8: How Low-Precision Formats Are Revolutionizing Deep Learning Throughput | by StackGpu | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters were excited that the 1-bit quantized model (397GB) could bring Opus 4.5-level performance to a machine a normal person can buy, but noted serving the bf16/fp8 release is hard and no QAT is available for q4. Some compared it to Kimi k3 and referenced DeepSeek V4-Pro benchmarks, while others were disappointed that the open model lacks vision and 1M context; one joked about running it on an Intel N100.

**Tags**: `#AI`, `#LLM`, `#Qwen`, `#MoE`, `#model release`

---

<a id="item-2"></a>
## [xAI Releases Grok 4.6, a New Frontier AI Model](https://x.ai/news/grok-4-6) ⭐️ 9.0/10

xAI has released Grok 4.6, a new frontier AI model, announced on its official site x.ai. The release comes amid strong community discussion about its API behavior, performance, and competitive positioning against models like GPT-5.6-Sol and Kimi K3. Grok 4.6 represents xAI's continued push into frontier AI, intensifying competition among major AI labs. If community comparisons hold, it could offer a compelling price-to-performance alternative for developers, especially through integrations like Cursor. Community members describe Grok 4.6 as 'Fable-like' in intelligence, beating GPT-5.6-Sol on most benchmarks and being cheaper than Kimi K3 via API. One user reports the API injects a default system prompt that can override user instructions and cause refusals to discuss system prompts.

hackernews · iLuddite · Aug 12, 15:32 · [Discussion](https://news.ycombinator.com/item?id=49274027)

**Background**: Grok is an AI chatbot developed by xAI (also referred to as SpaceXAI), built on a large language model architecture designed to compete with OpenAI's GPT and Google's Gemini. 'Frontier AI' refers to general-purpose, powerful AI models at the leading edge of capabilities, which are often the focus of intense competition and governance discussions. The new Grok 4.6 release continues xAI's expansion of its Grok model family and its investment in inference capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_(chatbot)">Grok (chatbot) - Wikipedia</a></li>
<li><a href="https://x.ai/">SpaceXAI — Creators of Grok, the AI Chatbot</a></li>
<li><a href="https://www.igmguru.com/blog/what-is-grok-ai">What is Grok AI: How Does It Work and Useful Features | igmGuru</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: many praise Grok 4.6's performance, speed, and value, with one user calling it a 'healthy competition' to other labs. However, others raise concerns about API system-prompt behavior that can override user instructions, and some express skepticism about how quickly all major labs achieved 'Fable-level' models, suggesting possible distillation or benchmark manipulation.

**Tags**: `#AI`, `#Grok`, `#xAI`, `#language models`, `#frontier AI`

---

<a id="item-3"></a>
## [Researcher publishes Windows zero-day after Microsoft legal threats](https://techcrunch.com/2026/08/12/after-microsoft-threatened-legal-action-a-security-researcher-publishes-a-new-windows-zero-day-bug/) ⭐️ 9.0/10

Security researcher Nightmare Eclipse has published a new Windows zero-day vulnerability, defying Microsoft's public threats of legal action over prior disclosures. This incident highlights the growing tension between security researchers and software vendors over vulnerability disclosure practices. The publication of a Windows zero-day can affect millions of users and raises questions about the legal limits of security research. The researcher, known as Nightmare Eclipse, has released multiple zero-day vulnerabilities, and Microsoft has accused them of failing to follow responsible disclosure practices. The actual technical impact and affected Windows versions have not yet been detailed in the article.

rss · TechCrunch · Aug 12, 15:18

**Background**: A zero-day vulnerability is an undiscovered flaw in software that the vendor has zero days to fix because no patch exists. Typically, security researchers follow a responsible disclosure model, where they privately report flaws and allow the vendor time to patch before going public. This dispute centers on the conflict between legal threats and the public interest in disclosing security flaws.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Coordinated_vulnerability_disclosure">Coordinated vulnerability disclosure - Wikipedia</a></li>
<li><a href="https://www.cisa.gov/resources-tools/programs/coordinated-vulnerability-disclosure-program">Coordinated Vulnerability Disclosure Program - CISA</a></li>

</ul>
</details>

**Tags**: `#security`, `#zero-day`, `#Windows`, `#vulnerability`, `#disclosure`

---

<a id="item-4"></a>
## [DeepSeek V4 Pro 0813 Released, Sparking Community Testing and Debate](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 8.0/10

DeepSeek released a preview version of DeepSeek-V4-Pro (0813), a 1.6-trillion-parameter Mixture-of-Experts model with 49B activated parameters and a 1M-token context window, now available via OpenRouter at $0.435 per million input tokens and $0.87 per million output tokens. This release continues DeepSeek's pattern of offering large open-weight models at very low cost, challenging incumbent frontier models on price-performance. Early community tests show competitive coding outputs at a fraction of the cost of rivals like Grok 4.6, which could pressure pricing and adoption across AI developer tools. The model is a preview, part of the V4 series alongside V4-Flash (284B total, 13B active), both supporting one million tokens of context. Community benchmarks show mixed results: one user found a bug after $0.12 spend, another noted issues in Docker Compose generation compared to gpt-5.6-terra-high, and Simon Willison reported an image-rendering bug.

hackernews · explosion-s · Aug 12, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49274600)

**Background**: DeepSeek is a Chinese generative AI lab whose R1 model topped the US App Store in January 2025, known for open weights, energy efficiency, and competitive pricing, though it has faced scrutiny over censorship and privacy. V4-Pro is a Mixture-of-Experts model—only a fraction of its parameters are active per token—which helps keep inference costs low, and its 1M-token context supports long-input tasks like repository analysis.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro">DeepSeek V4 Pro - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(product)">DeepSeek (product)</a></li>

</ul>
</details>

**Discussion**: Comments show active hands-on testing and debate: Palmik criticized the OpenRouter link as unhelpful, suggesting official docs and benchmarks instead; performance reports are mixed, with jklmnopqrstuvw finding DeepSeek slower (12 min vs 3 min) and buggier than Grok 4.6 but roughly 10x cheaper, while freakynit found it worse than gpt-5.6-terra-high on a dev-ops task; alecsm praised the new Flash for handling heavy development "for peanuts," and simonw shared a rendering bug example.

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#model release`, `#coding`

---

<a id="item-5"></a>
## [Tailscale Traces Database Corruption to 16-Year-Old SQLite WAL Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 8.0/10

Tailscale published a detailed post-mortem revealing that database corruption in its control plane was caused by a 16-year-old SQLite WAL-reset race condition. The company funded an open-source VFS shim that helped isolate the bug and can aid future debugging. The case shows that even mature, heavily tested software like SQLite can harbor subtle concurrency bugs for over a decade. It also highlights a valuable pattern of companies funding open-source debugging infrastructure that benefits the broader developer community. The race occurs when SQLite resets or clears the WAL file while another connection still needs it, and it can happen even with a single-writer design. Tailscale funded a new VFS shim specifically as a debugging tool rather than only patching the immediate symptom.

hackernews · ropbear · Aug 12, 14:22 · [Discussion](https://news.ycombinator.com/item?id=49272832)

**Background**: SQLite is an embedded SQL database often used in applications and services. In WAL (Write-Ahead Logging) mode, changes are appended to a separate WAL file before being checkpointed into the main database, which allows concurrent readers during writes. A VFS is SQLite's OS interface layer, and a VFS shim wraps another VFS to add behavior such as logging or checksums. Tailscale used such a shim to observe and isolate the WAL-reset race that caused corruption.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/vfs.html">The SQLite OS Interface or "VFS"</a></li>
<li><a href="https://blog.pecar.me/sqlite-wal/">SQLite Write-Ahead Logging | Anže's Blog</a></li>
<li><a href="https://til.simonwillison.net/sqlite/enabling-wal-mode">Enabling WAL mode for SQLite database files | Simon Willison’s TILs</a></li>

</ul>
</details>

**Discussion**: Commenters praised the write-up as a satisfying deep dive and appreciated that Tailscale funded open-source debugging tooling. Some noted the article took a while to get to the point, while others expressed hope that Tailscale continues its SQLite support contract.

**Tags**: `#sqlite`, `#tailscale`, `#database`, `#bug`, `#open-source`

---

<a id="item-6"></a>
## [Why Tiny JPEGs Render Differently in Chrome](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

The article explains that Chrome uses a specific downscaling algorithm that renders tiny JPEGs differently compared to other browsers, and offers practical advice on choosing appropriate image resolutions and formats. This matters because cross-browser image rendering inconsistencies can break UI designs, especially for icons and small graphics, affecting many web developers and users. Understanding the root cause helps developers choose better formats and sizes. Chrome's downscaling algorithm resizes images to a power-of-two smaller size before rendering when CPU rasterization is used, which can cause blurriness. The article advises against using JPEG for icons and suggests using appropriate resolution images; Firefox also has a bug report for lower-scale decompression.

hackernews · gutechh · Aug 12, 14:00 · [Discussion](https://news.ycombinator.com/item?id=49272549)

**Background**: Browsers use different image resampling algorithms (such as bilinear, bicubic, or Lanczos) when downscaling images, which can cause visible differences across browsers. Chrome in particular applies an optimization that downsizes large images to power-of-two sizes to save memory, but this can hurt quality for small images. Developers can sometimes control the scaling algorithm using the CSS image-rendering property.

<details><summary>References</summary>
<ul>
<li><a href="https://groups.google.com/a/chromium.org/g/chromium-discuss/c/vdL7dm-I2fA">Does Chrome load downscaled JPEGs when GPU rasterisation is disabled?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Image_scaling">Image scaling - Wikipedia</a></li>
<li><a href="https://bugzilla.mozilla.org/show_bug.cgi?id=486918">486918 - Add an option to use high-quality downscaling for images</a></li>

</ul>
</details>

**Discussion**: Commenters noted the same issue affects PNGs, and that using a 2000x2000 image for a 20x20 icon is wasteful regardless of format. One commenter linked to a Firefox bug for lower-scale decompression, while another mentioned CSS image-rendering as a potential control, and a third noted Firefox tends to be sharper with more ringing artifacts.

**Tags**: `#browsers`, `#image-scaling`, `#jpeg`, `#frontend`, `#web-performance`

---

<a id="item-7"></a>
## [uBlock Origin Gives Up on Blocking Facebook Ads](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

uBlock Origin, the popular open-source ad blocker, has stopped filtering ads on Facebook because the platform's obfuscation techniques have become too difficult to keep up with. The decision effectively concedes this front in the ad-blocking arms race to Facebook. Facebook users who rely on uBlock Origin will now see more ads, and the move signals that even the most popular community-driven ad blockers can be outmatched by a determined platform. It may push users toward alternative ad-blocking strategies, such as DNS-level filtering or future AI-based detection. Facebook's anti-adblocking measures rely on aggressive code obfuscation, making it impractical for filter lists to keep pace. The project's maintainers apparently made the call after community discussion, and the decision affects both desktop and mobile browsers that use uBlock Origin.

hackernews · Markoff · Aug 12, 11:28 · [Discussion](https://news.ycombinator.com/item?id=49270726)

**Background**: uBlock Origin is a free, open-source browser extension for content filtering and ad blocking, available for Firefox and Chromium-based browsers. Ad blockers work by matching requests and page elements against filter lists maintained by the community. Obfuscation in this context means deliberately concealing or distorting ad code so that it cannot be easily identified by static filters, forcing blockers into a continuous cat-and-mouse game.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://www.cs.princeton.edu/~arvindn/publications/ad-blocking-framework-techniques.pdf">The Future of Ad Blocking</a></li>
<li><a href="https://ublockorigin.com/">uBlock Origin - Free, open-source ad blocker extension</a></li>

</ul>
</details>

**Discussion**: Commenters in the Reddit thread had mixed reactions: some agreed that stopping is the correct decision given Facebook's relentless obfuscation, while others predicted the eventual solution would be a computer vision model that visually detects ads. One user expressed long-standing frustration with the cat-and-mouse dynamic and questioned the end goal of evading ad blockers, while another fondly recalled early ad blockers that replaced ads with artwork.

**Tags**: `#ad-blocking`, `#uBlock Origin`, `#Facebook`, `#privacy`, `#tech arms race`

---

<a id="item-8"></a>
## [Northrop's robot space mechanic makes first satellite thruster attachment attempt](https://techcrunch.com/2026/08/12/northrops-robot-space-mechanic-is-a-new-way-to-keep-satellites-at-work-longer/) ⭐️ 8.0/10

Northrop Grumman's Mission Robotic Vehicle (MRV) is making the first attempt to attach a new thruster to an aging satellite. This pioneering on-orbit servicing mission aims to extend the satellite's operational life. This milestone could revolutionize satellite maintenance by providing a cost-effective alternative to launching replacement satellites. Success would help reduce space debris and extend the value of existing space assets for operators. The MRV builds on Northrop Grumman's previous Mission Extension Vehicles (MEV), which have successfully serviced two Intelsat communications satellites. The vehicle is designed for inspection, repair, and life-extension missions, and could also operate in low Earth orbit (LEO).

rss · TechCrunch · Aug 12, 20:53

**Background**: On-orbit satellite servicing refers to refueling, boosting, or repairing satellites while in space. Traditionally, satellites that run out of fuel or malfunction are decommissioned, contributing to space debris. New commercial interest has grown due to lower launch costs and the rise of low Earth orbit constellations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/On-orbit_satellite_servicing">On-orbit satellite servicing</a></li>
<li><a href="https://satelliteprome.com/news/northrop-grumman-to-launch-robotic-arm-mrv-by-2026/">Northrop Grumman to launch robotic arm MRV by... - SatellitePro ME</a></li>
<li><a href="https://www.northropgrumman.com/what-we-do/space/satellite-services-in-space">Satellite Services in Space: Extending Life in Orbit | Northrop Grumman</a></li>

</ul>
</details>

**Tags**: `#space`, `#robotics`, `#satellite`, `#aerospace`

---

<a id="item-9"></a>
## [AI Pioneers Defend Open Source Amid Safety and China Competition Debate](https://techcrunch.com/2026/08/12/as-ai-safety-concerns-mount-three-pioneers-make-the-case-for-staying-open/) ⭐️ 8.0/10

At the Ai4 conference, Geoffrey Hinton, Fei-Fei Li, and Andrew Ng debated AI regulation and open source access, making the case for staying open even as safety concerns mount. This discussion reflects a pivotal tension in AI policy between safety and innovation, with potential to shape regulation and international competitiveness. The views of these three pioneers could influence both industry practice and government policy. Hinton, often called a 'godfather of AI,' has previously voiced serious concerns about AI risks, while Li and Ng have emphasized open research and development. Their debate at Ai4 focused on how the U.S. can compete as China advances in AI.

rss · TechCrunch · Aug 12, 17:51

**Background**: AI safety concerns have grown as powerful AI systems become more capable, leading to calls for regulation and even closed development. Open source advocates argue that transparency accelerates research and distributes power, while critics worry about misuse. Hinton, Li, and Ng are among the most influential figures in AI, and their positions carry significant weight in policy debates.

**Tags**: `#AI safety`, `#regulation`, `#open source`, `#AI policy`

---

<a id="item-10"></a>
## [Lovable raises $400M at $13.3B valuation on $500M ARR](https://techcrunch.com/2026/08/12/lovable-confirms-new-13-3b-valuation-raises-another-400m/) ⭐️ 8.0/10

Lovable has raised an additional $400 million at a $13.3 billion valuation, confirming the new round after reaching $500 million in annualized run rate revenue in June. The funding marks a major milestone for the Swedish AI startup. The round underscores the explosive growth of AI-powered 'vibe coding' tools and makes Lovable one of the fastest-scaling software startups ever, now valued at $13.3 billion just two years after launching. It also signals strong investor confidence in European AI startups and the broader AI app-building ecosystem. Lovable's valuation has more than doubled from $6.6 billion in December 2025, itself a tripling in less than six months at the time. The company previously raised a $15 million round in February 2025 and claims to be nearing 8 million users.

rss · TechCrunch · Aug 12, 16:04

**Background**: Lovable is a Swedish AI startup that allows users to create web applications simply by using natural-language prompts, a practice often called 'vibe coding'. It gained widespread attention after reaching the front pages of Product Hunt and Hacker News, and has since become one of the fastest-growing software companies in history. The 'vibe coding' movement leverages large language models to generate code, making app development accessible to non-programmers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/aliciapark/2025/12/19/ai-startup-lovable-just-minted-one-of-europes-youngest-ever-self-made-billionaires/">AI Startup Lovable Just Minted One Of Europe’s Youngest Ever Self-Made Billionaires</a></li>
<li><a href="https://techcrunch.com/2025/02/25/swedens-lovable-an-app-building-ai-platform-rakes-in-16m-after-spectacular-growth/">Sweden's Lovable, an app-building AI platform, rakes in $15M after spectacular growth | TechCrunch</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lovable_(company)">Lovable (company) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#funding`, `#startup`, `#valuation`, `#Lovable`

---

<a id="item-11"></a>
## [Zed introduces Delta, a real-time multiplayer environment for agentic coding](https://zed.dev/blog/introducing-delta) ⭐️ 7.0/10

Zed has announced Delta, a multiplayer environment for coding with AI agents, built on its new Git-compatible version control system called DeltaDB. In Delta, every edit and conversation between commits is recorded, while teammates who never open Delta still see a normal Git repository. Delta pushes the idea of real-time collaboration deeper into the coding workflow by extending it to agent conversations and version control. It could change how teams review AI-generated code, mentor junior developers, and audit how a result was produced—though commentators are split on whether multiplayer coding is truly useful. DeltaDB is a Git-compatible version control system that captures all edits and agent conversations between commits, so the full history of an agent's work is inspectable. Delta also builds on Zed's existing collaborative features, including remote development, multibuffer editing, and parallel agents.

hackernews · khy · Aug 12, 18:19 · [Discussion](https://news.ycombinator.com/item?id=49276574)

**Background**: Zed is a high-performance code editor written in Rust, known for its speed and built-in real-time collaboration. DeltaDB is a new Git-compatible version control layer from Zed Industries, and Delta is the collaborative agentic editor it powers. As AI agents start writing more code, tools like Delta aim to keep human oversight and collaboration at the center of the workflow.

<details><summary>References</summary>
<ul>
<li><a href="https://zed.dev/blog/introducing-delta">Introducing Delta — Zed 's Blog</a></li>
<li><a href="https://runtimewire.com/article/zed-deltadb-version-control-agent-conversations">Nathan Sobo's Zed takes aim at pull requests with... - RuntimeWire</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some commenters dismiss multiplayer coding as unnecessary since coding feels like a single-player activity, while others see value in mentoring junior engineers and inspecting agent-driven PRs. There are also technical complaints about verbose LLM summaries that skip edge cases, and an off-topic criticism of the blog page's low-contrast design.

**Tags**: `#Zed`, `#collaborative editing`, `#developer tools`, `#real-time`

---

<a id="item-12"></a>
## [Tim King, AmigaDOS Developer and UK Online Founder, Dies](https://amiga-news.de/en/news/AN-2026-08-00070-EN.html) ⭐️ 7.0/10

Tim King, the developer of AmigaDOS and founder of UK Online, has passed away, according to a tribute posted on amiga-news.de. His death prompted an outpouring of reflective tributes from the retro-computing community. Tim King's work on AmigaDOS shaped the Amiga computer's operating system, which influenced a generation of programmers and enthusiasts. His passing highlights the lasting legacy of early computing pioneers and the importance of preserving software history. AmigaDOS is the disk operating system component of AmigaOS, originally based on a TRIPOS port by MetaComCo and written in BCPL. It was later rewritten in C starting with AmigaOS 2.x, and AmigaOS 4.x added 64-bit file access; King also founded the UK ISP UK Online.

hackernews · doener · Aug 12, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49272655)

**Background**: The Amiga, introduced by Commodore in 1985, was a pioneering personal computer known for its multimedia capabilities and preemptive multitasking AmigaOS. AmigaDOS provided the command-line interface and file system management, acting as the 'DOS' layer of the system. Tim King was credited as a key developer of AmigaDOS in its early TRIPOS/BCPL form, and later became an internet entrepreneur in the UK.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AmigaDOS">AmigaDOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga_Operating_System">Amiga Operating System</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal memories and gratitude: one recalled stripping AmigaOS down to boot directly into AmigaDOS, another credited it as a 'gateway drug' to the Linux CLI, while others remembered King as a friendly founder of UK Online. A commenter also linked to a 2021 interview with King.

**Tags**: `#Amiga`, `#obituary`, `#retro-computing`, `#AmigaDOS`, `#software-history`

---

<a id="item-13"></a>
## [HTML over WebSockets: Real-Time SPAs with Minimal JavaScript](https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/) ⭐️ 7.0/10

The article by Andros Fenollosa explores the HTML-over-WebSockets pattern for building real-time single-page applications, where the server sends rendered HTML over a persistent WebSocket connection to minimize JavaScript. It compares this approach with Server-Sent Events (SSE) and traditional server-rendered applications. This pattern challenges the JavaScript-heavy SPA paradigm by offering a simpler, potentially more secure architecture with less client-side complexity. It aligns with the growing trend of server-centric frameworks like Phoenix LiveView, Django LiveView, and htmx, potentially influencing how developers choose their tools for real-time web apps. The pattern relies on a permanent bidirectional channel, similar to Phoenix LiveView or Django LiveView, where the server sends HTML fragments. The article also notes that WebSockets are best for bidirectional, low-latency communication such as chat or games, while SSE is simpler and cheaper to operate for one-way server pushes.

hackernews · redbell · Aug 12, 16:51 · [Discussion](https://news.ycombinator.com/item?id=49275335)

**Background**: In the traditional SPA model, a JavaScript framework handles data fetching, state management, and DOM updates, resulting in large client-side bundles. The HTML-over-WebSockets pattern moves rendering back to the server: the server sends complete HTML over a WebSocket, and the client swaps it into the DOM. This reduces JavaScript to a small WebSocket client and can simplify logic and improve security by centralizing rendering on the server. Libraries like htmx and frameworks like Phoenix LiveView popularize this server-centric approach.

<details><summary>References</summary>
<ul>
<li><a href="https://en.andros.dev/blog/ef4968f5/html-over-websockets-real-time-spas-with-barely-any-javascript/">HTML over WebSockets : real - time SPAs with... | Andros Fenollosa</a></li>
<li><a href="https://htmx.org/">htmx - high power tools for html</a></li>
<li><a href="https://rxdb.info/articles/websockets-sse-polling-webrtc-webtransport.html">WebSockets vs Server-Sent-Events vs Long-Polling vs WebRTC vs WebTransport | RxDB</a></li>

</ul>
</details>

**Discussion**: Commenters largely appreciate the historical context (Chris McCord's earlier 'Sync' for Rails) but push back on some claims. Several argue SSE (not WebSockets) suffices for most one-way realtime needs, and htmx with SSE and DOM morphing already provides this pattern. One commenter strongly disagrees that HTML over WebSockets is inherently more XSS-safe, noting the client still interprets HTML.

**Tags**: `#web-development`, `#websockets`, `#real-time`, `#server-sent-events`, `#htmx`

---

<a id="item-14"></a>
## [Discovered Materials (YC P26) Uses AI Agents to Discover New Chip Materials](https://discoveredmaterials.com/research/) ⭐️ 7.0/10

Discovered Materials, a Y Combinator-backed startup, launched on Hacker News, presenting AI agents that computationally discover new semiconductor materials. The team says they tested 7 frontier models from Anthropic, OpenAI, and Kimi, releasing hundreds of newly discovered materials and a benchmark, and they have already synthesized thermal interface materials that match the performance of trade secrets guarded by large chemical companies for over 20 years. This directly targets the growing heat dissipation crisis in GPUs, where TDP is nearly doubling each generation and datacenter cooling consumes enormous power and water. If AI agents can meaningfully shorten the 'lab-to-fab' materials timeline, it could accelerate advanced packaging techniques like HBM-on-logic and unlock large energy-efficiency gains across the semiconductor industry. The team cites GPU TDP rising from 700 W (H100) to 1.2 kW (Blackwell), with Rubin expected at 2.3 kW, and points to poor thermal conductors like SiO2 in HBM stacks as a key bottleneck for 3D packaging. They also release a benchmark and hundreds of discovered materials, while acknowledging that models still struggle with synthesis recipes, yet claim their first 3 months in the YC batch produced TIMs matching trade-secret performance.

hackernews · advaith08 · Aug 12, 07:51 · [Discussion](https://news.ycombinator.com/item?id=49269090)

**Background**: Thermal Design Power (TDP) is the maximum heat a chip can produce that its cooling system must dissipate, and it has become a critical constraint as GPUs grow more powerful. High Bandwidth Memory (HBM) is a 3D-stacked memory interface that places memory dies vertically; stacking HBM directly on logic could cut data-moving energy by 10–50×, but thermal issues currently block it. The 'lab-to-fab valley of death' describes the years and hundreds of millions of dollars typically required to bring a new material from discovery to manufacturing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Thermal_design_power">Thermal design power - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were cautiously optimistic, praising the team for addressing whether discovered materials are actually synthesizable — a step often missing in AI-driven materials discovery. Skeptics like timr questioned how truly novel compounds can be found if they already appear in model training data, while foven noted the gap between plausible synthesis and real-world cost. Others shared related research and suggested alternative architectures like HBM on the back side of the chip.

**Tags**: `#AI agents`, `#materials discovery`, `#semiconductors`, `#thermal management`, `#YC startup`

---

<a id="item-15"></a>
## [Amazon to Train AI on Twitch Streams by Default Unless Opt-Out](https://techcrunch.com/2026/08/12/amazon-will-train-on-twitch-streamers-content-by-default-unless-they-opt-out/) ⭐️ 7.0/10

Twitch, owned by Amazon, will by default use streamers' content for AI training unless creators explicitly opt out. Chief Product Officer Mike Minton admitted on a livestream that the policy is opt-out by design because opt-in would fail. This policy raises significant ethical and privacy concerns for the large Twitch creator community, shifting the burden of consent onto individual streamers. It also sets a precedent for how platforms may treat user-generated content in AI training without upfront permission. The CPO's candid remark confirms that the opt-out default is intentional, acknowledging that an opt-in model would not gain traction. No specific details were provided about which content types are used or how the opt-out process works.

rss · TechCrunch · Aug 12, 20:10

**Background**: Twitch is a livestreaming platform owned by Amazon, where millions of creators broadcast gameplay, chats, and creative content. AI training often relies on vast amounts of user-generated data, and companies have increasingly used such content to improve models. A default opt-out policy means users must take proactive steps to prevent their content from being used, which many argue is a less ethical form of consent than opt-in.

**Tags**: `#AI ethics`, `#data privacy`, `#Twitch`, `#Amazon`, `#content licensing`

---

<a id="item-16"></a>
## [AI coding startup Cognition reportedly in talks for $40B valuation](https://techcrunch.com/2026/08/12/ai-coding-startup-cognition-reportedly-already-in-talks-to-raise-at-40b-valuation/) ⭐️ 7.0/10

Cognition is reportedly in talks to raise a new funding round at a $40 billion valuation, just months after closing a $1 billion round at a $26 billion valuation. This rapid valuation jump underscores the intense investor demand for AI coding agents and could signal a continued boom in AI developer tools. It also places Cognition among the most valuable private AI startups. The report does not specify the amount being raised or lead investors. If completed, the new valuation would represent a roughly 54% increase from the $26 billion valuation just a few months prior.

rss · TechCrunch · Aug 12, 18:19

**Background**: Cognition is an American AI company based in San Francisco, known for Devin, an AI software engineer that can autonomously complete coding tasks. The company has drawn both praise and skepticism from software engineers, and its rapid succession of mega-rounds reflects the broader AI coding gold rush.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cognition_AI">Cognition AI - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Devin_AI">Devin AI - Wikipedia</a></li>
<li><a href="https://cognition.com/blog/introducing-devin">Introducing Devin , the first AI software engineer | Cognition</a></li>

</ul>
</details>

**Tags**: `#AI`, `#startups`, `#funding`, `#coding tools`

---

<a id="item-17"></a>
## [OpenAI-backed Thrive Holdings Raises $2B for Enterprise AI](https://techcrunch.com/2026/08/12/openai-backed-thrive-holdings-raises-2b-to-bring-ai-to-the-enterprise/) ⭐️ 7.0/10

Thrive Holdings, backed by OpenAI, raised $2 billion in new funding at a $12 billion valuation. The round included investors such as SoftBank, D1 Capital Partners, and Altimeter Capital. This large funding round signals strong investor confidence in OpenAI-backed enterprise AI solutions. It could accelerate the deployment of AI technologies across businesses and intensify competition in the enterprise AI market. The $2 billion raise values Thrive Holdings at $12 billion, a significant valuation for a company focused on bringing AI to the enterprise. The specific products or services were not detailed in the announcement.

rss · TechCrunch · Aug 12, 17:41

**Background**: Enterprise AI refers to the use of artificial intelligence technologies within organizations to improve efficiency, decision-making, and automation. Startup funding rounds typically involve private investors providing capital in exchange for equity or other ownership stakes. OpenAI's backing indicates a strategic relationship that may involve technical collaboration or preferred access to AI models.

**Tags**: `#funding`, `#enterprise AI`, `#OpenAI`, `#AI infrastructure`

---

<a id="item-18"></a>
## [Form Energy raises $750M to scale 100-hour iron-air batteries](https://techcrunch.com/2026/08/12/form-energy-raises-750m-to-build-more-100-hour-batteries-for-the-grid/) ⭐️ 7.0/10

Form Energy announced a $750 million funding round to expand manufacturing of its 100-hour iron-air grid batteries. Google and Crusoe are named as anchor customers for the technology. This is one of the largest investments in long-duration energy storage, signaling that multi-day batteries are moving from pilot to commercial scale. It will help grid operators integrate more renewable energy while reducing reliance on lithium-ion for long discharge durations. Form Energy's first commercial product is an iron-air battery that can discharge for 100 hours, using a 'reverse rusting' reaction. The new capital will go toward expanding manufacturing capacity to deliver these grid-scale batteries to customers.

rss · TechCrunch · Aug 12, 16:18

**Background**: Long-duration energy storage (LDES) refers to systems that discharge electricity for 10 hours or more, supporting grid reliability and renewable integration. Form Energy's iron-air battery chemistry stores energy in iron and releases it through controlled oxidation, offering a cheaper alternative to lithium-ion for multi-day storage. The company, spun out of MIT, has been developing this technology for several years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Long-duration_energy_storage">Long-duration energy storage</a></li>
<li><a href="https://formenergy.com/technology/battery-technology/">Battery Technology | Form Energy</a></li>
<li><a href="https://orennia.com/insights/form-energy-and-the-100-hr-battery">Form Energy and its 100-Hour Battery | Orennia</a></li>

</ul>
</details>

**Tags**: `#energy storage`, `#climate tech`, `#grid infrastructure`, `#funding`, `#clean energy`

---

<a id="item-19"></a>
## [Opaque AI Systems Are the Real Threat to Elections](https://restofworld.org/2026/ai-elections-deepfake-voter-chatbot/?utm_source=rss&utm_medium=rss&utm_campaign=feeds) ⭐️ 7.0/10

Rest of World article warns that deepfakes overshadow a more dangerous reality: opaque AI systems embedded in election infrastructure. The piece, by Lisa Poggiali and Samson Itodo, argues these systems can distort election integrity without public scrutiny. This reframes the AI-and-elections debate from flashy generative AI content to the mundane, often invisible machinery that actually runs elections. Because these opaque systems make consequential decisions, their lack of transparency could erode voter trust and democratic accountability. The authors include Lisa Poggiali, chief AI adviser at the International Foundation for Electoral Systems (IFES), lending institutional weight to the argument. The term “opaque” refers to so-called black-box AI, where internal decision-making remains hidden even from system developers.

rss · Rest of World · Aug 12, 10:00

**Background**: Deepfakes – realistic synthetic media generated by AI – have captured public attention as an election threat. Yet AI is increasingly embedded in election processes, offices, and vendor systems, where it affects how elections are run. Opaque AI systems, unlike deepfakes, make decisions that directly shape electoral outcomes without transparent logic. This creates risks of bias, errors, and manipulation that are far harder to spot than a viral video.

<details><summary>References</summary>
<ul>
<li><a href="https://restofworld.org/2026/ai-elections-deepfake-voter-chatbot/">Why we should all worry about AI in elections - Rest of World</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_intelligence_and_elections">Artificial intelligence and elections - Wikipedia</a></li>
<li><a href="https://ash.harvard.edu/resources/the-role-of-ai-in-the-2024-elections/">The Role of AI in the 2024 Elections – Ash Center</a></li>

</ul>
</details>

**Tags**: `#AI`, `#elections`, `#deepfakes`, `#AI governance`, `#ethics`

---

<a id="item-20"></a>
## [US-China Science Rift Opens Doors for Singapore, South Korea](https://www.scmp.com/news/china/diplomacy/article/3363767/singapore-and-south-korea-eye-science-opportunities-last-main-us-china-link-shatters?utm_source=rss_feed) ⭐️ 7.0/10

The United States is imposing new security-related restrictions on federally funded research collaborations with Chinese institutions, effectively closing one of the last remaining openings between Washington and Beijing. Singapore and South Korea are positioning themselves to capture new research opportunities as a result. This marks a significant geopolitical shift in international scientific collaboration, potentially redrawing global research networks and funding flows. Researchers, universities, and companies worldwide could be affected as traditional US-China partnerships are replaced or relocated. The restrictions target federally funded collaborations with Chinese institutions, representing the latest and most consequential step in a years-long US-China decoupling effort. The context includes President Xi Jinping's planned summit with Donald Trump in Washington next month.

rss · SCMP · Aug 12, 22:00

**Background**: Scientific research has been one of the most durable links in the US-China relationship, persisting even as trade and political frictions escalated. The new security-related restrictions now threaten this last significant connection, prompting regional players such as Singapore and South Korea to eye new roles as research hubs or intermediaries.

**Tags**: `#geopolitics`, `#science policy`, `#US-China relations`, `#research collaboration`

---

<a id="item-21"></a>
## [YMTC-backed fund invests in SOI Micro to advance FD-SOI chipmaking](https://www.scmp.com/tech/article/3363797/fund-backed-china-memory-giant-ymtc-invests-push-alternative-chipmaking-route?utm_source=rss_feed) ⭐️ 7.0/10

A venture capital fund backed by Yangtze Memory Technologies Co (YMTC) has taken a stake in SOI Micro, a Chinese semiconductor maker focused on FD-SOI technology. The investment adds a prominent backer to China's push for an alternative chipmaking ecosystem. FD-SOI offers a low-power alternative to mainstream finFET processes, potentially reducing dependence on advanced node equipment. This investment signals China's strategy to pursue diversified chipmaking routes amid export controls and global semiconductor competition. FD-SOI uses a buried oxide layer and thin silicon film to reduce leakage and lower power consumption. SOI Micro is led by a prominent figure in China's semiconductor industry, though specific financial terms were not disclosed.

rss · SCMP · Aug 12, 13:00

**Background**: FD-SOI, or fully depleted silicon-on-insulator, is a planar process technology that creates transistors with a thin silicon film atop an insulating buried oxide layer. This design improves energy efficiency and enables threshold voltage tuning, making it attractive for IoT, automotive and RF applications. European firms such as STMicroelectronics and Soitec have been leading FD-SOI commercialization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.st.com/content/st_com/en/about/innovation-and-technology/fd-soi.html">FD - SOI - STMicroelectronics</a></li>
<li><a href="https://anysilicon.com/fdsoi/">The Ultimate Guide: FDSOI - AnySilicon</a></li>
<li><a href="https://www.credenceresearch.com/report/fully-depleted-silicon-on-insulator-fd-soi-technology-market">Fully Depleted Silicon - on - Insulator ( FD - SOI ) Technology Market...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#FD-SOI`, `#YMTC`, `#China`, `#chipmaking`

---

<a id="item-22"></a>
## [2026 Eclipse Webcam Aggregator Gains Traction on Hacker News](https://jonty.github.io/2026_eclipse_webcams/) ⭐️ 6.0/10

A quickly-built website aggregating webcams for the 2026 total solar eclipse has gained attention on Hacker News. The author, jonty, built it in 2024 minutes before the US eclipse totality and only remembered it this morning when a friend asked, now coordinating a surge of traffic to cameras across Iceland and Spain. This matters because it provides a practical, crowdsourced way for people around the world to experience a rare astronomical event live, even if they cannot travel to the path of totality. It also highlights how small, timely web tools can go viral and serve a passionate niche community during major real-world moments. The website was originally built for the 2024 eclipse and repurposed for the 2026 event, whose path crosses Iceland and Spain. The author humorously calls the unexpected surge a 'DDOS' on cameras, while users also share observations of the corona and prominences, and one points to solar panel monitoring data as an interesting additional feed.

hackernews · zoenolan · Aug 12, 11:53 · [Discussion](https://news.ycombinator.com/item?id=49270953)

**Background**: A solar eclipse occurs when the Moon passes between Earth and the Sun, temporarily blocking sunlight. The August 12, 2026 total solar eclipse crossed Iceland and Spain, offering a narrow path of totality for observers. Webcam aggregator sites like this one compile multiple live feeds from cameras in the path, allowing people without direct access to watch the event online. The author had previously created a similar site for the 2024 North American eclipse.

**Discussion**: In the comments, the author revealed they built the site minutes before the 2024 totality and are now bracing for heavy traffic, while users shared personal eclipse-chasing stories, from driving hundreds of kilometers in 2024 to watching from Sierra this year. Others discussed the historical significance of eclipse prediction in the development of science, and some expressed awe at seeing the corona and pink prominences through binoculars. One user also suggested monitoring solar panel data as a fun companion view.

**Tags**: `#eclipse`, `#webcams`, `#astronomy`, `#tools`

---

<a id="item-23"></a>
## [Uber Freight Probes Claimed Data Breach by Extortion Gang](https://techcrunch.com/2026/08/12/uber-freight-reportedly-investigating-after-hacking-group-claims-data-breach/) ⭐️ 6.0/10

An extortion gang that targets transportation and private equity firms has claimed responsibility for a data breach at Uber Freight. The company is reportedly investigating the claim. A data breach at Uber Freight could expose sensitive shipment and carrier information across a major logistics network. If confirmed, it would underscore the rising threat of extortion gangs against supply-chain and transportation companies. The claim has not been confirmed, and the specific scope of the alleged breach is unknown. The gang is described as known for targeting transportation companies and private equity firms, suggesting a pattern of sector-focused attacks.

rss · TechCrunch · Aug 12, 17:15

**Background**: Uber Freight is a digital freight-matching and logistics platform that connects shippers with carriers. Extortion gangs, often ransomware operators, increasingly steal data and threaten to leak it to pressure victims into paying ransoms.

**Tags**: `#security`, `#data breach`, `#Uber Freight`, `#cyberattack`, `#extortion`

---

<a id="item-24"></a>
## [Tesla Plans $10B Solar Factory in Texas, Seeks State Incentives](https://techcrunch.com/2026/08/12/tesla-wants-to-build-a-10b-solar-factory-in-texas/) ⭐️ 6.0/10

Tesla has announced plans to build a $10 billion solar factory in Texas and is asking the state to provide financial incentives to help offset construction costs. The proposal marks a major new manufacturing venture for the company in the solar energy sector. This investment could significantly expand U.S. solar manufacturing capacity and strengthen domestic clean energy supply chains. It also signals Tesla's broader strategic shift from electric vehicles toward large-scale energy infrastructure, potentially influencing job creation and regional economic development. The proposed factory carries a $10 billion price tag, and Tesla is seeking state incentives to reduce its financial burden. Specific details about the factory's capacity, product lines, or construction timeline have not been disclosed.

rss · TechCrunch · Aug 12, 16:18

**Background**: Tesla already manufactures solar-related products such as solar roof tiles and energy storage systems, and adding a dedicated solar factory would deepen its presence in clean energy manufacturing. Texas has a history of offering incentive packages to attract large industrial projects, which is why Tesla is seeking similar support for this venture.

**Tags**: `#Tesla`, `#solar energy`, `#manufacturing`, `#clean tech`, `#Texas`

---

<a id="item-25"></a>
## [VideoVerse's $250M Acquisition Collapses Amid Fraud Allegations](https://techcrunch.com/2026/08/12/how-a-250-million-acquisition-collapsed-into-allegations-of-fraud-and-forged-signatures/) ⭐️ 6.0/10

The $250 million acquisition of VideoVerse has collapsed, and co-founder Vinayak Shrivastav is now facing multiple legal cases alleging fraud and forged signatures. Investors are still waiting for their share of the deal's proceeds. This case underscores the serious risks that can lurk in high-value tech acquisitions, potentially shaking investor confidence in startup exits. It also highlights the importance of rigorous due diligence and the severe consequences for founders accused of misconduct. The deal was valued at $250 million, and investors have not yet received their payouts. Shrivastav is at the center of multiple legal cases, though specific details of the fraud and forgery allegations have not been disclosed in the available information.

rss · TechCrunch · Aug 12, 15:44

**Background**: VideoVerse is an AI-powered video solutions company whose flagship platform, Magnifi, helps sports organizations, broadcasters, and content owners automatically detect key moments and create real-time highlights. The company has received industry recognition, including being named 'Most Innovative Company in Video Editing Technology' in 2022. The collapse of its $250 million acquisition now brings legal and financial uncertainty to the company and its investors.

<details><summary>References</summary>
<ul>
<li><a href="https://vverse.ai/">VideoVerse – AI Powered Video Solutions Company</a></li>
<li><a href="https://www.linkedin.com/company/videoverse">VideoVerse | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#tech acquisitions`, `#fraud`, `#startup legal issues`, `#venture capital`

---

<a id="item-26"></a>
## [Tech innovator uses AI to rebuild David Webb’s Hong Kong database](https://www.scmp.com/news/hong-kong/hong-kong-economy/article/3363803/tech-innovator-uses-ai-rebuild-david-webbs-hong-kong-database?utm_source=rss_feed) ⭐️ 6.0/10

Keith Li King-wah, co-founder and principal trainer of Allytic AI, announced on Facebook that he will use artificial intelligence to rebuild Webb-site's 27-year-old database of Hong Kong corporate governance data, originally created by the late activist David Webb. Webb-site has long been a critical free resource for transparency and research in Hong Kong's financial markets. Using AI to rebuild it ensures this valuable trove of corporate governance data remains accessible and up-to-date, potentially enabling more advanced analysis. The database contains highly synthesized public records on people, organizations, and listed company directors, among other statistics. Li plans to bring the 27-year-old database 'into the modern era' with AI, though specific technical methods have not been disclosed.

rss · SCMP · Aug 12, 11:29

**Background**: David Webb was a British-born Hong Kong corporate governance activist who maintained Webb-site.com, a free database widely relied upon by researchers and journalists. Webb passed away in January 2026 at the age of 60 after a long battle with cancer. Allytic AI is a consultancy focused on human-AI partnership and machine learning adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/David_Webb_(Hong_Kong_activist)">David Webb (Hong Kong activist) - Wikipedia</a></li>
<li><a href="https://webbsite.0xmd.com/dbpub/">Webb-site Database</a></li>
<li><a href="https://allyticai.com/">Allytic AI : The Discipline of Human– AI Partnership</a></li>

</ul>
</details>

**Tags**: `#AI`, `#database`, `#Hong Kong`, `#corporate governance`, `#data preservation`

---