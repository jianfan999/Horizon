---
layout: default
title: "Horizon Summary: 2026-11-09 (EN)"
date: 2026-11-09
lang: en
---

> From 104 items, 16 important content pieces were selected

---

1. [KetchUp: An Open-Source SketchUp Alternative Built in Rust and WebGPU](#item-1) ⭐️ 7.0/10
2. [Ask HN: What Are You Working On? Thread Draws ~475 Builder Comments](#item-2) ⭐️ 7.0/10
3. [Outlook.com Begins Rejecting Inbound Email From Domains Without DMARC](#item-3) ⭐️ 7.0/10
4. [Goldman Sachs reportedly pulls Claude Code from bankers and traders](#item-4) ⭐️ 7.0/10
5. [Writing as a Thinking Tool: Blog Post Sparks Hacker News Debate](#item-5) ⭐️ 7.0/10
6. [Developer's Guide to Surviving 'AI Brain Fry' From Parallel Coding Sessions](#item-6) ⭐️ 7.0/10
7. [Developer Switches From Claude Code to Pi Coding Harness](#item-7) ⭐️ 7.0/10
8. [Nvidia Probes CEO Jensen Huang's Ties to Alleged Chinese Spy](#item-8) ⭐️ 7.0/10
9. [China's Gradient EEG Electrodes Reach 94% Mind-Typing Accuracy in Day-Long Wear](#item-9) ⭐️ 7.0/10
10. [USPS Surveillance Program iCOP Lost Key Records, IG Finds](#item-10) ⭐️ 7.0/10
11. [Dux, the rebranded Dank Material Shell, ships as a free open-source Wayland desktop shell](#item-11) ⭐️ 6.0/10
12. [llama-modchip claims 284B DeepSeek inference on 64GB RAM without a GPU](#item-12) ⭐️ 6.0/10
13. [German Researchers Trace Mysterious Synchronized Power Drops Across Global Grids](#item-13) ⭐️ 6.0/10
14. [China adapts torpedo supercavitation tech to cut cargo ship fuel use by 5%](#item-14) ⭐️ 6.0/10
15. [Tencent AI chief warns AI will soon master biology, raising safety risks](#item-15) ⭐️ 6.0/10
16. [Nvidia's Jensen Huang Faces Bipartisan Congressional Scrutiny Over Reported China Spy Link](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [KetchUp: An Open-Source SketchUp Alternative Built in Rust and WebGPU](https://ketchup3d.github.io/app/) ⭐️ 7.0/10

KetchUp is a new open-source SketchUp-style 3D modeler written in Rust and rendered with WebGPU that runs entirely inside the browser at ketchup3d.github.io/app. The project reached the front page of Hacker News with roughly 206 points and 55 comments, where users praised how polished the Rust-based UI and even its text rendering feel in a browser. SketchUp's long decline — shrinking free tiers and years of stagnation under successive owners — has left a gap for a simple, approachable modeler, especially for hobbyist 3D printing and quick architectural sketching. A browser-native implementation also shows that Rust compiled to WebAssembly plus WebGPU can now deliver a full interactive 3D application without a native install, a pattern that could spread to other desktop-class tools. The project is early-stage: one commenter noted that drawing a rectangle immediately prompts for an object name, which feels like the wrong default behavior, and another suggested adding a feature showcase to the landing page. Performance-wise, the rendering pipeline runs on WebGPU, the W3C standard API that supersedes WebGL and now ships in all major browsers, with Rust implementations such as wgpu.

hackernews · dcoulmbe · Nov 8, 22:35 · [Discussion](https://news.ycombinator.com/item?id=50418176)

**Background**: SketchUp is a 3D modeling program known for its push-pull modeling style that makes it unusually easy to learn; it was widely adopted by architects, woodworkers and 3D-printing hobbyists, but users have long complained that it changed hands repeatedly (Google acquired it in 2006, Trimble in 2012) while the free version was progressively restricted. WebGPU is the successor to WebGL, standardized by the W3C, which gives web pages efficient access to the GPU through Vulkan, Metal or Direct3D 12 backends. Rust can target the browser via WebAssembly and drive WebGPU through the wgpu crate, which is why projects like KetchUp can ship a full 3D modeler as a web page.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebGPU">WebGPU</a></li>
<li><a href="https://webgpu.org/">WebGPU</a></li>
<li><a href="https://gist.github.com/dmnsgn/76878ba6903cf15789b712464875cfdc">A collection of WebGL and WebGPU frameworks and libraries · GitHub</a></li>

</ul>
</details>

**Discussion**: Sentiment is enthusiastic: commenters mourned SketchUp's decline and welcomed KetchUp as a "spiritual successor," with one 3D-printing hobbyist saying SketchUp 8 remains the only modeler that ever clicked for them after FreeCAD failed to stick, and another praising how good the Rust UI feels in a browser. A broader thread argued that AI coding agents make it increasingly practical to build bespoke tools instead of spending hours learning existing software, while others offered direct UX feedback on the rectangle-naming prompt and the lack of a feature showcase.

**Tags**: `#rust`, `#webgpu`, `#3d-modeling`, `#open-source`, `#web-apps`

---

<a id="item-2"></a>
## [Ask HN: What Are You Working On? Thread Draws ~475 Builder Comments](https://news.ycombinator.com/item?id=50417407) ⭐️ 7.0/10

The November 2026 edition of Hacker News' recurring "Ask HN: What are you working on?" thread collected roughly 475 comments from developers describing the side projects and startups they are currently building. Submissions ranged from a privacy-friendly open-source Microsoft Teams chat exporter with about 90,000 users to a CRM and ad-spend tracking tool built for a small carpet-cleaning business. Because the thread is an unfiltered, recurring snapshot of what independent developers actually ship, it works as a barometer of where builder attention is concentrated right now: AI coding-agent tooling, privacy-respecting browser extensions, and unglamorous small-business software. That makes it more informative about real-world priorities than vendor launch announcements. Maturity levels vary enormously: OneBusAway's open-source transit software is used by millions of riders daily in New York City, Seattle, San Diego and Washington, D.C., and UC San Diego has deployed its Wayfinder and Waystation web apps for 35,000+ students, while other posters are still at the prototype stage — one admits his AI coding-agent token-optimization tool is still slow. The comments are wide-ranging rather than technically deep, so the value is breadth of signal, not detailed engineering discussion.

hackernews · david927 · Nov 8, 21:20

**Background**: "Ask HN" is a long-running Hacker News format in which a user poses an open question to the community, and "What are you working on?" is posted roughly monthly so builders can show work in progress without the scrutiny of a formal launch. Hacker News is a link-and-discussion site operated by the startup accelerator Y Combinator, and these threads are one of the few venues where weekend side projects and production software used at scale appear side by side. Concepts referenced in the comments include Google Local Service Ads (Google's pay-per-lead advertising product for local service businesses), CRM (customer relationship management software), and token usage as a cost metric for AI coding agents.

**Discussion**: The discussion is broad rather than deep, consisting mostly of builders describing their own work, but several themes recur: privacy-respecting open-source tools, cost and token efficiency for AI agents, and niche business software born from personal frustration — one poster started building after being laid off and discovering his father's carpet-cleaning company was struggling.

**Tags**: `#hacker-news`, `#community-discussion`, `#side-projects`, `#open-source`, `#developer-tools`

---

<a id="item-3"></a>
## [Outlook.com Begins Rejecting Inbound Email From Domains Without DMARC](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Outlook.com has begun quietly rejecting inbound email from sender domains that publish no DMARC record, according to a Mailroute blog post that surfaced on Hacker News. Messages are bounced with permanent 5xx delivery failures rather than being accepted and filtered, catching some self-hosted senders off guard. Microsoft's consumer mail service handling this at the SMTP layer means small domains, hobbyist mail servers and legacy applications that never adopted DMARC can silently lose the ability to reach Outlook users. It signals that DMARC is shifting from a spam-scoring signal to a hard entry requirement at major providers, raising the baseline for anyone running mail infrastructure. DMARC builds on SPF and DKIM and gives domain owners a policy telling receivers what to do with unauthenticated mail, so a missing record leaves receivers with no stated policy to evaluate. Commenters noted the rejection appears as a 5xx permanent failure rather than a silent drop, though several self-hosters reported years of unexplained filtering even with SPF, DKIM and DMARC correctly configured.

hackernews · xmddmx · Nov 8, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50416158)

**Background**: DMARC (Domain-based Message Authentication, Reporting and Conformance, defined in RFC 7489) is an email authentication protocol introduced around 2012 that lets a domain owner publish a DNS policy specifying how receivers should treat mail that fails SPF and DKIM checks, thereby protecting the domain from spoofing. Receiving providers have increasingly used DMARC presence as a trust signal, and many large senders now enforce it. Separately, providers also rely on DNS-based blocklists (DNSBLs) to reject mail from IP ranges deemed abusive, which is a common pain point for self-hosted and VPS-hosted mail servers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMARC">DMARC - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/defender-office-365/create-block-sender-lists-in-office-365">Create blocklists for inbound email in Microsoft 365 ...</a></li>
<li><a href="https://mxtoolbox.com/blocklists.aspx">Email Blocklist Check - IP Blocklist Check - See if your ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were split: some welcomed the change as overdue hygiene and were surprised it took until now, while self-hosted mail admins described years of unexplained filtering and complained that Microsoft's blocklists are opaque and effectively impossible to appeal. One commenter pushed back on the framing, noting Outlook returns 5xx permanent failures rather than silently dropping mail.

**Tags**: `#email`, `#dmarc`, `#deliverability`, `#self-hosting`, `#infrastructure`

---

<a id="item-4"></a>
## [Goldman Sachs reportedly pulls Claude Code from bankers and traders](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 7.0/10

Goldman Sachs is reportedly withdrawing Anthropic's Claude Code from its bankers and traders, reversing a high-profile deployment of an agentic coding tool inside a major investment bank. According to the report and the accompanying Hacker News thread, the pullback stems from security exposure of semi-autonomous agents on sensitive finance workstations, chronic usage-based billing overages, and compliance/auditability constraints rather than from any single technical failure. This is an early, concrete signal of how agentic coding tools fare inside regulated enterprises: a marquee financial institution rolling back a flagship AI deployment may make other banks and compliance-heavy organizations far more cautious about broad rollouts. It also highlights that enterprise adoption is gated as much by billing predictability and audit trails as by model capability. Commenters point to the 'lethal trifecta' — an agent that can read private client/trade data, ingest untrusted content, and reach the open internet or email on the same workstation creates an unacceptable exfiltration path — and to consumption billing that Anthropic could not normalize into a flat rate, pushing teams toward competitors like Gemini that throttle rather than overage. Banks additionally require granular, auditable entitlements and approval chains for data access, which opaque semi-autonomous agents complicate.

hackernews · TheWiggles · Nov 8, 18:16 · [Discussion](https://news.ycombinator.com/item?id=50415628)

**Background**: Claude Code is Anthropic's agentic coding tool that runs in the terminal and IDE, capable of reading a codebase, editing files, and executing commands on the user's machine — meaning it operates with the same access as the person who launched it. In finance, agents are often viewed as opaque, and opacity is a regulated liability: accuracy, determinism, auditability and recoverability are core professional requirements. The 'lethal trifecta' is a widely cited security framing in which an AI system that combines access to private data, exposure to untrusted content, and outbound communication can be manipulated into leaking information.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI coding agent and assistant</a></li>
<li><a href="https://www.forbes.com/councils/forbestechcouncil/2026/03/19/trust-control-and-auditability-evaluating-ai-agents-in-finance/">Trust, Control And Auditability: Evaluating AI Agents In Finance</a></li>
<li><a href="https://www.checkpoint.com/cyber-hub/ai-security/what-is-ai-security/the-7-biggest-agentic-ai-security-risks/">The 7 Biggest Agentic AI Security Risks - Check Point Software</a></li>

</ul>
</details>

**Discussion**: The roughly 360-comment thread is largely sympathetic to Goldman's decision, with commenters arguing the real blocker is structural rather than model quality: agents on primary finance workstations hit the lethal trifecta, consumption billing has produced chronic overages that Anthropic could not fix with a flat rate, and banks need auditable entitlements that LLM tools do not provide. One commenter shared a secondhand account of a finance team dismissed after AI-introduced errors in regulatory communication transcripts that could have carried jail time, underscoring how high the compliance stakes are.

**Tags**: `#ai-coding-agents`, `#enterprise-ai-adoption`, `#security`, `#llm-tooling`, `#fintech-compliance`

---

<a id="item-5"></a>
## [Writing as a Thinking Tool: Blog Post Sparks Hacker News Debate](http://muratbuffalo.blogspot.com/2026/11/writing-as-thinking-tool.html) ⭐️ 7.0/10

Murat Buffalo's blog post "Writing as a Thinking Tool" argues that writing is not just a way to record ideas you already have, but the very process through which those ideas become clear and complete. The post reached the front page of Hacker News, drawing 282 points and 83 comments from readers who extended the argument to design, programming, and AI-assisted workflows. The discussion lands in the middle of an ongoing debate about whether AI drafting and prototyping tools make the manual work of writing, sketching, and coding obsolete. The comment thread's consensus — that the struggle to articulate an idea is where insight is generated, not just where it is reported — suggests these tools may change the artifact but not the cognitive value of the craft. The piece is a reflective essay rather than a technical result, so it offers no data or benchmarks; its substance is the argument plus the anecdotal evidence readers supply. Notable contributions include a PhD student's realization that writing papers is part of the science rather than an epilogue, and a designer's claim that prompting has not reproduced the tight think-and-make loop of hands-on design.

hackernews · jruohonen · Nov 8, 10:41 · [Discussion](https://news.ycombinator.com/item?id=50412067)

**Background**: Murat Buffalo writes a long-running software engineering and distributed systems blog, and posts from it regularly surface on Hacker News. "Writing as a thinking tool" is a familiar idea in that community: externalizing a half-formed thought into sentences forces you to confront gaps in logic, which is why techniques like freewriting — writing continuously without editing to surface ideas — are popular. The same logic underlies practices such as rubber-duck debugging and design sketching, where the artifact matters less than the thinking it triggers.

**Discussion**: Commenters largely agreed and pushed the thesis into adjacent domains: one described how paper-writing forced clarity of mind during a PhD, another argued that Figma-style hands-on design still generates insights that prompting cannot, and a third said manual coding is itself where requirements get understood. Others shared personal tooling and habits — a locally built freewriting app for idea exploration, and the practice of sketching systems on paper before starting a codebase.

**Tags**: `#writing`, `#thinking`, `#design`, `#programming`, `#productivity`

---

<a id="item-6"></a>
## [Developer's Guide to Surviving 'AI Brain Fry' From Parallel Coding Sessions](https://sergeykuhne.com/blog/fighting-ai-brain-fry) ⭐️ 7.0/10

Developer Sergey Kuhne published a blog post on his personal site describing strategies for coping with what he calls 'AI brain fry' — the cognitive overload that comes from orchestrating many concurrent AI coding sessions at once. The post sparked a Hacker News discussion with 156 points and 130 comments, where practitioners compared their own parallel-session habits and limits. As AI coding assistants become standard tooling, developers are discovering that the bottleneck has shifted from writing code to supervising, reviewing, and context-switching between machine-generated workstreams. This makes cognitive load and review capacity — not raw generation speed — the limiting factors in AI-assisted software engineering, a problem most teams have no established practices for yet. Commenters pushed back on the framing in useful ways: one argued the real bottleneck is reviewing multiple AI-generated diffs of over 10,000 lines while still handling colleagues' code reviews, since doing three at once dilutes context and understanding far more than doing one. Another noted that model latency — five minutes to an hour per run — is what drives compulsive parallelism in the first place, and a third suggested breaking a single task into steps rather than opening more parallel threads, since more output at lower quality is not progress.

hackernews · kyunez · Nov 8, 19:37 · [Discussion](https://news.ycombinator.com/item?id=50416363)

**Background**: AI coding assistants such as agentic CLI tools and chat-based coding models often run long tasks asynchronously, leaving the developer waiting for minutes at a time. To avoid idleness, many developers start several sessions in parallel, each working on a different task. 'Context dilution' refers to the well-documented tendency of large language models — and of humans — to lose focus as input grows longer and noisier, because attention is a limited resource spread across a bigger window.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/diffray_context-dilution-when-more-tokens-hurt-ai-activity-7409613606901673984-n9Mn">Context Dilution : How Adding More Context Hurts AI... | LinkedIn</a></li>
<li><a href="https://www.broadcastgems.com/post/introduction-to-llms-and-ai-assisted-coding-with-a-slant-towards-after-effects">Introduction to LLMs and AI Assisted Coding, with a slant towards After...</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread was largely sympathetic but skeptical of the parallel-session habit. Several commenters said they cap themselves at two or three concurrent sessions and accept idle time as a worthwhile trade for focus and recovery, while one dissenting voice argued that nothing has changed about human thinking capacity and developers should simply focus on one thing and finish it; a more cynical commenter said merely catching the 'smell' of AI writing now makes them tune out of blog posts entirely.

**Tags**: `#AI coding assistants`, `#developer productivity`, `#cognitive load`, `#LLM workflows`, `#code review`

---

<a id="item-7"></a>
## [Developer Switches From Claude Code to Pi Coding Harness](https://caleb.software/posts/claude-to-pi.html) ⭐️ 7.0/10

A developer published a blog post titled "Goodbye Claude, hello Pi" describing how they moved their daily coding workflow off Anthropic's Claude Code and onto Pi, a minimal open-source LLM coding harness, and the write-up reached the front page of Hacker News with roughly 703 points and 435 comments. The thread shows that the harness layer around a model — the CLI/agent program that supplies tools, manages context and drives prompts — has become a genuine point of competition, with developers weighing vendor lock-in, terms-of-service risk and open-weight alternatives rather than just model quality. That matters to anyone picking day-to-day AI coding tooling, since switching harnesses can be as consequential as switching models. Pi is deliberately minimal, shipping with only four default tools and pushing most behavior into extensions, skills and user-defined workflows, and it exposes a unified multi-provider LLM API covering OpenAI, Anthropic and Google models. Commenters note that pairing Pi with an Anthropic subscription carries ToS and possible ban risk, that alternative harnesses miss Anthropic's custom headers and undocumented API features that shape model behavior, and that Claude Code's automatic context compaction is still considered noticeably better.

hackernews · karagenit · Nov 8, 03:11 · [Discussion](https://news.ycombinator.com/item?id=50410107)

**Background**: Claude Code is Anthropic's agentic coding tool that runs in the terminal and IDE, letting a Claude model read a codebase, edit files and run commands. A "harness" is the surrounding program that actually makes this work: it defines the tools the model can call, manages the conversation context, decides when to compact or summarize history, and injects system prompts and provider-specific parameters. Pi is an open-source, hackable harness from earendil-works that emphasizes a small core plus extensions, and it is model-agnostic — so it can drive proprietary APIs or open-weight models whose parameters are publicly released and can be self-hosted or run through third parties.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/rosgluk/pi-coding-agent-review-minimal-hackable-ai-coding-cli-4ge8">Pi Coding Agent Review: Minimal, Hackable AI... - DEV Community</a></li>
<li><a href="https://github.com/earendil-works/pi">GitHub - earendil-works/ pi : AI agent toolkit: unified LLM API, agent...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open-weight_model">Open-weight model</a></li>

</ul>
</details>

**Discussion**: Sentiment was broadly positive toward Pi: one commenter said they went Claude Code → Opencode → Pi and "never looked back," praising its flexibility, using open-weight models exclusively since around January and building a forge-agnostic GitHub Action on top of Pi's SDK. Others pushed back on practical grounds, citing ToS ban risk when using Anthropic models through third-party harnesses, weaker compaction than Claude Code, and a preference for desktop GUIs once LLM usage scales across many projects. One commenter argued that most of a model's real-world efficiency now comes from the harness itself, a layer that may soon grow more complex than the models.

**Tags**: `#LLM coding agents`, `#developer tools`, `#Claude Code`, `#Pi harness`, `#open-weight models`

---

<a id="item-8"></a>
## [Nvidia Probes CEO Jensen Huang's Ties to Alleged Chinese Spy](https://techcrunch.com/2026/11/08/nvidia-says-its-investigating-ceo-jensen-huangs-relationship-with-possible-chinese-spy/) ⭐️ 7.0/10

Nvidia is investigating a relationship between CEO Jensen Huang and a person suspected of being a Chinese spy, according to a report based on a company memo. In that internal memo, Huang admitted to having had an affair. Nvidia is the central supplier of AI hardware, so any leadership instability or espionage exposure at the company could ripple across the entire AI industry and its supply chain. The case also lands at the intersection of corporate governance and U.S.–China national-security scrutiny, where Nvidia is already a focal point. The public record so far is thin: the news rests on a two-sentence summary of an internal company memo, and neither Nvidia nor investigators have disclosed the identity of the person involved, the nature of the suspected espionage, or a timeline. The internal review is a corporate investigation rather than a confirmed law-enforcement finding.

rss · TechCrunch · Nov 8, 21:00

**Background**: Jensen Huang is Nvidia's co-founder and long-serving CEO, and the company's GPUs are the workhorse hardware behind most large-scale AI training and inference. Because those chips are viewed as strategic technology, Washington has placed repeated export controls on Nvidia's advanced products sold to China, making the company a regular subject of U.S.–China tech-security tensions. Internal corporate investigations of this kind are typically handled by compliance, security and outside counsel before any findings are made public.

**Tags**: `#Nvidia`, `#Jensen Huang`, `#corporate governance`, `#national security`, `#AI industry`

---

<a id="item-9"></a>
## [China's Gradient EEG Electrodes Reach 94% Mind-Typing Accuracy in Day-Long Wear](https://www.scmp.com/news/china/science/article/3373477/chinas-comfortable-brain-reading-device-achieves-94-mind-typing-accuracy-day-long-use) ⭐️ 7.0/10

Chinese researchers developed "gradient electrodes" — designed to avoid the trade-off between uniformly soft and uniformly rigid designs — and integrated them into a commercial EEG cap for non-invasive brain-computer interface testing. In visual mind-typing tests the system exceeded 94% accuracy, while the electrodes delivered eight hours of stable EEG signal within a 14-hour continuous wear session. Durability and comfort over a full day of wear are practical bottlenecks that have kept non-invasive BCIs largely confined to short lab sessions, so a design that holds signal quality for many hours could make consumer and clinical EEG use far more realistic. If the results hold up, it strengthens the non-invasive route against intracortical implants for applications like assistive typing and communication. The reported gains are 94%+ mind-typing accuracy, eight hours of stable EEG recording, and a 14-hour wear session — but the available summary gives no information on participant sample size, per-subject variability, peer-review status, or how much of the accuracy depends on calibration. The core technical claim is that grading electrode stiffness across the contact surface resolves the soft-versus-rigid trade-off, though the mechanism's long-term behavior under sweating and hair interference is not detailed in the excerpt.

rss · SCMP · Nov 9, 02:00

**Background**: An EEG cap records the brain's electrical activity using electrodes pressed against the scalp, and it is the most common hardware for non-invasive brain-computer interfaces, which let users control software directly from neural signals without surgery. The classic engineering dilemma is that soft, gel-like or hydrogel electrodes are comfortable and conform well to the scalp but tend to degrade and dry out, while rigid dry electrodes hold their shape and signal but become uncomfortable and unstable over long sessions. "Mind-typing" typically relies on visually evoked brain responses, where the user focuses on specific flashing targets and the system decodes which one was attended.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Electroencephalography">Electroencephalography - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S0924424725012026">A comprehensive review of EEG electrode technologies ...</a></li>
<li><a href="https://www.brainaccess.ai/a-comparative-analysis-of-eeg-cap-technologies/">A Comparative Analysis of EEG Cap Technologies - BrainAccess</a></li>

</ul>
</details>

**Tags**: `#brain-computer-interface`, `#EEG`, `#electrodes`, `#neuroscience`, `#human-computer-interaction`

---

<a id="item-10"></a>
## [USPS Surveillance Program iCOP Lost Key Records, IG Finds](https://www.reddit.com/r/technology/comments/1xrduwo/the_postal_service_built_a_surveillance_program/) ⭐️ 7.0/10

Recently disclosed records obtained through a lawsuit by the Electronic Frontier Foundation (EFF) and other requesters show that the U.S. Postal Service ran the Internet Covert Operations Program (iCOP) to monitor protests in 2020 and 2021. The postal inspector general found that some searches exceeded legal authority, and key records from the program are now missing. This highlights how a government surveillance program can operate with limited transparency and then become difficult to audit when its records disappear, undermining public trust and accountability. It matters to privacy advocates, protesters, civil-liberties groups, and anyone concerned about law-enforcement agencies monitoring political activity. iCOP grew out of a “Dark Web Program” that was renamed in October 2018 and expanded to support all online covert operations, using open-source intelligence, cryptocurrency analysis, social-media monitoring, and facial-recognition support. Disclosed bulletins show it monitored both Black Lives Matter and conservative rallies, while the full scope of the program and the lost records remain unclear.

reddit · r/technology · /u/efap1701 · Nov 9, 00:40

**Background**: The U.S. Postal Service has its own law-enforcement arm, the U.S. Postal Inspection Service (USPIS), which investigates crimes involving the mail and postal infrastructure. The Internet Covert Operations Program (iCOP) was a semi-secret unit within USPIS that used online tools to monitor public posts, and its existence became widely known after reporting and a lawsuit by the Electronic Frontier Foundation (EFF) forced disclosures. Federal records-retention rules, including 39 CFR Part 263, require agencies to preserve records according to approved schedules, which is why the reported loss of iCOP records is central to accountability concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.snopes.com/articles/393823/usps-icop/">What Is USPS's Internet Covert Operations Program (iCOP)? The Postal Service Built a Surveillance Program. Then It Lost ... USPS Covertly Monitored Protests Across Political Spectrum ... U.S. Postal Inspection Service s Online Analytical Support ... Postal Service Surveilled Protest Activities Online With ... The USPS' Semi-Secret Internet Surveillance Apparatus</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/postal-built-surveillance-program-then-165709362.html?fr=sycsrp_catchall">The Postal Service Built a Surveillance Program. Then It Lost ...</a></li>
<li><a href="https://www.ecfr.gov/current/title-39/chapter-I/subchapter-D/part-263">eCFR :: 39 CFR Part 263 -- Records Retention and Disposition</a></li>

</ul>
</details>

**Tags**: `#surveillance`, `#privacy`, `#USPS`, `#government accountability`, `#technology policy`

---

<a id="item-11"></a>
## [Dux, the rebranded Dank Material Shell, ships as a free open-source Wayland desktop shell](https://duxlabs.dev/) ⭐️ 6.0/10

Dux is a free, open-source Wayland desktop shell — formerly known as Dank Material Shell (DMS) and rebranded a few weeks ago — that bundles a file manager, theming support, and tight integration with the Niri compositor. Its v2.0 release also adds official support for atomic distros such as Bazzite, a gap users had previously found annoying. A desktop shell is what turns a bare compositor into something a mainstream user can actually live in, so a polished shell with a built-in file manager and theming can meaningfully lower the barrier to adopting the scrollable-tiling Niri workflow. Long-term users describe it as stable enough to help mainstream Niri, which suggests the Niri ecosystem is maturing beyond pure enthusiast territory. Dux is built with Quickshell and Go and is optimized for Niri, Hyprland, sway, MangoWC, labwc, and MiracleWM, so it is not tied to a single compositor. Its convenience installer uses a curl | sh pattern, which commenters flagged as a trust concern, and some users worry the project is becoming more all-encompassing than they want from a shell.

hackernews · indigodaddy · Nov 8, 19:08 · [Discussion](https://news.ycombinator.com/item?id=50416053)

**Background**: Wayland is the modern display-server protocol for Linux, and it deliberately splits responsibilities: a compositor such as Niri handles drawing windows and input, while a separate "shell" supplies the panel, launcher, notifications, lock screen, and other desktop furniture. Niri is a relatively new compositor that implements scrollable tiling — inspired by the PaperWM GNOME extension — where windows sit in an endless horizontal strip instead of a grid. Dux is built on Quickshell, a QtQuick-based toolkit for writing such shells, and "ricing" refers to the Linux hobby of heavily customizing a desktop's look and feel.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/niri-wm/niri">GitHub - niri-wm/niri: A scrollable-tiling Wayland compositor.</a></li>
<li><a href="https://github.com/AvengeMedia/DankMaterialShell">GitHub - AvengeMedia/DankMaterialShell: Desktop shell for wayland...</a></li>
<li><a href="https://kodekloud.com/blog/is-it-safe-to-pipe-curl-into-bash/">Is curl Into Bash Safe? How to Run Install Scripts Carefully</a></li>

</ul>
</details>

**Discussion**: Commenters are broadly enthusiastic: one has run it for nearly a year and calls it "endlessly slick" and good enough to help mainstream Niri, while another compares sticking with it to "settling down, getting married." Skeptics raise two concerns — that the interface looks a lot like Android and that a curl | sh installer should instead be packaged and reviewed by a distro — and one user wants a leaner shell, eyeing Noctalia on the River-based triad compositor.

**Tags**: `#wayland`, `#linux-desktop`, `#open-source`, `#niri`, `#ricing`

---

<a id="item-12"></a>
## [llama-modchip claims 284B DeepSeek inference on 64GB RAM without a GPU](https://github.com/synchopate/llama-modchip) ⭐️ 6.0/10

A GitHub repository named llama-modchip (by user synchopate) claims it can run a 284B-parameter DeepSeek model on a machine with only 64GB of RAM and no GPU at all. The project drew 367 points and 159 comments on Hacker News, where commenters quickly noted the repo appears to be AI-generated and behaves much like stock llama.cpp on CPU. It reflects how quickly the floor for running very large Mixture-of-Experts models on consumer hardware is dropping, which matters to anyone doing local inference without datacenter GPUs. At the same time, the case shows the community's growing scrutiny of AI-generated repositories that mostly repackage existing tools. The repo's headline number depends entirely on aggressive quantization and on DeepSeek's MoE architecture, where only a small fraction of the 284B parameters are activated per token. Commenters reported that on a Ryzen 7945HX (16-core Zen 4) with 96GB DDR5, the tool runs about the same as plain llama.cpp on CPU except that prefill seemed much faster, and no obvious option exists to actually configure the advertised DeepSeek 'modchip' setup.

hackernews · joshcsimmons · Nov 8, 10:22 · [Discussion](https://news.ycombinator.com/item?id=50411961)

**Background**: Quantization stores model weights in fewer bits (e.g. 4-bit instead of 16-bit) so a model fits in far less memory, at some cost in quality. Mixture-of-Experts models such as DeepSeek's keep total parameter counts huge but only route each token through a few 'expert' subnetworks, so inference cost is far lower than the raw size suggests. llama.cpp is the open-source C/C++ inference engine (built on the GGML tensor library) that underpins most local LLM tools including Ollama and LM Studio, so many 'new' local inference projects are effectively wrappers around it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://ai.plainenglish.io/understanding-quantization-in-large-language-models-be9cdaa65bb8">Understanding Quantization in Large Language Models</a></li>
<li><a href="https://github.com/discover-Austin/Neural_Network_Mixture_of_Experts">GitHub - discover-Austin/ Neural _ Network _ Mixture _ of _ Experts ...</a></li>

</ul>
</details>

**Discussion**: Sentiment was mixed-to-skeptical: one commenter questioned whether the AI-generated repo actually does anything beyond stock llama.cpp, while another complained the description is a 'dense word salad' that never makes the quantization scheme clear. Others used the thread for practical benchmarking — an E5 workstation with ~$300 of RAM and a $100–$500 GPU reaching roughly 20 tok/s output, and antirez noting that 128GB of unified RAM runs coding agents at acceptable speed with ~300 tok/s prefill. A recurring warning was that quantization degrades non-linearly and 4-bit is generally the sweet spot, with quality dropping sharply below that.

**Tags**: `#local-llm-inference`, `#quantization`, `#llama.cpp`, `#consumer-hardware`, `#mixture-of-experts`

---

<a id="item-13"></a>
## [German Researchers Trace Mysterious Synchronized Power Drops Across Global Grids](https://techcrunch.com/2026/11/08/coordinated-disturbances-haunt-grids-worldwide-heres-how-researchers-solved-the-mystery/) ⭐️ 6.0/10

A team of researchers in Germany has identified the likely cause of coordinated power drops that have been observed on power grids around the world. According to reports on the finding, the synchronized disturbances appear to stem from fast, system-wide interactions among grid control systems, power electronics, and long-distance transmission links rather than from a single fault source. If confirmed, the explanation matters for grid operators everywhere, because unexplained simultaneous power drops make it harder to distinguish a genuine fault from a benign control artifact — and misreading them can trigger unnecessary disconnections or cascading outages. It also highlights how the growing share of power-electronic converters on modern grids is changing the dynamics that reliability planning was built around. The proposed mechanism is propagation rather than common cause: small local changes can spread across the grid as frequency and voltage waves, so disturbances that look simultaneous at distant locations may simply be one event arriving at slightly different times. The published coverage is a short summary and does not yet detail the measurement data, model, or specific grids studied, so the findings should be treated as preliminary until the underlying study is available.

rss · TechCrunch · Nov 8, 20:30

**Background**: Power grids constantly experience low-frequency oscillations — periodic changes in power flow, mostly below 1 Hz — which are a natural by-product of the negative feedback in power system control algorithms. When a generator or load suddenly changes, that disturbance does not stay local: it propagates through the network as travelling waves of voltage angle and frequency, crossing a continental grid such as Europe's within a few seconds. Traditionally, the spinning mass (inertia) of large synchronous generators damped these swings, but inverter-based sources such as solar, wind and batteries respond differently and can change how disturbances travel and amplify.

<details><summary>References</summary>
<ul>
<li><a href="https://www.androguider.com/2026/11/researchers-solve-mystery-behind.html">Researchers Solve the Mystery Behind Coordinated Power Grid ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Grid_oscillation">Grid oscillation - Wikipedia</a></li>
<li><a href="https://arxiv.org/pdf/1810.04982">Disturbance propagation, inertia location and slow modes in ...</a></li>

</ul>
</details>

**Tags**: `#power grids`, `#infrastructure`, `#energy systems`, `#research`, `#reliability`

---

<a id="item-14"></a>
## [China adapts torpedo supercavitation tech to cut cargo ship fuel use by 5%](https://www.scmp.com/news/china/science/article/3373333/chinese-engineers-reduce-cargo-ship-fuel-use-5-high-speed-torpedo-tech) ⭐️ 6.0/10

Chinese engineers have adapted drag-reduction principles derived from supercavitating torpedoes into a bubble-lubrication system for commercial cargo ships, reportedly cutting net energy use by roughly 5%. Reports describe it as a second-generation air-lubrication system, though the excerpt provides little detail on the underlying methodology or test conditions. Even a 5% fuel reduction is significant for commercial shipping, where fuel is the dominant operating cost and the IMO's decarbonisation targets are pushing operators toward efficiency retrofits. If the system can be validated and scaled, it offers a relatively low-cost efficiency path for the existing global fleet, which turns over slowly. Bubble or air-lubrication drag reduction works by injecting dispersed microbubbles into the turbulent boundary layer beneath the hull to lower skin-friction; the claimed ~5% figure is a net energy saving, so it presumably already accounts for the energy consumed by the gas-injection machinery. The public reporting lacks peer-reviewed detail on ship size, sea states, or how the effect holds up at full scale.

rss · SCMP · Nov 8, 12:00

**Background**: Supercavitation is the deliberate creation of a gas cavity around a submerged object so that it travels largely inside gas rather than water, dramatically cutting skin-friction drag and enabling very high underwater speeds; it is used in high-speed torpedoes and in supercavitating projectiles for mine clearance. Air-lubrication or bubble drag reduction applies a milder version of the same idea to ships, spreading microbubbles under the hull, and is already offered commercially by several marine suppliers. Ships consume large amounts of fuel to overcome hydrodynamic drag, so small percentage reductions translate into substantial cost and emissions savings across a fleet.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supercavitation">Supercavitation - Wikipedia</a></li>
<li><a href="https://glo-marine.com/solutions/decarbonisation-retrofits/air-lubrication-systems-bubble-drag-reduction">Bubble Drag Reduction | Air Lubrication Systems | GLO</a></li>
<li><a href="https://interestingengineering.com/energy/china-bubble-lubrication-system-energy-use">China’s bubble-lubrication system cuts cargo ships energy use ...</a></li>

</ul>
</details>

**Tags**: `#marine engineering`, `#drag reduction`, `#supercavitation`, `#energy efficiency`, `#fluid dynamics`

---

<a id="item-15"></a>
## [Tencent AI chief warns AI will soon master biology, raising safety risks](https://www.scmp.com/tech/big-tech/article/3373697/ai-will-soon-master-biology-unleashing-new-safety-risks-tencent-ai-chief-warns) ⭐️ 6.0/10

Vinces Yao Shunyu, Tencent Holdings' chief AI scientist and a former OpenAI researcher, said at a rare public appearance on Saturday that AI models will soon be powerful enough to truly master biology, a capability that brings major benefits alongside serious safety risks. He framed the development as imminent rather than speculative, warning that malicious actors could misuse such systems even as they accelerate drug and treatment discovery. The warning comes from a senior figure at one of China's largest technology companies, adding a prominent voice from the Chinese AI industry to the global debate over frontier-model biosecurity. If AI genuinely lowers the expertise barrier for biological work, the same models that speed up drug discovery could also make it easier to design harmful biological agents, affecting regulators, labs and model developers worldwide. The remarks were delivered as brief public commentary rather than a technical deep-dive, and no specific models, timelines, evaluation benchmarks or proposed safeguards were disclosed. What is notable is the dual-use framing: the same capability that could accelerate drug and treatment discovery is also what creates the misuse risk.

rss · SCMP · Nov 8, 10:22

**Background**: Recent years have seen AI systems increasingly applied to biology and medicine, most visibly in protein structure prediction and computational drug design, where models can screen candidate molecules far faster than manual methods. Because biological research is dual-use, safety experts have long warned that capable models could help bad actors design pathogens or toxins. Yao is a former OpenAI researcher now leading AI research at Tencent, and his public comments carry weight because they come from someone with direct insight into how frontier models are built.

**Tags**: `#AI safety`, `#biosecurity`, `#frontier AI`, `#AI in biology`, `#Tencent`

---

<a id="item-16"></a>
## [Nvidia's Jensen Huang Faces Bipartisan Congressional Scrutiny Over Reported China Spy Link](https://www.reddit.com/r/technology/comments/1xr4wwy/nvidia_ceo_jensen_huang_faces_bipartisan/) ⭐️ 6.0/10

Nvidia CEO Jensen Huang is reportedly facing scrutiny from lawmakers of both major U.S. parties in Congress over an alleged link to Chinese espionage, according to the headline of the submitted report. The submission itself contains only a headline and link, so the specific allegations, the members of Congress involved, and Nvidia's response are not detailed in the available material. Nvidia is the central supplier of the AI accelerators that underpin most large-scale AI development, and any congressional inquiry into its CEO raises the political risk around the company's China business. The development fits a broader pattern of U.S.-China technology tensions in which semiconductor firms are increasingly drawn into national-security politics, potentially affecting export rules, supply chains, and investor sentiment. The available material offers no specifics on the nature of the alleged link, the lawmakers leading the scrutiny, or whether it takes the form of letters, hearings, or a formal committee inquiry. Because the report is unverified in the provided material and lacks primary sources, readers should treat the details as unconfirmed until Nvidia or congressional offices issue statements.

reddit · r/technology · /u/MarvelsGrantMan136 · Nov 8, 18:11

**Background**: Nvidia, led by co-founder and CEO Jensen Huang, designs the GPUs that have become the de facto standard for training and running AI models, making it one of the world's most valuable companies. U.S. export controls imposed over recent years restrict sales of advanced Nvidia chips to China, forcing the company to design downgraded variants for that market while regulators debate how far restrictions should go. Congress does not directly write export rules but uses hearings, letters, and legislation to pressure agencies and companies on national-security matters, which is the kind of scrutiny described here.

**Tags**: `#Nvidia`, `#geopolitics`, `#US-China tech`, `#semiconductors`, `#policy`

---