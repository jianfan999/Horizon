---
layout: default
title: "Horizon Summary: 2026-11-25 (EN)"
date: 2026-11-25
lang: en
---

> From 97 items, 13 important content pieces were selected

---

1. [Matrix Multiplication is Θ(n^2.25) (pdf)](#item-1) ⭐️ 9.0/10
2. [Ternary Bonsai 2.5 27B: a 5.9 GB ternary model tuned for agentic coding](#item-2) ⭐️ 8.0/10
3. [GreyNoise: Attackers Forge Admin Cookies on Check Point Management Servers](#item-3) ⭐️ 8.0/10
4. [PenGPT: A Data-Centric Transformer for Handwriting and Sketches](#item-4) ⭐️ 7.0/10
5. [OpenAI says GPT-6.2 can design 3D minibinders, but specialized models still do sequence work](#item-5) ⭐️ 7.0/10
6. [Amazon buys Decart for $7.5B to boost Trainium chip efficiency](#item-6) ⭐️ 7.0/10
7. [New benchmark finds even top AI agents struggle with everyday tasks](#item-7) ⭐️ 6.0/10
8. [Tidal to ban and remove millions of fully AI-generated tracks](#item-8) ⭐️ 6.0/10
9. [Uber and Nuro Start Driverless Testing of Lucid Gravity Robotaxis in Bay Area](#item-9) ⭐️ 6.0/10
10. [CIA Unclassified Open-Source Intelligence System Breached in Cyberattack](#item-10) ⭐️ 6.0/10
11. [US Jury Finds Huawei Guilty on 10 of 12 Counts, Ending Seven-Year Case](#item-11) ⭐️ 6.0/10
12. [Nobel laureate Ferenc Krausz leads HKU 20-year blood screening study](#item-12) ⭐️ 6.0/10
13. [DR Congo Suspends Cobalt Exports, Chinese Firms Rush Shipments](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Matrix Multiplication is Θ(n^2.25) (pdf)](https://github.com/openai/math/blob/main/preprints/The-matrix-multiplication-exponent-is-nine-fourths-November-24-2026/paper.pdf) ⭐️ 9.0/10

A claimed preprint (attributed to OpenAI) argues the matrix multiplication exponent is exactly 9/4, refuting the conjecture that it equals two, alongside related breakthroughs in linear programming and game solving.

hackernews · E-Reverance · Nov 25, 01:19 · [Discussion](https://news.ycombinator.com/item?id=50637220)

**Tags**: `#algorithms`, `#matrix-multiplication`, `#theory`, `#AI-for-math`, `#OpenAI`

---

<a id="item-2"></a>
## [Ternary Bonsai 2.5 27B: a 5.9 GB ternary model tuned for agentic coding](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 8.0/10

PrismML released Ternary Bonsai 2.5 27B, a ternary (1.58-bit) quantized model derived from Qwen3.8-27B with the architecture left unchanged, shipping at the same 5.9 GB footprint as Bonsai 2 while adding substantially stronger agentic coding, multi-turn tool use and multi-step task execution. Early users report roughly 22–25 tokens/s with the Q2 GGUF on a Mac Mini M5 Pro (24 GB RAM) while holding a 128k context in memory. If a ~6 GB ternary model really lands near frontier-level scores on SWE-bench Verified, agentic coding becomes feasible on ordinary consumer Apple hardware rather than datacenter GPUs, which would meaningfully shift who can run coding agents locally. The release also serves as a public test case for how far extreme quantization can be pushed before capability degrades. The model keeps the hybrid-attention architecture of its Qwen3.8-27B base and restricts weights to three values (−1, 0, +1), which is where the large size reduction comes from; one community long-horizon benchmark shows Bonsai 2.5 finishing with 17% fewer steps and about 29% less wall-clock time than Bonsai 2, though with the same 5 of 8 tasks passed. Because it is a heavily quantized derivative rather than a new pretrained model, direct comparisons against full-precision or differently quantized models remain tricky.

hackernews · b0m · Nov 24, 20:08 · [Discussion](https://news.ycombinator.com/item?id=50633922)

**Background**: Ternary (1.58-bit) quantization is an extreme form of weight compression in which every weight is stored as one of three values: −1, 0, or +1, trading numerical precision for much smaller memory footprints and cheaper arithmetic. SWE-bench Verified, meanwhile, is a human-filtered set of 500 real GitHub issues from 12 popular Python repositories, where a model must produce a patch that actually resolves the reported problem — which is why it is widely used as a proxy for agentic coding ability.

<details><summary>References</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">PrismML — Introducing Ternary Bonsai 2.5 27B: Powering ...</a></li>
<li><a href="https://docs.prismml.com/models/bonsai-2-5-27b">Ternary Bonsai 2.5 27B - Bonsai - docs.prismml.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/1.58-bit_large_language_model">1.58-bit large language model - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread (385 points, 129 comments) was broadly impressed by the speed and 128k context on consumer hardware, with users sharing their own tok/s numbers and long-horizon task results. At the same time, commenters pushed back on the SWE-bench claim, asking whether the result reflects genuine small-model progress, benchmark drift, or deliberate 'benchmaxxing', and several called for apples-to-apples comparisons against comparably small Q1/Q2 quants of models like Qwen3.8.

**Tags**: `#local-llm`, `#quantization`, `#model-efficiency`, `#swe-bench`, `#agentic-coding`

---

<a id="item-3"></a>
## [GreyNoise: Attackers Forge Admin Cookies on Check Point Management Servers](https://www.greynoise.io/blog/check-point-security-management-servers-intrusion-campaign) ⭐️ 8.0/10

GreyNoise documented an active exploitation campaign against Check Point security management servers in which the actor repeatedly logged in to the HFS loginSrp1 endpoint, harvested the successive signed session cookies whose "sid" values come from JavaScript's Math.random(), and reconstructed the internal state of Node.js/V8's PRNG. With that state the attacker recovered an HFS session-cookie signing key and forged a signed administrator session cookie. Check Point security management servers are widely deployed in enterprises and govern firewall policy across entire networks, so a forged admin session effectively hands an attacker control of the security control plane. The case also demonstrates that relying on a non-cryptographic PRNG for security-sensitive values is exploitable in practice, not just in theory. The attack did not break the signing algorithm itself; it exploited the predictable, recoverable state of V8's Math.random() (an xorshift128+ PRNG) to obtain or derive the key material used to sign session cookies. Community members also noted that the initial access vector is not fully clear in the report, with CVE-2026-16232 suspected as the entry point and open questions about how many affected organizations exposed their management servers to the internet.

hackernews · louiereederson · Nov 24, 16:32 · [Discussion](https://news.ycombinator.com/item?id=50630594)

**Background**: Check Point security management servers are the central consoles that administrators use to define and push firewall and security policy to gateways; the report refers to an "HFS" web login endpoint on these servers. JavaScript's Math.random() is not a cryptographic random number generator: it is built on a deterministic pseudo-random algorithm whose entire internal state can be reconstructed from enough observed outputs, as V8's own engineers have explained. Because a cookie-signing key derived from such output becomes derivable, session cookies that look properly signed and unforgeable can in fact be forged.

<details><summary>References</summary>
<ul>
<li><a href="https://v8.dev/blog/math-random">There’s Math.random (), and then there’s Math.random () · V8</a></li>
<li><a href="https://stackoverflow.com/questions/78219837/predicting-v8s-math-random-truncated-outputs">Predicting V8's Math.random () truncated outputs</a></li>
<li><a href="https://www.greynoise.io/">GreyNoise | Real-Time Network Threat Intelligence</a></li>

</ul>
</details>

**Discussion**: Commenters relished the return of a classic PRNG weakness, with one arguing that Math.random() itself should be made secure rather than patched in hundreds of applications that use it incorrectly. Others pointed to the report's vague initial access vector and suspected CVE-2026-16232, while a broader thread warned that LLM-accelerated offensive tooling will soon let far less sophisticated criminals attack any internet-facing service, including critical infrastructure.

**Tags**: `#security`, `#vulnerability-exploitation`, `#prng-cryptography`, `#check-point`, `#incident-report`

---

<a id="item-4"></a>
## [PenGPT: A Data-Centric Transformer for Handwriting and Sketches](https://greydanus.github.io/2026/11/12/pengpt/) ⭐️ 7.0/10

The PenGPT project introduces a generative Transformer trained on curated handwriting and sketch data, with the author reporting that roughly 80% of the effort went into building clean datasets and quality control rather than architectural novelty. The model was trained on 8×H100 GPUs and represents pen strokes as tokens. It offers a concrete case study in the 'Bitter Lesson' debate: strong data engineering can matter more than clever architecture, especially for generating synthetic handwriting data that can augment OCR and handwriting-recognition systems. The discussion also highlights how modern vision models and multimodal APIs make data curation more accessible. The author cautions that an 8×H100 training run is not the most spectacular illustration of the Bitter Lesson, and notes that agentic workflows, open-weight vision models, and cheap multimodal APIs smoothed data filtering and caption generation. Commenters also singled out 'stroke tokens' and the potential to generate synthetic data for OCR of handwritten prescriptions.

hackernews · smusamashah · Nov 25, 00:54 · [Discussion](https://news.ycombinator.com/item?id=50637056)

**Background**: A generative Transformer is a neural network that learns to predict sequences and can sample new ones; for handwriting and sketches, pen movements can be encoded as sequences of stroke tokens. Synthetic handwriting data is already used in handwriting recognition to supplement scarce or sensitive real-world samples. The Bitter Lesson is Rich Sutton's argument that general methods that scale with compute tend to outperform approaches built around hand-crafted domain knowledge.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2508.09936">Quo Vadis Handwritten Text Generation for Handwritten Text...</a></li>
<li><a href="https://unidata.pro/blog/best-ml-handwriting-datasets/">21 Best Handwriting Datasets for Machine Learning — Unidata</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly positive and focused on the data-over-architecture lesson: one reader cited the author's 80% data-effort quote, while the author replied that the 8×H100 run is modest and that agentic workflows have made data quality work much smoother. Others saw practical value in generating synthetic handwriting data for OCR, noted the 'stroke tokens' design, and criticized the blog's prose as sounding overly AI-generated ('Claudish').

**Tags**: `#generative-models`, `#transformers`, `#handwriting-recognition`, `#synthetic-data`, `#machine-learning`

---

<a id="item-5"></a>
## [OpenAI says GPT-6.2 can design 3D minibinders, but specialized models still do sequence work](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) ⭐️ 7.0/10

OpenAI reported that GPT-6.2 was given the three-dimensional structures of five target proteins with the desired attachment sites marked, and then wrote code to generate three-dimensional minibinder designs on its own, without calling specialized protein AI models for the design step. However, converting those backbone designs into testable proteins still required the specialized model SolubleMPNN to propose amino acid sequences, plus other protein models to filter candidates for folding and binding-site accuracy. If general-purpose LLMs can competently orchestrate parts of a protein-design pipeline, it widens the pool of researchers who can attempt binder design without mastering each specialized tool, and it suggests a "glue layer" role for LLMs across scientific subfields. The claim also matters competitively, since AI-for-biology is a key battleground among frontier model labs. The work is computational: the headline claim covers 3D backbone design only, with sequence design (SolubleMPNN) and filtering for folding and on-target binding handled by specialized models, and community commenters noted the evidence is heavy on computation and light on laboratory validation. OpenAI's framing emphasizes code-writing as the mechanism — the model's advantage comes from expressing the design procedure in code rather than from implicit structural reasoning alone.

hackernews · acossta · Nov 24, 21:02 · [Discussion](https://news.ycombinator.com/item?id=50634658)

**Background**: Minibinders are small designed proteins that bind tightly to a specific target protein, and they are attractive as therapeutics and as building blocks for synthetic biology sensors. Computational protein design typically runs as a pipeline: a generative model proposes a 3D backbone structure, a sequence-design model such as ProteinMPNN (SolubleMPNN is a solubility-optimized variant) picks an amino acid sequence predicted to fold into that backbone, and further models filter candidates before lab testing. Because a protein's sequence largely determines its structure, skeptics argue that the sequence step is where the actual design happens.

<details><summary>References</summary>
<ul>
<li><a href="https://idl.uw.edu/mosaic/examples/protein-design.html">Protein Design Explorer | Mosaic</a></li>
<li><a href="https://arxiv.org/html/2104.04457">Protein sequence design with deep generative models</a></li>
<li><a href="https://www.nature.com/articles/s43586-025-00383-1">Computational protein design - Nature Reviews Methods Primers</a></li>

</ul>
</details>

**Discussion**: Commenters were interested but skeptical: the dominant view was that GPT-6.2 acts as a "glue layer" orchestrating specialized tools rather than independently designing proteins, and several questioned what exactly the model contributed given that SolubleMPNN supplied the sequences. Others praised LLMs' demonstrated strength at connecting specialized sub-tasks and code-based workflows, while some criticized the biological controls as thin compared with the computational exploration.

**Tags**: `#AI`, `#protein design`, `#LLMs`, `#computational biology`, `#OpenAI`

---

<a id="item-6"></a>
## [Amazon buys Decart for $7.5B to boost Trainium chip efficiency](https://techcrunch.com/2026/11/24/amazons-decart-acquisition-is-a-bet-on-using-software-to-narrow-the-gap-with-nvidia-in-the-ai-chip-race/) ⭐️ 7.0/10

Amazon is acquiring Israeli AI startup Decart for a reported $7.5 billion, a deal aimed squarely at improving the efficiency of its in-house Trainium AI chips. The move is widely read as a software bet: Decart's optimization stack is meant to squeeze more usable performance out of Amazon's silicon so it can compete more credibly with Nvidia. Nvidia's dominance in AI accelerators rests not only on hardware but on the maturity of its CUDA software ecosystem, so buying a compiler and kernel-tuning specialist is a shortcut to closing that gap. If it works, it could lower the cost of AI training and inference on AWS, giving cloud customers a genuinely competitive non-Nvidia option and putting pressure on Nvidia's pricing power. The reported $7.5 billion price is remarkable for a company whose main contribution here is software rather than silicon, suggesting Amazon values the optimization layer highly. The deal's payoff depends on how much of Decart's real-time world-model and inference expertise transfers to Trainium's architecture, which pairs NeuronCore-v2 cores with 32 GiB of device memory and roughly 820 GiB/sec of bandwidth per chip.

rss · TechCrunch · Nov 24, 15:51

**Background**: Trainium is AWS's purpose-built AI chip, designed to deliver better price-performance for training and inference than general-purpose GPUs. But raw chip specifications matter less than whether software — compilers, kernels and runtime schedulers — can actually keep the hardware's compute units busy. Decart's Optimization Stack sits between the model and the chip, tuning these layers so workloads like LLMs, agents, video and world models run efficiently on non-Nvidia hardware. That is precisely the moat Nvidia built with CUDA over more than a decade, and why competitors see software as the real bottleneck.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/24/amazons-decart-acquisition-is-a-bet-on-using-software-to-narrow-the-gap-with-nvidia-in-the-ai-chip-race/">Amazon's Decart acquisition is a bet on using software to narrow the...</a></li>
<li><a href="https://decart.ai/optimization-engine">Decart Optimization Stack</a></li>
<li><a href="https://aws.amazon.com/ai/machine-learning/trainium/">AI Accelerator - AWS Trainium - AWS - aws.amazon.com</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#Amazon`, `#Nvidia`, `#acquisitions`, `#Trainium`

---

<a id="item-7"></a>
## [New benchmark finds even top AI agents struggle with everyday tasks](https://techcrunch.com/2026/11/24/even-the-best-ai-agents-struggle-with-everyday-life/) ⭐️ 6.0/10

A newly reported benchmark shows that even the most advanced personal AI assistants fail to complete ordinary, everyday tasks reliably and safely, often introducing new problems while attempting them. The finding arrives as millions of consumers are already adopting personal AI agents for day-to-day use. Reliability and safety gaps in agentic AI directly affect ordinary users who delegate real tasks to these assistants, not just researchers running demos. The result underscores that impressive capability demonstrations do not yet translate into dependable autonomy in messy, real-world conditions. The publicly available report does not name the benchmark, the number of tasks evaluated, or the specific scores of individual models, so exact failure rates and methodology cannot be independently verified. Notably, the framing stresses safety as well as success rate, implying that agents can complete a task while still causing collateral problems.

rss · TechCrunch · Nov 24, 21:33

**Background**: AI agents are models that go beyond answering questions: they plan multi-step actions and use external tools such as browsers, file systems, and APIs to actually carry out tasks. Evaluating them is much harder than scoring a static question-answer test, because success depends on long sequences of actions where a single wrong step can break the whole task or cause unintended side effects. This is why agent benchmarks increasingly measure not only whether a task was finished, but whether it was finished safely and without damaging the user's data or accounts.

**Tags**: `#AI agents`, `#benchmarks`, `#AI safety`, `#reliability`, `#personal assistants`

---

<a id="item-8"></a>
## [Tidal to ban and remove millions of fully AI-generated tracks](https://techcrunch.com/2026/11/24/tidal-to-ban-and-remove-millions-of-ai-generated-tracks-as-ai-slop-inundates-music-streaming/) ⭐️ 6.0/10

Tidal announced it will ban and remove millions of tracks that are entirely generated by AI, while continuing to accept songs made with AI assistance. The company framed the policy as a distinction between fully synthetic tracks and human-led music that uses AI as a tool. Tidal is one of the first major streaming services to take a hard removal stance rather than just labeling or filtering AI content, which puts pressure on Spotify, Apple Music and others to follow suit. Artists and rights holders flooded by mass-produced "AI slop" could see fairer royalty splits and better discovery if such bans spread. The critical open question is enforcement: reliably distinguishing fully AI-generated tracks from AI-assisted ones is notoriously hard, since watermarking and artifact detection are both unreliable at scale. Tidal has not publicly detailed the detection method or the timeline and scope of the removals.

rss · TechCrunch · Nov 24, 16:46

**Background**: Tools such as Suno and Udio let anyone generate complete songs from a text prompt, and since 2025 streaming catalogs have been flooded with millions of such uploads. Platforms have responded unevenly: Bandcamp has banned AI music outright, Deezer built its own synthetic-audio detection system, and YouTube can use Google's SynthID watermark detection, while Spotify has experimented with "AI personas" and labeling. Because most AI music carries no watermark and is trained on real recordings, detection usually relies on statistical audio analysis and metadata signals rather than definitive proof.

<details><summary>References</summary>
<ul>
<li><a href="https://www.billboard.com/lists/how-each-music-listening-platform-treats-ai-music/">How Each Music Listening Platform Is Treating AI Music (Updating)</a></li>
<li><a href="https://soundiiz.com/blog/ai-generated-music-streaming-platforms/">How Streaming Platforms Detect AI-Generated Music | Spotify ...</a></li>
<li><a href="https://undetectr.com/blog/ai-music-detection-explained-2026">AI Music Detection Explained: Every Method Platforms... — Undetectr</a></li>

</ul>
</details>

**Tags**: `#AI-generated music`, `#content moderation`, `#music streaming`, `#Tidal`, `#platform policy`

---

<a id="item-9"></a>
## [Uber and Nuro Start Driverless Testing of Lucid Gravity Robotaxis in Bay Area](https://techcrunch.com/2026/11/24/uber-and-nuro-begin-driverless-testing-of-lucid-robotaxis-ahead-of-2027-launch/) ⭐️ 6.0/10

Uber and Nuro have begun testing driverless Lucid Gravity SUVs on public streets in the San Francisco Bay Area, marking the first time the partners' robotaxi hardware and software stack is operating without a safety driver on open roads. The testing phase precedes a planned commercial launch of the Uber-exclusive robotaxi service now targeted for 2027. Removing the safety driver is the decisive gate between a demo program and a commercial robotaxi business, so this milestone puts the Uber–Nuro–Lucid alliance in the same operational tier as Waymo and other players already running driverless rides. If the 2027 launch holds, Uber gains a third-party-supplied Level 4 fleet to sell rides on its network without building autonomy in-house, a model that could reshape how ride-hailing platforms source self-driving capacity. The Lucid Gravity robotaxi, unveiled in January 2026, is equipped with high-resolution cameras, solid-state lidar and radars feeding Nuro's licensed Nuro Driver software, which Nuro says is validated by more than 2 million autonomous miles with zero at-fault incidents. The partnership announced in July 2025 envisioned 20,000+ Level 4 Gravity robotaxis delivered exclusively through Uber starting in 2026, so the shift of the commercial launch to 2027 and the current testing being limited to the Bay Area indicate the rollout is proceeding more cautiously than originally announced.

rss · TechCrunch · Nov 24, 16:40

**Background**: Nuro began as a autonomous delivery-robot company and in September 2024 pivoted to licensing its AI-based self-driving stack, called Nuro Driver, to automakers, suppliers and mobility providers; the software is designed to enable up to Level 4 automation, meaning the vehicle can drive without a human in defined operational areas. Lucid Motors supplies the Gravity, an electric SUV positioned as the vehicle platform, while Uber contributes the demand side — the ride-hailing network and customer base — rather than the autonomy itself. This three-way split of vehicle, software and network is a common structure in the robotaxi industry, where platform companies increasingly partner instead of developing self-driving technology internally.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/11/24/uber-and-nuro-begin-driverless-testing-of-lucid-robotaxis-ahead-of-2027-launch/">Uber and Nuro begin driverless testing of Lucid robotaxis ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nuro">Nuro - Wikipedia</a></li>
<li><a href="https://lucidmotors.com/stories/lucid-nuro-uber-partner">Lucid, Nuro & Uber Launch Robotaxis | Lucid Motors</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#robotaxi`, `#Uber`, `#Nuro`, `#Lucid`

---

<a id="item-10"></a>
## [CIA Unclassified Open-Source Intelligence System Breached in Cyberattack](https://www.scmp.com/news/world/united-states-canada/article/3375693/unclassified-cia-system-breached-latest-us-cybersecurity-incident) ⭐️ 6.0/10

An unclassified CIA system used for handling open-source intelligence was breached in a cyberattack, according to a person familiar with the incident who spoke to the Associated Press on condition of anonymity. The source said no classified information was involved and that the issue has since been resolved. The incident adds to a string of recent cybersecurity breaches across US government systems, reinforcing concerns that even lower-sensitivity networks can be viable entry points for attackers. It also highlights how open-source intelligence platforms, which aggregate vast amounts of publicly available data, are increasingly treated as valuable targets by adversaries. Officials have not disclosed the attack vector, the suspected perpetrator, or the duration of the intrusion, and the claim that no classified data was exposed rests on an anonymous source rather than a public statement. Because the affected system handles open-source intelligence, its contents are by definition drawn from publicly available data, though the analytical tools, queries, and workflows built on top of it could still be sensitive.

rss · SCMP · Nov 25, 03:13

**Background**: Open-source intelligence, or OSINT, is the practice of collecting and analyzing publicly available information — such as news reports, social media posts, satellite imagery, and commercial data — to answer specific intelligence questions. Government agencies maintain dedicated OSINT systems that aggregate and analyze these sources at scale, which makes them attractive targets even when they hold no classified material. The CIA's breach follows a broader pattern of cyberattacks against US federal networks in recent years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open-source_intelligence">Open - source intelligence - Wikipedia</a></li>
<li><a href="https://spiderfoot.xyz/">SpiderFoot - Open Source Intelligence Automation</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#data breach`, `#CIA`, `#open source intelligence`, `#US government`

---

<a id="item-11"></a>
## [US Jury Finds Huawei Guilty on 10 of 12 Counts, Ending Seven-Year Case](https://www.scmp.com/news/us/article/3375673/huawei-guilty-10-12-counts-after-2-month-battle-us-courtroom) ⭐️ 6.0/10

A federal jury in Brooklyn, New York, on Tuesday found Huawei Technologies and three subsidiaries guilty on 10 of 12 counts, including bank fraud, wire fraud, conspiracy to steal trade secrets and evading US sanctions. The company was acquitted on the two remaining counts — conspiracy to obstruct justice and conspiracy under the Racketeer Influenced and Corrupt Organizations (RICO) Act — bringing the nearly seven-year criminal case to a close. The verdict marks one of the most significant criminal outcomes ever against a major Chinese technology company and could shape how multinationals structure their compliance programmes around US sanctions and trade-secret rules. It also lands amid ongoing US-China tensions over semiconductors and export controls, and may influence how other firms assess the legal risk of doing business with sanctioned entities. The trade-secret conspiracy charges, added in a superseding indictment in 2020, named Cisco Systems, Motorola Solutions, T-Mobile, Quintel USA and Fujitsu among the alleged victims. The acquittal on the RICO conspiracy count — the most serious charge — removes a theory that could have exposed the company to extended penalties for acts carried out as part of an ongoing criminal enterprise.

rss · SCMP · Nov 24, 20:36

**Background**: The case stems from a 2018 indictment that also led to the arrest of Huawei's then-CFO Meng Wanzhou in Canada, and the trade-secret and sanctions-evasion charges were layered on in a superseding indictment two years later. RICO is a 1970 federal statute originally aimed at organised crime that allows prosecutors to pursue extended penalties for a pattern of racketeering activity conducted through an enterprise; a RICO conspiracy conviction would have been the heaviest exposure in this case. Sanctions evasion refers to conduct intended to bypass financial or trade sanctions — here, allegedly using shell companies to conduct business in Iran — and is pursued through criminal law and anti-money-laundering controls.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Racketeer_Influenced_and_Corrupt_Organizations_Act">Racketeer Influenced and Corrupt Organizations Act</a></li>
<li><a href="https://www.zerohedge.com/geopolitical/huawei-found-guilty-plotting-steal-us-trade-secrets-and-lying-banks-over-iran">Huawei Found Guilty Of Plotting To Steal US Trade Secrets And Lying...</a></li>
<li><a href="https://www.sanctions.io/blog/what-is-sanctions-evasion-and-how-it-works">What Is Sanctions Evasion and How It Works | sanctions.io</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#legal`, `#trade secrets`, `#sanctions`, `#technology industry`

---

<a id="item-12"></a>
## [Nobel laureate Ferenc Krausz leads HKU 20-year blood screening study](https://www.scmp.com/news/hong-kong/health-environment/article/3375655/nobel-laureate-leads-university-hong-kong-study-spot-diseases-early) ⭐️ 6.0/10

The University of Hong Kong launched the "Protecting.Health Hong Kong" study on Tuesday through its Institute for Precision Prevention, aiming to collect and track blood samples from 15,000 local residents over 20 years. The project is led by institute director Professor Ferenc Krausz, the 2023 Nobel laureate in physics whom HKU recently recruited, and its goal is an affordable screening tool that detects cancer, diabetes, cardiovascular disease and chronic respiratory illness before symptoms appear. If it works, a cheap blood-based screen would shift these chronic diseases from late-stage treatment toward early detection and prevention, which matters most in ageing populations where cancer, diabetes and cardiovascular disease dominate the health burden. It also represents a concrete attempt to translate an attosecond-physics laboratory technique into routine preventive medicine, a path that has so far produced few population-scale validations. The study is described only in broad strokes: a 20-year follow-up of 15,000 volunteers, with no published protocol, target biomarkers, sensitivity/specificity figures or recruitment timeline disclosed. Because the endpoint is shifting from a physics measurement to a clinical screening product, the hard questions will be validation in a diverse Chinese population, regulatory approval and per-test cost at scale.

rss · SCMP · Nov 24, 13:09

**Background**: Ferenc Krausz shared the 2023 Nobel Prize in Physics for work on attosecond laser pulses — flashes of light lasting a trillionth of a second — which made it possible to observe electrons moving inside matter. His group extended the idea to biology: firing ultrashort infrared laser pulses at blood serum or plasma makes the molecules vibrate and emit light back, producing a detailed "molecular fingerprint" that machine learning can compare against disease states. The hope is that such a signature changes measurably long before clinical symptoms of cancer, diabetes or cardiovascular disease appear, so that a single inexpensive blood test could flag people who need further investigation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lmu.de/en/newsroom/news-overview/news/from-solid-state-physics-to-early-detection-of-diseases-8fd219d1.html">From solid-state physics to early detection of diseases - LMU Munich</a></li>
<li><a href="https://ferenckrausz.com/vision/">Vision | Ferenc Krausz</a></li>
<li><a href="https://nkfih.gov.hu/english/hungarian-and-international-rdi-news/another-hungarian-nobel-laureate-ferenc-krausz">Another Hungarian Nobel laureate: Ferenc Krausz, researcher ...</a></li>

</ul>
</details>

**Tags**: `#precision medicine`, `#biomarker screening`, `#early disease detection`, `#public health`, `#research initiative`

---

<a id="item-13"></a>
## [DR Congo Suspends Cobalt Exports, Chinese Firms Rush Shipments](https://www.scmp.com/economy/global-economy/article/3375611/chinese-cobalt-firms-race-beat-dr-congos-export-ban-key-battery-material) ⭐️ 6.0/10

The Democratic Republic of Congo's mining regulator ARECOMS announced on Monday that all cobalt exports will be suspended from November 30 until further notice, covering both industrial mines and artisanal production. Chinese operators holding cobalt assets in the country are now racing to accelerate shipments in the days before the ban takes effect. DR Congo holds the world's largest cobalt reserves and supplies the majority of global output, so a suspension of unknown duration injects significant supply risk into the battery supply chain for electric vehicles and consumer electronics. Chinese refiners and battery makers, which dominate cobalt processing, are the most directly exposed to price volatility and shipment disruptions. The suspension applies to all cobalt produced nationally, including artisanal mining output, not just large industrial operations, and comes with no stated end date, meaning buyers cannot plan around a fixed window. The rush to ship before November 30 suggests near-term tightening of spot supply even before the ban formally begins.

rss · SCMP · Nov 24, 12:00

**Background**: Cobalt is a key ingredient in lithium-ion battery cathodes, helping stabilize the chemistry and improve energy density and safety, and it is also used in superalloys and electronics. Cobalt is largely a by-product of copper and nickel mining, and DR Congo dominates global supply, with most of its output shipped to China for refining. Because supply is geographically concentrated and politically sensitive, cobalt has long been viewed as one of the most fragile links in the battery materials chain.

**Tags**: `#cobalt`, `#DR Congo`, `#battery materials`, `#supply chain`, `#export ban`

---