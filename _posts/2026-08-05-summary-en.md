---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 140 items, 28 important content pieces were selected

---

1. [Hackers steal over $130M by exploiting Coldcard hardware wallet bug](#item-1) ⭐️ 9.0/10
2. [Mistral releases Shieldstral, a 3B open-weights multimodal moderation model](#item-2) ⭐️ 8.0/10
3. [DeepSeek V4 Flash Runs on Single AMD MI300X at 150+ Tokens/s](#item-3) ⭐️ 8.0/10
4. [Troy Hunt: FedEx Emails Train Users to Accept Phishing](#item-4) ⭐️ 8.0/10
5. [Oxide Computer Raises $445M in Series D Round](#item-5) ⭐️ 8.0/10
6. [Chinese startup XinXiao cuts chip power sign-off from weeks to days](#item-6) ⭐️ 8.0/10
7. [SpaceX and Nvidia Team Up to Put Data-Center AI Compute in Orbit](#item-7) ⭐️ 8.0/10
8. [Samsung Unveils AI Memory Roadmap with zHBM and 400+ Layer V10 NAND](#item-8) ⭐️ 8.0/10
9. [EFF warns Android apps may leak location data via third-party code](#item-9) ⭐️ 8.0/10
10. [Open-weight AI Models Approach Frontier; Safety Gap Persists](#item-10) ⭐️ 8.0/10
11. [Anthropic signs $10B deal with AI cloud startup Volta](#item-11) ⭐️ 8.0/10
12. [AI fuels over half of Africa's cybercrime as scams surge, Interpol reports](#item-12) ⭐️ 7.0/10
13. [Simple algorithm and color space for generating diverse skin tones](#item-13) ⭐️ 7.0/10
14. [Automakers Roll Out Own Battery Brands to Challenge CATL](#item-14) ⭐️ 7.0/10
15. [Kimi K3与DeepSeek V4之间，隔着原生多模态的时间差](#item-15) ⭐️ 7.0/10
16. [Apple Asks Judge to Halt OpenAI's Use of Stolen Trade Secrets](#item-16) ⭐️ 7.0/10
17. [Waymo Opens Dallas Robotaxi Service to All](#item-17) ⭐️ 7.0/10
18. [Spotify partners with Merlin to expand AI remix and covers tool](#item-18) ⭐️ 7.0/10
19. [Texas Halts New Data Center Approvals Amid Power Grid Strain, Governor Orders Audits](#item-19) ⭐️ 7.0/10
20. [US AI Leaders Embrace Chinese Open-Weight Models, Challenge Closed-Source Safety Claims](#item-20) ⭐️ 7.0/10
21. [China's MiniMax restricts overseas use of open-source H3 video model](#item-21) ⭐️ 7.0/10
22. [Shenzhen-Based Mathematician Yurii Nesterov Wins Top Applied Maths Prize](#item-22) ⭐️ 7.0/10
23. [Glass Substrate Maker Xunlin Raises ¥200M Series B to Expand Capacity](#item-23) ⭐️ 6.0/10
24. [Precision Reducer Maker Taoshi Raises ¥100M+; Valuation Tops ¥1B](#item-24) ⭐️ 6.0/10
25. [Blackstone in Talks to Arrange $36B Debt for Anthropic AI Chips](#item-25) ⭐️ 6.0/10
26. [SpaceX doubles revenue on Anthropic, Google compute deals, Starlink growth](#item-26) ⭐️ 6.0/10
27. [Nvidia's Open Secure AI Alliance Proposes AI-Agent Defenses Within a Week](#item-27) ⭐️ 6.0/10
28. [Chinese startup Spirit AI tops Nvidia on RoboArena, sparking manipulation accusations](#item-28) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Hackers steal over $130M by exploiting Coldcard hardware wallet bug](https://techcrunch.com/2026/08/04/hackers-steal-over-130-million-by-exploiting-bug-in-offline-hardware-wallets/) ⭐️ 9.0/10

A vulnerability in Coldcard hardware wallets has been exploited to drain more than $130 million in cryptocurrency from victims' wallets, according to blockchain-monitoring firms. The incident was reported on August 4, 2026, and highlights a critical flaw in devices marketed as ultra-secure offline storage. Hardware wallets like Coldcard are considered the gold standard for cryptocurrency security because they keep private keys offline. This breach undermines trust in these devices and raises urgent questions about the security assurances of cold storage solutions, affecting all crypto users who rely on them. Coldcard is a Bitcoin-only hardware wallet made by Coinkite since 2017, featuring dual secure elements and air-gapped signing. The exact nature of the bug has not been disclosed in the brief report, but it allowed attackers to drain funds despite the wallet's offline design.

rss · TechCrunch · Aug 4, 16:27

**Background**: A hardware wallet is a physical device that stores cryptocurrency private keys in an offline environment, protecting them from online hacking attempts such as phishing or malware. Coldcard is a Bitcoin-only hardware wallet known for its verifiable source code and air-gapped signing capabilities, which allow transactions to be signed without connecting to a computer. The promise of such devices is that even if a computer is compromised, the private keys remain safe. However, this incident shows that hardware wallets can still contain software bugs that undermine those protections.

<details><summary>References</summary>
<ul>
<li><a href="https://coldcard.com/">COLDCARD - Bitcoin-Only Hardware Wallet</a></li>
<li><a href="https://bitcoin.org/en/wallets/hardware/coldcard/">Coldcard - Hardware - Choose your wallet - Bitcoin</a></li>

</ul>
</details>

**Tags**: `#security`, `#cryptocurrency`, `#hardware wallet`, `#vulnerability`, `#cybersecurity`

---

<a id="item-2"></a>
## [Mistral releases Shieldstral, a 3B open-weights multimodal moderation model](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral has released Shieldstral, a 3B open-weights multimodal safety classifier for content moderation. The model frames moderation as a policy-adaptive question-answering task and reportedly outperforms models up to 7x its size. Shieldstral addresses a concrete need for affordable, adaptable content moderation in the AI ecosystem. Its open-weights nature allows developers to run and fine-tune it themselves, potentially reducing reliance on closed moderation APIs. The 3B model supports prompt moderation, response moderation, prompt-response pair classification, refusal detection, and safety filtering for text and image inputs. It is available on Hugging Face as Shieldstral-1.0-3B, though like most AI classifiers it is non-deterministic and best used as a first-pass filter with human review.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**Background**: An open-weights model publicly releases its trained parameters, letting anyone download, run, study, or modify it. Multimodal content moderation uses AI to analyze multiple input types—such as text and images—to detect harmful content like hate, violence, or explicit material, which is increasingly important for social platforms and AI services.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.clarifai.com/blog/the-future-of-content-how-multimodal-moderation-is-changing-the-game">How Multimodal Moderation is Shaping the Future of Content</a></li>

</ul>
</details>

**Discussion**: Commenters responded positively, calling Shieldstral a realistic and cost-effective solution for small platforms. They showed interest in whether it supports arbitrary rulesets without retraining, compared it with OpenAI's Omni Moderation, and suggested a human-review pipeline as a practical safeguard.

**Tags**: `#AI`, `#content-moderation`, `#open-source`, `#Mistral`, `#multimodal`

---

<a id="item-3"></a>
## [DeepSeek V4 Flash Runs on Single AMD MI300X at 150+ Tokens/s](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

A developer ported DeepSeek V4 Flash, a 284B-parameter Mixture-of-Experts model, to run on a single AMD MI300X accelerator, achieving over 150 tokens per second with a 256k-token context window. The port intentionally trades the model's original 1M context for accessibility on one GPU. This demonstrates that frontier-class open-weights models can be served on a single, widely discussed AI accelerator instead of requiring a multi-GPU cluster, lowering hardware barriers for inference. It also highlights how quantization and context-window tradeoffs shape practical deployment choices in the industry. DeepSeek V4 Flash has 284B total parameters with 13B activated and natively supports a 1M-token context; the single-MI300X build keeps full intended inference weights and solves for 256k context. The MI300X's 192GB HBM3 memory is the key enabler, though the part ships as an OAM module typically sold in 8-GPU boards.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**Background**: DeepSeek V4 Flash is an efficiency-optimized preview of the DeepSeek V4 series, a Mixture-of-Experts model from DeepSeek designed for efficient reasoning across a 1M-token context. AMD Instinct MI300X is a data-center GPU with 304 compute units and 192GB of HBM3 memory, aimed at large-model inference. Quantization reduces the precision of model weights so they fit in a smaller memory footprint, which is part of what makes single-GPU inference of such large models possible.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash">DeepSeek V 4 Flash - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html">AMD Instinct™ MI300X Accelerators</a></li>

</ul>
</details>

**Discussion**: Commenters were generally positive but raised hardware-access concerns: majke notes a single MI300X isn't sold standalone and the 8-GPU system costs around 250K EUR, while Tepix suggests the PCIe-based MI350P with 144GB could be a better fit. WhitneyLand frames the port as a practical tradeoff, since inference quality and speed are preserved and only the context window drops from 1M to 256k. GTP adds that an alternative project called DwarfStar was not cited and can run the same model in less memory.

**Tags**: `#deepseek`, `#mi300x`, `#ai-inference`, `#quantization`, `#hardware`

---

<a id="item-4"></a>
## [Troy Hunt: FedEx Emails Train Users to Accept Phishing](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 8.0/10

In a 2024 blog post, security researcher Troy Hunt demonstrates how legitimate FedEx emails closely resemble phishing attempts, arguing that this 'cry wolf' effect trains users to ignore warning signs. He provides practical examples of such emails to illustrate the problem. This matters because legitimate companies are undermining users' ability to spot real phishing attacks, making people more susceptible to cybercrime. The issue affects anyone receiving such emails and can confuse even security-aware users, as shown by the community discussion. The article provides practical examples of FedEx notifications containing classic phishing red flags, such as unexpected sender names, plain-text links, or requests for personal details. These examples illustrate that even when authentication protocols like SPF and DMARC are correctly implemented, an email's content can still look deceptive.

hackernews · stymaar · Aug 4, 21:09 · [Discussion](https://news.ycombinator.com/item?id=49175192)

**Background**: Phishing is a form of cyberattack where criminals send emails that mimic trusted companies to trick recipients into revealing sensitive information. Email authentication standards such as SPF (Sender Policy Framework) and DMARC (Domain-based Message Authentication, Reporting & Conformance) help verify that messages originate from authorized servers, but they do not prevent legitimate companies from sending careless or confusing messages. When companies like FedEx send such emails, they inadvertently train users to ignore the red flags that usually indicate phishing, a phenomenon security experts call the 'cry wolf' effect.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMARC">DMARC - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Sender_Policy_Framework">Sender Policy Framework - Wikipedia</a></li>
<li><a href="https://dmarc.org/">dmarc.org – Domain Message Authentication Reporting & Conformance</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion expresses strong agreement with the article, with commenters sharing personal experiences of confusing legitimate emails from FedEx, Google, and the IRS. Several also point to systemic issues like the proliferation of new top-level domains and the use of similar text-to-speech systems in call centers, which further blur the line between legitimate and malicious communications.

**Tags**: `#phishing`, `#security`, `#email`, `#user-awareness`, `#FedEx`

---

<a id="item-5"></a>
## [Oxide Computer Raises $445M in Series D Round](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 8.0/10

Oxide Computer Company has raised $445 million in a Series D round, as disclosed in an SEC Form D filing. The new round follows a $200 million Series C announced on February 10, 2026, bringing Oxide's total disclosed funding to approximately $789 million. This significant funding round underscores investor confidence in Oxide's vision of replacing traditional enterprise servers with purpose-built, on-premises cloud infrastructure. It also reflects a broader trend where companies are seeking alternatives to public cloud and legacy hypervisor licensing, potentially putting competitive pressure on incumbents like AWS and VMware. The Form D filing does not list a lead investor or valuation, but the $445 million raise is one of the largest ever for an infrastructure hardware startup. Oxide's Series C was led by Thomas Tull's US Innovative Technology Fund (USIT), with backing from Eclipse, Riot Ventures, and other existing investors.

hackernews · depr · Aug 4, 20:13 · [Discussion](https://news.ycombinator.com/item?id=49174407)

**Background**: Oxide Computer Company, based in Emeryville, California, builds rack-scale systems that integrate compute, storage, and networking into a single appliance with co-designed open-source software. Its goal is to make on-premises infrastructure as easy to operate as a public cloud, eliminating separate hypervisor licenses and reducing power, cooling, and management overhead. A Form D is a brief notice that companies file with the SEC for private securities offerings under Regulation D, providing basic offering details rather than full audited financials.

<details><summary>References</summary>
<ul>
<li><a href="https://www.intelcapital.com/oxide-closes-200m-series-c-to-scale-on-premises-cloud-computing/">Oxide Closes $200M Series C to Scale On-Premises Cloud Computing – Intel Capital</a></li>
<li><a href="https://en.wikipedia.org/wiki/Form_D">Form D - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/company/oxidecomputer">Oxide Computer Company | LinkedIn</a></li>

</ul>
</details>

**Discussion**: Community reactions are broadly enthusiastic, with one user praising the rapid funding progression and the founders' technical storytelling. However, a VP of Engineering at a company spending $900K/year on AWS said Oxide ignored their sales inquiry, and another commenter questioned whether Oxide has actually shipped hardware to customers. Still, several users expressed strong trust in the team, particularly given Jessie Frazelle's involvement.

**Tags**: `#funding`, `#hardware`, `#startup`, `#infrastructure`, `#oxide-computer`

---

<a id="item-6"></a>
## [Chinese startup XinXiao cuts chip power sign-off from weeks to days](https://36kr.com/p/3925067918227591?f=rss) ⭐️ 8.0/10

Shanghai-based EDA startup XinXiao Technology has launched IcPower, its first digital power sign-off tool based on distributed matrix solving. In typical test cases, IcPower runs 4.5-8.5x faster than foreign vendors' tools, shortening a full power sign-off cycle from weeks to days. Power sign-off is the final gate before tape-out, so faster analysis directly shortens delivery cycles for advanced-node chips. It also strengthens the domestic EDA ecosystem amid the push for local substitution in China's semiconductor industry. The tool is based on domain decomposition: graph-based partitioning splits a sparse matrix with billions of unknowns into smaller submatrices, while optimized communication and numerical stability controls keep distributed results mathematically consistent with single-machine high-precision solvers. IcPower targets 10-billion-gate chips, covers CPU, GPU, and autonomous-driving chip designs, and the company plans thermal and stress analysis products for 3DIC in the second half of 2026.

rss · 36氪 · Aug 4, 10:27

**Background**: Power sign-off analyzes the entire power delivery network of a chip—often billions of nodes—for voltage drop, power consumption, and electromigration, which is equivalent to solving a sparse matrix equation with hundreds of millions of dimensions. As process nodes shrink and transistor counts grow exponentially, a full sign-off run can take weeks. The global EDA market is dominated by Synopsys, Cadence, and Siemens EDA, which hold about 74% of the market, so Chinese startups are targeting niche areas like power sign-off during the domestic-substitution wave.

<details><summary>References</summary>
<ul>
<li><a href="https://ask.csdn.net/questions/8999578">如何高效 求 解 大规模 稀 疏 矩 阵 方 程 ？_ 编 程 语言-CSDN问答</a></li>
<li><a href="https://juejin.cn/post/7288998044020293647">稀 疏 矩 阵 解 析：C++ 实现指南1. 引言 (Introduction)...</a></li>
<li><a href="https://www.semi.org.cn/site/semi/article/68f57c1b8188401fa071cb1c557b668a.html">雷娜科技破局“ EDA ...” - SEMI大半导体产业网</a></li>

</ul>
</details>

**Tags**: `#EDA`, `#芯片设计`, `#分布式计算`, `#电源签核`, `#半导体`

---

<a id="item-7"></a>
## [SpaceX and Nvidia Team Up to Put Data-Center AI Compute in Orbit](https://36kr.com/newsflashes/3925833212230023?f=rss) ⭐️ 8.0/10

On August 5, SpaceX and Nvidia announced a partnership to develop the Starmind AI1 satellite computing payload, with each satellite equipped with Nvidia's Rubin GPU and Vera CPU. The collaboration aims to deliver data-center-level AI compute to orbit. This marks the first major move to put data-center-class AI chips into satellite form, potentially enabling real-time on-orbit AI inference and reducing dependence on ground stations. It could reshape satellite computing, remote sensing, and AI infrastructure as space becomes the next frontier for compute. The payload pairs Nvidia's next-generation Rubin GPU, the successor to its Blackwell data-center platform, with the Vera CPU, a high-performance processor designed for agentic AI workloads. No specific figures on power, cooling, launch schedule, or radiation hardening were disclosed in the announcement.

rss · 36氪 · Aug 4, 23:38

**Background**: Nvidia Rubin is Nvidia's next-generation GPU architecture for AI training and inference, built for extreme bandwidth and scalability in data centers. Vera is Nvidia's new data-center CPU, leveraging Olympus cores to deliver higher performance on agentic and AI workloads. Traditional satellites rely on radiation-hardened, low-power chips, so placing full data-center AI compute in orbit requires solving major challenges in power, thermal management, and radiation tolerance. This announcement signals Nvidia's push to extend its AI computing platform beyond terrestrial data centers.

<details><summary>References</summary>
<ul>
<li><a href="https://digg.com/tech/b0pmfjo9">SpaceX Partners With Nvidia on Starmind AI Satellite Payload · Digg</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/vera-cpu/">Next Gen Data Center CPU | NVIDIA Vera CPU</a></li>
<li><a href="https://servers.asus.com/glossary/What-is-NVIDIA-Rubin-GPU">What is NVIDIA Rubin GPU ? | ASUS Servers</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Nvidia`, `#Satellite Computing`, `#AI Infrastructure`, `#Space Technology`

---

<a id="item-8"></a>
## [Samsung Unveils AI Memory Roadmap with zHBM and 400+ Layer V10 NAND](https://36kr.com/newsflashes/3925818953414792?f=rss) ⭐️ 8.0/10

At FMS 2026, Samsung introduced its next-generation AI memory roadmap, unveiling zHBM and zNAND-O concept products and a V10 BV-NAND prototype with over 400 layers using wafer bonding. The company said zHBM could deliver roughly 8x the performance and more than 10x the memory density of HBM5. This roadmap addresses the growing memory bottleneck in AI infrastructure, where feeding data fast enough to accelerators has become as critical as compute power. If realized, zHBM and 400+ layer NAND could significantly improve AI training/inference performance and energy efficiency, reinforcing Samsung's competitive position in AI memory. zHBM stacks HBM vertically above AI accelerators to shorten data paths, while V10 BV-NAND uses wafer bonding to achieve over 400 layers. The zHBM and zNAND-O are concept products, not yet on the market; zNAND-O is aimed at edge AI systems that need low-latency on-device storage.

rss · 36氪 · Aug 4, 23:26

**Background**: High Bandwidth Memory (HBM) stacks DRAM dies vertically beside a processor to provide a very wide, short data pipe, addressing the bandwidth limits of AI workloads. V-NAND (vertical NAND) stacks memory cells in 3D to increase density; wafer bonding is a technique that attaches a memory array wafer to a peripheral circuitry wafer, potentially improving performance and density. The FMS event is where major memory makers showcase their future storage and memory roadmaps.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flash_memory">Flash memory - Wikipedia</a></li>
<li><a href="https://read.siliconandsteel.co/p/the-real-ai-shortage-is-memory">The Real AI Shortage Is Memory</a></li>
<li><a href="https://www.devdiscourse.com/article/technology/3959605-samsung-electronics-launches-next-generation-ai-memory-technology">Samsung Electronics launches next-generation AI memory technology</a></li>

</ul>
</details>

**Tags**: `#AI memory`, `#HBM`, `#NAND`, `#AI infrastructure`, `#Samsung`

---

<a id="item-9"></a>
## [EFF warns Android apps may leak location data via third-party code](https://techcrunch.com/2026/08/04/android-app-developers-may-be-unwittingly-sharing-their-users-location-data-with-advertisers/) ⭐️ 8.0/10

The Electronic Frontier Foundation (EFF) published new findings warning Android developers that third-party code embedded in their apps may unintentionally collect and share users' location data. The report, surfaced on August 4, 2026, highlights a privacy risk that occurs when apps have been granted location permission. This matters because millions of Android users could have their location data silently shared with advertisers without their knowledge. It also signals that developers must carefully audit third-party dependencies to avoid violating user privacy expectations and potentially facing regulatory consequences. The issue arises when a user grants location permission to an app, and third-party libraries or SDKs bundled in the app use that permission to access and transmit location data. The EFF's goal is to educate developers about this behavior so they can vet their dependencies and reduce inadvertent data sharing.

rss · TechCrunch · Aug 4, 20:26

**Background**: The Electronic Frontier Foundation (EFF) is a non-profit digital rights group founded in 1990 that defends civil liberties online, including privacy and free expression. In Android development, third-party libraries are pre-built code components used to add features easily, but they inherit the permissions granted to the host app, which can lead to unexpected data collection and sharing. The Android permission system gives users control, yet developers are ultimately responsible for how all code in their apps—including third-party code—handles sensitive data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Electronic_Frontier_Foundation">Electronic Frontier Foundation</a></li>
<li><a href="https://medium.com/@mansikothari115/10-essential-third-party-libraries-in-android-794965601dd8">10 Essential Third - Party Libraries in Android | by Mansi Shah | Medium</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#Android`, `#location data`, `#third-party libraries`, `#EFF`

---

<a id="item-10"></a>
## [Open-weight AI Models Approach Frontier; Safety Gap Persists](https://techcrunch.com/2026/08/04/open-weight-ai-models-are-catching-up-to-the-frontier-the-safety-gap-remains/) ⭐️ 8.0/10

A SaferAI report finds that Z.ai's open-weight model GLM-5.2 is approaching frontier AI capability but lacks key safety mitigations. The report renews concerns about powerful open models outpacing governance and safeguards. This matters because open-weight models can be downloaded and customized by anyone, making advanced capabilities widely accessible without proportional oversight. It highlights a widening gap between AI capability growth and safety governance, affecting developers, enterprises, and policymakers. According to SaferAI, GLM-5.2 reaches near-frontier performance while missing required safety mitigations, raising the risk of misuse. The model supports a 1M-token context window and is designed for long-horizon agent workflows and project-level software engineering.

rss · TechCrunch · Aug 4, 20:05

**Background**: Open-weight AI models release the trained weights so users can download and customize them, but they are not fully open-source. Frontier AI refers to the most capable models available at a given time. SaferAI's report uses GLM-5.2 as a concrete example of how open models can gain advanced capabilities faster than safeguards are developed.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM - 5 . 2 - Overview - Z . AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.2">zai -org/ GLM - 5 . 2 · Hugging Face</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#open-weight models`, `#AI governance`, `#frontier AI`, `#GLM`

---

<a id="item-11"></a>
## [Anthropic signs $10B deal with AI cloud startup Volta](https://techcrunch.com/2026/08/04/anthropic-signs-10-billion-deal-with-ai-cloud-startup-volta/) ⭐️ 8.0/10

Anthropic reportedly signs a $10 billion partnership deal with AI cloud startup Volta.

rss · TechCrunch · Aug 4, 19:48

**Tags**: `#Anthropic`, `#AI Cloud`, `#Volta`, `#Partnership`, `#Business`

---

<a id="item-12"></a>
## [AI fuels over half of Africa's cybercrime as scams surge, Interpol reports](https://www.africanews.com/2026/08/04/ai-fuels-more-than-half-of-cybercrime-in-africa-as-digital-scams-surge-interpol/) ⭐️ 7.0/10

An Interpol report finds that AI is used in more than half of cybercrime cases in Africa, fueling a surge in digital scams. The report highlights how generative AI tools make fraud more convincing and scalable across the continent. The finding signals that AI-powered cybercrime is no longer a niche concern but a mainstream threat in emerging markets. Governments, businesses, and individuals across Africa will need stronger AI-driven defenses and coordinated law enforcement to counter scams. The report is the Interpol African Cyberthreat Assessment Report 2026, published on interpol.int. It attributes much of the increase to AI-generated phishing messages, deepfakes, and automated social engineering, though exact statistics beyond 'more than half' are not detailed in the article.

hackernews · bookofjoe · Aug 4, 22:01 · [Discussion](https://news.ycombinator.com/item?id=49175826)

**Background**: Interpol is the International Criminal Police Organization, which coordinates law enforcement cooperation across 196 member countries. Its regional reports assess cybercrime trends and help national police prioritize threats. AI tools can now write convincing scam messages, generate fake documents, and create realistic deepfake voices and videos, lowering the barrier for criminals. In Africa, rapid internet and mobile-money adoption has created both economic opportunity and a large pool of potential scam victims.

**Discussion**: Commenters generally agreed that AI makes scams more believable, but several argued that internet access, mobile phones, and social media are the real underlying drivers. One user running a SaaS said AI bots were overwhelming and that Cloudflare was essential, while another called AI a double-edged sword for defense. A few expressed skepticism about AI hype or surprise that the proportion was only half.

**Tags**: `#cybersecurity`, `#AI`, `#fraud`, `#Interpol`, `#Africa`

---

<a id="item-13"></a>
## [Simple algorithm and color space for generating diverse skin tones](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

A developer shared an interactive web project introducing a custom color space and a procedural generation algorithm for generating diverse, plausible skin tones. The project includes a color picker, several demos, and detailed explanations of the math behind it. This offers digital artists and game developers a practical tool for creating more inclusive skin tone palettes. The strong community engagement also highlights the demand for better tools and standards in skin tone representation in computer graphics. The color space appears to be derived from a 2D PCA-like projection of skin tone data, with a manually curve-fitted ellipse to define the valid region. Commenters note that the methodology lacks references to existing standards such as Pantone SkinTones, and that some sampled colors appear green or blue under certain conditions.

hackernews · automatoney · Aug 4, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49170165)

**Background**: A color space is a specific organization of colors, usually as a 3D coordinate system that maps numeric tuples to perceptual colors. Procedural generation is a method of creating data algorithmically rather than manually, commonly used in games and digital art to automatically produce textures, models, and palettes. Skin tones are particularly complex because they depend not only on physical skin pigments but also on lighting and human perception, making them difficult to model accurately.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Color_space">Color space</a></li>
<li><a href="https://en.wikipedia.org/wiki/Procedural_generation">Procedural generation</a></li>

</ul>
</details>

**Discussion**: Comments are largely positive, praising the author's creativity and the elegance of the hand-fitted function approach. Several commenters add useful context, such as the crescent shape also appearing in Oklab plotting of makeup shades, while others raise concerns about a lack of citations to existing skin tone standards and the presence of occasional unnatural colors.

**Tags**: `#color-space`, `#procedural-generation`, `#digital-art`, `#computer-graphics`, `#skin-tones`

---

<a id="item-14"></a>
## [Automakers Roll Out Own Battery Brands to Challenge CATL](https://36kr.com/p/3925382191708552?f=rss) ⭐️ 7.0/10

Xiaomi, Li Auto, and Huawei-backed Hongmeng Zhixing have each launched their own battery brands—Dragon Armor (龙甲电池), Li-branded, and Giant Whale (巨鲸电池) respectively—taking direct control over cell-to-pack development through "penetrating management." Xiaomi officially unveiled its Dragon Armor battery system on July 30, signaling a shift from buying turnkey packs from suppliers like CATL to automaker-led definition of battery standards. As batteries account for roughly 30% of an electric vehicle's cost, automakers gaining full-process control over battery development strengthens supply-chain stability and long-term cost leverage. This trend directly challenges CATL's market dominance and shifts the competitive battlefield from raw cell specifications to production consistency and BMS integration. CATL's key moat is production consistency, built on enormous output volumes that enable effective screening and iterative improvement; automaker-built lines and second-tier cell makers struggle to match it quickly. Automakers try to compensate with extra screening steps such as four-pass degaussing/ceramics removal, additional voltage-drop tests, and X-ray inspection, while CATL remains reluctant to open full pack design details to carmakers.

rss · 36氪 · Aug 4, 15:46

**Background**: Power batteries are the "heart" of electric vehicles; historically, dominant suppliers like CATL provided system-level "gray-box" solutions in which cell chemistry and manufacturing details stayed with the battery maker. Automakers have begun vertically integrating through self-owned battery brands, defining technical standards and quality control themselves—a strategy known as "penetrating management" (穿透式管理). This reflects a broader industry push where carmakers aim to reduce reliance on key suppliers and secure long-term cost and supply advantages.

<details><summary>References</summary>
<ul>
<li><a href="https://nev.ofweek.com/2021-12/ART-77012-8500-30539788.html">车企为何布局动力电池供应链？ - OFweek新能源汽车网</a></li>
<li><a href="https://finance.sina.com.cn/tech/roll/2022-07-22/doc-imizirav4988938.shtml">车企造电池，需要过三关|车企|电池_新浪科技_新浪网</a></li>
<li><a href="https://chejiahao.autohome.com.cn/info/26123727">小 米 龙 甲 电 池 ，凭什么姓「MI」？_ 车家号_发现车生活_汽车之家</a></li>

</ul>
</details>

**Tags**: `#EV batteries`, `#CATL`, `#supply chain`, `#automotive industry`, `#vertical integration`

---

<a id="item-15"></a>
## [Kimi K3与DeepSeek V4之间，隔着原生多模态的时间差](https://36kr.com/p/3924826666301831?f=rss) ⭐️ 7.0/10

The article analyzes how Kimi K3's native multimodal ability enables 'vision in the loop' for coding and agent tasks, distinguishing it from models like DeepSeek V4 and highlighting a broader industry shift toward integrating visual feedback into AI workflows.

rss · 36氪 · Aug 4, 06:32

**Tags**: `#AI`, `#large language models`, `#multimodal`, `#coding agents`, `#Kimi K3`

---

<a id="item-16"></a>
## [Apple Asks Judge to Halt OpenAI's Use of Stolen Trade Secrets](https://36kr.com/newsflashes/3925832206743942?f=rss) ⭐️ 7.0/10

Apple has asked a federal judge to immediately prohibit OpenAI from using trade secrets that Apple claims were stolen, and to return all confidential information while the litigation is ongoing. This legal dispute between two major tech companies could influence how AI firms handle confidential product information and set a precedent for trade secret protection in the AI industry. It may also affect their business relationship and future collaboration. Apple is seeking a court order that remains effective for the duration of the lawsuit, requiring OpenAI to return all confidential material and refrain from attempting to obtain further non-public information. This request follows Apple's earlier accusation that OpenAI systematically stole information about its upcoming products.

rss · 36氪 · Aug 4, 23:40

**Background**: Trade secrets are confidential business information that provides a competitive edge, such as product plans, algorithms, or customer data. Companies typically protect them through non-disclosure agreements and internal policies; when disputes arise, courts can issue injunctions to stop ongoing misuse while a case is being decided. Apple and OpenAI have overlapping interests in AI-related markets, making allegations of information misappropriation legally and commercially significant.

**Tags**: `#Apple`, `#OpenAI`, `#trade secrets`, `#legal`, `#AI`

---

<a id="item-17"></a>
## [Waymo Opens Dallas Robotaxi Service to All](https://techcrunch.com/2026/08/04/waymo-opens-up-robotaxi-service-in-dallas-to-everyone/) ⭐️ 7.0/10

Waymo has removed the waitlist for its robotaxi service in Dallas, making rides available to the general public. The move is part of the company's broader expansion across the U.S., U.K., and Europe. Opening a major metro without a waitlist marks a commercial milestone for autonomous ride-hailing, signaling Waymo's confidence in scaling its technology. It could intensify competition with human-driven ride-hailing services and accelerate adoption of self-driving transport. Dallas-Fort Worth is one of the largest, most car-dependent metroplexes in the U.S., posing a demanding test for autonomous vehicles. Waymo says the service is now available to everyone in the area, as part of its expansion strategy across the U.S., U.K., and Europe.

rss · TechCrunch · Aug 4, 17:31

**Background**: Waymo is a self-driving technology company that operates robotaxi services in several U.S. cities. 'Robotaxi' refers to autonomous ride-hailing vehicles that operate without a human driver. Many such services initially use a waitlist to gradually expand from an early rider program to full public access; dropping the waitlist in Dallas signals a step toward mainstream commercialization of autonomous driving.

**Discussion**: Commenters were largely positive, with one praising Waymo cars as very good road participants and another noting they cause fewer incidents than human drivers and quickly become normalized. Concerns included economic leakage for local drivers, while others highlighted driverless cars as affordable housing policy and welcomed the service in car-centric DFW.

**Tags**: `#autonomous-vehicles`, `#Waymo`, `#robotaxi`, `#self-driving`, `#transportation`

---

<a id="item-18"></a>
## [Spotify partners with Merlin to expand AI remix and covers tool](https://techcrunch.com/2026/08/04/spotify-adds-merlin-to-its-ai-music-remix-and-covers-effort/) ⭐️ 7.0/10

Spotify announced that Merlin, which represents more than 30,000 independent labels and distributors, has joined Universal Music Group in supporting its paid AI-powered remix and covers product. The tool will let fans create AI-generated covers and remixes of participating artists' music while ensuring artists opt in, receive credit, and are compensated. This signals growing industry backing for AI-generated music and establishes a template for artist opt-in, credit, and compensation. Independent labels' participation broadens the catalog available for AI remixing and could influence how other platforms handle AI music licensing. The paid tool requires artists to opt in, receive credit, and be compensated. Merlin acts as a digital rights agency for independent labels and distributors rather than representing artists directly, so its backing brings a large independent catalog into the project.

rss · TechCrunch · Aug 4, 15:50

**Background**: Generative AI tools can create new remixes and cover versions of existing songs, raising questions about rights and royalties. Spotify first partnered with Universal Music Group on this product, and Merlin's involvement extends similar terms to the independent sector. Merlin negotiates premium licensing agreements for thousands of independent labels and distributors worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://merlinnetwork.org/">Merlin - Digital Music Licensing for Independent Music Companies</a></li>
<li><a href="https://news.skrew.ai/spotify-merlin-ai-remix-covers-partnership/">Spotify Grows AI Music Remix Effort With Merlin Deal</a></li>
<li><a href="https://jackrighteous.com/blogs/mont-real/spotify-universal-ai-remix-deal-explained">Spotify & Universal AI Remix Deal Explained – Jack Righteous</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Music`, `#Spotify`, `#Licensing`, `#Partnership`

---

<a id="item-19"></a>
## [Texas Halts New Data Center Approvals Amid Power Grid Strain, Governor Orders Audits](https://techcrunch.com/2026/08/04/texas-halts-new-data-centers-as-governor-calls-for-audits/) ⭐️ 7.0/10

Texas has halted approvals for new data centers as surging electricity demand strains the state's power grid. The governor has called for audits of grid planning and the approval process. This marks a major reversal for Texas, which had attracted data center investment with loose regulations and seemingly abundant power. The pause signals that power constraints are now a binding factor in U.S. data center expansion, affecting tech companies, developers, and energy policy. The halt specifically targets new data center approvals, while existing or under-construction projects may be unaffected. The governor's audit request will examine how grid capacity forecasts accounted for the rapid growth in large-scale power demand.

rss · TechCrunch · Aug 4, 15:42

**Background**: Data centers require enormous amounts of electricity for servers and cooling, and their rapid growth across Texas has collided with the limitations of the state's isolated electricity grid, operated by ERCOT. Texas's light-touch regulation had made it a top destination for cloud and AI infrastructure. This move reflects a broader trend where states are re-evaluating data center incentives and grid reliability.

**Tags**: `#data centers`, `#energy`, `#Texas`, `#infrastructure`, `#policy`

---

<a id="item-20"></a>
## [US AI Leaders Embrace Chinese Open-Weight Models, Challenge Closed-Source Safety Claims](https://www.scmp.com/news/us/article/3362974/us-ai-leaders-turn-chinese-open-weight-models-challenging-closed-source-safety-claims?utm_source=rss_feed) ⭐️ 7.0/10

Andrew Ng and other American AI leaders now publicly state that open-weight models are safer than closed-weight models, directly challenging the long-held position of US companies like Anthropic. This marks a notable shift in the AI safety discourse, with influential figures favoring openness over proprietary secrecy. This development could reshape the AI safety debate and influence regulatory policy, as it challenges the assumption that closed-source models are inherently safer. It also puts pressure on companies like OpenAI and Anthropic, whose business models rely on proprietary models being seen as more trustworthy than open alternatives. Andrew Ng, former head of Google Brain and former chief scientist at Baidu, made the remarks, adding weight to the open-weight camp. Open-weight models publicly release their trained parameters, or weights, allowing anyone to download and study them, which supporters argue enables better external auditing and red-teaming.

rss · SCMP · Aug 4, 16:08

**Background**: An open-weight model is an AI model whose core components, specifically the trained numerical parameters known as weights, are publicly released for anyone to download and use. Proponents of open-weight models argue that transparency enables rigorous benchmarking, evaluation, and red teaming, making AI systems safer than closed systems that rely on secrecy. This debate mirrors the broader open-source versus proprietary software conflict, but now extends to AI safety and security, with major implications for industry leaders and policymakers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/news/us/article/3362974/us-ai-leaders-turn-chinese-open-weight-models-challenging-closed-source-safety-claims">US AI leaders turn to Chinese open-weight models, challenging closed-source safety claims | South China Morning Post</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#open-source`, `#open-weight models`, `#AI policy`, `#Andrew Ng`

---

<a id="item-21"></a>
## [China's MiniMax restricts overseas use of open-source H3 video model](https://www.scmp.com/tech/tech-trends/article/3362951/chinas-minimax-curbs-overseas-access-new-ai-video-model-over-copyright-disputes?utm_source=rss_feed) ⭐️ 7.0/10

On Monday, Shanghai-based MiniMax released the weights of its H3 multimodal video model, but the license restricts free access in the US, EU, UK, and South Korea. The move reflects copyright disputes in generative video AI, limiting open access despite the open-source release. This highlights the growing tension between open-source AI distribution and copyright compliance, particularly for generative video models trained on potentially copyrighted content. Developers and researchers in the restricted markets may lose access to a cutting-edge model, affecting global AI innovation and cross-border accessibility. MiniMax H3 is a general-purpose multimodal model that understands text, images, video, and audio in a unified context, generating up to 15 seconds of 2K video at 24fps with native stereo sound. The licensing restriction applies to 'free access' in the US, EU, UK, and South Korea, though the exact terms were not fully detailed in the report.

rss · SCMP · Aug 4, 12:00

**Background**: Model weights are the learnable parameters within a machine learning model that encode the knowledge learned from training data; they are what makes an AI model function. MiniMax H3 is the company's latest open-weights multimodal generation model, designed to handle text, images, video, and audio together. Open-sourcing weights typically allows developers worldwide to use and build upon a model, but copyright concerns over training data can lead to geographic restrictions. The H3 license restricts free access in several major markets, illustrating how legal issues can affect open-source AI distribution.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and Modalities - MiniMax Research | MiniMax</a></li>
<li><a href="https://www.ultralytics.com/glossary/model-weights">What are Model Weights in AI ? | Ultralytics</a></li>
<li><a href="https://fal.ai/minimax-h3">MiniMax H3 - Open-Weights General-Purpose Multimodal Video Model | fal</a></li>

</ul>
</details>

**Tags**: `#AI`, `#video generation`, `#copyright`, `#licensing`, `#open-source`

---

<a id="item-22"></a>
## [Shenzhen-Based Mathematician Yurii Nesterov Wins Top Applied Maths Prize](https://www.scmp.com/news/china/science/article/3362465/shenzhen-based-ai-mathematician-yurii-nesterov-wins-top-prize-applied-maths?utm_source=rss_feed) ⭐️ 7.0/10

Russian-born Belgian mathematician Yurii Nesterov, renowned for his accelerated gradient algorithm that underpins modern AI, has won a leading prize in applied mathematics while based in Shenzhen. The award recognizes his foundational contributions to optimization theory. Nesterov's algorithm is a core building block of machine learning, significantly speeding up the training of deep neural networks and other AI models. The prize highlights how classical mathematical discoveries continue to drive the current AI boom and underscores the value of fundamental research in applied fields. Nesterov, described as a 'master of international algorithm design,' reached retirement age in 2023 and decided to continue his research in Shenzhen rather than stop working. His accelerated gradient method, first derived in 1983, improves the convergence rate of smooth convex optimization from O(1/k) to O(1/k^2) compared with standard gradient descent.

rss · SCMP · Aug 4, 09:00

**Background**: Gradient descent is a fundamental optimization method used to train machine learning models by minimizing a loss function. On large, high-dimensional problems, standard gradient descent can converge slowly, so researchers developed accelerated variants that add a 'momentum' term to speed up the process. Nesterov's accelerated gradient (NAG) is one of the most influential such methods and is now widely used in AI training. Nesterov momentum is commonly taught alongside stochastic gradient descent (SGD) in machine learning courses.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Yurii_Nesterov">Yurii Nesterov - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nesterov_accelerated_gradient">Nesterov accelerated gradient</a></li>
<li><a href="https://pages.cs.wisc.edu/~yudongchen/cs726_sp23/Lecture_9_10_accelerated_GD.pdf">Lecture 9–10: Accelerated Gradient Descent</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#optimization`, `#artificial-intelligence`, `#algorithms`, `#awards`

---

<a id="item-23"></a>
## [Glass Substrate Maker Xunlin Raises ¥200M Series B to Expand Capacity](https://36kr.com/p/3924953058605444?f=rss) ⭐️ 6.0/10

Xunlin Technology, a Chinese glass substrate manufacturer, announced a nearly 200 million yuan Series B round, its third financing in six months. New investors include Inno Fund, Qiancheng Capital, Hymson, Guangpu and Tongxin, with existing shareholders increasing their stakes; proceeds will go toward capacity expansion, packaging line construction, and process precision R&D. The funding lands amid an AI-driven substrate shortage, with FR-4 copper-clad laminate prices up over 270% and ABF substrate lead times stretching beyond six months. As organic substrates approach physical limits, this investment signals growing confidence that glass substrates will move from lab to mass production in AI packaging. Xunlin operates a full-process glass substrate factory in Tianjin with annual capacity of 300,000 square meters, covering cutting, thinning, TGV drilling, PVD metallization, plating, and patterning. Its products for Mini LED backlight, COB direct display, and MIP display modules have entered volume shipment, and the company claims industry-leading copper adhesion strength from its self-developed PVD technology and Cu-ABX alloy seed layer.

rss · 36氪 · Aug 4, 08:31

**Background**: Glass substrates are emerging as an alternative to organic packaging substrates because their coefficient of thermal expansion naturally matches silicon, and they offer lower dielectric loss and higher wiring density. The organic substrate supply chain is strained: ABF, the insulating film used in substrates that connect AI accelerator chips to circuit boards, is in acute shortage as AI chips require many more layers than traditional GPUs. Intel has announced mass production of glass core substrates, and TSMC's CoPoS pilot line is expected to go online this year, reflecting the industry shift toward glass-based packaging.

<details><summary>References</summary>
<ul>
<li><a href="https://pcbmake.com/glass-substrate/">Glass Substrate in Semiconductor Packaging : Pros and Cons</a></li>
<li><a href="https://www.techtimes.com/articles/321754/20260728/ai-supply-crisis-moves-upstream-advanced-packaging-becomes-binding-constraint.htm">AI Supply Crisis Moves Upstream: Advanced Packaging Becomes the...</a></li>
<li><a href="https://en.eeworld.com.cn/news/manufacture/eic702503.html">Behind the " CoPoS fever": AI forces semiconductor packaging into the.....</a></li>

</ul>
</details>

**Tags**: `#glass substrate`, `#semiconductor packaging`, `#AI hardware`, `#funding`, `#advanced packaging`

---

<a id="item-24"></a>
## [Precision Reducer Maker Taoshi Raises ¥100M+; Valuation Tops ¥1B](https://36kr.com/p/3924628805351811?f=rss) ⭐️ 6.0/10

Chinese precision reducer maker Taoshi Intelligent Technology completed a funding round of over 100 million yuan, pushing its valuation past 1 billion yuan. The round was joined by Guochuang Group, Haichuan Juyi, Hangzhou Zhongshen, and Xinzhi Capital, with funds going to R&D, capacity expansion, and robot-market growth. As humanoid robots move toward mass production, actuators (motors, reducers, ball screws) account for roughly 45% of robot cost, making precision reducers a key link in China's localization push. Taoshi's funding signals maturing supply chains for dexterous hands and humanoid components, impacting hardware suppliers and integrators. Taoshi's micro-enveloping worm gear reducer claims 40% smaller volume, ±0.5 arcmin precision, 1300 MPa tensile strength, and 10,000-hour service life versus conventional solutions. It has signed a 100,000-unit supply agreement for dexterous-hand joint modules and is expanding capacity from 500,000–700,000 modules to 1–1.5 million modules.

rss · 36氪 · Aug 4, 02:59

**Background**: A worm gear reducer transmits motion between perpendicular (90-degree) shafts, but traditional designs usually need a separate angle mechanism that adds size, weight, and precision loss. Enveloping worm designs, where the worm is generated by a plane that envelops it, engage multiple teeth at once and offer higher load capacity, efficiency, and service life than ordinary cylindrical worm gears. Taoshi combines this enveloping structure with an orthogonal right-angle layout and developed its own 7-axis, 5-link grinding process to miniaturize the reducer.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sgr.com.cn/id65484797.html">平面二次包络环面蜗杆传动研究进展 - 上海合纵重工机械有限公司</a></li>
<li><a href="http://www.geartoutiao.com/tech/3210">平面二次包络环面蜗杆传动研究进展 - 齿轮头条</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#humanoid-robots`, `#precision-reducer`, `#hardware`, `#investment`

---

<a id="item-25"></a>
## [Blackstone in Talks to Arrange $36B Debt for Anthropic AI Chips](https://36kr.com/newsflashes/3925373322574209?f=rss) ⭐️ 6.0/10

Blackstone has held preliminary talks with investors about arranging at least $36 billion in debt financing to fund Anthropic's use of Google chips. The potential deal follows Anthropic's confidential U.S. IPO filing and would exceed the $35 billion financing package that Apollo and Blackstone closed about two months ago. This shows AI companies are turning to large-scale debt markets to fund compute infrastructure as they race to scale models. If completed, the deal would strengthen Anthropic's compute capacity and support its push to reach public markets before rival OpenAI. The reported proposal involves at least $36 billion in debt, which would top the roughly $35 billion package Apollo Global Management and Blackstone finalized about two months ago. The financing is tied to Anthropic's use of chips from Alphabet's Google, and it comes after Anthropic confidentially submitted its IPO filing.

rss · 36氪 · Aug 4, 23:30

**Background**: Anthropic is an AI company best known for its Claude models and is a major competitor to OpenAI. Training and running advanced AI models requires huge amounts of specialized chips, often from Nvidia or Google's TPUs, making compute one of the largest costs for AI startups. Debt financing tied to chip purchases or infrastructure helps companies secure compute without diluting equity, and can be a step toward an IPO by strengthening balance sheets.

**Tags**: `#AI`, `#Anthropic`, `#Financing`, `#Chips`, `#IPO`

---

<a id="item-26"></a>
## [SpaceX doubles revenue on Anthropic, Google compute deals, Starlink growth](https://techcrunch.com/2026/08/04/spacex-doubles-revenues-on-anthropic-and-google-compute-deals-starlink-growth/) ⭐️ 6.0/10

SpaceX reported doubled year-over-year revenue in its first quarterly earnings since going public in June 2026, boosted by compute deals with Anthropic and Google and by Starlink growth. This underscores how AI compute demand is becoming a major revenue stream for infrastructure providers, even for a company traditionally known as a rocket and satellite firm. It also makes SpaceX's public-market performance increasingly tied to AI infrastructure contracts and Starlink's commercial success. According to background reports, Anthropic has a contract to pay SpaceXAI $1.25 billion per month for all compute capacity at the Colossus 1 data center, which contains 1 million GPUs. Google has paid SpaceXAI $920 million monthly for cloud compute capacity since June 2026, ahead of SpaceX's IPO.

rss · TechCrunch · Aug 4, 20:36

**Background**: AI compute deals involve leasing access to high-performance hardware such as GPUs needed to train large machine-learning models. SpaceX has built a massive supercomputer called Colossus with 1 million GPUs and now sells its capacity to AI companies. SpaceX went public in June 2026, and Starlink, its satellite internet service, continues to drive consumer and enterprise revenue growth.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Compute_(machine_learning)">Compute (machine learning) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#AI infrastructure`, `#Starlink`, `#cloud computing`, `#business news`

---

<a id="item-27"></a>
## [Nvidia's Open Secure AI Alliance Proposes AI-Agent Defenses Within a Week](https://techcrunch.com/2026/08/04/nvidia-doesnt-mess-around-a-week-after-open-ai-industry-group-formed-its-already-showing-progress/) ⭐️ 6.0/10

Within a week of its founding, the Open Secure AI Alliance (OSAIA), led by Nvidia and comprising over 120 companies, has already released initial proposals for defending against malicious AI agents. This rapid progress underscores the industry's growing urgency around AI agent security and positions Nvidia as a leader in open, multi-vendor AI defense frameworks. It could influence how enterprises and governments protect themselves against emerging autonomous threats. The alliance aims to provide entities with access to advanced open models, agent harnesses, and security tools that can be independently deployed and adapted, reducing dependence on any single provider. Notably, major AI labs such as OpenAI, Google, and Anthropic are reportedly absent from the alliance.

rss · TechCrunch · Aug 4, 19:28

**Background**: AI agents are autonomous systems that perform tasks with minimal human oversight, but they also introduce new security risks such as unauthorized actions or data leaks. The Open Secure AI Alliance (OSAIA), launched by Nvidia, aims to address these threats by providing open models, agent harnesses, and security tools that organizations can deploy and adapt independently. The alliance's rapid formation—a signature list becoming a founding roster within days—reflects urgency in the AI security community.

<details><summary>References</summary>
<ul>
<li><a href="https://supercrzy.com/news/the-open-secure-ai-alliance-is-a-direct-response-to-openais-rogue-agent-openai-isnt-invited">The Open Secure AI Alliance Is a Direct Response to... | SUPERCRZY</a></li>
<li><a href="https://spoonai.me/posts/2026-07-29-nvidia-open-secure-ai-alliance-jul2026-en">A Letter Became an Institution in Three Days — Nvidia's Open Secure ...</a></li>
<li><a href="https://tech.yahoo.com/ai/articles/openai-google-anthropic-absent-nvidia-190347277.html">OpenAI, Google, and Anthropic absent from Nvidia-led Open Secure ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#Nvidia`, `#industry group`

---

<a id="item-28"></a>
## [Chinese startup Spirit AI tops Nvidia on RoboArena, sparking manipulation accusations](https://www.scmp.com/tech/tech-war/article/3362923/has-chinese-physical-ai-start-manipulated-global-ranking-beat-nvidia?utm_source=rss_feed) ⭐️ 6.0/10

In June, Spirit AI, a Hangzhou-based startup founded in 2024, briefly took the top spot on the RoboArena physical AI benchmark with its Spirit v1.6 model, overtaking Nvidia's Cosmos 3. The achievement has sparked accusations that the company manipulated the ranking. This incident highlights the intense US-China competition in next-generation AI and the inherent challenges of evaluating physical AI systems. It raises questions about the credibility of benchmarking in robotics and autonomous systems, which are critical for investment and strategic decisions. Spirit AI scored 1,924 on RoboArena, narrowly beating Nvidia's Cosmos 3, which scored 1,881. The company's advantage reportedly came from a data strategy based on real-world interaction rather than simulated scale.

rss · SCMP · Aug 4, 10:30

**Background**: Physical AI refers to AI agents that interact with the physical world, such as robots and autonomous systems. RoboArena is a distributed, scalable benchmark designed to evaluate generalist robot policies in real-world environments. The ranking competition between China and the US is seen as a proxy for broader technological leadership.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/robo-arena/roboarena">GitHub - robo - arena / roboarena : Distributed, scalable benchmarking ...</a></li>
<li><a href="https://arxiv.org/pdf/2506.18123">RoboArena : Distributed Real-World Evaluation of Generalist Robot...</a></li>
<li><a href="https://thefrontrunners.io/article/roboarena-benchmark-spirit-ai-beats-nvidia">Hangzhou Startup Beat Nvidia on Its Own Benchmark Two Days After...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Robotics`, `#Benchmarking`, `#China`, `#Nvidia`

---