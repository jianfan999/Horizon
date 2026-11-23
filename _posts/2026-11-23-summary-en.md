---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 89 items, 12 important content pieces were selected

---

1. [OpenAI Examines Perplexity as a Measure of Model Intelligence](#item-1) ⭐️ 8.0/10
2. [Lean formalization progress map tracks disputed Masullo Riemann Hypothesis proof](#item-2) ⭐️ 8.0/10
3. [Tim O'Reilly asks what game Silicon Valley should play](#item-3) ⭐️ 8.0/10
4. [Beginner's Guide to Running Local AI with Inkling, Qwen, and Unsloth](#item-4) ⭐️ 7.0/10
5. [GL.iNet Cloud Flaw Exploited to Infect Routers and KVM Devices](#item-5) ⭐️ 7.0/10
6. [Tencent Touts Third-Party Safety Assessment of Open-Weight Hy4 Model](#item-6) ⭐️ 7.0/10
7. [Spelunkr.tv turns forgotten Internet Archive videos into a free retro linear TV network](#item-7) ⭐️ 6.0/10
8. [Interactive miniature 3D San Francisco with live buses, planes, and boats](#item-8) ⭐️ 6.0/10
9. [Nyx, a Long-Running ISP With 1980s BBS Roots, Sparks First-ISP Debate](#item-9) ⭐️ 6.0/10
10. [Show HN: Browser game casts you as a subagent working for an LLM](#item-10) ⭐️ 6.0/10
11. [TechCrunch Interviews Paris Marx on Data Center Backlash](#item-11) ⭐️ 6.0/10
12. [China's CXMT and YMTC close the memory-chip gap as AI boom cools](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI Examines Perplexity as a Measure of Model Intelligence](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 8.0/10

OpenAI published an analysis exploring the relationship between language-model perplexity and intelligence, framing perplexity as a simple benchmark for model capability and sparking a large community discussion. If perplexity—an old, cheap-to-compute metric—reliably tracks intelligence, it could offer a simpler alternative to increasingly complex LLM benchmarks and reshape how progress in reasoning models is measured. Commenters defined perplexity as the model’s average surprise in predicting the next token—1 is perfect and vocabulary size is the worst case—and noted it is mathematically tied to exponentiated cross-entropy; one commenter also cited Microsoft reporting MAI-2 Base log-perplexity of 0.819 on OpenAI’s evaluation set.

hackernews · acossta · Nov 22, 17:06 · [Discussion](https://news.ycombinator.com/item?id=50601525)

**Background**: Perplexity is a standard metric for language models: it measures how well a model predicts a sequence of tokens, with lower values meaning the model is less surprised by the text. It is derived from cross-entropy loss, the objective commonly used to train language models, and is typically reported on held-out text. Because perplexity depends on the tokenizer and evaluation corpus, raw scores are most meaningful when compared on the same setup.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Perplexity">Perplexity - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cross-entropy">Cross-entropy - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was largely enthusiastic: commenters found the clear perplexity–intelligence trend surprising and welcomed a simple benchmark, while adding definitions, historical context, and notes that Microsoft is now reporting MAI model scores on OpenAI’s evaluation set. Some debated how the trend holds up for reasoning models trained with reinforcement learning and wondered where GPT-4.5 fits.

**Tags**: `#AI/ML`, `#language models`, `#perplexity`, `#benchmarking`, `#OpenAI`

---

<a id="item-2"></a>
## [Lean formalization progress map tracks disputed Masullo Riemann Hypothesis proof](https://claude.ai/artifact/CtQyX8qfYAF822bgHJHHE3) ⭐️ 8.0/10

A publicly tracked progress map has been created for the Lean formalization of Alessandro Masullo's claimed proof of the Riemann Hypothesis, and it reached the front page of Hacker News. The map is backed by a GitHub repository (mccorvie/riemann-masullo) where contributing mathematicians are logging errata—hundreds of issues found so far—and soliciting outside compute from AI agents. This is a rare real-time case study of formal verification being applied to a contested, high-profile proof before the mathematical community has reached any consensus on whether it works. It shows how Lean plus crowd-sourced and AI-assisted effort can turn the messy business of checking a proof into a visible, incremental, publicly auditable process—and how easily a progress bar can be misread as evidence of correctness. Contributors caution that the hundreds of logged errata range from minor to substantial and that it is still too early to tell whether the core idea has a fatal gap, since a single hole is enough to collapse the whole formalization. The work is being partly driven by volunteers pointing agentic LLM tooling at the repository, and formalizing even a flawed argument in Lean requires resolving every step explicitly, which is exactly why the errata list keeps growing.

hackernews · Qision · Nov 22, 23:12 · [Discussion](https://news.ycombinator.com/item?id=50605045)

**Background**: Lean is an open-source proof assistant and functional programming language, based on the calculus of constructions with inductive types, in which mathematicians write proofs that a machine checks line by line. Formal verification of this kind guarantees that a proof follows from the axioms, but it says nothing about whether the original informal argument actually matches what was formalized—and any gap must be filled or the formalization simply stalls. The Riemann Hypothesis, which conjectures that all non-trivial zeros of the Riemann zeta function lie on the critical line, is one of the most famous unsolved problems in mathematics and has resisted proof for over 160 years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_proof">Formal proof - Wikipedia</a></li>
<li><a href="https://cacm.acm.org/research/formally-verified-mathematics/">Formally Verified Mathematics – Communications of the ACM</a></li>

</ul>
</details>

**Discussion**: The 146-comment discussion is deeply skeptical: one contributing mathematician gives an insider view of the errata and asks readers to donate agent compute, while others warn that the progress bar says nothing about correctness. Commenters also note that Ravi Vakil, who posted the announcement on Masullo's behalf, now says he never read the manuscript, and that Brian Conrad—seemingly the only professor vouching for it—told Scientific American it needs "major revision"; another thread laments that agentic AI may make mathematical careers feel less rewarding.

**Tags**: `#Lean`, `#formal-verification`, `#mathematics`, `#Riemann-Hypothesis`, `#AI-assisted-research`

---

<a id="item-3"></a>
## [Tim O'Reilly asks what game Silicon Valley should play](https://www.oreilly.com/radar/what-happened-to-silicon-valley/) ⭐️ 8.0/10

Tim O'Reilly published an essay on O'Reilly Radar arguing that Silicon Valley has abandoned human flourishing for shareholder-value optimization, using mechanism design as a lens to ask what game the industry ought to be playing. The piece sparked a large Hacker News debate with hundreds of comments on capitalism, ZIRP-era excess, and AI-driven strategy. As a widely respected tech publisher and early Web 2.0 evangelist, O'Reilly's critique carries weight in shaping how founders, investors, and policymakers think about the purpose of innovation. It also connects longstanding debates about capitalism and incentives to current anxieties about AI spending and market consolidation. The essay's central prescription appears near the end: mechanism design as "reverse game theory" should lead us to ask "what game ought we be playing?" and O'Reilly answers "the game of human flourishing." Commenters add that the analysis is an opinion essay rather than a technical breakthrough, with CoolestBeans arguing ZIRP let companies grow to "grotesque proportions" and is now pushing AI-driven cannibalization of core competencies.

hackernews · greenyouse · Nov 22, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50602947)

**Background**: Tim O'Reilly founded O'Reilly Media and helped popularize terms such as Web 2.0, making him a longstanding voice in Silicon Valley's self-understanding. Mechanism design is a branch of economics and game theory that starts from a desired outcome and works backward to design rules or institutions that produce it, which is why it is sometimes called reverse game theory; the 2007 Nobel Memorial Prize in Economic Sciences went to Leonid Hurwicz, Eric Maskin, and Roger Myerson for laying its foundations. ZIRP refers to a zero interest rate policy, a near-zero central bank target rate that makes cheap capital abundant and can encourage risk-taking and growth-at-all-costs strategies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanism_design">Mechanism design</a></li>
<li><a href="https://www.investopedia.com/terms/m/mechanism-design-theory.asp">Mechanism Design Theory: Principles, Applications, and Economics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Interest_rate">Interest rate - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely engaged constructively with the essay: Animats argued that markets are a built "machine" whose mechanism designers must be held accountable and reprogrammed for human flourishing, while michalsustr highlighted the buried thesis that society should deliberately optimize for human flourishing. CoolestBeans pointed to ZIRP-era excess as the proximate cause of current AI-driven cannibalization, and others questioned Milton Friedman's shareholder-profit framing and joked about Wall Street "yuppies" becoming today's VC influencers.

**Tags**: `#silicon-valley`, `#tech-industry`, `#mechanism-design`, `#capitalism`, `#ai-economics`

---

<a id="item-4"></a>
## [Beginner's Guide to Running Local AI with Inkling, Qwen, and Unsloth](https://www.gpupartner.com/blog/beginners-guide-local-ai-inkling-qwen-unsloth) ⭐️ 7.0/10

GPUPartner published a beginner-oriented walkthrough for running large language models on your own machine, using Thinking Machines' open-weights Inkling models, Alibaba Cloud's Qwen family, and Unsloth's quantization and fine-tuning tooling. The post was paired with a substantial Hacker News discussion in which practitioners shared concrete sub-$1,000 hardware builds for local inference. Local inference has become a realistic option for individuals and small teams who want to avoid per-token cloud costs, keep sensitive data on-device, and experiment without API rate limits. Guides that pair specific open models with concrete hardware advice lower the entry barrier for a much broader group of developers than the flagship-GPU crowd. The practical path is quantized GGUF weights — Unsloth's model hub hosts pre-quantized builds such as Inkling 2 Mini GGUF that can be pulled directly in its chat interface or loaded from local files. According to one VRAM configurator, Inkling needs roughly 21 GB of VRAM at 4-bit NVFP4 precision, so 12–16 GB cards generally require lower-bit quants, MoE layer offloading to system RAM, or reduced context length, all of which trade speed and quality for memory.

hackernews · Retell15 · Nov 22, 21:01 · [Discussion](https://news.ycombinator.com/item?id=50603845)

**Background**: Running an LLM locally means downloading a model's weights and doing inference on your own GPU or Mac instead of calling a hosted API. Open-weights releases — Qwen from Alibaba Cloud's DAMO Academy (open-sourced under Apache 2.0 since 2023), and Thinking Machines' Inkling, whose Inkling 2 Mini is an Apache 2.0 multimodal model designed to fit on a single desktop GPU or a 32 GB MacBook Pro — make this legally and technically possible. Quantization compresses weights to 4-bit or lower so they fit in far less memory, and Unsloth is a Python framework that speeds up fine-tuning (roughly 2x versus plain Transformers) and publishes ready-made quantized builds. The main constraint is VRAM: model size, context length, and precision all compete for it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Inkling_(large_language_model)">Inkling (large language model) - Wikipedia</a></li>
<li><a href="https://unsloth.ai/docs/models/inkling-2-mini">Inkling 2 Mini - Run Locally Guide | Unsloth Documentation</a></li>
<li><a href="https://llmconfigurator.com/en/models/inkling">Inkling — VRAM Requirements & Local Setup | LLM Configurator</a></li>

</ul>
</details>

**Discussion**: Commenters largely pushed back on the idea that local AI requires a $5,000 flagship GPU, sharing budget builds: a used Dell T5820 with 64 GB RAM plus a 16 GB Tesla P100 for under $1,000 at around 30 tok/s, a $300 24 GB Tesla P40 running a 27B-class Qwen model at 14 tok/s via llama.cpp, and an AMD R9700 32 GB card at roughly a fifth of an RTX 5090's price. Others reported running 27B models on 12 GB consumer cards using low-bit quants and llama.cpp tweaks, while one skeptic compared today's local AI to the early, heavy and expensive "plasma TV phase" and predicted roughly five years before most practical AI runs on personal machines.

**Tags**: `#local-ai`, `#llm`, `#qwen`, `#unsloth`, `#hardware`

---

<a id="item-5"></a>
## [GL.iNet Cloud Flaw Exploited to Infect Routers and KVM Devices](https://www.gl-inet.com/en-us/blogs/blog/glinet-security-notice-2026-11-20) ⭐️ 7.0/10

On November 20, 2026, GL.iNet published a security notice stating that an unauthorized party exploited a vulnerability in its cloud remote management services to access and install malicious software on some of its routers and KVM devices. The disclosure was accompanied by a forum thread and has since been picked up by security press such as BleepingComputer. GL.iNet devices are popular among homelab users, travelers and privacy-conscious buyers precisely because they are small, cheap and flexible, so a compromise delivered through the vendor's own cloud management channel undermines the core trust assumption behind buying them. It also reinforces a broader lesson for the IoT and consumer networking market: any always-on remote-access service bundled with a device becomes an attractive, high-leverage target for attackers. The notice covers GL.iNet's cloud remote management services (GoodCloud) and explicitly names both routers and KVM devices as affected; community members point to a forum thread suggesting related malware findings dating back to at least the previous year. Notably, while many GL.iNet routers are well supported by OpenWrt, the KVM models are not, leaving owners of those devices with fewer firmware-level mitigation options.

hackernews · gregsadetsky · Nov 22, 23:06 · [Discussion](https://news.ycombinator.com/item?id=50604988)

**Background**: GL.iNet makes compact travel routers and KVM-over-IP devices that can be managed remotely through the company's GoodCloud service, which is convenient but means the device maintains an outbound link to vendor infrastructure. OpenWrt is an open-source Linux-based firmware replacement for routers and embedded networking gear, and a large share of GL.iNet's router lineup is officially supported by it, so flashing OpenWrt is a common way to strip out vendor cloud features entirely. KVM-over-IP devices, by contrast, depend on proprietary firmware to handle remote keyboard, video and mouse redirection, which is why open firmware alternatives are far rarer for that product category.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gl-inet.com/en-us/blogs/blog/glinet-security-notice-2026-11-20">GL.iNet Security Notice 2026-11-20</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-exploit-glinet-cloud-flaw-to-infect-routers-kvm-devices/">Hackers exploit GL.iNet cloud flaw to infect routers, KVM devices</a></li>
<li><a href="https://www.whatismyip.com/what-is-openwrt/">What Is OpenWrt ? Features, Benefits, and Router Compatibility</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly unforgiving: several urged users to abandon cloud-connected appliances altogether, flash OpenWrt, or build a router from an old PC, and to disable cloud/remote access before something bad happens. Others raised the more worrying possibility that devices had been compromised since at least the previous year, and one user noted that the lack of OpenWrt support for GL.iNet's KVM models makes the situation especially concerning. A more measured view came from a user who had kept the vendor UI for its convenience over LuCI and had not used the cloud, but is now strongly considering moving to upstream OpenWrt and switching from Tailscale to Headscale.

**Tags**: `#security`, `#routers`, `#IoT`, `#OpenWrt`, `#privacy`

---

<a id="item-6"></a>
## [Tencent Touts Third-Party Safety Assessment of Open-Weight Hy4 Model](https://www.scmp.com/tech/tech-trends/article/3375374/tencent-touts-latest-ai-model-hy4s-performance-independent-safety-assessment) ⭐️ 7.0/10

Tencent Holdings worked with an international group of independent AI safety organisations to assess the risk level of its new open-weight Hy4 model before releasing it. This is the first time a leading Chinese tech company has disclosed that it used independent third-party evaluators for pre-release safety testing of a new model. Because open-weight models can be downloaded and run by anyone once released, safety problems cannot be patched or recalled after the fact, so pre-release evaluation carries outsized weight. Tencent's disclosure sets a precedent that could pressure other Chinese labs such as DeepSeek, Alibaba's Qwen team and Moonshot to adopt similar external reviews, and gives regulators and enterprise buyers an external yardstick for judging Chinese models. The published excerpt does not name the participating evaluators, the specific risk categories tested (such as cyber-offence or biological misuse capability), or whether results and mitigations will be made public. Per publicly available model documentation, Hy4 is a flagship Mixture-of-Experts model aimed at coding, office workflows, game development and scientific research, with an unusually large context window and its own listed limitations.

rss · SCMP · Nov 22, 13:30

**Background**: An open-weight model is one whose trained parameters are published under a licence, so anyone can download them, run them on their own hardware and often fine-tune them; this differs from open source, which would also include training code and data. AI safety evaluation is the practice of red-teaming a model before release to probe for dangerous capabilities, and third-party evaluators are considered more credible than in-house teams because they have no commercial stake in the outcome. Western labs such as Anthropic and OpenAI have faced pressure to submit frontier models to independent reviewers, while Chinese companies have generally relied on internal review, making Tencent's disclosure a notable shift in AI governance practice.

<details><summary>References</summary>
<ul>
<li><a href="https://aibuildercourse.com/glossary/open-weight-model">What Is Open - weight Model ? Definition & Examples</a></li>
<li><a href="https://kie.ai/blog/what-is-tencent-hy4">What Is Tencent Hy 4 ? 770B MoE, 1M Context</a></li>
<li><a href="https://restofworld.org/2026/ai-safety-independent-evaluation/">Why countries need their own AI safety evaluators - Rest of World</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#Tencent`, `#open-weight models`, `#AI governance`, `#China tech`

---

<a id="item-7"></a>
## [Spelunkr.tv turns forgotten Internet Archive videos into a free retro linear TV network](https://spelunkr.tv/) ⭐️ 6.0/10

Spelunkr.tv launched as a free, retro-styled linear TV network that streams forgotten videos pulled directly from the Internet Archive and presents them as always-on, scheduled channels rather than an on-demand catalog. The project reached roughly 148 points and 21 comments on Hacker News, where users praised its design and immediately asked for M3U/XMLTV endpoints. It shows how the Internet Archive's vast public media corpus can be re-packaged into a lean-back, channel-surfing experience that feels like cable TV, a format that on-demand streaming has largely abandoned. It also highlights growing hobbyist demand for IPTV-compatible outputs so such channels can plug into Jellyfin, Plex or dedicated IPTV players. Because the site streams directly from the Internet Archive rather than hosting its own copies, the bandwidth load and any content-governance questions land on the Archive itself. The current build is web-only: there is no M3U playlist or XMLTV program guide URL yet, which is exactly what multiple commenters requested for integration with external IPTV clients.

hackernews · SockThief · Nov 23, 01:13 · [Discussion](https://news.ycombinator.com/item?id=50606192)

**Background**: The Internet Archive is a non-profit digital library that hosts millions of public-domain and archived media items, each with directly linkable stream and download URLs, which makes it a popular raw source for side projects. 'Linear TV' means programming scheduled on channels at fixed times, as opposed to choosing a title on demand. In the IPTV world, an M3U file is the standard plain-text playlist that lists channel stream URLs, while XMLTV is the standard XML format for electronic program guide (EPG) data; players like Jellyfin, Plex and TiviMate combine the two to show channels with a TV guide. ErsatzTV is an open-source tool that builds similar scheduled channels out of locally stored media and exposes exactly these M3U/XMLTV URLs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/M3U">M 3 U - Wikipedia</a></li>
<li><a href="https://epg.best/">EPG for IPTV & XMLTV TV Guide | EPG .best</a></li>

</ul>
</details>

**Discussion**: Sentiment was enthusiastic, with commenters calling the design and execution "dope" and reporting "instant flashbacks" to old TV guides, including a joke about whether an Amiga generated the scrolling schedule. The most substantive point was a governance question: since the site streams from the Internet Archive directly, one commenter wondered how the Archive feels about a third-party UI bypassing its own user experience. Several others asked for exposed M3U and XMLTV URLs for existing IPTV players, and ErsatzTV was recommended for people who want to build similar channels from local media.

**Tags**: `#internet-archive`, `#iptv`, `#streaming`, `#side-projects`, `#retro-tv`

---

<a id="item-8"></a>
## [Interactive miniature 3D San Francisco with live buses, planes, and boats](https://smallsf.com/) ⭐️ 6.0/10

A side project at smallsf.com renders San Francisco as a browser-based, interactive miniature 3D city in which buses, planes, and boats move around in real time, and it drew hundreds of points of attention on Hacker News. The demo lets visitors pan and zoom around the city and watch animated vehicles follow their routes, all inside a normal web page without plug-ins. It shows how far browser-based 3D has come: a full city with live vehicle animation now runs as a shareable link rather than an installed app or game engine. Projects like this make geospatial data and transit simulation approachable for hobbyists and could inspire more real-time digital-twin style visualizations of urban infrastructure. Commenters noted that the model is not uniformly detailed — zooming into specific neighborhoods can reveal missing geometry, such as the park at Patricia's Green in Hayes Valley. Others raised concerns that such WebGL-heavy scenes can consume large amounts of browser memory and become sluggish on ordinary machines, and the creator's identity and build approach were left unclear in the discussion.

hackernews · dutilh · Nov 22, 20:33 · [Discussion](https://news.ycombinator.com/item?id=50603589)

**Background**: WebGL is a JavaScript API that lets browsers render hardware-accelerated 3D graphics inside an HTML canvas, conforming closely to OpenGL ES, without any plug-ins — the same foundation used by tools like Three.js. Rendering a whole city in real time is demanding: developers typically rely on LOD (level-of-detail) switching, geometry merging, texture compression, and careful model loading to keep frame rates high. Real-time transit tracking normally comes from live GPS feeds published by transit agencies, which can then be animated on top of a 3D or 2D map.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API">WebGL: 2D and 3D graphics for the web - Web APIs | MDN</a></li>
<li><a href="https://www.geeksforgeeks.org/javascript/how-to-optimize-webgl-performance/">How to Optimize WebGL Performance? - GeeksforGeeks</a></li>
<li><a href="https://medium.com/@kazukimiyazaki33/from-modeling-to-rendering-a-comprehensive-guide-to-optimizing-3d-model-loading-performance-in-da9f60dedd9d">From Modeling to Rendering: A Comprehensive Guide to ... - Medium</a></li>

</ul>
</details>

**Discussion**: The Hacker News reaction was positive but skeptical: simonw pointed out that zooming in breaks the illusion, since landmarks like Patricia's Green are simply missing, while ChaseRensberger questioned whether such sites ever run smoothly or just eat browser memory. Others added value by pointing to related projects — the US Army Corps of Engineers' physical Bay Model in Sausalito and an isometric Seattle version at isometricseattle.fun — and one commenter asked who built it and how.

**Tags**: `#visualization`, `#webgl`, `#maps`, `#3d-graphics`, `#side-projects`

---

<a id="item-9"></a>
## [Nyx, a Long-Running ISP With 1980s BBS Roots, Sparks First-ISP Debate](https://nyx.net/) ⭐️ 6.0/10

A Hacker News post has drawn attention to Nyx.net, a still-running ISP whose history traces back to a circa-1987 BBS and Netnews login host, and the thread has turned into a debate over which service was actually the first ISP. The item is a piece of internet-history nostalgia that illustrates how early online services blurred the line between BBSes, login hosts, and true ISPs, a distinction that still shapes how the pre-Web Internet is remembered. Commenters point out that Nyx's own history describes a BBS/Netnews login host rather than a modern ISP, and that TLGNet in 1990 may better fit today's ISP definition because users did not log into a shared host. One commenter also notes that Nyx's current IP block appears to be hosted on AWS EC2 rather than in its own colocation.

hackernews · o_-_o · Nov 22, 20:15 · [Discussion](https://news.ycombinator.com/item?id=50603465)

**Background**: A BBS was an online system where users dialed in to post messages, exchange files, and join discussions; these systems were popular before the Web and declined in the mid-1990s as the Internet took over. Usenet/Netnews was a distributed discussion network often described as an early social network, and early Internet access often meant dialing into a university or service host and logging in rather than getting a direct IP connection from an ISP. The WELL, founded in 1985, is one of the oldest still-operating online communities and is often mentioned alongside these transitional services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Timeline_of_social_media">Timeline of social media - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/computer-networks/what-is-bulletin-board-system/">What is Bulletin Board System ? - GeeksforGeeks</a></li>
<li><a href="https://www.cs.columbia.edu/~smb/papers/netnews-hist.pdf?ref=upstract.com">Netnews : The Origin Story</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion is nostalgic but historically corrective: gumby argues Nyx was a BBS/Netnews login host and cites world.std.com, The WELL, and TLGNet as better candidates for early ISP status, while icedchai asks whether world.std.com was older. Others add technical color, noting Nyx's apparent EC2 hosting and reminiscing about 1990s regional ISP work; one commenter only flags a missing word on the page.

**Tags**: `#internet-history`, `#isp`, `#bbs`, `#nostalgia`, `#hackernews`

---

<a id="item-10"></a>
## [Show HN: Browser game casts you as a subagent working for an LLM](https://github.com/gulivan/worker755) ⭐️ 6.0/10

A developer published a Show HN browser game called "worker755" (hosted on GitHub) in which the player acts as a subagent that receives tasks and instructions from an LLM playing the role of manager. The project is a small playable demo rather than a full product, and it drew a modest thread of comments debating AI middle managers and the reversal of human–AI roles. Multi-agent LLM systems increasingly use an orchestrator that decomposes work and delegates subtasks, so a game that puts a human at the bottom of that hierarchy is a useful provocation about where real workflows are heading. It also feeds an active debate about AI taking over managerial roles and what that does to human autonomy at work. It runs in the browser and is distributed as a GitHub demo, so scope is limited and the experience is short. One player reported that the LLM manager handed out the exact commands needed for each task instead of leaving the approach open, making it unclear whether the standalone-challenge mode shown in the GitHub demo is actually reachable.

hackernews · ivantgam · Nov 22, 13:56 · [Discussion](https://news.ycombinator.com/item?id=50599762)

**Background**: Modern LLM agent architectures often follow an orchestrator-worker pattern: a top-level model plans, then spawns or calls subagents that each handle a narrow task and report back, sometimes through tools and shared memory. This game inverts that arrangement, placing a human in the worker slot. Cory Doctorow's term "reverse centaur" describes exactly this: instead of a human augmented by a machine, a human reduced to an appendage of an automated system. Interest in the idea is real — Anthropic and Andon Labs ran an experiment letting a Claude model run an office vending machine, concluding that AI middle managers are "plausibly on the horizon."

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2025/06/28/anthropics-claude-ai-became-a-terrible-business-owner-in-experiment-that-got-weird/">Anthropic’s Claude AI became a terrible business owner... | TechCrunch</a></li>
<li><a href="https://www.theguardian.com/technology/2026/may/15/ai-manager-purge-tech">‘I didn’t want to be the guinea pig’: inside tech’s AI -fueled manager purge</a></li>

</ul>
</details>

**Discussion**: Commenters largely treated the game as a preview of real workplace dynamics rather than pure fantasy. One quoted Cory Doctorow's "reverse centaur" framing for humans working for AI, another predicted AI middle managers will arrive soon since management is easier for the model than assisting, and a third suggested it may already be reality given how opaque top-level decisions are. A reviewer who enjoyed the demo nonetheless faulted the LLM manager for over-specifying commands, and one commenter fired off a tongue-in-cheek "Butlerian Jihad Now" — a Dune reference to revolt against thinking machines.

**Tags**: `#LLM`, `#AI agents`, `#Show HN`, `#game`, `#human-AI collaboration`

---

<a id="item-11"></a>
## [TechCrunch Interviews Paris Marx on Data Center Backlash](https://techcrunch.com/2026/11/22/why-data-centers-are-at-the-center-of-the-big-tech-backlash/) ⭐️ 6.0/10

TechCrunch published an interview with journalist Paris Marx about his new book "Hyperscale," in which he argues that data centers have become the central target of public and political backlash against Big Tech. The piece, published on November 22, 2026, is a conversational book discussion rather than a report of a new technical development. As AI infrastructure spending accelerates, hyperscale buildouts are increasingly running into local opposition over electricity demand, water use, land consumption and tax incentives, making data centers a live political issue rather than a purely technical one. The framing matters for cloud providers, utilities, regulators and the communities that host these facilities. The item is a book-interview/podcast format with limited technical depth and no new data or disclosures behind it, so it functions more as commentary than as a breaking development. For scale context, hyperscale facilities can require power capacity well above 100 megawatts and span millions of square feet.

rss · TechCrunch · Nov 22, 18:08

**Background**: Hyperscale data centers are the largest class of cloud computing facilities, operated by providers such as Amazon Web Services, Google Cloud, Microsoft Azure and IBM Cloud, and can house thousands of servers along with kilometers of high-speed networking cable. Google opened what is often cited as the first hyperscale data center in The Dalles, Oregon, in 2006, a facility now occupying roughly 1.3 million square feet. According to the 2024 U.S. Data Center Energy Usage Report from Lawrence Berkeley National Laboratory, hyperscale and colocation centers together housed 74% of computer servers in 2023. As AI training and inference workloads grow, these facilities' demand for power, cooling and land has turned siting decisions into contested local political fights.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hyperscale_data_center">Hyperscale data center</a></li>
<li><a href="https://www.ibm.com/think/topics/data-centers">What Is a Data Center ? | IBM</a></li>

</ul>
</details>

**Tags**: `#data centers`, `#AI infrastructure`, `#Big Tech`, `#energy policy`, `#regulation`

---

<a id="item-12"></a>
## [China's CXMT and YMTC close the memory-chip gap as AI boom cools](https://www.scmp.com/tech/big-tech/article/3375363/chinas-memory-chipmakers-are-catching-industry-leaders-what-happens-when-they-do) ⭐️ 6.0/10

China's two largest memory chipmakers, ChangXin Memory Technologies (CXMT) in DRAM and Yangtze Memory Technologies (YMTC) in NAND flash, have expanded faster and more aggressively than ever over the past two years, using state backing, new fabrication plants and advancing process technology to close the gap with industry leaders such as Samsung, SK Hynix and Micron. The Korea Times/South China Morning Post analysis warns that early signs of a memory market cool-down could now test that momentum. Memory chips are a foundational input for AI servers, smartphones and PCs, and a credible domestic Chinese supplier base would erode the pricing power and market share of Korean and US incumbents. It also strengthens Beijing's push for semiconductor self-sufficiency in a segment where China has historically depended heavily on imports. CXMT, based in Hefei, Anhui, is mainland China's largest DRAM integrated device manufacturer, and has reported progress on a new memory cell architecture aimed at raising density; YMTC, founded in Wuhan in 2016, focuses on 3D NAND flash and has reportedly targeted sourcing as much as 70% of the equipment for a planned fab from domestic suppliers. Both firms still face export controls on advanced chipmaking tools and must prove they can scale leading-edge output profitably once memory prices turn down.

rss · SCMP · Nov 23, 02:00

**Background**: Memory chips split into two main families: DRAM, the working memory that holds data temporarily for active computing tasks, and NAND flash, which stores data persistently in SSDs and phones. The market has long been dominated by a handful of players — Samsung, SK Hynix and Micron in DRAM, and Samsung, SK Hynix, Kioxia and Micron in NAND — and is notoriously cyclical, with boom years of high prices followed by sharp downturns. China has poured state capital into CXMT and YMTC since the mid-2010s to build domestic capacity, and the AI server build-out has sharply increased demand for high-bandwidth and high-density memory, giving both firms an opening to scale.

<details><summary>References</summary>
<ul>
<li><a href="/url?opi=89978449&q=CAEStgEBxCJF13Wz1xFr7C3TJ8Br90uNOPBf6bgGfDFzzN1iVVKqVpjpbddaq0DkLbQEhXLw0OqOhqFod6j_qP5TjOi-I7uamHnBoKhYKmaJUj-39bp49AaEiD3a43IWutHPrZPChGYYxpG-Mmy81h8Vr9mN9v5djsy3obVStBedaR-JEEeOPu_hysrcd2tnKOkIxeHD11-m6X49xtXgxyjDNTHR_ESdOypXOceZKFdm0yvV5J_RJ77T_A&sa=U&uoh=3&ved=2ahUKEwiArJGEkp2YAxWhmmoFHTkCB-sQFnoECAkQAg&usg=AOvVaw3O1tsNxK3uPSHkSvC52bnX">China's top flash memory chipmaker targets more homegrown ... - Reuters</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#memory-chips`, `#China-tech`, `#AI-hardware`, `#supply-chain`

---