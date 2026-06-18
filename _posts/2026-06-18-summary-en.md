---
layout: default
title: "Horizon Summary: 2026-06-18 (EN)"
date: 2026-06-18
lang: en
---

> From 158 items, 39 important content pieces were selected

---

1. [Epic Games Open Sources Lore, a Scalable VCS for Game Dev](#item-1) ⭐️ 8.0/10
2. [US delays blacklisting DeepSeek, still eyes 100+ Chinese firms](#item-2) ⭐️ 8.0/10
3. [Leaked docs show OpenAI losing billions annually](#item-3) ⭐️ 8.0/10
4. [GLM-5.2 tops open weights leaderboard on Artificial Analysis](#item-4) ⭐️ 8.0/10
5. [U.S. science in chaos as funding and trust collapse](#item-5) ⭐️ 8.0/10
6. [Tesco Moves 40,000 Workloads Off VMware Over Broadcom Pricing](#item-6) ⭐️ 8.0/10
7. [New HTTP QUERY Method Introduced in RFC 10008](#item-7) ⭐️ 8.0/10
8. [Physis Raises $100M+ for General World Foundation Model](#item-8) ⭐️ 8.0/10
9. [Leaders fear US AI cutoff; Anthropic blackout validates concern](#item-9) ⭐️ 8.0/10
10. [Hackers breach tens of thousands of Fortinet firewalls using known passwords](#item-10) ⭐️ 8.0/10
11. [Odyssey hits $1.45B valuation with Amazon backing](#item-11) ⭐️ 8.0/10
12. [Adam (YC W25) Launches Open-Source AI CAD Platform](#item-12) ⭐️ 7.0/10
13. [8-bit Live MLB Gamecast Website](#item-13) ⭐️ 7.0/10
14. [Robot battle royale compares AI model cost efficiency](#item-14) ⭐️ 7.0/10
15. [Human Connection: The AI-Proof Competitive Advantage](#item-15) ⭐️ 7.0/10
16. [Volkswagen blocks GrapheneOS users from app and API](#item-16) ⭐️ 7.0/10
17. [Robotics scientist: Real scaling law lies in deployment, not data stacking](#item-17) ⭐️ 7.0/10
18. [SK hynix Ships 12-Layer HBM4E Samples to Key Customers](#item-18) ⭐️ 7.0/10
19. [Enterprises struggle with AI ROI after tokenmaxxing craze](#item-19) ⭐️ 7.0/10
20. [FTC lawsuit exposes subscription scam network tactics](#item-20) ⭐️ 7.0/10
21. [Anthropic first AI startup to join Frontier carbon removal coalition](#item-21) ⭐️ 7.0/10
22. [Collecting robot training data is dirty work; AI labs pay XDOF](#item-22) ⭐️ 7.0/10
23. [Pramaana Labs raises $27M seed for formal verification in AI](#item-23) ⭐️ 7.0/10
24. [SpaceX alum raises $22M for rocket-engine geothermal plants](#item-24) ⭐️ 7.0/10
25. [US developers embrace Chinese AI for cost savings](#item-25) ⭐️ 7.0/10
26. [AI enables more elaborate cyber fraud in Asia: Interpol](#item-26) ⭐️ 7.0/10
27. [Kingboard unit $1.5B stake sale to boost PCB capacity for AI](#item-27) ⭐️ 7.0/10
28. [Thinking Out Loud with Others Boosts Problem-Solving](#item-28) ⭐️ 6.0/10
29. [XianGong Intelligent files for HK IPO, five key insights from prospectus](#item-29) ⭐️ 6.0/10
30. [Taiwei Quantum, a USTC PhD startup, secures funding for quantum components](#item-30) ⭐️ 6.0/10
31. [China Regulators Announce Phased Launch of Active ETFs](#item-31) ⭐️ 6.0/10
32. [Glass Substrate Stocks Surge but Companies Say Still Early Stage](#item-32) ⭐️ 6.0/10
33. [ASML CEO Warns of Supply Risks for Musk's Terafab](#item-33) ⭐️ 6.0/10
34. [VC: Real AI winners won't sell AI](#item-34) ⭐️ 6.0/10
35. [Social media’s next evolution: user-controlled algorithms](#item-35) ⭐️ 6.0/10
36. [Stanford Grads Raise $11M for Noninvasive Hormone Tracker](#item-36) ⭐️ 6.0/10
37. [Google bets on Gemini to reinvent smart home speaker](#item-37) ⭐️ 6.0/10
38. [PayPal Ventures Shuts Down After a Decade](#item-38) ⭐️ 6.0/10
39. [China vows new legal shield to counter US sanctions, protect finance](#item-39) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Epic Games Open Sources Lore, a Scalable VCS for Game Dev](https://lore.org/) ⭐️ 8.0/10

Epic Games has open-sourced Lore, a centralized version control system designed for large binary files and game development workflows, positioning it as a competitor to Perforce. Game developers have long struggled with Git's poor handling of large binary files, and Lore offers a native solution built from the ground up for game assets. This could reduce reliance on Perforce and lower costs for studios of all sizes. Lore uses a content-addressed Merkle tree structure, deduplication, and sparse on-demand data hydration to efficiently store and retrieve large files. It is already used internally by Epic for Unreal Editor for Fortnite (UEFN).

hackernews · regnerba · Jun 17, 14:30 · [Discussion](https://news.ycombinator.com/item?id=48571081)

**Background**: Version control systems (VCS) track changes to files over time. Git is the most popular VCS for code but struggles with large binary files because it stores full copies. Perforce is a centralized VCS favored in game development for its file locking and scalability with binaries. Lore aims to provide a modern, open-source alternative tailored to these needs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">GitHub - EpicGames/lore: Lore is a next-generation, open source revision control system · GitHub</a></li>
<li><a href="https://epicgames.github.io/lore/explanation/system-design/">The Lore Version Control System - Lore Developer Documentation</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System - Phoronix</a></li>

</ul>
</details>

**Discussion**: The HN community largely supports Lore as a much-needed Perforce alternative for game development, noting Git's unsuitability for binary assets. Some commenters appreciate that Lore is already proven in UEFN, while others highlight the complexity of Perforce administration and hope Lore simplifies it.

**Tags**: `#version-control`, `#game-development`, `#open-source`, `#scalability`, `#perforce`

---

<a id="item-2"></a>
## [US delays blacklisting DeepSeek, still eyes 100+ Chinese firms](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 8.0/10

The United States has decided to postpone blacklisting Chinese AI company DeepSeek, while continuing to designate over 100 other Chinese firms as national security risks. This decision was reported by Reuters on June 17, 2026. This move signals ongoing geopolitical tensions in the AI sector, affecting global supply chains and investment flows. DeepSeek's low-cost, open-weight models have already disrupted the industry, and any future restrictions could reshape competition. DeepSeek is a Chinese AI company known for its cost-efficient large language models like DeepSeek-R1, which rival OpenAI's GPT-4. The US has not added DeepSeek to the Entity List yet, but it remains under scrutiny alongside many other Chinese tech firms.

hackernews · giuliomagnifico · Jun 17, 03:55 · [Discussion](https://news.ycombinator.com/item?id=48565498)

**Background**: DeepSeek, founded in July 2023 and based in Hangzhou, is owned by hedge fund High-Flyer. It gained attention in January 2025 with the release of DeepSeek-R1, which achieved performance comparable to leading models at a fraction of the cost. The US government has been using the Entity List to restrict Chinese companies' access to American technology, particularly advanced AI chips, citing national security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters express mixed views; some appreciate DeepSeek's practical utility and affordability, while others criticize US policy as hypocritical and reminiscent of China's Great Firewall. A few note that many Chinese AI firms already face export restrictions, so the blacklist may have limited impact.

**Tags**: `#AI regulation`, `#geopolitics`, `#DeepSeek`, `#national security`, `#tech policy`

---

<a id="item-3"></a>
## [Leaked docs show OpenAI losing billions annually](https://arstechnica.com/ai/2026/06/leaked-financial-docs-show-openai-is-losing-billions-of-dollars-a-year/) ⭐️ 8.0/10

Leaked financial documents reveal that OpenAI had $13 billion in gross revenue in 2025 but lost billions due to $7.5 billion in cost of revenue and massive R&D spending. This disclosure highlights the unsustainable cost structure of leading AI companies, raising concerns about the long-term viability of current business models and the need to balance R&D with profitability. OpenAI reported 900 million weekly active ChatGPT users but only 50 million paid subscribers, indicating a low conversion rate. R&D costs account for the largest portion of expenses.

hackernews · greenchair · Jun 17, 21:31 · [Discussion](https://news.ycombinator.com/item?id=48577208)

**Background**: OpenAI was founded as a non-profit but later transitioned to a capped-profit model. Training and running large AI models requires enormous computing resources, leading to high operational costs. Competitors like DeepSeek offer cheaper alternatives, pressuring OpenAI to justify its pricing.

**Discussion**: Commenters note that R&D is the main cost driver and question whether focus should shift to inference efficiency. Some observe the low paid-to-free user ratio and suggest OpenAI needs to grow 10x to become profitable. Others humorously remark that OpenAI remains a non-profit at heart.

**Tags**: `#OpenAI`, `#financials`, `#AI industry`, `#business model`, `#R&D costs`

---

<a id="item-4"></a>
## [GLM-5.2 tops open weights leaderboard on Artificial Analysis](https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index) ⭐️ 8.0/10

GLM-5.2, developed by Zhipu AI, has become the leading open-weights model on the Artificial Analysis intelligence index, approaching frontier performance at significantly lower cost. This release challenges proprietary models from Anthropic, OpenAI, and Google by offering near-frontier quality at a fraction of the price, potentially democratizing access to advanced AI. While GLM-5.2 excels on benchmarks, community users report that it can be inefficient on reasoning tasks, taking over 15 minutes and 45k tokens for a simple coding task.

hackernews · himata4113 · Jun 17, 09:12 · [Discussion](https://news.ycombinator.com/item?id=48567759)

**Background**: Open-weights models make their trained parameters publicly available, allowing anyone to use, modify, and deploy them. Artificial Analysis is an independent platform that compares AI models across intelligence, speed, and price metrics.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open-Weights Model? | AI21</a></li>
<li><a href="https://artificialanalysis.ai/models">Comparison of AI Models across Intelligence, Performance, and Price</a></li>
<li><a href="https://artificialanalysis.ai/leaderboards/models">LLM Leaderboard - Comparison of over 100 AI models from OpenAI...</a></li>

</ul>
</details>

**Discussion**: The community is highly engaged, with users praising the model's price-performance ratio but expressing concerns about reasoning efficiency. Some users note that unofficial providers offer even cheaper API rates, undercutting the official ZAI API.

**Tags**: `#AI`, `#open weights`, `#LLM`, `#model comparison`, `#artificial analysis`

---

<a id="item-5"></a>
## [U.S. science in chaos as funding and trust collapse](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

A Scientific American report details how the U.S. scientific enterprise is crippled by funding cuts, visa restrictions, and political interference, leading to a brain drain and widespread demoralization among researchers. This crisis threatens U.S. global leadership in research and innovation, potentially slowing critical scientific progress and weakening national competitiveness for decades. The article garnered 618 points and 702 comments, with personal accounts of scientists leaving the country, grant non-renewals, and visa barriers preventing hiring of international talent.

hackernews · presspot · Jun 17, 09:54 · [Discussion](https://news.ycombinator.com/item?id=48568058)

**Background**: For decades, U.S. science thrived on robust federal funding and a welcoming environment for global talent. Recent policy shifts have eroded this foundation, with cuts to agencies like NSF and NIH, and tightened immigration rules driving away researchers.

**Discussion**: Comments reflect deep despair: one user's wife is leaving the U.S. due to the research mess, another reports colleagues abandoning academia. However, a few see chaos as an opportunity for new funding models.

**Tags**: `#U.S. science`, `#research funding`, `#science policy`, `#brain drain`, `#academia`

---

<a id="item-6"></a>
## [Tesco Moves 40,000 Workloads Off VMware Over Broadcom Pricing](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

Tesco, the UK's largest supermarket chain, is migrating 40,000 server workloads off VMware due to Broadcom's abusive pricing and licensing practices. The migration is expected to take 18 months and involves switching to an unnamed alternative virtualization platform. This large-scale migration signals a growing enterprise exodus from VMware following Broadcom's acquisition, as major customers seek more cost-effective and flexible virtualization solutions. The move could accelerate industry-wide shifts away from VMware and encourage other large organizations to follow suit. The migration faces challenges because Tesco's new virtualization platform is incompatible with its existing Veeam and Zerto backup software. The 18-month timeline reflects the complexity of moving 40,000 workloads, though community members note that migration paths from VMware are now well-established.

hackernews · Bender · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576838)

**Background**: VMware is a leading virtualization platform that allows multiple operating systems to run on a single physical server. Broadcom acquired VMware in 2023 and subsequently made controversial changes to pricing, licensing, and support models, leading many customers to reconsider their reliance on VMware. Tesco operates one of the largest retail IT infrastructures in the UK, managing tens of thousands of virtual machines across its operations.

**Discussion**: Community commenters express strong support for Tesco's decision, with one noting that Broadcom's marketing is effectively driving customers to Proxmox. Another user questions the 18-month migration timeline, speculating it may stem from poor configuration management or lack of automation. A comment also highlights compatibility issues with backup software as a key challenge.

**Tags**: `#VMware`, `#Broadcom`, `#Virtualization`, `#Migration`, `#Tesco`

---

<a id="item-7"></a>
## [New HTTP QUERY Method Introduced in RFC 10008](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 8.0/10

RFC 10008 defines the new HTTP QUERY method, which allows safe and idempotent requests with a request body. This addresses the long-standing issues of using GET with a body and the non-idempotency of POST for queries. This method is significant for API design, providing a standardized way to perform complex queries (e.g., with large JSON filters or binary inputs) while preserving idempotency and cacheability. It bridges a gap between GET and POST, improving consistency in web standards. The QUERY method is both safe and idempotent, allowing request bodies that can be used for caching via bitwise comparison. It was preferred over extending GET with a body due to historical interoperability and architectural compliance considerations in HTTP.

hackernews · schappim · Jun 17, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48568502)

**Background**: In HTTP, GET is idempotent and cacheable but does not define semantics for a request body; POST can have a body but is not idempotent, causing issues like resubmission warnings on form refresh. The IETF working group considered allowing a body in GET but ultimately rejected it due to existing implementations that would break. The QUERY method solves this by providing a clean, new method with the desired properties.

<details><summary>References</summary>
<ul>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://horovits.medium.com/http-s-new-method-for-data-apis-http-query-1ff71e6f73f3">HTTP ‘s New Method For Data APIs: HTTP QUERY | Medium</a></li>
<li><a href="https://http.dev/query">QUERY - Expert Guide to HTTP methods</a></li>

</ul>
</details>

**Discussion**: Community comments expressed mixed views: some questioned the practicality of caching request bodies with unbounded size, while others appreciated the potential for HTML forms to avoid POST resubmission warnings. Overall, there was support for the new method but with lingering concerns about implementation complexity.

**Tags**: `#HTTP`, `#RFC`, `#web standards`, `#API design`, `#caching`

---

<a id="item-8"></a>
## [Physis Raises $100M+ for General World Foundation Model](https://36kr.com/p/3826129009234824?f=rss) ⭐️ 8.0/10

Physis, a world model startup, has raised over $100 million in seed++ funding and released its general world foundation model Physis-v0.1, with plans for a flagship model by end of 2026. This signals a major push toward general-purpose world models that understand physics, which could accelerate breakthroughs in embodied AI, robotics, and simulation, comparable to the GPT-3 to ChatGPT leap. Physis-v0.1 claims four capabilities: physical correctness, long-term consistency, action causality, and general generalization. The company will open-source model slices and publish technical reports. The team includes co-founders from Peking University and engineers from top tech firms.

rss · 36氪 · Jun 17, 01:00

**Background**: World models are AI systems that learn to simulate physical environments by predicting future states given actions, moving beyond text or video generation. A general world foundation model aims to unify physics reasoning across diverse domains like robotics, gaming, and scientific simulation. Unlike large language models, world models face challenges in data collection and must learn causality, not just correlation.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2024/12/14/what-are-ai-world-models-and-why-do-they-matter/">What are AI ' world models ,' and why do they matter? | TechCrunch</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/world-models/">What Is a World Model? | NVIDIA Glossary</a></li>
<li><a href="https://www.humai.blog/world-models-the-quiet-ai-revolution-that-could-make-llms-look-like-a-warmup-act/">World Models : The Quiet AI Revolution That Could Make LLMs Look...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#World Model`, `#Funding`, `#General Foundation Model`, `#Startup`

---

<a id="item-9"></a>
## [Leaders fear US AI cutoff; Anthropic blackout validates concern](https://techcrunch.com/2026/06/17/world-leaders-want-american-ai-they-just-dont-want-america-to-be-able-to-turn-it-off/) ⭐️ 8.0/10

At the G7 summit, French President Macron and Indian PM Modi expressed fears that the US could cut off access to American AI overnight, a concern made tangible by a recent blackout of Anthropic's AI services. This highlights growing international unease about US dominance in AI and the potential geopolitical leverage that control entails, affecting global AI adoption and governance. The meeting reportedly followed a brief blackout of Anthropic's AI systems, which some leaders saw as a demonstration of US ability to unilaterally restrict access to critical AI infrastructure.

rss · TechCrunch · Jun 17, 19:01

**Background**: The United States currently hosts most leading AI companies, including OpenAI, Google, and Anthropic. Many countries rely on these American AI services, creating a dependency that raises sovereignty concerns. The fear is that the US could enforce policies that cut off access, affecting national security and economic competitiveness.

<details><summary>References</summary>
<ul>
<li><a href="https://www.niemanlab.org/2025/05/anthropics-new-ai-model-didnt-just-blackmail-researchers-in-tests-it-tried-to-leak-information-to-news-outlets/">niemanlab.org/2025/05/anthropics-new-ai-model-didnt-just-blackmail...</a></li>

</ul>
</details>

**Tags**: `#AI governance`, `#geopolitics`, `#US AI dominance`, `#Anthropic`, `#policy`

---

<a id="item-10"></a>
## [Hackers breach tens of thousands of Fortinet firewalls using known passwords](https://techcrunch.com/2026/06/17/cybercriminals-allegedly-hacked-tens-of-thousands-of-fortinet-firewalls-used-by-major-companies-all-over-the-world/) ⭐️ 8.0/10

An alleged Russian-speaking cybercriminal group is compromising tens of thousands of Fortinet firewalls and VPNs used by major companies worldwide, exploiting previously known passwords rather than novel zero-day vulnerabilities. This large-scale breach affects major enterprises globally, highlighting the persistent risk of credential reuse and the importance of password hygiene, even as Fortinet and CISA have issued patches for related vulnerabilities. The attackers used previously known passwords to gain unauthorized access, not zero-day exploits. Fortinet has faced multiple critical vulnerabilities in 2025-2026, including CVE-2026-24858 and CVE-2025-59718/59719, which enable authentication bypass.

rss · TechCrunch · Jun 17, 18:20

**Background**: Fortinet firewalls and VPNs are widely used by enterprises to secure network perimeters. Cybercriminals often target these devices, and previous Fortinet vulnerabilities have been exploited in the wild. Using known passwords suggests the attackers may have obtained credentials from prior breaches or weak password practices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cisa.gov/news-events/alerts/2026/01/28/fortinet-releases-guidance-address-ongoing-exploitation-authentication-bypass-vulnerability-cve-2026">Fortinet Releases Guidance to Address Ongoing Exploitation of Authentication Bypass Vulnerability CVE-2026-24858 | CISA</a></li>
<li><a href="https://cybernews.com/security/fortinet-fortigate-vulnerability-exploit/">Hackers actively target Fortinet Firewall vulnerabilities | Cybernews</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#Fortinet`, `#firewall`, `#data breach`, `#cybercrime`

---

<a id="item-11"></a>
## [Odyssey hits $1.45B valuation with Amazon backing](https://techcrunch.com/2026/06/17/world-model-maker-odyssey-nabs-1-45b-valuation-backed-by-amazon-and-other-big-names/) ⭐️ 8.0/10

Odyssey, a world model AI startup, achieved a $1.45 billion valuation in a funding round backed by Amazon and other investors, signaling strong confidence in its approach. This funding validates world models as the next major AI frontier beyond large language models, and positions Odyssey as a key player in this emerging space. The round involved high-profile backers including Amazon, though the exact amount raised was not disclosed; the valuation nearly doubled from the previous round, reflecting rapid growth expectations.

rss · TechCrunch · Jun 17, 17:43

**Background**: World models are AI systems that build internal representations of environments to simulate dynamics like physics and causality, enabling planning and reasoning without continuous real-world interaction. They differ from traditional AI that merely classifies or generates outputs, and are considered a critical step toward more general intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#world models`, `#funding`, `#startups`, `#venture capital`

---

<a id="item-12"></a>
## [Adam (YC W25) Launches Open-Source AI CAD Platform](https://github.com/Adam-CAD/CADAM) ⭐️ 7.0/10

Adam (YC W25) launched CADAM, an open-source text-to-CAD platform that uses AI agents to generate parametric 3D models from natural language prompts and image references. This could democratize mechanical design by lowering the barrier to creating 3D models, and the open-source approach invites community contributions to advance AI-assisted CAD. It also signals growing integration of generative AI into engineering workflows. CADAM generates OpenSCAD code with automatically extracted parameters exposed as interactive sliders for instant dimension tweaking, runs fully in-browser via WebAssembly, and supports multiple LLMs including Claude, Gemini, and OpenAI via the Vercel AI SDK.

hackernews · zachdive · Jun 17, 16:14 · [Discussion](https://news.ycombinator.com/item?id=48572553)

**Background**: Text-to-CAD uses AI models to convert natural language descriptions into 3D models, often by generating script-based CAD code. Parametric modeling defines a model using adjustable parameters, enabling quick iterations. OpenSCAD is a script-based CAD tool that produces models from code. CADAM combines these by leveraging LLMs to write OpenSCAD code and expose parameters for editing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Parametric_modeling">Parametric modeling</a></li>
<li><a href="https://zoo.dev/zookeeper">ML CAD Model Generator | Create CAD Files With Text | Zoo</a></li>

</ul>
</details>

**Discussion**: Some engineers expressed skepticism, arguing that AI CAD is not yet practical for real mechanical design due to verification overhead. Others reported successful rapid generation for simple parts like grommets. The discussion also referenced competing projects such as Quidities and ModelRift.

**Tags**: `#AI CAD`, `#open source`, `#mechanical engineering`, `#text-to-CAD`, `#YC`

---

<a id="item-13"></a>
## [8-bit Live MLB Gamecast Website](https://ribbie.tv/watch) ⭐️ 7.0/10

A new website called ribbie.tv streams live MLB games as 8-bit pixel art gamecasts, converting real-time data into near-live visualizations. This project shows a creative use of real-time sports data and retro pixel art, engaging the community with an innovative viewing experience. It could inspire similar data-driven visualizations for other sports or events. The site features actual stadiums, day/night modes, between-inning graphics, and live scoreboards. Currently it streams multiple MLB games daily with near real-time updates.

hackernews · brownrout · Jun 17, 16:44 · [Discussion](https://news.ycombinator.com/item?id=48573012)

**Background**: 8-bit pixel art refers to a low-resolution, blocky visual style reminiscent of early video games. MLB provides official live data feeds that developers can use to create alternative gamecast experiences. This project combines both to offer a nostalgic and accessible way to follow baseball games.

**Discussion**: Feedback was generally positive, with praise for the concept and execution. Suggestions included using a real pixel font, adding sound effects, implementing a play-by-play view, and improving runner animations. Some users also shared related projects like a physical scoreboard using Raspberry Pis.

**Tags**: `#visualization`, `#baseball`, `#MLB`, `#pixel art`, `#web development`

---

<a id="item-14"></a>
## [Robot battle royale compares AI model cost efficiency](https://openrouter.ai/blog/insights/royale-last-agent-standing/) ⭐️ 7.0/10

A blog post describes an experiment where AI models including Claude and Grok compete in a battle royale game, with cost per kill as the key metric. This comparison highlights the real-world cost of deploying frontier AI models, showing that cost efficiency varies dramatically, which is critical for scaling AI applications. The experiment ran 30 games costing $482; frontier models like Opus 4.7 would have cost around $3,000. DeepSeek V4 Flash emerged as the most cost-effective.

hackernews · Usu · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576824)

**Background**: AI model comparison typically focuses on accuracy or speed, but this experiment uses a game environment to assess cost efficiency in a dynamic scenario. Battle royale games require both strategic reasoning and fast responses.

**Discussion**: Commenters noted the disturbing term 'cost per kill' (CPK) and discussed Grok's silent model upgrade and pricing change. DeepSeek V4 Flash was praised for coding performance.

**Tags**: `#AI`, `#cost-efficiency`, `#model comparison`, `#llm`

---

<a id="item-15"></a>
## [Human Connection: The AI-Proof Competitive Advantage](https://ghostinthedata.info/posts/2026/2026-06-13-human-connection-moat/) ⭐️ 7.0/10

An article argues that genuine human connection provides a durable competitive moat that AI cannot replicate, especially in customer service and hospitality. As companies increasingly automate customer interactions, this analysis challenges the assumption that efficiency alone wins, highlighting the strategic value of authentic human relationships. The article uses a restaurant example where online booking was adopted but reservation staff were retained, emphasizing that service and hospitality must both be present.

hackernews · speckx · Jun 17, 17:14 · [Discussion](https://news.ycombinator.com/item?id=48573435)

**Background**: A 'competitive moat' refers to a sustainable advantage that protects a business from competitors. In the AI era, many firms focus on automation to reduce costs, but this article argues that human connection creates loyalty and differentiation that technology cannot easily match.

**Discussion**: Commenters offered diverse perspectives: some rejected the desire for connection with businesses, wanting efficient transactions instead; others noted the irony of an AI-written post on human connection; and one emphasized the need for both hospitality and a good product, citing a personal banking example.

**Tags**: `#AI`, `#customer service`, `#human connection`, `#competitive advantage`, `#business strategy`

---

<a id="item-16"></a>
## [Volkswagen blocks GrapheneOS users from app and API](https://discuss.grapheneos.org/d/35949-volkswagen-app?page=3) ⭐️ 7.0/10

Volkswagen has started blocking users of the privacy-focused Android operating system GrapheneOS from accessing its official app and API, effectively cutting off community-driven integrations like Home Assistant automations. This move highlights growing corporate control over device ecosystems, forcing privacy-conscious users to choose between using their preferred OS and accessing vehicle features. It also raises concerns about anti-competitive behavior and user autonomy in connected cars. The block appears to be based on Play Integrity API checks, denying access to devices without Google Play Protect certification, which GrapheneOS intentionally avoids. Community projects like Home Assistant integrations for vehicle preheating and other automations are now broken.

hackernews · microtonal · Jun 17, 15:04 · [Discussion](https://news.ycombinator.com/item?id=48571526)

**Background**: GrapheneOS is a security-hardened, privacy-focused open-source operating system for Android devices, designed to minimize reliance on Google services. It does not include Google Play Services by default, meaning it fails hardware-level Play Integrity checks, which many apps use to ensure the device is 'safe'.

<details><summary>References</summary>
<ul>
<li><a href="https://www.layeronematerials.com/insights/what-is-graphene">What is Graphene ? — LayerOne Advanced Materials</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely negative, with users expressing frustration at Volkswagen's decision and its broader implications for privacy and open ecosystems. Some users are reconsidering purchasing Volkswagen vehicles, while others criticize the EU mandates that force connectivity in cars.

**Tags**: `#GrapheneOS`, `#Volkswagen`, `#privacy`, `#API`, `#Android`

---

<a id="item-17"></a>
## [Robotics scientist: Real scaling law lies in deployment, not data stacking](https://36kr.com/p/3856871787189252?f=rss) ⭐️ 7.0/10

In an interview, Luo Jianlan (Chief Scientist at Zhiyuan Robotics) argued that embodied AI cannot blindly replicate LLM-style scaling laws, and emphasized that real breakthroughs require closed-loop real-world deployment, not just offline training. This challenges the prevailing assumption that simply scaling data and model size will lead to general-purpose robots. It refocuses the industry on the practical bottlenecks of data collection, deployment, and iterative learning in physical environments. Luo introduced three technical pillars—SOP (scalable online post-training), LWD (learning while deploying), and τ0-WM (an action-conditioned world model). He also noted that most current 'robot foundation models' are closer to mid-training or fine-tuning, not true pre-training.

rss · 36氪 · Jun 17, 06:14

**Background**: In large language models, scaling laws describe predictable relationships between training loss and model performance as compute and data increase. Embodied AI faces additional challenges because low offline loss does not guarantee success in the open physical world. Luo argues that the true 'Scaling Law' for robotics emerges only when real-world deployment forms a closed loop of data collection, model improvement, and reduced adaptation cost.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2411.04434v1">Scaling Laws for Pre-training Agents and World Models</a></li>
<li><a href="https://medium.com/@wuxigudeyu/from-demos-to-deployment-the-real-bottleneck-in-humanoid-robotics-e1852575f416">From Demos to Deployment : The Real Bottleneck in... | Medium</a></li>

</ul>
</details>

**Tags**: `#embodied AI`, `#robotics`, `#Scaling Law`, `#real-world deployment`, `#industry analysis`

---

<a id="item-18"></a>
## [SK hynix Ships 12-Layer HBM4E Samples to Key Customers](https://36kr.com/newsflashes/3857909508576517?f=rss) ⭐️ 7.0/10

SK hynix announced that it has delivered samples of its 12-layer HBM4E memory chips to core customers. This marks a significant step in the advancement of high-bandwidth memory for AI and machine learning workloads, as HBM4E offers higher bandwidth and capacity than previous generations. The 12-layer HBM4E samples likely achieve over 3.6 TB/s bandwidth per stack and a 20% speed increase over HBM4, similar to Samsung's competing product.

rss · 36氪 · Jun 17, 23:48

**Background**: High Bandwidth Memory (HBM) is a 3D-stacked DRAM interface used in high-performance computing, especially AI accelerators and GPUs. HBM4E is an enhanced version of HBM4, offering higher data rates and efficiency. SK hynix is one of the leading manufacturers of HBM, along with Samsung and Micron.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://nerds.xyz/2026/06/samsung-hbm4e-memory/">Samsung ships industry-first HBM 4 E memory as AI infrastructure race...</a></li>
<li><a href="https://news.skhynix.com/meet-the-sk-hynix-team-behind-the-worlds-first-12-layer-hbm3/">Meet the SK hynix Team Behind the World's First 12 - Layer HBM 3</a></li>

</ul>
</details>

**Tags**: `#HBM`, `#Memory`, `#SK hynix`, `#AI Hardware`, `#Semiconductor`

---

<a id="item-19"></a>
## [Enterprises struggle with AI ROI after tokenmaxxing craze](https://techcrunch.com/video/neas-tiffany-luck-says-enterprises-are-still-figuring-out-their-ai-roi/) ⭐️ 7.0/10

NEA's Tiffany Luck highlighted that enterprises are grappling with AI ROI challenges after an aggressive push to maximize token usage, citing examples like Uber exceeding its annual AI budget in months and companies cutting Claude licenses. This signals a shift from unchecked AI spending to a demand for measurable returns, impacting enterprise AI adoption strategies and vendor relationships. Uber reportedly blew through its annual AI budget in a few months, some organizations cut Claude licenses for parts of their org, and Meta removed its internal AI leaderboard.

rss · TechCrunch · Jun 17, 20:17

**Background**: Tokenmaxxing is a trend where companies encourage employees to consume as many AI tokens as possible as a productivity benchmark. This often leads to inflated costs and lower code quality. AI vendors like Anthropic charge per token in higher-tier plans, making usage-based budgeting challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Token_maxxing">Token maxxing - Wikipedia</a></li>
<li><a href="https://blog.pragmaticengineer.com/the-pulse-tokenmaxxing-as-a-weird-new-trend/">The Pulse: ‘Tokenmaxxing’ as a weird new trend - The Pragmatic Engineer</a></li>
<li><a href="https://support.claude.com/en/articles/9797531-what-is-the-enterprise-plan">What is the Enterprise plan? | Claude Help Center</a></li>

</ul>
</details>

**Tags**: `#AI`, `#ROI`, `#enterprise`, `#tokenmaxxing`, `#industry-trends`

---

<a id="item-20"></a>
## [FTC lawsuit exposes subscription scam network tactics](https://techcrunch.com/2026/06/17/ftc-lawsuit-reveals-how-subscription-scam-networks-evade-app-store-enforcement/) ⭐️ 7.0/10

A new FTC lawsuit details how subscription scam app operators use shell companies and payment infrastructure to evade detection and remain active on app stores despite consumer complaints. This case highlights systemic weaknesses in app store enforcement and consumer protection, potentially leading to stronger regulations and improved fraud detection by platforms. The lawsuit alleges that scam networks employ shell companies to resurface under new identities and use complex payment systems to hide transactions, making it difficult for app stores to track and remove them.

rss · TechCrunch · Jun 17, 19:46

**Background**: Subscription scams trick users into paying for unwanted recurring charges. App stores like Apple's App Store and Google Play have policies against such practices, but enforcement relies on detecting patterns across thousands of apps, which scammers evade by constantly changing corporate identities and payment processors.

**Tags**: `#FTC`, `#subscription scams`, `#app store enforcement`, `#fraud`, `#consumer protection`

---

<a id="item-21"></a>
## [Anthropic first AI startup to join Frontier carbon removal coalition](https://techcrunch.com/2026/06/17/anthropic-becomes-first-ai-startup-to-join-the-frontier-carbon-removal-coalition/) ⭐️ 7.0/10

Anthropic has joined the Frontier coalition, which has received $915 million in pledges to fund carbon removal projects. This marks the first time an AI startup has joined the coalition. Anthropic's participation signals growing interest from AI companies in climate action and could encourage other tech firms to invest in carbon removal. The Frontier coalition's large fund helps scale emerging carbon removal technologies. The $915 million in pledges is a total amount from various members, not a new injection. Frontier was founded by Stripe, Shopify, and Alphabet, and pre-purchases carbon removal credits to de-risk startups.

rss · TechCrunch · Jun 17, 18:30

**Background**: Carbon removal technologies aim to extract CO2 from the atmosphere to mitigate climate change. The Frontier coalition is an advance market commitment that pools funds from major tech companies to buy future carbon removal credits, providing revenue certainty for developers. This model helps scale nascent technologies like direct air capture or BECCS.

<details><summary>References</summary>
<ul>
<li><a href="https://www.canarymedia.com/articles/emissions-reduction/frontier-bets-58.3m-on-carbon-removal-startup-vaulted-deep">Frontier bets $58.3M on carbon removal startup... | Canary Media</a></li>
<li><a href="https://trellis.net/article/mckinsey-google-others-invest-41million-next-gen-carbon-removal-project/">Google, McKinsey, others put $41 million in carbon removal plan</a></li>

</ul>
</details>

**Tags**: `#AI`, `#carbon removal`, `#climate`, `#Anthropic`, `#industry news`

---

<a id="item-22"></a>
## [Collecting robot training data is dirty work; AI labs pay XDOF](https://techcrunch.com/2026/06/17/collecting-robot-training-data-is-dirty-unglamorous-work-some-ai-labs-are-already-paying-xdof-to-do-it/) ⭐️ 7.0/10

AI labs are paying a company called XDOF to handle the labor-intensive and messy process of collecting real-world training data for robots, highlighting a key bottleneck in physical AI development. This matters because the quality and diversity of training data directly impacts the performance of embodied AI systems, and outsourcing the dirty work could accelerate progress in robotics. The article notes that collecting robot training data is 'dirty, unglamorous work,' and unlike text data for LLMs, robotics data collection often requires physical presence and domain expertise.

rss · TechCrunch · Jun 17, 15:00

**Background**: Embodied AI refers to AI systems that interact with the physical world through sensors and actuators, such as robots and autonomous vehicles. Training such systems requires vast amounts of real-world data, which is harder to collect than text or image data because it involves physical manipulation and environmental variability.

<details><summary>References</summary>
<ul>
<li><a href="https://toloka.ai/blog/robotics-training-data-collection-annotation/">How to build robotics training data that works in the real world</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/embodied-ai/">Embodied AI: What Is It and How to Build It?</a></li>
<li><a href="https://labelstud.io/blog/the-rise-of-real-world-robotics-and-the-data-behind-it/">The Rise of Real-World Robotics—and the Data Behind It | Label Studio</a></li>

</ul>
</details>

**Discussion**: No community comments were provided for this news item.

**Tags**: `#robotics`, `#AI`, `#training data`, `#embodied AI`

---

<a id="item-23"></a>
## [Pramaana Labs raises $27M seed for formal verification in AI](https://techcrunch.com/2026/06/17/pramaana-labs-raises-27-million-seed-round-from-khosla-ventures-to-bring-formal-verification-to-ai/) ⭐️ 7.0/10

Pramaana Labs, a startup applying formal verification to AI, has raised a $27 million seed round led by Khosla Ventures. The company will target high-stakes domains like law, drug discovery, and tax preparation. Formal verification provides mathematical guarantees of system correctness, which is critical for AI in high-stakes applications where errors are costly. This investment signals growing industry recognition of the need for rigorous AI safety methods. Formal verification uses mathematical models to prove or disprove correctness against a formal specification. Pramaana Labs plans to apply these methods to AI systems, starting with verticals where reliability is paramount.

rss · TechCrunch · Jun 17, 14:15

**Background**: Formal verification is a technique from hardware and software engineering that proves system correctness using mathematical logic. It is used in critical systems like cryptographic protocols and operating system kernels. Applying it to AI is a nascent but growing field, aiming to provide proofs of model behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification</a></li>
<li><a href="https://baohua.medium.com/formal-verification-the-final-line-of-defense-in-the-ai-era-494657f9c3c3">Formal Verification : The Final Line of Defense in the AI Era | Medium</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#AI safety`, `#funding`, `#Khosla Ventures`, `#high-stakes AI`

---

<a id="item-24"></a>
## [SpaceX alum raises $22M for rocket-engine geothermal plants](https://techcrunch.com/2026/06/17/spacex-alum-nabs-22m-to-turn-rocket-engines-into-geothermal-power-plants/) ⭐️ 7.0/10

Critical Energy, founded by a SpaceX veteran, raised $22 million to commercialize modular geothermal power plants based on rocket engine technology, aiming to build 300 GW per year by 2045. This cross-industry innovation could significantly reduce the cost and deployment time of geothermal energy, making it a more viable clean power source for AI data centers and other high-demand applications. The company's factory-built plants are shipped in standard containers and can be installed in as little as two weeks, leveraging rocket engine regenerative cooling technology for efficient heat extraction.

rss · TechCrunch · Jun 17, 13:30

**Background**: Rocket engines use regenerative cooling, where propellant is circulated around the combustion chamber to manage extreme heat. Critical Energy adapts this closed-loop heat transfer to extract geothermal heat from deep underground, enabling modular, rapidly deployable power plants. Traditional geothermal requires extensive drilling and custom construction, but this approach promises lower costs and faster scaling.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/17/spacex-alum-nabs-22m-to-turn-rocket-engines-into-geothermal-power-plants/">SpaceX alum nabs $22M to turn rocket engines into geothermal power plants | TechCrunch</a></li>
<li><a href="https://criticalenergy.com/">Critical Energy</a></li>

</ul>
</details>

**Tags**: `#geothermal energy`, `#space technology`, `#energy innovation`, `#startup`

---

<a id="item-25"></a>
## [US developers embrace Chinese AI for cost savings](https://restofworld.org/2026/when-americans-choose-chinese-ai/?utm_source=rss&utm_medium=rss&utm_campaign=feeds) ⭐️ 7.0/10

American developers are increasingly choosing Chinese AI models like DeepSeek, which provide sufficient quality at a fraction of the cost of alternatives like GPT-4. This trend indicates a shift in the AI industry where cost-effectiveness is becoming a key competitive factor, potentially challenging the dominance of expensive models from companies like OpenAI and Meta. DeepSeek's V3 model was trained for only $6 million, compared to the $100 million cost of GPT-4, and uses a Mixture-of-Experts (MoE) architecture with 671 billion total parameters, activating 37 billion per token.

rss · Rest of World · Jun 17, 10:00

**Background**: DeepSeek is a Chinese AI company that has developed large language models at a fraction of the cost of Western counterparts. Its success highlights how efficient architectures and training methods can achieve competitive performance without massive budgets. The company claims its V3 model uses one-tenth the computing power of Meta's Llama 3.1.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>
<li><a href="https://github.com/deepseek-ai/DeepSeek-V3">GitHub - deepseek-ai/DeepSeek-V3 · GitHub</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Chinese AI`, `#DeepSeek`, `#cost-effectiveness`, `#industry trends`

---

<a id="item-26"></a>
## [AI enables more elaborate cyber fraud in Asia: Interpol](https://www.scmp.com/news/asia/article/3357422/cyberfriendly-asia-online-crime-dominates-underworld-interpol-survey?utm_source=rss_feed) ⭐️ 7.0/10

According to a new Interpol report, illegal cyber activities now account for about a third of all crimes in some Asian countries, with AI enabling more elaborate and deceptive scams. The report highlights that online crimes are increasingly dominant compared to traditional illicit activities. This matters because the rapid adoption of digital services in Asia is being exploited by criminals using AI to create more convincing scams, posing persistent, large-scale challenges across multiple jurisdictions. It underscores the urgent need for enhanced cybersecurity measures and international cooperation. The Interpol report describes these online crimes as 'persistent, large-scale challenges affecting multiple jurisdictions' linked to rapid digital adoption. Scams are identified as the most widespread and financially damaging type of cyber fraud.

rss · SCMP · Jun 17, 09:09

**Background**: Interpol's cyber threat assessment surveys law enforcement agencies across member countries. AI technologies, such as deepfakes and automated phishing, are increasingly used by cybercriminals to enhance the credibility and reach of their scams. Asia's high digital penetration makes it a fertile ground for such activities.

**Tags**: `#cybersecurity`, `#AI`, `#fraud`, `#Asia`, `#Interpol`

---

<a id="item-27"></a>
## [Kingboard unit $1.5B stake sale to boost PCB capacity for AI](https://www.scmp.com/business/banking-finance/article/3357412/ai-boom-sparks-kingboard-subsidiarys-us15-billion-stake-sale-ramp-pcb-capacity?utm_source=rss_feed) ⭐️ 7.0/10

Kingboard Holdings is raising HK$11.77 billion (US$1.5 billion) by selling a stake in its listed subsidiary Kingboard Laminates Holdings, with proceeds earmarked to expand production capacity for laminates used in AI server circuit boards. This signals surging demand for AI hardware infrastructure and confirms that PCB laminate suppliers are scaling up to meet record server backlogs. The investment highlights the critical role of materials like copper-clad laminates in enabling high-performance AI computing. Kingboard Laminates is one of the world's largest laminate makers; the stake sale will fund capacity expansion for laminates used in AI servers. The fundraising occurs as AI server backlogs hit record highs at major manufacturers.

rss · SCMP · Jun 17, 08:45

**Background**: PCB laminates are base materials for printed circuit boards, typically made of fiberglass cloth impregnated with epoxy resin and bonded with copper foil. Copper-clad laminate (CCL) is the most common type, providing structural support and electrical connectivity. AI servers require advanced, high-layer-count PCBs that demand premium laminates with superior thermal and electrical properties, driving increased investment in production capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://jhdpcb.com/blog/pcb-laminate-materials-understand/">Fully Understand PCB Laminate Materials - Jhdpcb</a></li>
<li><a href="https://www.victorypcb.com/news/pcb-laminates.html">A Deep Dive into PCB Laminate Materials - VictoryPCB</a></li>
<li><a href="https://www.ourpcb.com/pcb-laminate-materials.html">PCB Laminate Materials: The Ultimate Guide</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#PCB manufacturing`, `#supply chain`, `#investment`

---

<a id="item-28"></a>
## [Thinking Out Loud with Others Boosts Problem-Solving](https://www.thesignalist.io/s/the-dialogue-dividend/) ⭐️ 6.0/10

An article argues that verbalizing thoughts to another person forces clarity and improves problem-solving, drawing parallels to the well-known rubber duck debugging technique in software engineering. This concept reinforces the value of pair programming and collaborative debugging, potentially improving team productivity and code quality in software development. The article highlights that the act of verbalization forces abstract thoughts into structured sentences, similar to writing. Rubber duck debugging relies on explaining code aloud to reveal errors.

hackernews · kodesko · Jun 17, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48569894)

**Background**: Rubber duck debugging is a method where a programmer explains their code step by step to an inanimate object or person to find bugs. It leverages the cognitive process of translating code into natural language, often revealing logical gaps. The article extends this technique to general problem-solving and communication.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubber_duck_debugging">Rubber duck debugging</a></li>
<li><a href="https://rubberduckdebugging.com/">Rubber Duck Debugging – Rubber Duck Debugging – Debugging ...</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree with the concept. Some argue that the key is the act of verbalization itself rather than the listener. Others share personal anecdotes about using the technique in pair programming or with non-technical partners. One commenter mentions Einstein thanking a colleague for similar discussions.

**Tags**: `#communication`, `#debugging`, `#thinking`, `#pair programming`

---

<a id="item-29"></a>
## [XianGong Intelligent files for HK IPO, five key insights from prospectus](https://36kr.com/p/3857011810112521?f=rss) ⭐️ 6.0/10

XianGong Intelligent, a leading robot controller maker, has filed for a Hong Kong IPO under Chapter 18C for specialty technology companies, with an offer price of HKD 101.60 per share and a market cap of approximately HKD 11.227 billion. The company, which claims the world's largest market share in robot controllers at 24.8%, is set to list on June 24, 2025. This IPO highlights the growing trend of robotics companies seeking public listings, and the detailed financial analysis reveals critical nuances about profitability and valuation that investors should understand. The company's unique business model—selling high-margin controllers but generating most revenue from low-margin robots—raises questions about long-term profitability and valuation sustainability at 22x price-to-sales. After adjusting for share-based payments, XianGong's 2025 net loss narrowed to RMB 4.71 million from RMB 47.7 million in 2023, but its adjusted net loss margin was only 0.6%, while the actual net loss margin was 10.7%. Additionally, its positive net assets depend on the termination of pre-IPO investor redemption rights; without that, net assets would have been negative in 2023 and 2024.

rss · 36氪 · Jun 17, 08:36

**Background**: Hong Kong's Chapter 18C listing rules allow specialty technology companies with high R&D spending but low revenue or losses to list on the HKEX. Pre-IPO investor redemption rights are common clauses that allow investors to demand repayment if an IPO does not occur by a certain date; their termination is often a condition for listing. XianGong Intelligent is a robot controller manufacturer; its controller acts as the 'brain' for various robots, with high gross margins of 79.8% compared to 38.4% for its complete robots.

<details><summary>References</summary>
<ul>
<li><a href="https://sp.capco.org.cn:82/file/202603/lianxihuiyuanshijiao/40.pdf">MEMBERS</a></li>
<li><a href="https://time-weekly.com/post/318346">华芢生物 IPO 投 研报告：不到3年累计净亏损3.55...</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#IPO`, `#AI`, `#controllers`, `#financial analysis`

---

<a id="item-30"></a>
## [Taiwei Quantum, a USTC PhD startup, secures funding for quantum components](https://36kr.com/p/3856755190551811?f=rss) ⭐️ 6.0/10

Taiwei Quantum (MQTEK), a neutral atom quantum computing component supplier founded by a USTC PhD, has completed angel and angel+ funding rounds from investors including Inno Angel, Dongfang Jiafu, and others. The funds will be used to expand production and R&D of its three core product lines: quantum gas microscopes, high-precision current sources, and a control system under development. As a 'water seller' providing upstream core components for quantum computing, Taiwei Quantum fills a critical gap in domestic supply chain for neutral atom and ion trap quantum computers. Its products offer superior performance at lower cost and shorter delivery times compared to foreign competitors, supporting China's self-reliance in quantum technology. The quantum gas microscope supports wavelengths from 313–1700 nm and millimeter-scale field of view, serving over ten domestic quantum startups. The current source achieves noise levels below 1 ppm, one-fifth of foreign competitors, at two-thirds the price and delivery within 2 months.

rss · 36氪 · Jun 17, 04:14

**Background**: Neutral atom quantum computing uses arrays of neutral atoms (e.g., rubidium-87) trapped in optical tweezers to encode qubits, offering scalability at room temperature. Quantum gas microscopes enable single-atom imaging and manipulation, crucial for building large atomic arrays. Ion trap quantum computing confines ions using electromagnetic fields for high-fidelity qubit operations.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/neutral_atom_quantum_computer">Neutral atom quantum computer</a></li>
<li><a href="https://www.emergentmind.com/topics/ion-trap-quantum-computing">Ion Trap Quantum Computing</a></li>

</ul>
</details>

**Tags**: `#quantum computing`, `#startup`, `#components`, `#funding`

---

<a id="item-31"></a>
## [China Regulators Announce Phased Launch of Active ETFs](https://36kr.com/newsflashes/3857922846283009?f=rss) ⭐️ 6.0/10

At the 2026 Lujiazui Forum on June 17, China Securities Regulatory Commission Chairman Wu Qing announced support for launching active ETFs on the Shanghai and Shenzhen stock exchanges, and the exchanges subsequently issued business guidelines clarifying development and investment operation requirements. This marks a major innovation in China's mutual fund industry, expanding investment tools and aligning China's market with global peers that already offer actively managed ETFs. It provides investors with more options for potential outperformance beyond passive index-tracking funds. The rollout will follow a phased, step-by-step approach, with pilot products launched first while supporting systems and ecosystem development are concurrently improved. Active ETFs differ from passive ETFs in that a professional manager actively selects and weights securities rather than tracking an index.

rss · 36氪 · Jun 18, 00:02

**Background**: Active ETFs are exchange-traded funds where a professional manager continuously picks and weights securities, aiming to outperform a benchmark. They combine the tax efficiency and intraday trading flexibility of traditional ETFs with active management. While active ETFs have grown dramatically in the U.S. and other markets, China's market has primarily offered passive ETFs until now. The introduction of active ETFs is seen as a way to enhance market efficiency and product diversity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-06-17/china-s-regulator-to-support-launch-of-active-etf-products">China ’s Regulator to Support Launch of Active ETF ... - Bloomberg</a></li>
<li><a href="https://www.fidelity.com/learning-center/investment-products/etf/actively-managed-etfs">Actively managed ETFs | Fidelity</a></li>

</ul>
</details>

**Tags**: `#mutual funds`, `#ETF`, `#China regulation`, `#financial innovation`

---

<a id="item-32"></a>
## [Glass Substrate Stocks Surge but Companies Say Still Early Stage](https://36kr.com/newsflashes/3857901341840388?f=rss) ⭐️ 6.0/10

A-share glass substrate concept stocks surged on June 17 following TSMC's announcement of its CoWoS glass substrate development plan, but companies like Qibin Group, Xingsen Tech, and Meidikai clarified that the technology is still in the technology reserve or R&D verification stage, with no immediate revenue impact. This highlights the gap between market speculation and technical reality in advanced semiconductor packaging; glass substrates could revolutionize chip performance, but commercialization is years away, affecting investors and the supply chain. Qibin Group achieved a three-day limit-up, while Changxin Technology, Meidikai, and Woge Optoelectronics also hit daily limits. The companies explicitly stated that glass substrate products are in early stages and not yet contributing to revenue.

rss · 36氪 · Jun 17, 23:40

**Background**: CoWoS (Chip-on-Wafer-on-Substrate) is an advanced packaging technology from TSMC that integrates multiple chips on a silicon interposer. Glass substrates are an emerging alternative to traditional organic substrates, offering better heat dissipation, flatness, and electrical performance for high-performance computing and AI. However, manufacturing challenges such as through-glass via (TGV) formation and handling remain unsolved for mass production.

<details><summary>References</summary>
<ul>
<li><a href="https://3dfabric.tsmc.com/english/dedicatedFoundry/technology/cowos.htm">CoWoS ® - Taiwan Semiconductor Manufacturing Company Limited</a></li>
<li><a href="https://www.3dgsinc.com/">Advanced Glass Substrates for Semiconductor Packaging - 3DGS</a></li>
<li><a href="https://anyglasstgv.com/en/sub/applications/glass/void-free-glass-substrates.php">Strengthen Packaging with Glass Substrate , ANYCASTING</a></li>

</ul>
</details>

**Tags**: `#Glass Substrate`, `#Advanced Packaging`, `#CoWoS`, `#Semiconductor Industry`, `#Stock Market`

---

<a id="item-33"></a>
## [ASML CEO Warns of Supply Risks for Musk's Terafab](https://www.bloomberg.com/news/articles/2026-06-17/asml-ceo-warns-of-possible-supply-constraints-on-musk-s-terafab) ⭐️ 6.0/10

ASML CEO Christophe Fouquet expressed concern that the company may face supply constraints when servicing new projects like Elon Musk's Terafab, a massive semiconductor manufacturing facility. This highlights potential bottlenecks in the chip equipment supply chain that could delay ambitious projects like Terafab, affecting the broader semiconductor industry's ability to meet future demand for AI and advanced chips. ASML is the sole supplier of extreme ultraviolet (EUV) lithography machines essential for advanced chip manufacturing, making its supply chain health critical for projects like Terafab.

rss · Bloomberg Markets · Jun 17, 15:27

**Background**: ASML is a Dutch company that dominates the market for lithography systems used to print circuit patterns onto silicon wafers. Its EUV machines are crucial for producing the most advanced chips at scale. Elon Musk's Terafab, announced in March 2026, is a proposed $25 billion AI and semiconductor facility in Austin, Texas, aiming to boost chip production for AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/terafab-25-billion-gamble-rewrite-rules-silicon-data-center-david-cao-gsibc">Terafab : Elon Musk 's $25 Billion Gamble to Rewrite the Rules of...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#ASML`, `#supply chain`, `#Elon Musk`, `#chip manufacturing`

---

<a id="item-34"></a>
## [VC: Real AI winners won't sell AI](https://techcrunch.com/2026/06/17/chi-hua-chien-saw-facebook-coming-now-he-says-the-real-ai-winners-wont-be-selling-ai/) ⭐️ 6.0/10

Venture capitalist Chi-Hua Chien argues that the most successful AI companies will integrate AI into broader products rather than selling AI as a standalone offering. This contrarian view challenges the current hype around standalone AI startups and suggests long-term value lies in AI-enhanced applications and platforms. Chien, a veteran VC who correctly anticipated Facebook's rise, draws on two decades of experience to emphasize that integration beats commoditization in technology markets.

rss · TechCrunch · Jun 17, 21:30

**Background**: The AI industry is currently flooded with startups selling AI models and APIs directly. Historical patterns in tech show that the biggest winners often embed new technology into existing products or create new user experiences around it.

**Tags**: `#AI`, `#venture capital`, `#business strategy`, `#technology trends`

---

<a id="item-35"></a>
## [Social media’s next evolution: user-controlled algorithms](https://techcrunch.com/2026/06/17/social-medias-next-evolution-user-controlled-algorithms/) ⭐️ 6.0/10

Platforms like Threads, Instagram, and TikTok are introducing tools that allow users to directly influence their recommendation algorithms. This shift could improve user satisfaction by giving people more control over their feeds, reducing frustration from missing important updates, and potentially altering content moderation dynamics. The article does not specify technical implementations or release dates, but highlights a broader industry trend toward algorithmic transparency and user empowerment.

rss · TechCrunch · Jun 17, 18:19

**Background**: Social media algorithms typically use machine learning to rank content based on predicted relevance, often prioritizing engagement. User-controlled algorithms represent a departure from this opaque, one-size-fits-all approach, giving individuals the ability to shape their own experience.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/17/social-medias-next-evolution-user-controlled-algorithms/">Social media ’s next evolution: user - controlled algorithms</a></li>
<li><a href="https://www.okoone.com/spark/product-design-research/why-social-media-feels-so-frustrating-and-how-it-got-this-way/">Why social media feels so frustrating and how it got this way | Okoone</a></li>

</ul>
</details>

**Tags**: `#social media`, `#algorithms`, `#personalization`, `#tech news`

---

<a id="item-36"></a>
## [Stanford Grads Raise $11M for Noninvasive Hormone Tracker](https://techcrunch.com/2026/06/17/two-stanford-grads-raise-11m-to-build-a-noninvasive-wearable-for-hormone-tracking/) ⭐️ 6.0/10

Clair Health, founded by two Stanford graduates, raised $11 million to develop a noninvasive wearable that tracks hormones by monitoring inflammation, energy levels, and menstrual cycle phases. This funding advances continuous hormone monitoring, which could help millions manage cycle irregularities, perimenopause, and overall hormonal health without invasive blood draws. The device features 10 biosensors including a novel biomagnetic sensor, and offers insights into inflammation, bloating, energy, and cycle phase classification, though it trades some accuracy for continuous convenience compared to blood tests.

rss · TechCrunch · Jun 17, 16:54

**Background**: Traditional hormone testing relies on blood draws that are expensive, infrequent, and invasive. Noninvasive wearables aim to provide real-time, continuous estimates by analyzing biomarkers in sweat or other bodily fluids, but they have historically been limited to tracking only a few hormones like cortisol or estrogen. Clair's device seeks to broaden the scope to include cycle phase and perimenopause markers, addressing a significant gap in women's health monitoring.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/17/two-stanford-grads-raise-11m-to-build-a-noninvasive-wearable-for-hormone-tracking/">Two Stanford grads raise $11M to build a noninvasive wearable for...</a></li>
<li><a href="https://healthcarediscovery.ai/clair-continuous-hormone-monitoring-wearable/">Clair: Non - Invasive Continuous Hormone Tracking Wearable</a></li>

</ul>
</details>

**Tags**: `#wearable`, `#hormone tracking`, `#health tech`, `#startup`, `#funding`

---

<a id="item-37"></a>
## [Google bets on Gemini to reinvent smart home speaker](https://techcrunch.com/2026/06/17/google-bets-on-gemini-to-reinvent-the-smart-home-speaker/) ⭐️ 6.0/10

Google launched a $99.99 Google Home Speaker that replaces rigid Google Assistant commands with conversational Gemini generative AI interactions. This marks a shift from traditional voice assistants to generative AI, potentially making smart home interactions more natural and engaging, and setting a new standard for the industry. The new speaker is priced at $99.99 and replaces the previous Google Assistant-based smart speaker. It leverages Gemini's large language model for more fluid, context-aware conversations rather than fixed command phrases.

rss · TechCrunch · Jun 17, 16:30

**Background**: Google Gemini is a family of large language models developed by Google, succeeding LaMDA and PaLM. It powers conversational AI across Google products, including a new smart speaker. Traditional smart speakers rely on predefined commands, whereas Gemini enables open-ended dialogue.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Gemini_image_generation_controversy">Google Gemini image generation controversy</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Gemini">Google Gemini - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#generative AI`, `#smart home`, `#Google`, `#Gemini`, `#voice assistants`

---

<a id="item-38"></a>
## [PayPal Ventures Shuts Down After a Decade](https://techcrunch.com/2026/06/17/paypal-ventures-shutters-as-company-restructuring-continues/) ⭐️ 6.0/10

PayPal has shut down its corporate venture capital arm, PayPal Ventures, after 10 years and approximately 80 investments, as part of a broader restructuring at the company. This indicates a strategic shift at PayPal, potentially reducing its direct influence on the fintech startup ecosystem and signaling a more conservative approach to external innovation. PayPal Ventures was launched in 2016 and invested in companies including Acorns, Honey (later acquired by PayPal), and TripActions. The closure follows other restructuring moves, such as layoffs and divestitures.

rss · TechCrunch · Jun 17, 16:10

**Background**: Corporate venture capital (CVC) arms allow large companies to invest in startups for strategic and financial returns. PayPal Ventures was one of many fintech-focused CVC funds. Its closure reflects a trend of large tech firms reassessing their venture investment strategies amid economic pressures.

**Tags**: `#venture capital`, `#corporate restructuring`, `#PayPal`, `#fintech`, `#startup ecosystem`

---

<a id="item-39"></a>
## [China vows new legal shield to counter US sanctions, protect finance](https://www.scmp.com/economy/china-economy/article/3357417/china-vows-new-legal-shield-could-counter-us-sanctions-and-protect-finance?utm_source=rss_feed) ⭐️ 6.0/10

Vice-Premier He Lifeng announced at the Lujiazui Forum that China will incorporate blocking and countermeasure provisions into upcoming financial legislation to counter what it considers improper extraterritorial sanctions. This move could legally empower Chinese firms to resist US secondary sanctions, potentially impacting international businesses operating in China and escalating legal tensions between the US and China. The announcement was made at the Lujiazui Forum in Shanghai on Wednesday. China has previously used its blocking law against US sanctions on Chinese refineries in 2026, notably targeting Hengli Petrochemical and others.

rss · SCMP · Jun 17, 09:00

**Background**: Blocking statutes are laws designed to nullify the effects of foreign extraterritorial sanctions within the enacting country's jurisdiction. The European Union enacted a similar blocking regulation in 1996 to counter US sanctions on Cuba, Iran, and Libya. China's move builds on its 2021 Blocking Rules, which provide a framework for countermeasures. Extraterritorial sanctions impose legal obligations on entities outside the sanctioning country, which is controversial under international law.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blocking_statute">Blocking statute - Wikipedia</a></li>
<li><a href="https://www.geopolitechs.org/p/china-uses-blocking-law-for-first">China Uses Blocking Law for First Time to Counter U.S. Sanctions on Chinese Teapot Refineries Before Trump Visit</a></li>
<li><a href="https://en.wikipedia.org/wiki/Extraterritorial_jurisdiction">Extraterritorial jurisdiction - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#sanctions`, `#China`, `#finance`, `#geopolitics`, `#legal`

---