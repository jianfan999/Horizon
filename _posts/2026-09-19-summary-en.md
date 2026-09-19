---
layout: default
title: "Horizon Summary: 2026-09-19 (EN)"
date: 2026-09-19
lang: en
---

> From 114 items, 18 important content pieces were selected

---

1. [Android 17 Adds New APIs Without Releasing Them to AOSP, GrapheneOS Says](#item-1) ⭐️ 8.0/10
2. [Photon-Emission-Guided Laser Fault Injection Enables RP2350 Secure Debug](#item-2) ⭐️ 8.0/10
3. [AI hallucination nearly triggers US military operation](#item-3) ⭐️ 8.0/10
4. [Cloudflare Saves Another 100TB of RAM Using Applied Math](#item-4) ⭐️ 7.0/10
5. [Anthropic reportedly runs its own biology lab for experiments](#item-5) ⭐️ 7.0/10
6. [Joby Aviation completes 3,100-mile fully autonomous cross-country flight](#item-6) ⭐️ 7.0/10
7. [FBI and Coast Guard Board Hacked Tankers Nearing US Coast](#item-7) ⭐️ 7.0/10
8. [China Claims Early Sub-3nm Progress Using Older DUV Lithography](#item-8) ⭐️ 7.0/10
9. [Alibaba's Damo Academy open-sources medical AI for 150 abdominal conditions](#item-9) ⭐️ 7.0/10
10. [Claude Code falls back to reading AGENTS.md when no CLAUDE.md exists](#item-10) ⭐️ 6.0/10
11. [OpenJev: Browser-Run 'Jev' Structured-Output Clone Sparks HN Debate](#item-11) ⭐️ 6.0/10
12. [Stanford study finds forebrain and hindbrain arise from two distinct neural progenitors](#item-12) ⭐️ 6.0/10
13. [Disney names Character.AI's former CEO as its first CTO](#item-13) ⭐️ 6.0/10
14. [Manus Seeks $4B Valuation in $500M Raise After Meta Deal Collapses](#item-14) ⭐️ 6.0/10
15. [Meta's Muse AI agent lands on Mac, taking actions for users](#item-15) ⭐️ 6.0/10
16. [UK air traffic chaos traced to millisecond software defect, NATS says](#item-16) ⭐️ 6.0/10
17. [Ant International embeds AI agents across all global platforms in biggest-ever upgrade](#item-17) ⭐️ 6.0/10
18. [AI-exposed majors' graduates since 2022 pushed into retail and food service, Reddit post claims](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Android 17 Adds New APIs Without Releasing Them to AOSP, GrapheneOS Says](https://grapheneos.social/@GrapheneOS/117282080803799576) ⭐️ 8.0/10

The GrapheneOS project reported that Android 17 has become the first Android release since the Android 3.x era to add new APIs without releasing the corresponding source code to the Android Open Source Project (AOSP). The new APIs instead shipped first in a Pixel-only update, so the matching AOSP source and documentation are not available to anyone outside Google's own devices. AOSP is the shared upstream that OEMs, custom ROMs and privacy-focused projects like GrapheneOS build on, so withholding API source breaks the assumption that Android is developed in the open. If this becomes a pattern, downstream systems could be forced to either reverse-engineer features or fall permanently behind Google's Pixel releases. Commenters highlighted a nuance from the full thread: the real problem is reportedly not that a single new API is Pixel-exclusive, but that the first and third quarterly release patches each year are now Pixel-exclusive, leaving AOSP-based projects without those changes. Google still backports monthly security fixes to select "trusted" OEMs, an arrangement GrapheneOS has had access to for years, and previously upstreamed source every half-year.

hackernews · theanonymousone · Sep 18, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49758736)

**Background**: Android is developed by Google behind closed doors and then periodically "upstreamed", meaning the source is pushed publicly into AOSP, the open-source codebase that device makers and custom ROMs build from. Because AOSP is the common starting point, any delay or omission in these source drops directly affects how quickly alternative distributions can adopt new platform features. GrapheneOS is a non-profit, security- and privacy-hardened Android-based operating system, historically available only on Google Pixel devices, that depends heavily on these AOSP releases as well as on Google's security patches.

<details><summary>References</summary>
<ul>
<li><a href="https://source.android.com/">Android Open Source Project</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS : the private and secure mobile OS</a></li>

</ul>
</details>

**Discussion**: Sentiment in the 218-comment thread was overwhelmingly distrustful of Google: one commenter called the roadblocks absurd and said Google simply regrets Android being open source, while another described their perception of the company as irreparably damaged. One user jokingly asked about the "token budget" to remove the Google dependency entirely and whether Valve could offer an alternative app store, and another (Ajedi32) corrected the framing by pointing out that the real issue is the Pixel-exclusive quarterly patches rather than one exclusive API.

**Tags**: `#Android`, `#AOSP`, `#GrapheneOS`, `#Google`, `#Open Source`

---

<a id="item-2"></a>
## [Photon-Emission-Guided Laser Fault Injection Enables RP2350 Secure Debug](https://donjon.ledger.com/blog/rp2350-secure-debug-laser-fault-injection/) ⭐️ 8.0/10

A blog post detailing how photon emission analysis can guide laser fault injection to bypass the RP2350's secure debug, with community discussion on replicability and security implications.

hackernews · synack · Sep 18, 16:54 · [Discussion](https://news.ycombinator.com/item?id=49757050)

**Tags**: `#hardware security`, `#laser fault injection`, `#RP2350`, `#embedded security`, `#side-channel attack`

---

<a id="item-3"></a>
## [AI hallucination nearly triggers US military operation](https://techcrunch.com/2026/09/18/ai-hallucination-nearly-triggers-us-military-operation/) ⭐️ 8.0/10

An AI hallucination reportedly nearly triggered a US military operation, prompting warnings about the uncertainty inherent to LLMs in defense settings.

rss · TechCrunch · Sep 18, 23:12

**Tags**: `#AI safety`, `#hallucination`, `#LLM`, `#military`, `#national security`

---

<a id="item-4"></a>
## [Cloudflare Saves Another 100TB of RAM Using Applied Math](https://blog.cloudflare.com/saving-100-tb-of-ram-with-math/) ⭐️ 7.0/10

Cloudflare published a new entry in its recurring engineering series, titled "Saving another 100TB of RAM with math," describing how applied mathematical techniques cut its memory footprint by an additional 100TB. The post covers concrete storage and data-structure changes, including a Rust struct used to store hashes where shaving just 2 bytes per entry reportedly mattered. At cloud scale, memory is one of the largest cost drivers, so a 100TB reduction translates directly into lower infrastructure spend and higher service density; the post is also a case study in how mathematical reasoning still yields large wins where brute-force hardware scaling is increasingly expensive. It arrives amid rising RAM prices, which the discussion treats as a signal that optimization discipline is becoming economically relevant again. The savings come from rethinking how data is laid out and encoded rather than from a single trick, and one highlighted change involves shrinking the struct that stores a hash by about 2 bytes per entry. The article does not fully explain why that many hash entries exist or why 2 bytes per entry justifies the effort, leaving some readers wanting more detail on the scale assumptions behind the win.

hackernews · f311a · Sep 18, 18:51 · [Discussion](https://news.ycombinator.com/item?id=49758580)

**Background**: Cloudflare runs a large global edge network, where every byte of per-connection state multiplied across millions of concurrent requests becomes a major memory bill, so small per-object savings compound dramatically. Hash tables and related lookup structures are the backbone of routing, caching, and security services, and their memory layout can often be improved with mathematical techniques such as better hashing, probabilistic data structures, and compact encoding. Cloudflare has published previous installments of this "saving RAM" series, making it a well-known reference for engineers interested in performance work.

**Discussion**: Commenters largely praised the series, with one recalling the era when scarce RAM and CPU forced creative optimization and lamenting that abundance led to bloated software. Others debated the labor implications, arguing that deep engineering and applied math cannot be "vibe coded" and will remain valuable as problems grow larger, while one raised the risk that extreme optimization turns codebases into impenetrable silos and another questioned whether shaving 2 bytes off a hash struct is really justified.

**Tags**: `#performance-optimization`, `#memory-management`, `#cloudflare`, `#software-engineering`, `#system-design`

---

<a id="item-5"></a>
## [Anthropic reportedly runs its own biology lab for experiments](https://techcrunch.com/2026/09/18/anthropic-is-operating-a-lab-that-conducts-biology-experiments/) ⭐️ 7.0/10

TechCrunch reported on September 18, 2026 that Anthropic is operating a laboratory that conducts biology experiments, a disclosure that sits uneasily alongside the company's long-standing warnings about AI-enabled catastrophic risk. The report is thin on specifics — it does not detail what experiments are run, at what biosafety level, or under what oversight — but it marks a concrete step by a frontier AI lab into wet-lab biology rather than purely computational work. Anthropic running wet-lab biology sits exactly at the intersection of AI safety, biosecurity, and AI-driven drug discovery, the same dual-use space where AI protein design tools have already raised alarms among DNA synthesis providers. If a leading safety-focused lab is doing bench science, it could either build credibility for AI-assisted biology or intensify scrutiny from biosecurity regulators who worry that capable models lower the barrier to dangerous research. The available excerpt offers no technical specifics on the lab's location, funding, biosafety level, or whether it performs its own experiments or partners with external researchers. For context, 'dual-use research of concern' (DURC) is a formal category in life-science governance covering work that could be repurposed for harm, and it typically requires institutional risk-benefit review and mitigation plans.

rss · TechCrunch · Sep 18, 23:13

**Background**: Dual-use research has a long history: the Haber process revolutionized agriculture with fertilizers but also enabled chemical weapons in World War I, and nuclear physics moved from medical radiography to atomic bombs. In AI, the same tension appears because models that help design therapeutic proteins could in principle also help design harmful ones, which is why DNA synthesis screening and biosecurity evaluation of AI models have become active policy topics. Separately, Anthropic's leadership, including CEO Dario Amodei, has repeatedly signed statements framing AI extinction risk as a global priority comparable to pandemics or nuclear war, making any move into biology especially closely watched.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dual_Use_Research_of_Concern">Dual Use Research of Concern</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_existential_risk">AI existential risk</a></li>
<li><a href="https://www.belfercenter.org/publication/biosecurity-age-ai-whats-risk">Biosecurity in the Age of AI : What’s the Risk ? | The Belfer Center for...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#biosecurity`, `#Anthropic`, `#AI in biology`, `#dual-use research`

---

<a id="item-6"></a>
## [Joby Aviation completes 3,100-mile fully autonomous cross-country flight](https://techcrunch.com/2026/09/18/joby-aviations-3100-mile-autonomous-flight-signals-its-push-beyond-electric-air-taxis/) ⭐️ 7.0/10

Joby Aviation announced on Friday that an aircraft equipped with its autonomy technology flew more than 3,100 miles across the United States without a human pilot taking control at any point. The company described it as a first-ever fully autonomous cross-country flight, a demonstration that goes well beyond its core electric air taxi business. The milestone signals Joby's push to extend its autonomy stack beyond crewed electric air taxis into wider commercial and defense applications, where autonomous cargo, logistics and surveillance missions are a fast-growing market. It also hands the company a strong technical proof point at a time when the eVTOL sector faces long certification timelines and doubts about near-term commercial viability. Publicly available details remain thin: the announcement did not specify the aircraft type, the route, the number of stopovers or the level of ground-based human oversight, although trade press reported the flight involved a Cessna Caravan-type aircraft fitted with Joby's autonomy stack. Joby says its aircraft, propulsion and autonomy technologies span both commercial aviation and defense applications, suggesting the company is positioning the technology for military and cargo customers as well as passenger service.

rss · TechCrunch · Sep 18, 17:26

**Background**: Joby Aviation is a California-based next-generation aviation company best known for developing electric vertical take-off and landing (eVTOL) aircraft for urban air taxi service. eVTOLs use electric propulsion to hover, take off and land vertically, and are a central part of advanced air mobility (AAM), an emerging sector that also covers highly automated cargo, regional and public-service flights and requires new infrastructure such as vertiports and drone traffic management systems. Autonomy is generally considered harder to certify than piloted electric flight, so a fully autonomous coast-to-coast demonstration is notable because it targets a capability that regulators have not yet broadly approved for civil operations.

<details><summary>References</summary>
<ul>
<li><a href="https://ir.jobyaviation.com/news-events/press-releases/detail/192/joby-completes-first-ever-fully-autonomous-flight-across">Joby Completes First-Ever Fully Autonomous Flight Across the...</a></li>
<li><a href="https://www.flyingmag.com/joby-autonomous-caravan-cross-country-no-pilot/">Joby Autonomous Caravan Flies Cross-Country Without Pilot Input</a></li>
<li><a href="https://en.wikipedia.org/wiki/Advanced_air_mobility">Advanced air mobility</a></li>

</ul>
</details>

**Tags**: `#autonomous flight`, `#Joby Aviation`, `#aviation autonomy`, `#eVTOL`, `#advanced air mobility`

---

<a id="item-7"></a>
## [FBI and Coast Guard Board Hacked Tankers Nearing US Coast](https://techcrunch.com/2026/09/18/fbi-coast-guard-boarded-hacked-oil-tankers-heading-towards-us-coast/) ⭐️ 7.0/10

The FBI and the US Coast Guard boarded oil tankers approaching the US coast as part of a federal investigation into compromises of the vessels' networks. In at least one case, the intrusion interfered with a tanker's navigation and propulsion systems. Cyber intrusions that reach a ship's navigation and propulsion systems cross a dangerous line, since a compromised tanker near a coastline can threaten crew safety, port operations, and the marine environment. The involvement of the FBI and Coast Guard signals that maritime cyberattacks are now being treated as a national-security and critical-infrastructure problem rather than a purely commercial IT issue. Details remain sparse because this is a brief news item: the number of tankers boarded, their flags or operators, the suspected attackers, and the method of compromise have not been disclosed. The reported interference with navigation and propulsion points to access to operational technology systems rather than only administrative or cargo-management networks.

rss · TechCrunch · Sep 18, 15:44

**Background**: Modern ships rely on interconnected digital systems for navigation, propulsion control, cargo handling, and communications, and these systems increasingly connect to satellite links and shore-side networks. The Coast Guard has authority to board and inspect vessels in US waters, and it works with agencies such as the FBI and CISA on maritime cybersecurity. Attacks on shipping have grown in recent years, with ports and shipping companies targeted by ransomware and state-linked actors, prompting regulators and insurers to tighten cyber requirements for vessels.

**Tags**: `#cybersecurity`, `#critical-infrastructure`, `#maritime-security`, `#cyberattack`, `#national-security`

---

<a id="item-8"></a>
## [China Claims Early Sub-3nm Progress Using Older DUV Lithography](https://www.scmp.com/tech/tech-war/article/3368042/china-makes-progress-3-nm-chips-without-advanced-lithography-tools?utm_source=rss_feed) ⭐️ 7.0/10

Chinese researchers have reportedly made early progress toward semiconductor process nodes below 3nm using older deep ultraviolet (DUV) lithography instead of advanced extreme ultraviolet (EUV) tools. The advance is framed as an alternative path to advanced chipmaking, since ASML's state-of-the-art EUV machines remain blocked from sale to China under US export controls. If validated at scale, this would undercut the effectiveness of US-led export controls aimed at keeping China behind at the most advanced nodes, and could reshape the global chipmaking landscape long dominated by ASML's EUV monopoly and foundries like TSMC and Samsung. It signals that sanctions pressure may push China toward genuinely different manufacturing approaches rather than simply slowing its roadmap. The report is a brief and offers no detail on the specific technique, achievable transistor density, yield, or independent verification, so the claims should be treated as preliminary. Working around EUV with DUV typically means multi-patterning, which raises cost, complexity, and defect rates, making commercial viability the key open question.

rss · SCMP · Sep 19, 00:00

**Background**: Photolithography uses light to print circuit patterns onto silicon wafers, and shorter wavelengths allow finer features. EUV lithography uses 13.5nm light and is the mainstream route for 5nm and 3nm-class nodes, but ASML is the only company that builds EUV systems, and export rules bar sales to China. DUV lithography uses longer-wavelength ultraviolet light and is the older, more widely available workhorse, which Chinese firms can still obtain but must stretch with multi-patterning to approach advanced nodes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EUV_lithography">EUV lithography</a></li>
<li><a href="https://en.wikipedia.org/wiki/3_nm_process">3 nm process - Wikipedia</a></li>
<li><a href="https://www.asml.com/en/products/duv-lithography-systems">DUV lithography systems | Products</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#lithography`, `#China-tech`, `#export-controls`, `#hardware`

---

<a id="item-9"></a>
## [Alibaba's Damo Academy open-sources medical AI for 150 abdominal conditions](https://www.scmp.com/tech/big-tech/article/3368055/alibaba-open-sources-medical-ai-model-can-detect-cancer-and-nearly-150-conditions?utm_source=rss_feed) ⭐️ 7.0/10

Alibaba's research arm, Damo Academy, has open-sourced a vision-language AI model called Damo Radar that analyzes contrast-enhanced CT scans to identify nearly 150 abdominal conditions, including cancers, across 18 abdominal organs. The institute announced the release on Friday, describing it as a model capable of spotting malignant tumours and a broad range of other abnormalities. By releasing the model openly rather than keeping it proprietary, Alibaba adds a capable, freely available tool to the fast-growing field of medical imaging AI, potentially lowering the barrier for hospitals and researchers to build diagnostic assistance systems. It also signals the intensifying competition among Chinese tech giants to establish a foothold in healthcare AI, an area with substantial clinical and commercial stakes. Damo Radar is a vision-language model, meaning it pairs image understanding with natural-language reasoning rather than functioning as a pure image classifier, and it is specifically designed for contrast-enhanced CT scans of the abdomen. The reported figure of nearly 150 conditions spanning 18 organs is broad, but such models still typically require validation on diverse real-world patient populations and clinical workflows before routine deployment.

rss · SCMP · Sep 18, 14:30

**Background**: Contrast-enhanced CT is a common imaging technique in which a contrast agent is injected or ingested to make blood vessels, organs and tumours show up more clearly, and it is frequently used to diagnose and stage abdominal malignancies. Vision-language models are AI systems trained jointly on images and accompanying text (such as radiology reports), which lets them connect visual findings with clinical descriptions. Recent research has focused heavily on such foundation models for 3D medical imaging, including CT, as a way to automate detection and reporting tasks that traditionally depend on radiologists.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/tech/big-tech/article/3368055/alibaba-open-sources-medical-ai-model-can-detect-cancer-and-nearly-150-conditions">Alibaba open-sources medical AI model that can detect cancer and nearly 150 conditions | South China Morning Post</a></li>
<li><a href="https://www.nature.com/articles/s44387-025-00015-9">Vision-language foundation model for 3D medical imaging | npj Artificial Intelligence</a></li>
<li><a href="https://link.springer.com/article/10.1007/s13534-025-00484-6">Vision-language foundation models for medical imaging: a review of current practices and innovations | Biomedical Engineering Letters | Springer Nature Link</a></li>

</ul>
</details>

**Tags**: `#medical-ai`, `#open-source`, `#computer-vision`, `#healthcare`, `#vision-language-model`

---

<a id="item-10"></a>
## [Claude Code falls back to reading AGENTS.md when no CLAUDE.md exists](https://code.claude.com/docs/en/changelog) ⭐️ 6.0/10

Claude Code's changelog announces that the tool now falls back to reading an AGENTS.md file when no CLAUDE.md is present in a project, so it can pick up instructions written for other coding agents. This removes the need to duplicate the same guidance across separate tool-specific files. AGENTS.md has become a de facto cross-tool convention used by tens of thousands of open-source projects, and Claude Code's adoption reduces lock-in and duplicated configuration for developers who switch between Claude Code, Codex, and similar agents. It signals that the AI coding agent ecosystem is converging on shared standards rather than each vendor pushing its own proprietary filename. CLAUDE.md still takes precedence, so existing Claude-specific setups keep working exactly as before; the fallback only kicks in when that file is absent. Notably, the change does not extend to other conventions, and as one commenter pointed out, Claude Code still does not detect skills placed in a .agents/skills directory.

hackernews · datadrivenangel · Sep 18, 21:00 · [Discussion](https://news.ycombinator.com/item?id=49760187)

**Background**: Claude Code is Anthropic's agentic coding tool that runs in the terminal and the IDE, reading project files, editing code, and executing commands on the developer's behalf. To steer that behavior, tools historically required their own instruction files — .cursorrules for Cursor, CLAUDE.md for Claude Code, GEMINI.md for Gemini, and copilot-instructions for GitHub Copilot. AGENTS.md emerged as a simple, open, tool-agnostic alternative: essentially a README for agents, giving them a predictable place to find project context and conventions, and it is now used by over 60,000 open-source projects.

<details><summary>References</summary>
<ul>
<li><a href="https://agents.md/">AGENTS . md</a></li>
<li><a href="https://www.getlockstep.dev/blog/agents-md">AGENTS . md : what to put in it, and what it can't carry — Lockstep</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Reaction on Hacker News was largely positive but light-hearted: one commenter called it "the obvious, non-stupid thing to do, like Apple switching to USB-C," while others shared anecdotes about Claude already inferring and creating AGENTS.md symlinks on its own. The main caveat raised was that the compatibility is partial — Claude Code still ignores skills in .agents/skills — so the update was seen as a sensible but incremental interoperability step rather than a breakthrough.

**Tags**: `#Claude Code`, `#AGENTS.md`, `#AI coding agents`, `#developer tools`, `#interoperability`

---

<a id="item-11"></a>
## [OpenJev: Browser-Run 'Jev' Structured-Output Clone Sparks HN Debate](https://openjev.com/) ⭐️ 6.0/10

A project called OpenJev (openjev.com, with source at github.com/TheoLeeCJ/openjev) launched as a way to run typed option logits and autoregressive JSON locally in the browser using open models and WebGPU, claiming to reproduce the interface pattern of "Jev" — described as TypeSafe's closed service for runtime-defined semantic decisions. The submission reached the Hacker News front page with roughly 545 points and 243 comments. The discussion highlights growing demand for open, locally runnable alternatives to closed AI services, and it reopens a live debate over whether "Jev"-style runtime-defined semantic decisions are a genuinely new model paradigm or simply a rebranding of the structured-output features (OpenAI structured outputs, JSON-schema decoding) that developers already use. How that question is answered affects whether teams adopt new tools or stick with existing schema-enforcement stacks. The project's own GitHub description is candid that it only reproduces the interface pattern with open models and "does not reproduce Jev's undisclosed model or training," so it is an interface-compatible reimplementation rather than a copy of the original system. It runs entirely in-browser via WebGPU with no waitlist, contrasting with the closed service it imitates.

hackernews · ilreb · Sep 18, 09:42 · [Discussion](https://news.ycombinator.com/item?id=49752041)

**Background**: Structured output is a widely used LLM technique in which a model is constrained to emit output that conforms to a schema — typically JSON — rather than free-form text, and it is now a standard feature of providers such as OpenAI, Gemini, Anthropic and Mistral, as well as frameworks like LangChain's with_structured_output and validation libraries such as Pydantic and Zod. "Runtime-defined" structured output extends this by letting the schema itself be determined dynamically at execution time instead of being hard-coded in advance. Jev, as described in the submission, is a new kind of AI model pitched as a cheaper and faster path to software intelligence, and OpenJev is an attempt to offer an open, browser-based equivalent.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/TheoLeeCJ/openjev">GitHub - TheoLeeCJ/ openjev : Can we run something like Jev on...</a></li>
<li><a href="https://openjev.com/">OpenJev in your browser</a></li>
<li><a href="https://techsy.io/en/blog/llm-structured-outputs-guide">Reliable JSON from Any LLM : Pydantic + Zod (2026) | TECHSY</a></li>

</ul>
</details>

**Discussion**: Sentiment was largely skeptical: commenters called the site a cluttered "vibecoded" mess with poor usability, and one asked how it differs from OpenAI's structured output paradigm that everyone already moved on from, noting the GitHub admits it "isn't actually Jev." Others offered concrete alternatives — a vLLM patch that turns DiffusionGemma into a Jev-style model (reported to match their evals on an NVIDIA DGX Spark) and an open Jev architecture with model, dataset and papers (arXiv 2503.23303 and 2510.01237, a Hugging Face model from DeepMostInnovations).

**Tags**: `#LLM`, `#structured-output`, `#AI/ML`, `#model-architecture`, `#hacker-news`

---

<a id="item-12"></a>
## [Stanford study finds forebrain and hindbrain arise from two distinct neural progenitors](https://www.newscientist.com/article/2589739-our-brain-evolved-from-two-primitive-nervous-systems-that-merged/) ⭐️ 6.0/10

A Stanford-led team led by Kyle Loh, PhD, associate professor of developmental biology, reported in a bioRxiv preprint (2025.07.02.662771) that the front of the brain arises from a completely different progenitor cell population than the back of the brain, and that this distinction lets them grow hindbrain neurons in a petri dish. The researchers frame the finding as the first demonstration that these two brain regions come from separate neural ectoderm progenitors. If the result holds up, it gives researchers a new way to generate and study hindbrain neurons in vitro, which could aid modeling of diseases affecting the lower brain regions. It also sharpens the picture of how the vertebrate nervous system is partitioned during development, even though the evolutionary story told in press coverage goes well beyond what the paper claims. The work is a bioRxiv preprint and therefore has not been peer reviewed, and the media framing that "our brain evolved from two primitive nervous systems that merged" overstates the authors' own claim, which is about distinct progenitors and growing hindbrain neurons in culture. Community commenters also note that the study describes the same structure in acorn worms, which undercuts a human-specific evolutionary narrative.

hackernews · Jimmc414 · Sep 18, 15:12 · [Discussion](https://news.ycombinator.com/item?id=49755533)

**Background**: During early embryonic development the ectoderm, the outermost of the three germ layers, gives rise to the neural ectoderm (neuroectoderm), which folds into the neural tube and later forms the forebrain, midbrain and hindbrain. A progenitor cell is a cell that can differentiate into a specific target cell type but, unlike a stem cell, can only divide a limited number of times. bioRxiv is an open-access preprint server for biology where papers are posted before peer review, so their conclusions should be treated as preliminary.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neuroectoderm">Neuroectoderm</a></li>
<li><a href="https://en.wikipedia.org/wiki/Progenitor_cell">Progenitor cell</a></li>
<li><a href="https://en.wikipedia.org/wiki/BioRxiv:_The_Preprint_Server_for_Biology">BioRxiv: The Preprint Server for Biology</a></li>

</ul>
</details>

**Discussion**: Commenters broadly pushed back on the media framing: rolph quoted the researchers' actual statement to argue the paper claims only that front and back of the brain come from different progenitors, and networkOne noted the study describes the same structure in acorn worms, making the "our brains" framing misleading. Others used the thread to recommend background reading, with jschveibinz pointing to Carl Sagan's Broca's Brain and The Dragons of Eden and Sapolsky's lectures, while carefree-bob raised Julian Jaynes' bicameral mind hypothesis about ancient consciousness.

**Tags**: `#neuroscience`, `#developmental biology`, `#brain evolution`, `#preprint`, `#science communication`

---

<a id="item-13"></a>
## [Disney names Character.AI's former CEO as its first CTO](https://techcrunch.com/2026/09/18/disneys-first-cto-led-an-ai-startup-it-once-accused-of-copying-its-characters/) ⭐️ 6.0/10

Disney has hired the former CEO of Character.AI as its first-ever chief technology officer, a newly created role at the company. The startup is the same one Disney previously sent a cease-and-desist letter to over the copying of its characters. The appointment is a striking signal that Disney intends to build serious in-house AI capability at the top of the company while it simultaneously fights AI firms over its intellectual property. It also puts a leader from a controversial AI chatbot platform inside one of the world's largest owners of copyrighted characters, blurring the line between AI disruptor and IP defender. The CTO position itself is new for Disney, which has never had one before, so the hire effectively creates a technical leadership layer that did not previously exist. Character.AI lets users chat with customizable characters, many based on fictional media or celebrities — precisely the kind of use that has drawn IP complaints — and the brief report does not name the executive or give a start date.

rss · TechCrunch · Sep 18, 17:59

**Background**: Character.AI is a generative AI chatbot service founded in November 2021 by Noam Shazeer and Daniel de Freitas, former Google engineers who worked on the LaMDA language model. Its beta was released publicly in September 2022, and its iOS and Android app, launched in May 2023, topped 1.7 million downloads within a week. Users create and publish "characters" with custom personalities — many modeled on fictional media figures or celebrities — making the platform a flashpoint in debates over whether and how AI systems may use copyrighted characters. Disney, whose business depends heavily on owned franchises and characters, previously sent the company a cease-and-desist letter over exactly this issue.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Character.ai">Character.ai</a></li>
<li><a href="https://grokipedia.com/page/Character.ai">Character.ai</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Disney`, `#Character.AI`, `#CTO`, `#intellectual property`

---

<a id="item-14"></a>
## [Manus Seeks $4B Valuation in $500M Raise After Meta Deal Collapses](https://techcrunch.com/2026/09/18/manus-seeks-4b-valuation-in-new-500m-fundraise-as-it-resumes-independent-ops/) ⭐️ 6.0/10

Manus, the autonomous AI agent startup that had to break off a merger with Meta earlier this year, is reportedly in discussions to raise $500 million at a $4 billion valuation as it resumes operating as an independent company. The raise would mark a swift re-entry into the capital markets for a company whose exit to Meta was unwound under regulatory pressure, and it signals that investors still see strong value in general-purpose AI agent platforms despite the geopolitical complications of Chinese-founded AI firms. The reported $4 billion valuation is roughly in line with, or above, the figures reported around Meta's earlier acquisition attempt, and the deal is still described as being in discussions rather than closed, so terms could change.

rss · TechCrunch · Sep 18, 16:35

**Background**: Manus is an autonomous AI agent built by Butterfly Effect, a company founded in China and based in Singapore; it launched in invitation-only beta on March 6, 2025, and its launch demo showed the agent completing multi-step tasks like resume screening and stock analysis with little prompting. Meta reportedly agreed to acquire Manus in a multi-billion-dollar deal around late 2025, but the transaction was undone after Chinese regulators intervened, reportedly ordering both parties to restore Manus's Chinese assets to their pre-acquisition state over technology export concerns. That reversal left Manus independent again, which is why it is now raising on its own.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>
<li><a href="https://www.squaredtech.co/metas-2b-manus-deal-is-falling-apart-and-beijing-pulled-the-trigge">Meta Manus Deal : Beijing Forces Major $2B Unwind</a></li>
<li><a href="https://www.linkedin.com/posts/mighty-glory-corporate-solutions_what-is-manus-the-singapore-based-ai-startup-activity-7411919062869401601-8YSS">Meta Acquires Manus , Singapore AI Startup , for Specialized... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#AI startups`, `#funding`, `#Manus`, `#Meta`, `#valuation`

---

<a id="item-15"></a>
## [Meta's Muse AI agent lands on Mac, taking actions for users](https://techcrunch.com/2026/09/18/metas-muse-hits-mac-letting-the-ai-take-actions-on-your-computer/) ⭐️ 6.0/10

Meta's Muse AI assistant is now available on macOS, where it can work with the user's files and apps to take actions on their behalf. The Mac launch follows Meta's September 2026 unveiling of Muse as a personal AI agent that carries out tasks for users. This puts Meta directly into the fast-growing "computer use" agent race on the desktop, where OpenAI's Operator/Computer-Using Agent and a wave of macOS-native startups are already competing. It also shows Meta pushing its assistant from a chat interface toward an agent layer that spans devices and its own apps like Instagram and WhatsApp, which could affect hundreds of millions of consumers if it ships broadly. Muse is powered by Meta's latest Muse Spark 1.3 model and can tap into Meta's other apps such as Instagram and WhatsApp, with users able to give the agent a custom name and avatar and shape how it communicates. The brief Mac announcement did not disclose which macOS apps are supported, how system permissions are handled, or whether processing runs locally or in the cloud.

rss · TechCrunch · Sep 18, 15:22

**Background**: A computer-use agent is an AI program that reasons about a task, plans a sequence of steps, and then acts inside a graphical interface — clicking buttons, typing text, or running commands — rather than only answering questions in chat. Meta announced Muse in September 2026 as an agent designed to carry out tasks on a user's behalf, part of Mark Zuckerberg's vision of a personalized AI assistant for everyone. The Mac desktop is already crowded with similar tools such as Simular, Fazm, and AgentiLoop, so Meta is entering a market with established specialist competitors.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/meta-debuts-muse-ai-assistant-190000718.html">Meta Debuts Muse AI Assistant for Personal Tasks and Organization</a></li>
<li><a href="https://openai.com/index/computer-using-agent/">Computer-Using Agent | OpenAI</a></li>
<li><a href="https://docs.aws.amazon.com/prescriptive-guidance/latest/agentic-ai-patterns/computer-use-agents.html">Computer-use agents - AWS Prescriptive Guidance</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Meta`, `#macOS`, `#automation`, `#computer use`

---

<a id="item-16"></a>
## [UK air traffic chaos traced to millisecond software defect, NATS says](https://www.scmp.com/news/world/europe/article/3368068/over-2000-uk-flight-cancellations-traced-millisecond-software-defect?utm_source=rss_feed) ⭐️ 6.0/10

NATS (formerly National Air Traffic Services) published a preliminary report on Friday stating that a software defect in its National Airspace System caused the September 8 outage that led to more than 2,000 flight cancellations in and out of the UK. The fault corrupted flight data "in the space of a millisecond", triggering a roughly six-hour outage, and the report explicitly rules out human error as the root cause. The incident shows how a single, extremely brief logic error in critical national infrastructure can cascade into hundreds of thousands of disrupted passengers and mass airline cancellations, raising questions about redundancy and failover design in air traffic control software. It also puts pressure on NATS and regulators to explain why no human or procedural safeguard caught a defect that only manifests for a millisecond. The defect was in the subsystem that allocates four-digit transponder codes ("squawks") so controllers can identify and track aircraft on radar; when it failed, flight plan data became corrupted and controllers had to fall back to manual processing. The report is preliminary, so the full root-cause analysis and any remediation plan are still pending.

rss · SCMP · Sep 18, 15:05

**Background**: National Air Traffic Services (NATS) is the UK's main air traffic control provider, handling en-route traffic over England and Wales plus major airports; it was partially privatised in 2001 and is now usually branded simply as NATS. Its National Airspace System handles flight data and assigns each aircraft a four-digit transponder code, a "squawk", which radar systems use to link a blip on screen to a specific flight. If code allocation breaks down, controllers lose automated identification of aircraft, which is why the failure forced a drastic reduction in traffic and led to cancellations. The September 8 disruption was widely reported at the time, with speculation about staff shortages or a cyberattack before NATS pointed to the software defect.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/cw0kl1571lpmo">Flight chaos caused by millisecond software defect , says air traffic ...</a></li>
<li><a href="https://www.theguardian.com/world/2026/sep/18/flight-chaos-affecting-hundreds-of-thousands-caused-in-millisecond-by-software-error-uk">Flight chaos for hundreds of thousands was caused in ‘ millisecond ’ by...</a></li>
<li><a href="https://www.adsadvance.co.uk/nats-report-airspace-software-fault/">NATS report reveals root cause of UK air traffic control failure</a></li>

</ul>
</details>

**Tags**: `#software reliability`, `#critical systems`, `#air traffic control`, `#software defect`, `#incident analysis`

---

<a id="item-17"></a>
## [Ant International embeds AI agents across all global platforms in biggest-ever upgrade](https://www.scmp.com/tech/tech-trends/article/3367998/ant-international-embeds-ai-agents-across-all-platforms-biggest-ever-product-upgrade?utm_source=rss_feed) ⭐️ 6.0/10

Ant International, the Singapore-based overseas affiliate of China's Ant Group, is rolling out AI-native agents across its entire global financial services portfolio, covering cross-border payments, foreign exchange and treasury operations. The company calls it its largest-ever product upgrade, embedding the agents into cross-border payment network Alipay+, merchant services provider Antom, and its account and treasury platform. The move signals that AI agents are shifting from experiments to production infrastructure in fintech, with a major player betting that autonomous software can handle complex multi-market payment, FX and treasury workflows. If it works, it could raise expectations for competitors in cross-border payments, where fragmented regulation and multiple currencies make automation particularly valuable. The upgrade spans multiple named products rather than a single service: Alipay+ for cross-border payments, Antom for merchant payments and digitization, and the account and treasury platform. The announcement offers little technical detail on how the agents operate, what models they use, or how much autonomy they are granted, and no timeline for full rollout was disclosed.

rss · SCMP · Sep 18, 13:00

**Background**: Ant International is the overseas arm of Ant Group, the Chinese fintech giant behind the Alipay payment app, and is headquartered in Singapore. Alipay+ is a unified wallet gateway that connects global merchants to many mobile payment methods through a single integration, while Antom provides payment and digitization services to merchants internationally. AI agents are software systems that can perceive context and take actions on a user's or business's behalf, and in fintech they are increasingly used for tasks such as payment routing, compliance checks and treasury management.

<details><summary>References</summary>
<ul>
<li><a href="https://www.alipayplus.com/">Alipay+ | Connecting Global Brands with Mobile Consumers</a></li>
<li><a href="https://en.wikipedia.org/wiki/Antom">Antom - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Alipay">Alipay - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#fintech`, `#Ant Group`, `#payments`, `#cross-border payments`

---

<a id="item-18"></a>
## [AI-exposed majors' graduates since 2022 pushed into retail and food service, Reddit post claims](https://www.reddit.com/r/Economics/comments/1wjs68p/college_grads_shut_out_of_aiexposed_majors_since/) ⭐️ 6.0/10

A Reddit post on r/Economics claims that college graduates who studied fields most exposed to AI automation since 2022 are increasingly taking jobs in retail and food service instead of the white-collar positions they trained for. The item as provided consists only of the post title and a link, with no article text, data, or methodology included. If the claim holds up, it points to AI reshaping entry-level white-collar hiring, which would affect the return on investment of a college degree, early-career earnings, and the pipeline of junior talent that firms have traditionally used to train future professionals. It also feeds into the broader policy debate over whether AI-driven displacement differs from earlier waves of automation by hitting cognitive, degree-holding work rather than routine manual tasks. The post offers no supporting evidence in the supplied content, so the claim remains unverified; the key caveat is that "AI-exposed majors" is a constructed category whose meaning depends heavily on how exposure is measured — for example, by task-level automation scores rather than whole occupations — and correlation with a weak entry-level job market in general makes causal attribution to AI difficult.

reddit · r/economics · /u/Puzzleheaded-King584 · Sep 18, 14:44

**Background**: Economists often measure an occupation's AI exposure by analyzing the mix of tasks it involves and how well those tasks match current AI capabilities, rather than by looking at the job title alone. Jobs that are heavily exposed are not necessarily automated away; they may instead see tasks shifted to AI tools, reducing the number of junior hires needed. "Underemployment" describes the situation where graduates work in jobs that do not require their degree, and retail and food service are commonly used as examples of such roles in labor statistics. The claim in this post is essentially that this underemployment rate has risen specifically for AI-exposed majors since 2022 — the year ChatGPT was released and generative AI adoption accelerated.

**Tags**: `#AI and employment`, `#labor economics`, `#higher education`, `#automation`, `#job displacement`

---