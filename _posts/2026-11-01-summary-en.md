---
layout: default
title: "Horizon Summary: 2026-11-01 (EN)"
date: 2026-11-01
lang: en
---

> From 87 items, 9 important content pieces were selected

---

1. [Jepsen Finds Severe Transactional Anomalies in ParticleDB 1.1.4, Urges Halt](#item-1) ⭐️ 9.0/10
2. [Linux kernel IPv4/TCP use-after-free CVE-2026-98432 rated CVSS 9.8](#item-2) ⭐️ 8.0/10
3. [Molly, the hardened Signal fork, is reportedly three months behind on security fixes](#item-3) ⭐️ 8.0/10
4. [Parameter Labs chains ChatGPT share-link bugs into account takeover](#item-4) ⭐️ 8.0/10
5. [Karpathy Launches HackerTube: A YouTube-Style UI Built From HN Recommendations](#item-5) ⭐️ 7.0/10
6. [FBI Attributes Record $6.3B Binance Hack to North Korea's TraderTraitor](#item-6) ⭐️ 7.0/10
7. [Apple Intelligence to Launch in China in December With Alibaba's Help](#item-7) ⭐️ 7.0/10
8. [Blog Post Argues Memory Latency, Not Compute, Is the Real Bottleneck](#item-8) ⭐️ 6.0/10
9. [China tests focused ultrasound to rouse brain-injury coma patients](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Jepsen Finds Severe Transactional Anomalies in ParticleDB 1.1.4, Urges Halt](https://jepsen.io/analyses/particledb-1.1.4) ⭐️ 9.0/10

Jepsen published a safety analysis of ParticleDB, a multi-model database marketed for AI-agent workloads and claiming Postgres compatibility, testing versions 1.1.4 through 1.1.18.11.rc-22. The report documents 96 issues, including routine loss of committed writes, internal consistency violations, G1a (Aborted Read), G1b (Intermediate Read), and P4 (Lost Update), and recommends that users halt deployment and migrate to other databases as soon as possible. A Jepsen teardown is one of the highest-signal events in the database world, and a recommendation to halt deployment is about as bad an outcome as a vendor can receive. It is a cautionary tale for teams adopting new AI-oriented databases on the strength of marketing claims about Postgres compatibility and 'formally proven' designs that turn out to be unverifiable. Jepsen notes that ParticleDB's homepage advertised a 'formally proven' TLA+ design, but no TLA+ specification was ever made available during the collaboration, so it is unclear what properties were proven or whether they describe the system as built. Beyond the isolation anomalies, the report lists odd failures such as partially invisible rows that could not be deleted, a WHERE 4 = 5 predicate, dropped tables re-emerging in distorted forms, and strings turning into integers.

hackernews · aphyr · Oct 31, 13:39 · [Discussion](https://news.ycombinator.com/item?id=50316100)

**Background**: Jepsen is a Clojure-based distributed systems testing framework created by Kyle Kingsbury (aphyr) that runs workloads against a database while injecting faults such as network partitions, process crashes, and clock skew, then checks the recorded operation history against consistency models using tools like the Elle transactional checker. Its published analyses have become the de facto standard for database safety auditing. The anomaly names G1a, G1b, and P4 come from the Adya isolation-model taxonomy, where G1a is reading data from an aborted transaction, G1b is reading an intermediate value written by an uncommitted transaction, and P4 is a lost update. TLA+ is Leslie Lamport's formal specification language for modelling and verifying concurrent and distributed systems, and writing an actual proof in it is a substantial, expert-intensive undertaking.

<details><summary>References</summary>
<ul>
<li><a href="https://jepsen.io/analyses/particledb-1.1.4">Jepsen: ParticleDB 1.1.4</a></li>
<li><a href="https://github.com/jepsen-io/jepsen">GitHub - jepsen-io/jepsen: A framework for distributed ... Jepsen · GitHub Analysis - Jepsen Testing Distributed Systems for Consistency and Partition ... Testing Distributed Systems | Curated list of resources on ... Testing distributed systems | Andi Skrgat</a></li>
<li><a href="https://en.wikipedia.org/wiki/TLA+">TLA+ - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters reacted with blunt disbelief, with one summarizing the report as 'brutal' and another joking that this is what happens when you 'vibecode a database.' A widely echoed framing distinguished software that is 'correct by construction' — where failures are local bugs — from software that is 'incorrect by construction' and only works through luck and carefully placed workarounds; several commenters also voiced skepticism about vendors claiming formal proofs that cannot be inspected, noting that AI can be quite effective at inserting such workarounds.

**Tags**: `#databases`, `#distributed-systems`, `#transactions`, `#consistency`, `#jepsen`

---

<a id="item-2"></a>
## [Linux kernel IPv4/TCP use-after-free CVE-2026-98432 rated CVSS 9.8](https://atlasum.net/blog/cve-2026-98432-linux-ipv4-tcp-uaf) ⭐️ 8.0/10

A use-after-free race condition in the Linux kernel's IPv4 TCP handshake path — specifically during SYNACK processing — has been assigned CVE-2026-98432 and a maximum-severity CVSS score of 9.8, affecting kernel versions 4.4 and later. At the time of posting, neither Ubuntu nor RHEL had shipped a fix, and the flaw drew 337 points and 158 comments on Hacker News. Because the flaw sits in the core TCP stack rather than an optional module, virtually any Linux server with a listening socket could be exposed, and a remote unauthenticated attacker sending crafted IPv4 TCP packets could potentially achieve code execution. The simultaneous patch gap at Ubuntu and RHEL — two of the most widely deployed server distributions — leaves a large share of production fleets waiting for remediation. Community analysis notes that MPTCP is not required (it is a generic use-after-free), that internet-wide exploitation is unlikely because most ISP routers drop packets carrying IP options, and that a successful exploit requires multiple CPU cores processing packets — so single-core systems or setups pinning packet processing to one core are not affected. Red Hat states that dropping IP-option packets yourself helps but is not a complete mitigation.

hackernews · oger · Oct 31, 19:16 · [Discussion](https://news.ycombinator.com/item?id=50319143)

**Background**: A use-after-free (CWE-416) bug occurs when a program frees a chunk of memory but keeps using the dangling pointer, letting an attacker influence what gets written there and potentially hijack control flow; in kernel space this can escalate to full system compromise. CVSS 9.8 is the highest band short of 10.0, typically indicating a network-reachable, low-complexity, unauthenticated issue with high confidentiality, integrity and availability impact. The affected code sits in the TCP handshake — the SYN/SYN-ACK exchange that opens every connection — which is why a listening socket alone can be enough to reach the buggy path.

<details><summary>References</summary>
<ul>
<li><a href="https://aws.amazon.com/security/security-bulletins/2026-160-aws/">CVE-2026-98432 - Linux kernel IPv4 TCP use-after-free ...</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-98432/">CVE-2026-98432: Linux Kernel Use-After-Free Vulnerability</a></li>
<li><a href="https://www.rescana.com/post/linux-kernel-tcp-cve-2026-98432-use-after-free-prepare-now">Linux Kernel CVE-2026-98432: Critical TCP Use-After-Free, No ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely focused on three things: annoyance that the title edit dropped the word "Linux" (making it unclear that BSD, macOS and Windows are unaffected), technical corrections about exploitability (MPTCP not required, IP-options filtering by ISP routers, multi-core requirement, dropping IP options as only partial mitigation), and frustration that Ubuntu and RHEL — heavily server-oriented distributions — had no patches yet. One user also asked for recommendations on CVE RSS feeds after noting this vulnerability never surfaced in their monitoring list.

**Tags**: `#linux-kernel`, `#security`, `#cve`, `#tcp-ip`, `#vulnerability`

---

<a id="item-3"></a>
## [Molly, the hardened Signal fork, is reportedly three months behind on security fixes](https://piefed.world/post/1503394) ⭐️ 8.0/10

A community report on Piefed/Hacker News claims that Molly, the security-hardened Signal fork for Android, has not shipped an update in roughly three months and is therefore missing recent upstream fixes. Commenters specifically point to the RingRTC 2.73.0-1 call-teardown fix (a hang-up/hot-mic issue) and Signal's blacklist of eight compromised eMudhra TLS intermediates as protections Molly users currently lack. Molly is popular among privacy-conscious and de-Googled Android users (including GrapheneOS circles) precisely because it adds encryption at rest, UnifiedPush and Tor support on top of Signal, so a stalled release cadence means a security-focused fork is quietly falling behind on the very fixes its users care about. The episode also highlights a structural risk of small volunteer-maintained forks that depend on tracking a fast-moving upstream codebase. Molly tracks Signal's source and connects to Signal's servers, so upstream changes such as Signal Android's new linked-device support for phones and tablets and its improved notification handling without Google Play services are only inherited when the fork ships a new build. In the discussion, developer lone-cloud released a stopgap fork called Polly (v8.19.2-6, based on Signal 8.19.2, arm64-only and Android 14+) containing the RingRTC fix and the eMudhra certificate blacklist, suggesting the missing patches are straightforward to backport.

hackernews · DeepLogin · Oct 31, 10:23 · [Discussion](https://news.ycombinator.com/item?id=50314666)

**Background**: Signal is an open-source encrypted messenger, and Molly is an independent Android fork that hardens it with passphrase encryption of the local message database (a feature Signal removed after Android introduced file-based encryption), a secure RAM wiper, automatic lock, unknown-contact blocking, and optional Tor and UnifiedPush support. Molly comes in two flavors: the standard build includes Google's proprietary components like Firebase Cloud Messaging, while Molly-FOSS strips them for a fully free and auditable app. Because forks must manually rebase onto each new Signal release, their security posture depends entirely on maintainers keeping pace with upstream.

<details><summary>References</summary>
<ul>
<li><a href="https://molly.im/">Molly - An improved Signal app</a></li>
<li><a href="https://github.com/mollyim/mollyim-android/releases">Releases · mollyim/mollyim-android - GitHub</a></li>
<li><a href="https://signal.org/blog/linked-devices-and-android-tablets/">Signal >> Blog >> More linked devices are on the...</a></li>

</ul>
</details>

**Discussion**: Commenters were largely pragmatic rather than alarmed: several noted that Signal's own Android app now supports linking a second phone or tablet, removing a main reason people chose Molly, and one corrected the misconception that the Signal APK from signal.org doesn't self-update (it does, often earlier than the Play Store). Others criticized Signal for refusing to support UnifiedPush or offer a Google-free build for F-Droid, while a counterpoint argued that Signal's rejection of third-party clients is a deliberate, pragmatic trade-off that has kept it secure and successful.

**Tags**: `#Signal`, `#security`, `#Android`, `#open-source`, `#privacy`

---

<a id="item-4"></a>
## [Parameter Labs chains ChatGPT share-link bugs into account takeover](https://www.parameter.ai/labs/we-found-a-gap-at-openai) ⭐️ 8.0/10

Security researchers at Parameter Labs disclosed a chain of web vulnerabilities that let a single public ChatGPT share link run JavaScript inside a logged-in victim's session, achieving cross-account takeover. The chain abused the MathLive math-input library's postMessage listener, which trusted messages from any origin, together with a ChatGPT Content Security Policy that allowed YouTube's oEmbed endpoint as a script host for a JSONP-style bypass. OpenAI fixed the issue on October 26, rated it P1, and paid a total bounty of $5,000. Account takeover on ChatGPT is high-impact because a session holds conversation history and any connected integrations, and the attack needed essentially nothing from the victim beyond clicking a shared link. The disclosure also spotlights how third-party components embedded in AI products — math renderers, video embeds, preview sandboxes — become the weak link in otherwise well-defended frontends, and it has reignited debate over whether OpenAI's bounty payouts match the blast radius. The exploit required the victim to click a link, and OpenAI stated that both of its frontends rejected the reported messages before the fix landed. The payout of $5,000 for a P1 cross-account session takeover was widely viewed as low relative to ChatGPT's user base, and commenters also flagged a separate reported issue allowing remote file-system access on machines that had started a "Work" chat in the ChatGPT desktop app.

hackernews · armcat · Oct 31, 10:30 · [Discussion](https://news.ycombinator.com/item?id=50314699)

**Background**: The attack is a textbook example of vulnerability chaining, in which several individually modest bugs combine into a serious compromise. postMessage is the browser API that lets an iframe and its parent page exchange data, and it is only safe when the receiver checks the sender's origin; MathLive did not, so a malicious page could push code into ChatGPT's context. Content Security Policy (CSP) restricts which hosts may serve scripts, and JSONP is an older cross-origin data-loading trick that works by loading a remote script — so allowing a trusted-looking host such as YouTube's oEmbed endpoint gave the researchers a way to load attacker-influenced script past the CSP.

<details><summary>References</summary>
<ul>
<li><a href="https://explainx.ai/blog/chatgpt-share-link-account-takeover-mathlive-postmessage-csp-youtube-jsonp-fixed-oct-26-2026">ChatGPT Account Takeover via Share Link: P1 Bug, $5,000 ...</a></li>
<li><a href="https://aiweekly.co/alerts/openai-patches-chatgpt-share-link-flaw-that-hijacked-sessions">OpenAI Patches ChatGPT Share-Link Flaw That Hijacked Sessions</a></li>
<li><a href="https://openai.com/index/bug-bounty-program/">Announcing OpenAI ’s Bug Bounty Program | OpenAI</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely critical of the $5,000 payout, arguing that such a small reward for a P1 account takeover discourages researchers from reporting future issues, with one calling it "a joke" given OpenAI's resources. Others linked a related report of remote file-system access in the ChatGPT desktop app and said the combination looks "pretty bad," while several readers complained that the writeup's explanation of the JSONP stage is unclear about what was actually bypassed.

**Tags**: `#security`, `#vulnerability-disclosure`, `#openai`, `#bug-bounty`, `#web-security`

---

<a id="item-5"></a>
## [Karpathy Launches HackerTube: A YouTube-Style UI Built From HN Recommendations](https://karpathy.bearblog.dev/hacker-tube/) ⭐️ 7.0/10

Andrej Karpathy released HackerTube (hackertube.org), a YouTube-like browsing interface built on top of 6,454 videos that were linked in 39,834 Hacker News comments dating back to 2007. Instead of an algorithmically ranked feed, the site surfaces videos that humans chose to share in a technical discussion forum. The project is a working counter-example to engagement-optimized recommendation feeds, showing that a human-curated corpus can be browsed without clickbait or attention traps. It matters both as a practical discovery tool for developers and as a design provocation about how much of the web's content routing is shaped by a handful of platform algorithms. The corpus is limited to videos someone bothered to link on Hacker News, so coverage is skewed toward technical talks, demos and long-form engineering content rather than general-interest material. Commenters noted the interface lacks a newest-to-oldest sort (easy to add), and the site's source is packaged as a downloadable zip with an agent-oriented DATA.md so others can fork it into different interfaces or feeds.

hackernews · karpathy · Oct 31, 19:56 · [Discussion](https://news.ycombinator.com/item?id=50319510)

**Background**: Hacker News is Y Combinator's long-running tech discussion site, where users routinely link to YouTube talks, conference presentations and engineering videos in comment threads. Mainstream platforms rank content to maximize watch time and engagement, which critics argue pushes clickbait and reduces serendipity. Karpathy is a well-known AI researcher and educator (a founding member of OpenAI and former director of AI at Tesla) known for teaching-focused projects such as nanoGPT and his 'Let's build GPT' video series.

**Discussion**: Commenters welcomed the absence of bait, with one calling the experience refreshing compared to YouTube and another praising it as '100% pure nerd content' free of influencers and clickbait. A recurring theme was that personalized feeds fail to surprise: several readers said what they actually want online is expansion of horizons and breadth of perspective, not more of what they already like. The author chimed in inviting people to fork the project, even handing the source zip to an AI coding agent to rebuild it however they wish.

**Tags**: `#content-curation`, `#recommender-systems`, `#hacker-news`, `#youtube`, `#open-source`

---

<a id="item-6"></a>
## [FBI Attributes Record $6.3B Binance Hack to North Korea's TraderTraitor](https://www.scmp.com/news/world/united-states-canada/article/3372858/fbi-blames-north-korea-stolen-billions-binance-biggest-hack-history) ⭐️ 7.0/10

In a statement released on Saturday, the FBI said this week's theft of more than US$6 billion in virtual assets from Binance — the largest cryptocurrency heist on record — was the work of TraderTraitor, the North Korean state-backed hacking group also blamed for the US$1.5 billion Bybit hack in February 2025. The bureau urged cryptocurrency exchanges, blockchain analytics companies and other industry players to block and flag the stolen funds as they move on-chain. The attribution confirms that a state actor pulled off the biggest crypto theft ever recorded, underscoring how stolen digital assets have become a major revenue channel for North Korea's sanctions-hit economy. It also puts fresh pressure on exchanges and analytics firms to enforce blocking and sanctions controls quickly, and raises hard questions about Binance's own security posture. According to reports, the funds were drained from Binance within minutes, and the FBI's alert asks exchanges, blockchain analytics firms and other intermediaries to block addresses tied to the theft rather than merely monitor them. TraderTraitor is tracked as a cluster within the broader Lazarus Group, and stolen funds from such operations are typically laundered through mixers, cross-chain bridges and over-the-counter brokers.

rss · SCMP · Oct 31, 23:49

**Background**: TraderTraitor is the name used by US authorities and threat-intelligence firms for a North Korean state-sponsored hacking cluster linked to the Lazarus Group, which has been accused of stealing billions in crypto over several years to fund Pyongyang's weapons programmes. Blockchain analytics companies such as Chainalysis and TRM Labs trace these flows on public ledgers and publish wallet addresses so exchanges can freeze or block them. The February 2025 Bybit breach, in which roughly US$1.5 billion was taken, was previously the largest known exchange hack and is now cited by the FBI as evidence that the same actors are escalating.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fbi.gov/investigate/cyber/alerts/2026/north-korea-responsible-for-6-billion-binance-attack">North Korea Responsible for $6 Billion+ Binance Attack — FBI</a></li>
<li><a href="https://www.firstpost.com/explainers/who-is-tradertraitor-north-korean-hackers-behind-6-3-billion-binance-hack-14056556.html">Who is TraderTraitor? North Korean hackers behind the $6.3 ...</a></li>
<li><a href="https://www.trmlabs.com/resources/blog/the-bybit-hack-following-north-koreas-largest-exploit">The Bybit Hack : Following North Korea’s Largest Exploit | TRM Labs</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#cryptocurrency`, `#North Korea`, `#state-sponsored hacking`, `#blockchain`

---

<a id="item-7"></a>
## [Apple Intelligence to Launch in China in December With Alibaba's Help](https://www.scmp.com/tech/big-tech/article/3372831/apple-intelligence-roll-out-iphones-china-december-alibaba-backing) ⭐️ 7.0/10

Apple will officially roll out Apple Intelligence to Chinese iPhone users in December alongside the iOS 27.3 update, following an open beta for developers that begins on November 4. The launch, made possible through a partnership with Alibaba Group, ends roughly two years of regulatory uncertainty dating back to Apple Intelligence's announcement in June 2024. China is Apple's second-largest market, and the absence of AI features there has put the iPhone at a disadvantage against domestic rivals such as Huawei and Xiaomi that ship heavily marketed on-device AI. The launch makes Apple the highest-profile foreign company to deliver generative AI in China under the country's approval regime, setting a template for how overseas tech firms may partner with local model providers. The Chinese version of Apple Intelligence is expected to rely on Alibaba's Qwen models, with Baidu technology also reported as part of the stack, rather than the ChatGPT integration used internationally. Apple had to register the service with China's cyberspace regulator before launch, and the localized feature set may differ from the global version because foreign generative AI services are not approved for direct use in the country.

rss · SCMP · Oct 31, 10:02

**Background**: Apple Intelligence is Apple's collection of AI features — including Writing Tools, notification summaries, a smarter Siri, Genmoji, Image Playground and ChatGPT integration — announced at WWDC in June 2024 and built into iOS 18 and later. It combines on-device processing with server-side models, and outside China it leans on OpenAI's ChatGPT for certain queries. China requires generative AI services offered to the public to be registered with the Cyberspace Administration of China and to use approved domestic models, which is why Apple needed a local partner such as Alibaba to bring the features to Chinese users.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>
<li><a href="https://www.digitaltrends.com/phones/china-approves-apple-intelligence-for-iphones-with-alibaba-baidu-emerging-as-partners/">China approves Apple Intelligence for iPhones, with Alibaba ...</a></li>
<li><a href="https://felloai.com/apple-intelligence-china/">Apple Intelligence in China: Powered by Alibaba's Qwen</a></li>

</ul>
</details>

**Tags**: `#Apple Intelligence`, `#China tech`, `#Alibaba`, `#AI regulation`, `#iOS`

---

<a id="item-8"></a>
## [Blog Post Argues Memory Latency, Not Compute, Is the Real Bottleneck](https://pivotlake.io/blog/its-the-memory-latency-stupid/) ⭐️ 6.0/10

A blog post titled "It's the memory latency, stupid" on pivotlake.io argues that memory latency — not raw compute throughput or memory bandwidth — is usually the dominant performance bottleneck, illustrated with performance-engineering examples drawn from the author's own query/analytics work. The post reached 122 points and 39 comments on Hacker News, where commenters both praised its coherence and questioned its novelty. Most performance reasoning defaults to roofline thinking about FLOPs and bandwidth, so reframing a workload as latency-bound changes which optimizations are worth pursuing — cache blocking, prefetching, reducing pointer-chasing, or restructuring data layout rather than adding vectorization or more bandwidth. This matters to anyone tuning databases, query engines, or latency-sensitive systems on modern CPUs where a DRAM miss costs hundreds of cycles. The article leans on profiling evidence such as flamegraphs and perf-style measurements to show where cycles are actually lost, and critics on Hacker News observed that the proposed fix closely resembles radix-partitioned or fixed two-level hierarchical aggregation already common in analytical databases. Commenters also noted the gains are incremental rather than order-of-magnitude, and questioned what the approach offers over existing engines like DuckDB and ClickHouse.

hackernews · ntur1337 · Oct 31, 18:38 · [Discussion](https://news.ycombinator.com/item?id=50318720)

**Background**: Memory latency is the time a CPU waits to retrieve data that is not in cache; a DRAM access costs roughly 60–100 nanoseconds (hundreds of cycles), while an L1 hit costs well under a nanosecond, so a latency-bound program spends most of its time stalled rather than computing. Bandwidth and latency are distinct limits: bandwidth caps total bytes moved per second, while latency caps how fast a dependent chain of accesses can proceed, which is why pointer chasing, hash lookups and joins suffer even when bandwidth is plentiful. Tools like Linux perf and flamegraphs visualize where those stalls accumulate, and the classic reference on the topic is a widely circulated 2007 talk/article on CPU and memory, which one commenter asked to have updated for 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://safari.ethz.ch/architecture/fall2018/lib/exe/fetch.php?media=onur-comparch-fall2018-lecture11a-memorylatency-afterlecture.pptx">Computer ArchitectureLecture 11a: Memory Latency , Energy, and...</a></li>
<li><a href="https://www.linkedin.com/posts/asmpt-semi-solutions_bandwidth-vs-latency-activity-7472105619978600448-I9Fm">Memory Monday: Bandwidth vs Latency in Memory ... | LinkedIn</a></li>
<li><a href="https://exanode.eu/wp-content/uploads/2017/04/D2.5.pdf">Report on the HPC application bottlenecks</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was skeptical about novelty: quotemstr called the technique "just radix-partitioned aggregation" and asked why the project exists when DuckDB and ClickHouse already do, while drivebyhooting described it as a clustered hashmap that is "still not orders of magnitude better." Others were more positive — boricj contrasted a message-passing, virtual-method-heavy codebase on a Cortex-A7 against hand-rolled inline-allocating containers and index-plus-generation object pools on a smaller MCU, and happyPersonR praised the flamegraphs while suggesting LLM agents could be used to inspect assembly and PMU counters.

**Tags**: `#memory-latency`, `#performance-engineering`, `#systems`, `#databases`, `#HN`

---

<a id="item-9"></a>
## [China tests focused ultrasound to rouse brain-injury coma patients](https://www.scmp.com/tech/tech-trends/article/3372779/china-joins-global-race-reawaken-brain-injury-patients-through-ultrasound-therapy) ⭐️ 6.0/10

A Chinese clinical trial reported that a patient who had been in a coma for three months after a brain haemorrhage regained the ability to speak, eat and walk with support after receiving focused ultrasound stimulation of deep brain regions. State broadcaster CCTV reported that 13 of 24 patients with chronic disorders of consciousness showed improved conscious behaviour, according to the South China Morning Post. If the results hold up, focused ultrasound could offer a non-invasive way to modulate deep brain circuits, a capability that currently requires implanted electrodes or is limited to shallow targets with TMS and tDCS. That would matter for the roughly large population of patients with prolonged disorders of consciousness, and it puts China into a global race in ultrasound neuromodulation alongside US and European groups. The report rests on state-media coverage rather than a peer-reviewed paper, so stimulation parameters, patient selection criteria, blinding and the durability of the gains remain unpublished. Focused ultrasound can transiently open the blood-brain barrier and has known safety questions, meaning larger sham-controlled trials will be needed before any clinical claims are treated as established.

rss · SCMP · Oct 31, 07:00

**Background**: Low-intensity focused ultrasound (LIFU, also called transcranial focused ultrasound) uses converging sound waves to reach structures deep inside the brain without surgery, offering better spatial precision than scalp-based electrical or magnetic stimulation. Depending on parameters, it modulates neural activity through mechanisms such as acoustic radiation force, cavitation and mild heating. The technology has been explored for depression, substance use disorder and disorders of consciousness, but most human evidence so far comes from small studies and individual case reports. The work described here involves a coalition including the Shenzhen Institutes of Advanced Technology under the Chinese Academy of Sciences.

<details><summary>References</summary>
<ul>
<li><a href="https://www.frontiersin.org/journals/psychiatry/articles/10.3389/fpsyt.2022.825802/full">Frontiers | Low Intensity Focused Ultrasound for Non-invasive and...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC13000543/">Low Intensity Focused Ultrasound Neuromodulation in ...</a></li>
<li><a href="https://www.nature.com/articles/s43586-024-00368-6">Low-intensity focused ultrasound for human neuromodulation A Comprehensive Review of Low-Intensity Focused Ultrasound ... Focused ultrasound reportedly got coma patient talking Progress in Noninvasive Low-Intensity Focused Ultrasound ... Low-intensity ultrasound neuromodulation: An overview of ...</a></li>

</ul>
</details>

**Tags**: `#focused ultrasound`, `#neuromodulation`, `#brain injury`, `#clinical trials`, `#neurotechnology`

---