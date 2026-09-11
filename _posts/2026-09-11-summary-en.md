---
layout: default
title: "Horizon Summary: 2026-09-11 (EN)"
date: 2026-09-11
lang: en
---

> From 120 items, 23 important content pieces were selected

---

1. [OpenAI's Navier–Stokes counterexample ships with a Lean 4 formal proof](#item-1) ⭐️ 9.0/10
2. [Shopify moves its mobile app from React Native back to native Swift and Kotlin](#item-2) ⭐️ 8.0/10
3. [Researchers question whether OpenAI can be trusted with unpublished math](#item-3) ⭐️ 8.0/10
4. [Forgejo 16.0.4 Patches Critical RCE Flaws](#item-4) ⭐️ 8.0/10
5. [IDScan Confirms Breach Affecting Over 150 Million Driver's Licenses](#item-5) ⭐️ 8.0/10
6. [OpenAI Launches Hosted Agents API With Managed Harness](#item-6) ⭐️ 7.0/10
7. [Cognition launches SWE-2 coding model, drawing benchmark skepticism](#item-7) ⭐️ 7.0/10
8. [NASA's Decorrelation Stretch Reveals Hidden Ancient Rock Art](#item-8) ⭐️ 7.0/10
9. [PlanetScale Launches Neki, a Closed-Source Sharded Postgres](#item-9) ⭐️ 7.0/10
10. [Microsoft Elevates Rust to Tier-1 Language Status](#item-10) ⭐️ 7.0/10
11. [China Halts New Battery Factory Construction Pending Capacity Review](#item-11) ⭐️ 7.0/10
12. [Pocket FM doubles revenue run rate to $500M with AI-made audio content](#item-12) ⭐️ 7.0/10
13. [Google Earth's 24-hour AI feature exposed deepfake trust risks](#item-13) ⭐️ 7.0/10
14. [Anthropic accuses DeepSeek and Moonshot of covertly routing requests to Claude](#item-14) ⭐️ 7.0/10
15. [Chinese scientists quadruple hydrogen fuel cell power in new design](#item-15) ⭐️ 7.0/10
16. [Huawei unveils industry-first 7.2 Tbps near-packaged optics module](#item-16) ⭐️ 7.0/10
17. [Meta Reportedly Takes Over Muse's Social Media Handles for Its AI Product](#item-17) ⭐️ 7.0/10
18. [IDScan confirms breach exposing 150M+ driver's licenses](#item-18) ⭐️ 7.0/10
19. [Anthropic Alleges Distillation Attacks by Alibaba, Moonshot AI, DeepSeek](#item-19) ⭐️ 6.0/10
20. [Proxima Fusion to build €140M factory for fusion-grade HTS tape](#item-20) ⭐️ 6.0/10
21. [Bending Spoons to buy collaboration tools maker Miro for $1.36B, 90% less than its 2022 valuation](#item-21) ⭐️ 6.0/10
22. [DeepSeek launches V4.1 Flash, claiming it beats Kimi K3 on coding](#item-22) ⭐️ 6.0/10
23. [Florida Woman Sues Over Wrongful Arrest Tied to Flock Camera Data](#item-23) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI's Navier–Stokes counterexample ships with a Lean 4 formal proof](https://www.johndcook.com/blog/2026/09/09/formal-method-revolution/) ⭐️ 9.0/10

OpenAI's September 2026 release of an unbounded counterexample to the Navier–Stokes existence and smoothness problem included a Lean 4 formal proof, meaning the argument was written in a machine-checkable form rather than only as prose mathematics. A write-up on John D. Cook's blog frames the episode as evidence of a broader "formal method revolution" in which AI systems emit verified proofs alongside their results. If the formalization holds up, this would be the first time an AI system has produced a machine-checked proof for a problem on the scale of a Millennium Prize problem, which could change how mathematicians, journals, and funding bodies think about validating results. It also raises a hard practical question: formal verification is only as useful as it is affordable, and the community discussion suggests checking such proofs can already take hours of compute and hundreds of gigabytes of memory. The Lean 4 proof is machine-checkable in principle, but the underlying counterexample has not yet been independently verified by external mathematicians, and researchers Levent Alpöge and Tristan Buckmaster have raised concerns about whether their related work entered OpenAI's training data (OpenAI calls this "categorically impossible"). Community commenters also point to the economics involved: roughly 880,000 hours of human labor at $150/hour would cost about $132 million, versus an estimated $40 million of agent compute for the release, and Lean's checking of a Fermat's Last Theorem-scale proof reportedly took around 15 hours with 230GB of RAM compared with 11 days to generate the code.

hackernews · ibobev · Sep 10, 21:22 · [Discussion](https://news.ycombinator.com/item?id=49650326)

**Background**: The Navier–Stokes equations describe the motion of viscous fluids, and the existence and smoothness problem asks whether smooth (infinitely differentiable) solutions always exist in three-dimensional space; it is one of the seven Millennium Prize Problems for which the Clay Mathematics Institute offered $1 million in 2000. Lean 4 is an open-source interactive theorem prover and dependently typed functional programming language based on the calculus of inductive constructions, self-hosting since version 4 in 2023, in which a mathematical proof is expressed as a program that a small kernel checks for correctness. OpenAI announced the counterexample on 8 September 2026, following published work by Alpöge and Buckmaster on finite-time blowup for the 3D incompressible Euler equations with smooth forcing; the result still awaits external validation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier-Stokes_equations">Navier-Stokes equations</a></li>
<li><a href="https://en.wikipedia.org/wiki/Navier–Stokes_existence_and_smoothness">Navier–Stokes existence and smoothness - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lean_(proof_assistant)">Lean (proof assistant)</a></li>

</ul>
</details>

**Discussion**: Commenters largely accepted the result as remarkable while arguing about everything around it: one noted that Lean is slow enough that verifying a Fermat's Last Theorem-scale proof was only about an order of magnitude faster than agents generating it (15 hours and 230GB of RAM versus 11 days), and asked whether Lean can be optimized without sacrificing auditability. Others felt the discussion avoided the actual mathematics, estimating that the "four orders of magnitude" cost comparison is overstated (about $132M of human labor versus ~$40M of agents), argued the old "forty hours per page" benchmark reflects the lack of proof automation in 2005 rather than Lean's limits, and raised the unsettling scenario of an AI solution that humans cannot independently verify because checking it needs intelligence or resources they do not have.

**Tags**: `#AI`, `#Lean 4`, `#formal verification`, `#Navier-Stokes`, `#theorem proving`

---

<a id="item-2"></a>
## [Shopify moves its mobile app from React Native back to native Swift and Kotlin](https://shopify.engineering/back-to-native) ⭐️ 8.0/10

Shopify published an engineering post announcing it is migrating its flagship mobile app away from React Native and back to platform-native Swift for iOS and Kotlin for Android, reversing a decision it originally made in 2020. In the discussion, Shopify's Fahd N. Thawar explained that LLMs changed one of the core assumptions behind the 2020 decision, so the team reevaluated its approach rather than sticking with a choice just because it had once worked. This is one of the highest-profile reversals of the cross-platform bet by a major e-commerce company, and it lands in the middle of a long-running debate over shared codebases versus fully native apps. If LLM-assisted rewrites really do lower the cost of going native, the calculus that pushed many startups toward React Native — reusing web developers for mobile — could weaken for larger product teams as well. Commenters stress that LLMs were not the whole story: one engineer who led a similar React Native-to-Swift/Kotlin rewrite said most of that work happened before 2026 and without LLM code assistance, implying the migration was viable on its own. Another developer reported that with an LLM coding agent plus an existing UI-test setup such as Maestro, an app with roughly 15–20 screens was ported to both iOS and Android largely overnight, with a few days of follow-up polish.

hackernews · fnthawar2 · Sep 10, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49643982)

**Background**: React Native is an open-source UI framework created by Meta (then Facebook) that lets developers build Android and iOS apps in JavaScript using React, with the slogan "learn once, write anywhere." Its main selling point is a single shared codebase and the ability to reuse web developers for mobile work, at the cost of indirect access to native platform APIs and the performance/polish that platform-specific Swift and Kotlin code can offer. Shopify adopted React Native around 2020 as part of that shared-codebase strategy, and its flagship shopping app is a large, long-lived production codebase, which makes a reversal costly and therefore notable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/React_Native">React Native - Wikipedia</a></li>
<li><a href="https://reactnative.dev/">React Native · Learn once, write anywhere</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (737 points, 491 comments) is broadly sympathetic to leaving React Native, with one iOS engineer saying the decision validated a career spent arguing against C-level pushes for a shared codebase. The sharpest disagreement targets the framing that LLMs made an otherwise unaffordable migration possible: several commenters argue the migration would have been worth doing anyway, and that RN's original appeal — letting web developers ship mobile — fades now that so much code is machine-generated, making it more sensible to simply start native.

**Tags**: `#React Native`, `#mobile development`, `#iOS`, `#Android`, `#Shopify`

---

<a id="item-3"></a>
## [Researchers question whether OpenAI can be trusted with unpublished math](https://mathstodon.xyz/@andreasthom/117240535270608201) ⭐️ 8.0/10

A Hacker News thread (628 points, 611 comments) has surfaced a debate over whether mathematicians can trust OpenAI with unpublished work, following allegations that researcher chats with OpenAI models may have shaped results OpenAI later claimed as its own without attribution. The discussion was seeded by posts on Mathstodon from @andreasthom, plus a linked X thread from Valerio Capraro and a Bluesky post. If a frontier AI lab can absorb unpublished research through user chats and then publish results without credit, the norms of academic attribution and the willingness of researchers to use hosted models are both put at risk. This matters well beyond mathematics, since it touches on the data-provenance and consent questions now facing every AI lab that trains on user interactions. The core dispute is one of provenance rather than capability: commenters note it is hard to distinguish genuine reinforcement-learning-driven discovery from recall of a human's hint that was absorbed during pretraining, and OpenAI's claim that the model was not trained on the collaborative chats is precisely the claim being questioned. The thread also cites OpenAI's practice of granting large numbers of researchers free access to its models, which expands the surface area for such contamination.

hackernews · pred_ · Sep 10, 06:49 · [Discussion](https://news.ycombinator.com/item?id=49639408)

**Background**: Mathstodon is a Mastodon (fediverse) instance set up by mathematicians as a Twitter alternative, which is why the original posts appear there rather than on a major platform; the thread also links to mirrors such as xcancel.com, a privacy-respecting X/Twitter frontend, and to a Bluesky post identified by a did:plc decentralized identifier. Open mathematical problems are long-standing unsolved conjectures, and claims that an AI model solved or advanced one are difficult to verify without knowing whether the model had seen related human reasoning. Attribution norms in mathematics are strong, so an uncredited reuse of a collaborator's idea is treated as serious misconduct when the collaborator is human.

<details><summary>References</summary>
<ul>
<li><a href="https://terrytao.wordpress.com/2022/11/20/trying-out-mathstodon/">Trying out Mathstodon | What's new - Terence Tao</a></li>
<li><a href="https://docs.bsky.app/docs/advanced-guides/resolving-identities">Resolving Identities | Bluesky</a></li>

</ul>
</details>

**Discussion**: Sentiment is largely skeptical, though not unanimous. nezi argues via analogy that if OpenAI were a human collaborator who took researchers' ideas and published without credit, it would be plainly unethical; sashank_1509 counters that both claims can be true at once, since pretraining recall and genuine RL-driven discovery are not mutually exclusive; bertonvv wonders whether rapid AI progress on open problems is partly an artifact of researchers feeding fresh results into the models; and aprentic broadens the point to the generally weak protection of user data by companies with strong profit incentives to exploit it.

**Tags**: `#AI ethics`, `#OpenAI`, `#research integrity`, `#data provenance`, `#mathematics`

---

<a id="item-4"></a>
## [Forgejo 16.0.4 Patches Critical RCE Flaws](https://codeberg.org/forgejo/forgejo/src/branch/forgejo/release-notes-published/16.0.4.md) ⭐️ 8.0/10

Forgejo released version 16.0.4, fixing critical remote code execution (RCE) vulnerabilities, most notably a template-expansion flaw that occurs during repository initialization from a template. The issue arises because Forgejo clones a template repository, removes the .git folder, performs variable template expansion on files listed in .forgejo/template, and then initializes a new git repository, allowing malicious expansion during that process. Forgejo is a widely used self-hosted Git forge, so a critical RCE affects anyone running an unpatched instance and could let attackers execute arbitrary code on the server. The disclosure also fuels a broader debate about vulnerability discovery in open-source forges, including whether AI-assisted hunting gives attackers an edge. The release notes highlight the fix as a 'Critical' item, specifically preventing template expansion from interfering with git repo initialization, with a linked pull request (#14301) documenting the change. Notably, Gitea project leadership stated that Gitea is protected against both issues, and the release notes page was initially hard to read due to Codeberg rate limits.

hackernews · weierstass · Sep 10, 15:57 · [Discussion](https://news.ycombinator.com/item?id=49645907)

**Background**: Forgejo is a cross-platform, open-source, self-hosted software forge written in Go that uses Git for version control and adds features like bug tracking, code review, continuous integration, and wikis; it is a community-driven fork of Gitea, which itself is a fork of Gogs. The vulnerable workflow involves creating a new repository from a template repository: Forgejo clones the template, strips the .git folder, expands template variables in specified files, and re-initializes a fresh git repository. Remote code execution (RCE) is among the most severe classes of vulnerabilities, as it lets an attacker run arbitrary commands on the victim's server.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Forgejo">Forgejo</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gitea">Gitea</a></li>
<li><a href="https://forgejo.org/">Forgejo – Beyond coding. We forge .</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the release notes page was unreadable due to Codeberg rate limits and helpfully quoted the fixes, while Gitea's project lead (with a bias disclosure) confirmed Gitea was unaffected and urged people not to shame vulnerability reporters. A notable debate emerged over whether Forgejo's ban on LLM contributions leaves it at a disadvantage, since attackers may still use AI to hunt for vulnerabilities.

**Tags**: `#security`, `#forgejo`, `#gitea`, `#remote-code-execution`, `#vulnerability-disclosure`

---

<a id="item-5"></a>
## [IDScan Confirms Breach Affecting Over 150 Million Driver's Licenses](https://techcrunch.com/2026/09/10/id-verification-giant-idscan-confirms-data-breach-with-more-than-150-million-drivers-licenses-stolen/) ⭐️ 8.0/10

Identity-verification company IDScan confirmed that it suffered a data breach in which more than 150 million driver's licenses and other government-issued identity documents were stolen, along with people's full names. The company acknowledged the incident publicly, confirming the massive scale of the exposure. IDScan is a third-party identity-verification provider, so a breach of this size means the compromised documents likely originate from many different organizations and services that relied on it to check customers' IDs. Because driver's licenses and similar documents are widely used as proof of identity, the stolen data could fuel identity theft, account takeover, and fraud for years, affecting far more people than just IDScan's direct users. The exposed data includes full names and driver's licenses plus other government-issued identity documents, according to the company's confirmation. The available reporting does not detail how the breach occurred, when it happened, or how many distinct individuals are affected versus how many document records were taken.

rss · TechCrunch · Sep 10, 13:21

**Background**: Identity-verification (often called IDV or KYC) companies sit between businesses and their customers: banks, crypto exchanges, gig platforms and others send photos of a customer's government ID to a service like IDScan to confirm the person is real and matches the document. That business model requires accumulating huge repositories of sensitive identity documents, including driver's licenses, passports and other government IDs, which makes such vendors high-value targets for attackers. When these troves leak, criminals can use the document images and personal details to open fraudulent accounts, pass verification checks elsewhere, or impersonate victims.

**Tags**: `#data-breach`, `#cybersecurity`, `#privacy`, `#identity-verification`, `#drivers-licenses`

---

<a id="item-6"></a>
## [OpenAI Launches Hosted Agents API With Managed Harness](https://developers.openai.com/api/docs/guides/agents-api/overview) ⭐️ 7.0/10

OpenAI released a hosted Agents API that runs the Codex harness and manages the underlying agent infrastructure, so developers can create a production-ready agent in a single API call by specifying the task, model, tools and environment. The API is organized around four concepts — Agent, Environment, Session, and Events/items — and includes automatic context compaction, multi-agent orchestration, programmatic tool calling, and MCP server support. This is a strategically important platform play in the fast-growing agent harness space, positioning OpenAI as the host of agent execution rather than just a model provider. It could simplify agent development for teams that lack the resources to build their own harness, while simultaneously raising vendor lock-in concerns for those who already run self-managed stacks. The Environment concept is optional and OpenAI says you can self-host your sandbox instead of using the OpenAI-hosted one, which materially eases switching between providers. Community members also noted that reasoning tokens are not exposed to paying customers, and that the hosted harness may be aimed at bundling capabilities that aren't offered as standalone API endpoints.

hackernews · aquir · Sep 10, 19:43 · [Discussion](https://news.ycombinator.com/item?id=49649213)

**Background**: An "agent harness" is the scaffolding around a large language model that lets it call tools, read and write files, keep state across steps, and recover from errors; building one from scratch is a large engineering effort. OpenAI's Agents API abstracts that layer away, keeping the agent's session state on OpenAI's servers and running the agent in a sandbox environment that can access files, load skills and execute commands. Alternatives exist, ranging from open-source harness libraries to self-hosted sandboxes built on containers or microVMs.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/agents-api/overview">Agents API | OpenAI API</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/agents">Agents SDK | OpenAI API</a></li>
<li><a href="https://openai.com/index/introducing-the-agents-api/">Introducing the Agents API | OpenAI</a></li>

</ul>
</details>

**Discussion**: HN commenters agreed the right abstraction for agents-as-a-product is still unsettled, noting that building your own harness is a deep rabbit hole while open-source harnesses remain coupled to an environment. Several pointed to self-hosting paths that reduce lock-in — one reported great success running Codex inside a QEMU VM with remote control from a phone, and another flagged the self-hosted sandbox option in the docs as making the offering much more enticing. Sceptics criticized the push toward lock-in and the withholding of reasoning tokens, and speculated that this may become a durable moat and a vector for bundling capabilities not available as direct APIs.

**Tags**: `#OpenAI`, `#AI Agents`, `#API Design`, `#Vendor Lock-in`, `#LLM Infrastructure`

---

<a id="item-7"></a>
## [Cognition launches SWE-2 coding model, drawing benchmark skepticism](https://cognition.com/blog/swe-2) ⭐️ 7.0/10

Cognition, the company behind the Devin coding agent, announced SWE-2, a new coding model post-trained from Moonshot AI's Kimi K3. The company claims the model reaches parity with rival frontier systems such as Fable 5.1 and GPT-Astra. The release shows that a relatively small player can build a frontier-competitive coding agent by post-training on top of a strong open-weight base model rather than training from scratch, which lowers the barrier to entry for coding-agent startups. At the same time, the sharp pushback on Hacker News highlights how much the industry's trust now hinges on benchmark rigor and weight openness rather than launch-day claims. Commenters point to a striking gap between SWE-2's Terminal Bench 2.1 score of 92.8% and its 27.3% on the newer Terminal Bench 4, released only a couple of weeks earlier, as a possible sign of benchmark overfitting rather than genuine generalization. The model also appears to be closed-weight, which critics contrast unfavorably with open alternatives like DeepSeek Flash 4.1.

hackernews · seelos · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645443)

**Background**: Cognition is best known for Devin, an AI agent marketed as able to autonomously complete software engineering tasks. Kimi K3 is an open-weight multimodal reasoning model from Moonshot AI with roughly 2.8 trillion parameters, noted for handling large repositories, tool use and long-horizon agentic workflows. Terminal Bench is a benchmark that measures how well a model can operate a command-line environment to complete real tasks, and its newer versions use fresh problems that are harder to game. Post-training refers to further training a base model on curated data and reinforcement learning to specialize it for a task such as coding.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3">moonshotai/ Kimi - K 3 · Hugging Face</a></li>
<li><a href="https://platform.claude.com/docs/en/models/fable-5-1/overview">Claude Fable 5.1 - Claude Platform Docs</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT -6 Astra : A new generation of intelligence | OpenAI</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were broadly skeptical: the top objection is the 92.8% versus 27.3% split between Terminal Bench 2.1 and Terminal Bench 4, read as evidence of heavy benchmark optimization. Others questioned why anyone would choose another closed-weight model over DeepSeek Flash 4.1, and several reminded readers of Cognition's past demo credibility problems and their negative experience with Devin, while a few conceded that a reinforcement-learned Kimi K3 reaching Fable 5-level capability is a genuinely encouraging signal.

**Tags**: `#AI/ML`, `#LLM`, `#coding-agents`, `#benchmarks`, `#model-release`

---

<a id="item-8"></a>
## [NASA's Decorrelation Stretch Reveals Hidden Ancient Rock Art](https://spinoff.nasa.gov/Manipulating_Satellite_Photos_Now_Reveals_Ancient_Images) ⭐️ 7.0/10

NASA's decorrelation stretch, an image-processing technique originally developed to enhance satellite and planetary imagery, is now being used to reveal faded ancient rock art and other details invisible in ordinary photographs. The NASA Spinoff report documents how this same algorithm has been repurposed for archaeology and cultural-heritage imaging. This is a textbook example of space-technology transfer, showing how a remote-sensing tool built for satellites can create new value in archaeology, conservation and forensics decades later. It also underscores a broader lesson: how optical sensors and human eyes render the world is not canonical, so computational processing can expose information that was always present but never perceived. A decorrelation stretch works by removing the correlation between the color bands of an image and then stretching their contrast, so subtle color differences between bands become visible rather than being masked by the dominant shared signal. It is implemented in tools such as MATLAB's decorrstretch function and ENVI, and can be approximated in general-purpose editors like GIMP by decomposing an image into LAB channels, auto-leveling the chroma channels, and recomposing.

hackernews · gumby · Sep 10, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49645437)

**Background**: Multispectral imaging captures light in several wavelength bands, including near-infrared, which human eyes cannot see; false-color composites assign these invisible bands to visible colors, which is why vegetation often appears red in such imagery because plants reflect strongly in the near-infrared. In multispectral data the bands are usually highly correlated with one another, so the interesting differences occupy only a small part of the available color range. Decorrelation stretch is a statistically motivated way of expanding those differences so the eye can actually distinguish them, and it has long been a standard step in remote sensing and planetary image processing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Decorrelation">Decorrelation - Wikipedia</a></li>
<li><a href="https://nl.mathworks.com/help/images/ref/decorrstretch.html">decorrstretch</a></li>
<li><a href="https://davinci.mars.asu.edu/index.php?title=decorrelation_stretch">decorrelation stretch - DavinciWiki</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were enthusiastic and practical: one shared a GIMP recipe using LAB decompose/compose with auto input levels, while others recalled the "eureka" moment in remote-sensing classes of realizing that vegetation is red, not green, in false-color composites. A commenter described unsuccessfully trying multi-bandpass filters to find hidden rock art at Angkor Wat, and another asked whether an ImageMagick implementation exists for pipeline use.

**Tags**: `#remote-sensing`, `#image-processing`, `#archaeology`, `#NASA-spinoff`, `#signal-processing`

---

<a id="item-9"></a>
## [PlanetScale Launches Neki, a Closed-Source Sharded Postgres](https://planetscale.com/blog/introducing-neki) ⭐️ 7.0/10

PlanetScale announced Neki, a sharded Postgres product that places a router, sidecars, and a control plane on top of ordinary Postgres shards so a database can scale beyond a single machine. The launch post stopped short of describing what Neki actually is or who it is for, and PlanetScale confirmed it will only be released as open source once it is tested in real production workloads. PlanetScale, best known for its MySQL-based serverless database platform, is extending into the Postgres ecosystem, which is the fastest-growing major relational database and already crowded with sharding and distributed options such as Citus. Because the product is closed source at launch, the announcement also intensifies the debate over open-source versus proprietary approaches to distributed Postgres, especially given the company's public criticism of competitors' open-source efforts. Every Neki shard is real Postgres, with PlanetScale adding routing, sidecar, and control-plane layers for horizontal scaling, and the company says it will open source the project only after production testing. Notably, the announcement does not address how Neki handles eventual-consistency and CAP tradeoffs for highly available distributed Postgres, a gap commenters flagged as a central unresolved question.

hackernews · simon_weber · Sep 10, 15:43 · [Discussion](https://news.ycombinator.com/item?id=49645686)

**Background**: Sharding splits a database's data across multiple machines so each node handles a smaller slice of the workload, which is how systems scale past the limits of one server; Postgres has no built-in sharding, so tools must add routing and coordination on top. The CAP theorem states that during a network partition a distributed system must choose between consistency and availability, and eventual consistency — where replicas may briefly disagree — is often unacceptable for transactional workloads, making it a pivotal design question for any distributed Postgres offering.

<details><summary>References</summary>
<ul>
<li><a href="https://planetscale.com/neki">Neki — PlanetScale</a></li>
<li><a href="https://neki.dev/?ref=upstract.com">Neki | Sharded Postgres by PlanetScale</a></li>
<li><a href="https://en.wikipedia.org/wiki/CAP_theorem">CAP theorem - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely critical rather than celebratory: the top comment complained that the launch post explains the problem, alternatives, and components but never actually describes what Neki is or what it's for. Others criticized the CEO's public attacks on Supabase's open-source multigres while Neki itself remains closed source, and one commenter raised a sharp technical concern about whether Neki solves the eventual-consistency and CAP tradeoffs that make highly available distributed Postgres unsuitable for many workloads.

**Tags**: `#postgres`, `#database-sharding`, `#planetscale`, `#distributed-systems`, `#open-source`

---

<a id="item-10"></a>
## [Microsoft Elevates Rust to Tier-1 Language Status](https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/) ⭐️ 7.0/10

A guest post published by the Rust Foundation announced that Rust now holds "tier-1 language" engineering status at Microsoft, sitting alongside C++, C#, and TypeScript as one of the best-supported languages for internal development. According to the post, this status gives internal teams a paved path from local development to production, including secure toolchain builds. Microsoft is one of the largest producers of both operating-system code and C/C++ tooling, so formally backing Rust signals that a memory-safe systems language is now a first-class option for greenfield development at a major OS vendor. The move also strengthens Rust's position against newer "better C/C++" contenders such as Zig and Odin, which have far smaller corporate backing and less mature tooling. Tier-1 status is an internal engineering designation covering supported toolchains, secure builds, and production readiness rather than a formal product or licensing change, and much of Microsoft's Rust investment has been known publicly for years. Community discussion also pointed to related efforts, including a Microsoft hiring manager's stated vision of converting 1 billion lines of C/C++ to Rust by 2030 with "1 engineer, 1 month, 1 million lines of code" tooling, and DARPA-funded work splitting C-to-Rust transpilation across six different teams.

hackernews · mmastrac · Sep 10, 13:39 · [Discussion](https://news.ycombinator.com/item?id=49643546)

**Background**: Rust is a general-purpose programming language created by Graydon Hoare at Mozilla in 2006 and first stabilized with version 1.0 in May 2015; it emphasizes performance, type safety, concurrency, and memory safety. Instead of a garbage collector, Rust uses a compile-time "borrow checker" that tracks reference lifetimes to prevent memory errors and data races. The language has been stewarded by the Rust Foundation since February 2021, with Microsoft joining as a founding Platinum Member after years of early investment. Microsoft's interest is closely tied to security: a large share of the CVEs affecting its products, roughly 70% by its own accounts, stem from memory-safety bugs typical of C and C++ code.

<details><summary>References</summary>
<ul>
<li><a href="https://rustfoundation.org/media/guest-post-rust-is-tier-1-language-at-microsoft/">Guest Post: Rust Is Tier - 1 Language at Microsoft</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_Foundation">Rust Foundation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust (programming language) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread (590 points, 329 comments) was broadly welcoming: a developer with five years of professional Rust experience argued there is no longer a technical reason to pick another language for high-level application work, while another commenter said the announcement shows Rust is no longer a fledgling "move fast and break things" language but a mature competitor to C++ and C#. Others noted that all major OS vendors with a stake in C/C++ tooling have now diversified their systems-language options, and welcomed long-rumored MSVC integration for Rust.

**Tags**: `#rust`, `#microsoft`, `#programming-languages`, `#systems-programming`, `#memory-safety`

---

<a id="item-11"></a>
## [China Halts New Battery Factory Construction Pending Capacity Review](https://www.bloomberg.com/news/articles/2026-09-11/china-halts-new-battery-factories-on-capacity-concerns-caixin) ⭐️ 7.0/10

China has temporarily suspended construction of new projects for manufacturing power batteries and energy-storage batteries, pending a year-end review of industry capacity, according to a Caixin report cited by Bloomberg. The halt applies to new manufacturing projects rather than existing production lines. China supplies the large majority of the world's lithium-ion batteries, so a pause on new capacity can ripple through global EV and grid-storage supply chains and shape battery prices worldwide. It also signals a policy shift from maximizing volume growth toward curbing overcapacity and consolidating a sector battered by price wars. The suspension is described as temporary and tied to a year-end capacity review, and it explicitly covers both power batteries (used in EVs) and energy-storage batteries (used in grid and stationary storage). The report does not make clear how projects already under construction or already approved will be treated.

rss · Bloomberg Markets · Sep 11, 00:22

**Background**: Power batteries are optimized for high power output and fast discharge, making them suited to electric vehicles, while energy-storage batteries are optimized for long duration and durability in fixed grid or backup installations. China's battery industry expanded rapidly over the past decade, and the resulting oversupply has driven intense price competition and squeezed manufacturer margins. Beijing has increasingly talked about reining in 'involutionary' competition in strategic industries, and this suspension is consistent with that direction.

<details><summary>References</summary>
<ul>
<li><a href="https://jmbatteries.com/blogs/blog/power-battery-vs-energy-storage-battery">Power Battery vs Energy Storage Battery – JMBatteries</a></li>
<li><a href="https://energy.ecoflow.com/us/blog/energy-storage-vs-power-battery-guide">Power vs Energy Storage Battery : What's the Real... | EcoFlow US</a></li>

</ul>
</details>

**Tags**: `#China`, `#batteries`, `#manufacturing`, `#energy storage`, `#industrial policy`

---

<a id="item-12"></a>
## [Pocket FM doubles revenue run rate to $500M with AI-made audio content](https://techcrunch.com/2026/09/10/indias-pocket-fm-doubles-revenue-run-rate-to-500m-as-ai-powers-93-of-audio-content/) ⭐️ 7.0/10

India-based audio streaming platform Pocket FM said it has doubled its revenue run rate to $500 million, while AI now produces the overwhelming majority of its audio content — 93% of content according to the headline figure and 99% of newly produced content according to the summary. The company says this AI-driven pipeline has made content production roughly 80 times cheaper. It is one of the clearest examples so far of generative AI being applied at industrial scale in consumer media, showing that AI-driven production can support both rapid revenue growth and a dramatic cost reduction. If the model holds, it could pressure other audio, publishing, and entertainment companies to rethink how much human-produced content they can afford to keep making. The reported figures mix two different metrics: the $500 million is an annualized revenue run rate rather than audited annual revenue, and the AI share is cited both as 93% of content and 99% of new content, suggesting legacy human-made shows still make up part of the catalog. The roughly 80x cost reduction is a company-stated comparison and no details were given about which AI models, voice technologies, or languages are involved.

rss · TechCrunch · Sep 10, 17:45

**Background**: Pocket FM is an Indian startup that distributes short, episodic "audio series" — serialized fiction delivered as spoken audio, closer to streaming TV soap operas than to podcasts or audiobooks — and monetizes them through paid episodes and microtransactions. Like other media companies, it has been experimenting with generative AI for text-to-speech narration and voice cloning, which can replace expensive human recording, studio time, and translation work. A "revenue run rate" is a projection that annualizes a recent period's revenue, and it is typically higher than the actual revenue eventually booked.

**Tags**: `#Generative AI`, `#Audio Content`, `#Media Industry`, `#AI Application`, `#Pocket FM`

---

<a id="item-13"></a>
## [Google Earth's 24-hour AI feature exposed deepfake trust risks](https://restofworld.org/2026/google-earth-ai-deepfake-iran-war/?utm_source=rss&utm_medium=rss&utm_campaign=feeds) ⭐️ 7.0/10

Google briefly shipped a generative AI feature in Google Earth that let users create fake satellite imagery, then pulled it within roughly 24 hours. According to Rest of World, the episode shows how unvetted AI tools released during a conflict can cause lasting damage to trust. Satellite imagery is a cornerstone of open-source verification, used by journalists, humanitarian groups and analysts to confirm what is really happening on the ground, so a tool that fabricates it threatens that shared evidentiary foundation. Releasing such a feature during an active conflict — and then quietly removing it — risks normalizing AI-generated fakes and making real images harder to trust. The feature survived only about a day before being disabled, yet the concern is less about the tool itself than about how quickly a generative capability can reach users without evident safety review. The episode unfolded amid a wider surge of AI-generated fake satellite imagery, including a fabricated image of a destroyed US base in Qatar circulated by an Iranian news outlet.

rss · Rest of World · Sep 10, 10:00

**Background**: Generative AI models — including text-to-image systems — have become capable of producing synthetic satellite-style imagery that mimics real orbital photography, a technique researchers study for both its promise and its risks to monitoring and verification. Satellite imagery has long served as one of the most trusted sources of evidence in conflicts, where the 'fog of war' already makes facts contested. When realistic fakes become easy to make and share, the burden of verification grows for everyone relying on these images.

<details><summary>References</summary>
<ul>
<li><a href="https://thearabweekly.com/fake-ai-satellite-imagery-flourishes-fog-us-iran-war">Fake AI satellite imagery flourishes in the fog of US-Iran war | | AW</a></li>
<li><a href="https://arxiv.org/abs/2404.07754">[2404.07754] Generating Synthetic Satellite Imagery With...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#misinformation`, `#deepfakes`, `#Google Earth`, `#generative AI`

---

<a id="item-14"></a>
## [Anthropic accuses DeepSeek and Moonshot of covertly routing requests to Claude](https://www.scmp.com/news/us/diplomacy/article/3367112/moonshot-deepseek-secretly-routed-user-requests-claude-anthropic-claims?utm_source=rss_feed) ⭐️ 7.0/10

On Thursday, Anthropic accused its Chinese AI rivals DeepSeek and Moonshot of covertly routing customer requests to its Claude models and then presenting the answers to users as if they came from their own models. The allegation escalates Washington's criticism of China's AI industry, coming the same week that three US government agencies, including the NSA and FBI, made related claims about Chinese AI practices. If substantiated, the claim could damage the credibility of two of China's most prominent AI labs, raise terms-of-service and legal exposure around API proxying, and deepen the already tense US–China AI rivalry. It also matters to enterprises that care about model provenance, since customers may have unknowingly been served by a US model while believing they were using a Chinese one. The accusation is an allegation rather than a proven finding, and the provided report does not include a public response from DeepSeek or Moonshot. It follows a separate February claim by Anthropic that Moonshot, DeepSeek and MiniMax were distilling from Claude models — a related but distinct practice from covertly proxying live user traffic through a competitor's API.

rss · SCMP · Sep 10, 23:23

**Background**: DeepSeek is a Hangzhou-based developer of open-weights large language models, owned and funded by the hedge fund High-Flyer, while Moonshot AI is a Beijing-based company and one of China's six "AI Tigers", known for its Kimi series of open-weights models. Claude is the family of large language models built by the American company Anthropic and offered to third parties through a paid API. Sending user requests to a competitor's API and passing off the outputs as your own typically violates those providers' terms of service, and the practice of training on another model's outputs is known as distillation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(AI)">Claude ( AI ) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#Anthropic`, `#DeepSeek`, `#Moonshot`, `#API misuse`

---

<a id="item-15"></a>
## [Chinese scientists quadruple hydrogen fuel cell power in new design](https://www.scmp.com/news/china/science/article/3367077/chinese-scientists-boost-hydrogen-fuel-cell-power-fourfold-new-design?utm_source=rss_feed) ⭐️ 7.0/10

Researchers at the Beijing Institute published a peer-reviewed study in the journal Science on Thursday describing a new hydrogen fuel cell design that achieves a fourfold increase in power output. The team says the advance could broaden fuel cell applications from road vehicles to space missions. Hydrogen fuel cells produce electricity with water as their only exhaust, so a fourfold jump in power density could make them viable in weight- and volume-constrained settings such as vehicles and spacecraft where they previously fell short. The result, published in a top-tier peer-reviewed journal, signals that clean hydrogen energy is advancing on the materials science front, not just in policy and deployment. The work appears in Science, indicating it passed independent peer review, and the reported gain is a fourfold increase in power output rather than a marginal efficiency tweak. The excerpt does not disclose the specific materials, catalyst chemistry or operating conditions behind the improvement, so questions about durability, cost and manufacturability at scale remain open.

rss · SCMP · Sep 10, 18:00

**Background**: A hydrogen fuel cell converts the chemical energy stored in hydrogen into electricity through an electrochemical reaction, with water vapour as the only by-product — unlike combustion engines, which emit carbon dioxide and pollutants. Their adoption has been limited by high cost, limited hydrogen infrastructure and relatively low power density compared with batteries and fossil fuels. Improvements in power output therefore matter because they allow a smaller, lighter stack to deliver the same performance, which is especially valuable on spacecraft where every kilogram counts.

**Tags**: `#hydrogen fuel cells`, `#clean energy`, `#materials science`, `#research breakthrough`, `#energy storage`

---

<a id="item-16"></a>
## [Huawei unveils industry-first 7.2 Tbps near-packaged optics module](https://www.scmp.com/tech/tech-trends/article/3367093/ai-bottleneck-breaker-chinas-huawei-touts-high-speed-optical-module?utm_source=rss_feed) ⭐️ 7.0/10

Huawei Technologies showcased what it calls the industry's first 7.2-terabit-per-second (Tbps) near-packaged optics (NPO) product at the China International Optoelectronic Exposition (CIOE) in Shenzhen this week. The company positions the module as a way to eliminate bottlenecks in AI infrastructure and to stake an early claim in setting standards for next-generation data centre connections. As AI clusters scale, performance is increasingly limited not by compute or memory but by data movement between chips, so interconnect optics has become a critical bottleneck. By shipping an NPO module ahead of rivals, Huawei is positioning itself in the standards race for next-generation data centre interconnect, which directly affects systems and networking engineers designing large AI fabrics. NPO sits between traditional pluggable optics and co-packaged optics (CPO): the optical engine is moved off the switch's main ASIC but kept within a few centimetres of it on the same board. The announcement is a news brief, so key engineering specifics such as power per bit, reach, laser source and commercial availability were not disclosed.

rss · SCMP · Sep 10, 13:30

**Background**: Large AI training clusters link thousands of accelerators, and the fibre-optic links between them have become a limiting factor as models grow. Traditional pluggable optics plug into the front panel of a switch, while co-packaged optics integrates the optical engine directly with the switch ASIC; near-packaged optics is a middle path that shortens the electrical path to cut power and signal loss. The optical supply chain is also under strain, with industry reports pointing to shortages of indium phosphide (InP) and laser components as AI data centres drive up optical interconnect density.

<details><summary>References</summary>
<ul>
<li><a href="https://resources.l-p.com/glossary/what-is-near-packaged-optics-benefits-network-upgrades">Beyond Pluggables: What is NPO ( Near - Packaged Optics ) and Why...</a></li>
<li><a href="https://dev.to/aicplight/lpo-vs-npo-vs-cpo-the-evolution-of-optical-interconnects-in-ai-data-centers-33ha">LPO vs NPO vs CPO: The Evolution of Optical ... - DEV Community</a></li>
<li><a href="https://www.trendforce.com/news/2026/08/06/news-inp-shortage-emerges-as-ai-optical-interconnect-bottleneck/">[News] InP Shortage Emerges as AI Optical Interconnect Bottleneck</a></li>

</ul>
</details>

**Tags**: `#optical-interconnects`, `#AI-infrastructure`, `#Huawei`, `#data-center-networking`, `#hardware`

---

<a id="item-17"></a>
## [Meta Reportedly Takes Over Muse's Social Media Handles for Its AI Product](https://www.reddit.com/r/technology/comments/1wckyn3/meta_confiscates_social_media_handles_of/) ⭐️ 7.0/10

A post on r/technology alleges that Meta confiscated the social media handles belonging to the British rock band Muse and reassigned them to its own AI product, effectively stripping the band of usernames tied to its identity. The submission itself contains no screenshots, links, or additional documentation, so the specific platform, handle, and timeline remain unconfirmed. The incident highlights how much control platforms wield over digital identity: a username a band has used for decades can apparently be reassigned at the platform owner's discretion, with no recourse for the original holder. It also feeds a broader debate about trademark rights, handle squatting, and how aggressively Meta is branding and promoting its AI products across its own apps. Because the Reddit post is a bare submission with no supporting evidence, the claim should be treated as unverified, and there is no confirmed information on which handle was affected or whether the band still retains access to its other accounts. Even if true, such a move would not necessarily be unprecedented: platforms typically reserve the right to reclaim or reassign usernames under their terms of service and inactive-account or trademark policies.

reddit · r/technology · /u/indorock · Sep 10, 14:34

**Background**: Usernames and handles on platforms like Instagram are not owned by users in the way a trademark or domain name might be; they are effectively licences granted under the platform's terms of service, which the platform can revoke or reassign. Trademark holders can file complaints through a platform's trademark policy, but that process is normally used by a brand to take a handle from someone else, not to have its own handle taken away. Against this backdrop, Meta has spent recent years heavily branding its AI assistant and AI-generated profiles across Facebook, Instagram and WhatsApp, which makes any reclaiming of existing handles for AI use particularly sensitive.

**Tags**: `#Meta`, `#AI`, `#social-media`, `#platform-policy`, `#digital-identity`

---

<a id="item-18"></a>
## [IDScan confirms breach exposing 150M+ driver's licenses](https://www.reddit.com/r/technology/comments/1wckfeb/id_verification_giant_idscan_confirms_data_breach/) ⭐️ 7.0/10

Identity verification provider IDScan has confirmed a data breach in which more than 150 million driver's licenses were exposed, with hackers allegedly offering the stolen records for sale. Multiple lawsuits have since been filed against the company, and reports put the volume of affected records at around 153 million. Driver's licenses are among the most sensitive and reusable identity documents, so their exposure can fuel identity theft, account takeover, synthetic identity fraud, and loan or benefits fraud on a massive scale. Because IDScan sits in the verification chain for many businesses, the incident also creates downstream compliance and liability exposure for every enterprise that relied on it for know-your-customer checks. Unlike a typical breach of email addresses and passwords, this one reportedly involves government-issued ID documents and the personal data printed on them, which cannot simply be reset like a password. Reported figures differ slightly across coverage, with some accounts citing more than 153 million driver's licenses, and the company is already facing litigation over the incident.

reddit · r/technology · /u/lurker_bee · Sep 10, 14:14

**Background**: Identity verification providers like IDScan supply the technology businesses use to scan and validate government IDs, check ages for restricted sales, and perform KYC checks required by financial and other regulated industries. That means these vendors accumulate large centralized stores of ID images and associated personal data — full names, dates of birth, addresses, license numbers, and photographs. Because driver's license data is permanent and hard to change, a breach at such a vendor is generally considered far more damaging than a leak of passwords, and it can turn a single compromised provider into a systemic risk for its many client organizations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bleepingcomputer.com/tag/idscan/">Latest IDScan news</a></li>
<li><a href="https://botcrawl.com/idscan-data-breach/">IDScan Data Breach May Expose 153 Million Driver's Licenses</a></li>

</ul>
</details>

**Tags**: `#security`, `#data-breach`, `#privacy`, `#identity-verification`, `#cybersecurity`

---

<a id="item-19"></a>
## [Anthropic Alleges Distillation Attacks by Alibaba, Moonshot AI, DeepSeek](https://techcrunch.com/2026/09/10/anthropic-details-distillation-campaigns-from-alibaba-moonshot-ai-and-deepseek/) ⭐️ 6.0/10

Anthropic released a report on Thursday alleging persistent distillation attacks on its models by China-based AI companies Alibaba, Moonshot AI, and DeepSeek, saying the activity has escalated in recent months as competition in the field has intensified. The report frames these campaigns as systematic efforts to extract model behavior at scale rather than isolated incidents. The allegation raises the stakes in the US-China AI rivalry by turning model distillation from a technical footnote into a security, intellectual-property, and policy issue that major labs, regulators, and enterprise customers will all have to weigh. If distillation is treated as a terms-of-service violation or even a security threat, it could reshape how API access is gated, monitored, and enforced across the industry. Anthropic has previously described the hallmarks of a distillation attack as massive query volume concentrated in a few areas, highly repetitive request structures, and content that maps directly onto what is most valuable for training a model — reporting that has cited figures on the order of millions of Claude queries. The current report is summarized only at a high level, with no technical methodology, named accounts, or precise query numbers disclosed in the available material.

rss · TechCrunch · Sep 10, 20:57

**Background**: Knowledge distillation is a standard machine-learning technique in which a smaller "student" model is trained to imitate the outputs of a larger "teacher" model, which is a legitimate and widely used way to build cheaper, faster models. A distillation attack is the same idea applied without permission: someone queries a commercial model's API at scale, collects the responses, and uses them as training data to replicate the original model's capabilities. Because the extracted data is essentially the model's behavior rather than its source code or weights, it sits awkwardly between conventional IP infringement, terms-of-service abuse, and a novel form of security risk.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.mindstudio.ai/blog/ai-model-distillation-attacks-explained">AI Model Distillation Attacks : What They Are and Why... | MindStudio</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#model distillation`, `#Anthropic`, `#China AI`, `#AI security`

---

<a id="item-20"></a>
## [Proxima Fusion to build €140M factory for fusion-grade HTS tape](https://techcrunch.com/2026/09/10/proxima-fusion-bets-e140m-on-a-critical-fusion-ingredient-dominated-by-asian-suppliers/) ⭐️ 6.0/10

Proxima Fusion announced on Wednesday that it plans to build a €140 million ($162.6 million) factory to produce fusion-grade high-temperature superconducting (HTS) tape, a key component of its stellarator-based reactor design. The move is intended to give the Munich-based startup an in-house supply of a material currently dominated by Asian manufacturers. HTS tape is a supply-chain bottleneck for essentially every compact, high-field fusion concept, so an in-house production line could reduce Proxima's exposure to a handful of Asian suppliers and to price and allocation decisions it does not control. If it works, the factory could also strengthen Europe's position in a strategically important energy technology and serve as a template for other fusion developers facing the same constraint. The announcement is a short news brief: the specific factory location, production capacity, timeline, and tape supplier or manufacturing partner are not disclosed, and no technical specifications for the tape were given. The comparison point is that HTS tape is already produced at scale for applications such as MRI magnets and power grid equipment, but fusion magnets demand higher performance and consistency than many commercial grades.

rss · TechCrunch · Sep 10, 18:38

**Background**: Proxima Fusion is a Munich-based fusion energy company founded in 2023 as the first research spin-off from the Max Planck Institute for Plasma Physics, and it aims to design fusion power plants based on a quasi-isodynamic (QI) stellarator. A stellarator confines plasma with complex, twisted magnetic coils rather than the simpler tokamak geometry, which makes the performance of those magnets decisive for the whole design. High-temperature superconducting tape is a ribbon-like conductor that carries large currents without resistance at relatively high temperatures, allowing much stronger magnetic fields in smaller devices than conventional low-temperature superconductors. Production of fusion-grade HTS tape is currently concentrated among a small number of suppliers in Asia, which is why fusion startups have begun looking at building their own capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proxima_Fusion">Proxima Fusion</a></li>
<li><a href="https://techcrunch.com/2026/09/10/proxima-fusion-bets-e140m-on-a-critical-fusion-ingredient-dominated-by-asian-suppliers/">Proxima Fusion bets €140M on a critical fusion ... | TechCrunch</a></li>
<li><a href="https://nationalmaglab.org/magnet-development/applied-superconductivity-center/research/science-highlights/high-temperature-superconducting-tape">High - Temperature Superconducting Tape Suitable for Magnets at 50...</a></li>

</ul>
</details>

**Tags**: `#fusion energy`, `#superconductors`, `#HTS tape`, `#supply chain`, `#clean energy`

---

<a id="item-21"></a>
## [Bending Spoons to buy collaboration tools maker Miro for $1.36B, 90% less than its 2022 valuation](https://techcrunch.com/2026/09/10/bending-spoons-to-buy-collaboration-tools-maker-miro-for-1-36b-90-less-than-its-2022-valuation/) ⭐️ 6.0/10

Bending Spoons is acquiring workplace collaboration tool Miro for $1.36 billion, a 90% drop from its 2022 valuation of $17.5 billion.

rss · TechCrunch · Sep 10, 14:34

**Tags**: `#acquisitions`, `#Miro`, `#Bending Spoons`, `#startup valuations`, `#collaboration tools`

---

<a id="item-22"></a>
## [DeepSeek launches V4.1 Flash, claiming it beats Kimi K3 on coding](https://www.scmp.com/tech/big-tech/article/3367051/deepseek-says-new-flash-ai-model-beats-kimi-k3-cyber-coding-benchmarks?utm_source=rss_feed) ⭐️ 6.0/10

DeepSeek announced its V4.1 Flash model, saying it outperforms the company's own previous flagship and Moonshot AI's Kimi K3 on cyber and coding benchmarks while cutting inference costs and improving speed. The model uses a new "Causal-Encoder-Decoder" architecture and, despite being built on a 552-billion-parameter framework, relies on a Mixture-of-Experts (MoE) design. The release intensifies the aggressive price-and-performance race among Chinese AI labs, where each new flagship tries to undercut rivals on cost while matching or beating them on benchmarks. If the claims hold up, it pressures both closed US frontier models and open-weight competitors like Kimi K3 on the cost-efficiency frontier that enterprise adopters care about most. The headline 552-billion-parameter figure is the total size of the model, but the MoE design means only a fraction of those parameters are activated per query, which is what enables the claimed cost and latency reductions. The benchmark claims — particularly the cyber and coding scores against Kimi K3 — are self-reported by DeepSeek and have not been independently verified.

rss · SCMP · Sep 10, 09:26

**Background**: Mixture-of-Experts (MoE) is an architectural technique in which a model contains many specialized sub-networks ("experts") plus a gating mechanism that routes each token to only a few of them, so a huge model can run far cheaper than a dense model of the same size — used by systems such as Mixtral and Gemini. "Causal" refers to the standard decoder-only language-model setup, where each token can only attend to previous tokens, and combining it with an encoder-decoder structure is an unusual hybrid. Kimi K3, from Chinese startup Moonshot AI, is a 2.8-trillion-parameter open-weights model that leads the Chinese market and rivals US frontier models, making it a natural yardstick for DeepSeek's claim.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_K3">Kimi K3</a></li>
<li><a href="https://medium.com/ramses-engineering/not-one-brain-but-many-how-mixture-of-experts-moe-makes-ai-smarter-and-faster-568f41220852">Not One Brain, But Many: How Mixture of Experts ( MoE )... | Medium</a></li>
<li><a href="https://www.unite.ai/decoder-based-large-language-models-a-complete-guide/">Decoder -Based Large Language Models: A Complete Guide – Unite.AI</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#LLM`, `#Mixture-of-Experts`, `#AI benchmarks`, `#model release`

---

<a id="item-23"></a>
## [Florida Woman Sues Over Wrongful Arrest Tied to Flock Camera Data](https://www.reddit.com/r/technology/comments/1wcraby/florida_woman_sues_over_wrongful_arrest_tied_to/) ⭐️ 6.0/10

A woman in Florida is suing after she was wrongfully arrested based on data generated by Flock Safety's automated license plate reader (ALPR) cameras. The lawsuit directly challenges how law-enforcement agencies rely on Flock's AI-powered camera network during criminal investigations. The case puts the accuracy and legal accountability of AI-driven surveillance infrastructure on trial at a moment when thousands of police departments, homeowners associations and schools have adopted Flock cameras. If courts find that plate-reader data can lead to wrongful arrests, it could force agencies to add verification requirements, audit trails and stronger oversight of automated policing tools. Flock Safety's cameras use AI to capture a vehicle's license plate along with its make, model and colour, and the company sells these systems primarily to police departments, HOAs, school districts and private businesses. ALPR technology has long been criticised for misidentification, high error rates and functioning as a form of mass surveillance, since it stores the location, date and time of every passing vehicle rather than only vehicles of interest.

reddit · r/technology · /u/consultinglove · Sep 10, 18:21

**Background**: Flock Safety was founded in 2017 in Atlanta and sells automated license plate recognition cameras that use optical character recognition on images of vehicle plates to build location data. ALPR systems are used by police worldwide to check whether a vehicle is registered or licensed, and they are also deployed for electronic toll collection and traffic cataloguing. Privacy advocates have raised concerns that such systems enable government tracking of citizens' movements even when no crime is suspected.

<details><summary>References</summary>
<ul>
<li><a href="https://deflock.org/">DeFlock is an open-source project that maps license plate readers ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Automated_license_plate_recognition">Automated license plate recognition</a></li>
<li><a href="https://trafficvision.live/blog/flock-cameras">Flock Cameras: What They Are & Can You Watch... | TrafficVision.Live</a></li>

</ul>
</details>

**Tags**: `#surveillance`, `#privacy`, `#AI ethics`, `#law enforcement technology`, `#wrongful arrest`

---