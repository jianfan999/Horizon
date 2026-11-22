---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 81 items, 12 important content pieces were selected

---

1. [Lean formalization claims to settle the Riemann Hypothesis](#item-1) ⭐️ 9.0/10
2. [Anthropic Goes Public as a Test of Investor Appetite for Frontier AI](#item-2) ⭐️ 8.0/10
3. [Xi and Trump agree humans must stay in military AI decisions, Bessent says](#item-3) ⭐️ 8.0/10
4. [Army to Detonate Massive Pile of Unstable Lead Azide in Iowa](#item-4) ⭐️ 7.0/10
5. [Monitor's USB Hub Latency Cut Ethernet Download Speed by 75%](#item-5) ⭐️ 7.0/10
6. [Retracted UK COVID-19 vaccine study raises integrity concerns for pan-coronavirus research](#item-6) ⭐️ 7.0/10
7. [Guide Demonstrates Building PostgreSQL Extensions in Go](#item-7) ⭐️ 6.0/10
8. [Zero C#: Experimental C# toolchain without .NET runtime or GC](#item-8) ⭐️ 6.0/10
9. [Goldman Sachs and Apollo reportedly structure $32B SpaceX bond deal to fund AI chips](#item-9) ⭐️ 6.0/10
10. [Signal Restricts Mobile Screenshots to Block AI Surveillance](#item-10) ⭐️ 6.0/10
11. [UN talks pledge to draft 'killer robot' rules by 2028 despite Russian pushback](#item-11) ⭐️ 6.0/10
12. [China's EV share of car sales set to top 70% in November](#item-12) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Lean formalization claims to settle the Riemann Hypothesis](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 9.0/10

A Lean Prover Community blog post announced a Lean formalization/verification claimed to settle the Riemann Hypothesis, reportedly involving large-scale formalization of modern mathematics and heavy AI assistance. If valid, it would be a paradigm-shifting mathematical result and a major test case for AI-assisted formal proof at scale, affecting mathematicians, proof engineers, and AI-for-math researchers. The reported formal statement is said to match mathlib’s RiemannHypothesis with no extra hypotheses, leaving the formal statement, axioms, and kernel as the main audit targets; commenters also cite a past fake Collatz refutation that passed an independent checker and note that a human expert was in the loop.

hackernews · g-b-r · Nov 21, 14:36 · [Discussion](https://news.ycombinator.com/item?id=50589618)

**Background**: The Riemann Hypothesis is a central open conjecture about the distribution of nontrivial zeros of the Riemann zeta function. Lean is an interactive theorem prover whose small kernel type-checks proof terms, and Mathlib is its large community library of formalized mathematics. In formal verification, a proof is accepted only if the kernel accepts a term of the stated theorem type, so trust shifts to the kernel, definitions, axioms, and the formal statement itself.

<details><summary>References</summary>
<ul>
<li><a href="https://lean-lang.org/papers/system.pdf">The Lean Theorem Prover (system description) Why should we trust Lean? - pepamontero.github.io Should we trust AI-generated formal proofs in Lean 4? The Lean kernel - The Invariance Itself Validating a Lean Proof Lean Theorem Prover - pepamontero.github.io</a></li>
<li><a href="https://pepamontero.github.io/tfg-topologia-lean4/en/lean-theorem-prover/por-que-fiarnos-de-lean/">Why should we trust Lean? - pepamontero.github.io</a></li>
<li><a href="https://proveriemannhypothesis.github.io/">Verifying a Riemann Hypothesis Formalization in Lean</a></li>

</ul>
</details>

**Discussion**: Commenters are largely impressed but cautious: they debate kernel independence and the vanishingly small chance of exploiting a bug across multiple checkers, note the historical Collatz-checker incident, credit Levent with rare skill in getting the most out of Claude, and ask whether such a huge result opens even larger mathematical questions.

**Tags**: `#formal-verification`, `#lean`, `#riemann-hypothesis`, `#mathematics`, `#ai-assisted-proofs`

---

<a id="item-2"></a>
## [Anthropic Goes Public as a Test of Investor Appetite for Frontier AI](https://www.bloomberg.com/news/videos/2026-11-21/anthropic-makes-its-public-market-debut-video) ⭐️ 8.0/10

Bloomberg reported that Anthropic completed a landmark IPO, giving the company fresh capital to fund its enormous computing needs, while OpenAI weighs its own route to the public markets. In the same segment, Bloomberg's Ed Ludlow examined turmoil at Nvidia following Jensen Huang's departure and the chipmaker's uncertain search for new leadership. Anthropic's listing would be a defining moment for the frontier AI sector, providing a public-market benchmark for how investors value AI labs that burn enormous amounts of capital on compute. A simultaneous leadership vacuum at Nvidia, the dominant supplier of AI accelerators, would add serious uncertainty to the hardware layer that the entire industry depends on. The Bloomberg segment was short on specifics, offering no IPO price, valuation, exchange or share count, and no detail on the circumstances of Huang's departure or Nvidia's succession process. The framing suggests the offering is primarily a capital-raising event to fund compute rather than an exit for early backers, and that OpenAI may follow a similar path.

rss · Bloomberg Markets · Nov 21, 12:59

**Background**: An IPO (initial public offering) is the process by which a private company sells shares to the public and lists on a stock exchange, subjecting itself to quarterly disclosure and shareholder pressure. Anthropic is an AI safety-focused lab known for its Claude model family and is one of a small group of organizations building "frontier AI" — the most capable, general-purpose and least predictable models, which raise distinctive governance concerns because capability is concentrated among very few developers. Nvidia designs the GPUs that train and run most of these models, and Jensen Huang co-founded the company and served as its long-time chief executive, making his departure a structural shock rather than a routine transition.

<details><summary>References</summary>
<ul>
<li><a href="https://contentmind.ai/glossary/frontier-ai">Frontier AI : Definition & Meaning | THE LONG VIEW</a></li>

</ul>
</details>

**Tags**: `#AI industry`, `#Anthropic`, `#IPO`, `#Nvidia`, `#AI business`

---

<a id="item-3"></a>
## [Xi and Trump agree humans must stay in military AI decisions, Bessent says](https://www.scmp.com/news/china/diplomacy/article/3375321/xi-trump-agree-military-ai-decisions-must-involve-humans-bessent-says) ⭐️ 8.0/10

At the APEC summit, Presidents Xi Jinping and Donald Trump reportedly agreed that "humans should always be involved" in military decisions involving AI, according to US Treasury Secretary Scott Bessent, who told CNBC on Friday that the consensus was a breakthrough from the leaders' meeting the previous day. Bessent framed the agreement as covering any military decision that AI systems make. This is a rare publicly stated point of convergence between the world's two largest militaries on AI governance, and it signals that the "human in the loop" principle could become a baseline norm in bilateral arms-control discussions. If it holds, it would shape how both countries design and deploy AI-enabled command, targeting and weapons systems, affecting defense contractors and policy debates far beyond the two capitals. The claim rests on a single official's account of a closed-door leaders' meeting, with no joint statement, signed document or technical definition of what counts as "human involvement" — a gap that matters because a human who merely rubber-stamps a machine's recommendation is widely criticized as no safeguard at all. The public reporting is a short news snippet with limited detail on scope, verification or which categories of systems would be covered.

rss · SCMP · Nov 21, 07:17

**Background**: The "human in the loop" (HITL) principle holds that a person should retain meaningful control over—and responsibility for—lethal or escalatory decisions, rather than delegating them fully to software. It sits at the center of a long-running diplomatic and academic debate over lethal autonomous weapons systems (LAWS) and "meaningful human control," with critics arguing that in practice human oversight often becomes a formality that merely approves machine outputs, especially as AI decision-making becomes harder to interpret. APEC is an economic forum, so a security-related consensus emerging from its sidelines is itself notable.

<details><summary>References</summary>
<ul>
<li><a href="https://www.technologyreview.com/2026/04/16/1136029/humans-in-the-loop-ai-war-illusion/">Why having “humans in the loop” in an AI war is an illusion</a></li>
<li><a href="https://www.defensenews.com/opinion/2026/03/26/the-militarys-fabled-human-in-the-loop-for-ai-is-dangerously-misleading/">The military’s fabled ‘human in the loop’ for AI is ...</a></li>
<li><a href="https://link.springer.com/article/10.1007/s10676-025-09874-x">Lethal autonomous weapon systems (LAWS): meaningful human ...</a></li>

</ul>
</details>

**Tags**: `#military-ai`, `#ai-governance`, `#us-china-relations`, `#ai-safety`, `#policy`

---

<a id="item-4"></a>
## [Army to Detonate Massive Pile of Unstable Lead Azide in Iowa](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really) ⭐️ 7.0/10

A Science.org blog post examines the decision to destroy a large stockpile of deteriorated lead azide — a highly sensitive primary explosive used to prime ammunition — by controlled detonation in place at the Iowa Army Ammunition Plant, a former government-run explosives facility now operated by a contractor. The plan, which was elevated for approval to former Army Secretary Dan Driscoll, drew attention because the blast could send a plume of lead dust over southeastern Iowa and into northwestern Illinois, and the Army subsequently suspended or delayed the operation. The case is a stark illustration of how deferred maintenance and contractor-operated hazardous sites can reach a point where no clean solution remains: moving the material is deemed more dangerous than blowing it up, yet blowing it up disperses toxic lead. It matters to anyone interested in industrial risk management, government contracting oversight, and environmental health, since the fallout — literal and regulatory — extends far beyond the fence line. Lead azide is a primary explosive that can be set off by minor friction, shock or static, and the EPA noted the stored material had deteriorated and recrystallized, making it even more sensitive; officials also warned that the risk of accidental detonation rises in cold weather. Because the barrels reportedly cannot be shifted without triggering a mass detonation, the alternatives — moving, reburying under more dirt and concrete, or chemical neutralization — were all judged riskier or impractical.

hackernews · beginning_end · Nov 21, 13:23 · [Discussion](https://news.ycombinator.com/item?id=50588982)

**Background**: Primary explosives differ from secondary explosives like TNT in that they need no booster shock wave — they detonate from a spark or a nudge — which is why they are used in small quantities in detonators and primers rather than as bulk charges. The Iowa Army Ammunition Plant was built for World War II production and for decades loaded and packed artillery ammunition; like many such sites, it passed into contractor operation and accumulated legacy stocks of unstable material. Explosives that recrystallize or dry out over years in storage become progressively more dangerous, and standard practice at labs handling such compounds is to call a bomb squad to destroy them in place rather than attempt transport.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fox32chicago.com/news/what-is-lead-azide-from-iowa-army-explosion">What is lead azide —and why is the Army blowing it... | FOX 32 Chicago</a></li>
<li><a href="https://www.newsweek.com/army-issues-evacuation-warning-massive-toxic-lead-dust-cloud-12735122">Army suspends detonation after toxic lead dust cloud... - Newsweek</a></li>
<li><a href="https://www.cbsnews.com/chicago/news/army-lead-azide-detonation-iowa-toxic-dust-plume/">U.S. Army delays planned detonation of unstable explosives in Iowa...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely critical of institutional failure: one noted the plant was government-built for WWII, shut down in the 1960s, then handed to a contractor in 1998, which allegedly cut corners on the ordnance under its care. Others pushed back on armchair suggestions of using robots or moving the barrels, explaining that a bomb squad would simply destroy such material in place, and several framed the episode as a broader pattern of hiding problems until only bad options remain, with no consequences for those responsible.

**Tags**: `#explosives safety`, `#industrial accidents`, `#risk management`, `#chemistry`, `#government contracting`

---

<a id="item-5"></a>
## [Monitor's USB Hub Latency Cut Ethernet Download Speed by 75%](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

Blogger tymscar published a debugging post explaining how routing his Ethernet connection through his monitor's built-in USB hub cut his download speed by roughly 75%. The culprit was not raw USB bandwidth but added latency: the hub delayed TCP acknowledgements enough that the Ethernet adapter's buffer overflowed and began dropping packets, and swapping to a different USB Ethernet adapter that required less frequent acknowledgement restored normal speeds. The case shows that performance problems in layered hardware stacks can hide far from where they appear, since a monitor accessory silently degraded a network link with no obvious error message. It is a useful reminder for anyone using USB-C docks, monitor hubs, or KVM setups for wired networking that these paths are not transparent pass-throughs. The bottleneck was latency and buffering rather than bandwidth, so the monitor itself is largely incidental — as one commenter put it, the real headline is 'my USB network switch was cutting my download speed.' Different USB Ethernet adapters behave differently because of how often they require acknowledgement and how they batch transfers, which is why simply swapping the adapter fixed a problem that looked like a network fault.

hackernews · soheilpro · Nov 21, 10:36 · [Discussion](https://news.ycombinator.com/item?id=50587875)

**Background**: USB Ethernet adapters encapsulate network traffic over USB transfers, and when they sit behind a hub — such as the hub built into many USB-C monitors — all attached devices share that link and incur additional forwarding latency. TCP throughput depends on acknowledgements returning promptly; if the round trip stretches and the adapter's internal buffer is small, packets get dropped and the sender backs off. Community threads on Dell monitors and USB-C hubs document similar symptoms, where Ethernet through a monitor's hub underperforms a direct connection.

<details><summary>References</summary>
<ul>
<li><a href="https://superuser.com/questions/1592635/does-a-usb-c-ethernet-adapter-have-a-higher-latency-than-a-regular-ethernet-port">networking - Does a USB -C ethernet adapter have a higher latency ...</a></li>
<li><a href="https://laptopjudge.com/monitor-usb-hub-ethernet-dropouts/">Monitor USB Hub Ethernet Dropouts (Bandwidth Fix) - LaptopJudge</a></li>
<li><a href="https://www.dell.com/community/en/conversations/monitors/u3821dw-slow-ethernet-speed-using-the-built-in-usb-hub/647f99a9f4ccf8a8ded16e84">U3821DW, slow ethernet speed using the built in USB hub - Dell</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the post for untangling genuinely opaque USB hub behavior, with several clarifying that the extra latency — not bandwidth — broke TCP acknowledgement timing and caused buffer overflow and packet drops. One reader argued the framing should have focused on the USB network switch rather than the monitor, while others shared analogous debugging war stories, such as a terminal emulator's io_uring usage being misread as I/O pressure and throttling game shader compilation, and a year-long Thunderbolt dock slowdown.

**Tags**: `#networking`, `#USB`, `#debugging`, `#hardware`, `#latency`

---

<a id="item-6"></a>
## [Retracted UK COVID-19 vaccine study raises integrity concerns for pan-coronavirus research](https://www.scmp.com/news/china/science/article/3375190/how-retracted-uk-covid-19-vaccine-study-tainted-global-hunt-mutation-proof-shots) ⭐️ 7.0/10

A 2022 study that proposed a vaccine design for pan-SARS-CoV-2 immunity was retracted last month after its lead author, then based in Britain, admitted to fabricating data and falsifying images in the paper. The paper had been widely cited by international scientists up until this year, making the retraction a notable blow to the field. The case highlights how fabricated preclinical evidence can propagate through the literature and distort the global effort to develop mutation-proof, broadly protective coronavirus vaccines. It matters to researchers, funders and policymakers who rely on citation records when prioritizing vaccine design strategies, even though virologists say the underlying science of targeting conserved coronavirus regions remains sound. The retraction was triggered by the lead author's own admission of data fabrication and image falsification, rather than by a failed replication alone, and the paper had accumulated high citation counts before being pulled. Experts quoted stress that the broader body of pan-coronavirus vaccine work does not depend on this single paper, so the retraction taints a strand of the literature rather than invalidating the conserved-region approach.

rss · SCMP · Nov 22, 00:00

**Background**: Pan-SARS-CoV-2 (or pan-coronavirus) vaccine designs aim to elicit immunity against many variants and related coronaviruses by targeting parts of the virus spike protein that mutate less, such as conserved regions, rather than only the fast-changing receptor-binding domain. Because SARS-CoV-2 keeps evolving new variants that partly evade antibodies raised by earlier vaccines, next-generation 'mutation-proof' shots are a major research priority. Retraction is the formal withdrawal of a published paper, typically used when data or images are found to be unreliable or fraudulent.

<details><summary>References</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9040821/">The Impact of Evolving SARS-CoV-2 Mutations and Variants on ...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10188376/">A novel mutation-proof, next-generation vaccine to fight ...</a></li>
<li><a href="https://www.sciencedaily.com/releases/2026/06/260605023357.htm">AI- designed universal coronavirus vaccine passes first... | ScienceDaily</a></li>

</ul>
</details>

**Tags**: `#research integrity`, `#COVID-19 vaccines`, `#scientific misconduct`, `#retractions`, `#virology`

---

<a id="item-7"></a>
## [Guide Demonstrates Building PostgreSQL Extensions in Go](https://jespino.github.io/gopgext/) ⭐️ 6.0/10

Developer Jesús Espino published a guide at jespino.github.io/gopgext/ that walks through writing PostgreSQL extensions in Go instead of the traditional C or the Rust-based pgrx framework. The project reached the front page of Hacker News, gathering 122 points and 22 comments. Go is one of the most widely used languages for backend services, so a working path to Postgres extensions could let a much larger pool of developers extend the database without learning C and the server's internal APIs. It also adds to a broader trend of bringing memory-safe, higher-level languages into Postgres extension development, where Rust's pgrx has already gained traction. Because PostgreSQL loads extensions as shared libraries into the backend process and calls them through its C function-manager ABI, a Go-based extension has to bridge into C (typically via cgo), which drags the Go runtime and garbage collector into the database backend. The guide also sits alongside the author's related experiment gokm (Linux kernel modules in Go), and commenters pointed to the older plgo project for a similar approach.

hackernews · valyala · Nov 21, 17:08 · [Discussion](https://news.ycombinator.com/item?id=50591260)

**Background**: PostgreSQL extensions are normally C shared libraries loaded directly into a server backend process, hooked into well-defined APIs such as fmgr, SPI and various planner/executor hooks. That design gives extensions near-native speed and deep access, but it also means a bug can crash the whole backend, and developers must manage Postgres memory contexts manually. Go can export and call C functions through cgo, which is the mechanism any Go-based extension would rely on to talk to the server.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/xfunc-c.html">PostgreSQL : Documentation: 19: 36.10. C -Language Functions</a></li>
<li><a href="https://go.dev/blog/cgo">C ? Go ? Cgo ! - The Go Programming Language</a></li>

</ul>
</details>

**Discussion**: Commenters were cautiously positive: one argued that more people extending Postgres is a big ecosystem win but doubted Go's fit, noting that Go shines at platform-level work like Kubernetes and proxies while extensions live at the data plane. Others shared pointers to related work, namely the author's gokm kernel-module project and the plgo project, and one made a lighthearted digression about the Go gopher mascot.

**Tags**: `#postgresql`, `#golang`, `#databases`, `#extensions`, `#systems-programming`

---

<a id="item-8"></a>
## [Zero C#: Experimental C# toolchain without .NET runtime or GC](https://onurgumus.github.io/zero-csharp/index.html) ⭐️ 6.0/10

A Show HN project called Zero C# presents an experimental toolchain that compiles C# code to run without the .NET runtime or garbage collector. It is positioned as a proof of concept rather than a production-ready .NET replacement. The experiment probes whether C# can be used in GC-free, runtime-free environments such as games, embedded systems, and low-level tooling, where deterministic memory management matters. Its reception also highlights how much of that niche is already served by NativeAOT and modern low-level C# features. Commenters point out that NativeAOT already produces standalone native executables, while unsafe pointers, Span<T>, ref structs, and unmanaged allocation APIs give developers manual memory control; the prior bflat project occupies similar territory. The trade-off is that existing C# code and libraries generally assume the standard runtime and GC, so compatibility is likely limited.

hackernews · reverseblade2 · Nov 21, 15:39 · [Discussion](https://news.ycombinator.com/item?id=50590279)

**Background**: C# normally runs on the .NET runtime, where a garbage collector automatically reclaims memory and a large standard library provides core functionality. NativeAOT is Microsoft's ahead-of-time compilation option that can produce self-contained native binaries without requiring the .NET runtime to be installed, though it still relies on runtime services and GC. Zero C# explores going further by removing the runtime and collector entirely.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/dotnet/runtime/blob/main/docs/workflow/building/coreclr/nativeaot.md">runtime/docs/workflow/building/coreclr/nativeaot.md at main ...</a></li>
<li><a href="https://github.com/topics/nativeaot">nativeaot · GitHub Topics · GitHub</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was largely skeptical: one commenter argued C# already offers unsafe pointers, Span<T>, and NativeAOT and is “sufficient enough,” while another asked what Zero C# adds over NativeAOT, noting NativeAOT can even be slower than RyuJIT except for smaller binaries. Others compared it to bflat and said C, Rust, or Zig are better choices for GC-free work, though one comment defended the GC as a productivity feature rather than a flaw.

**Tags**: `#C#`, `#.NET`, `#NativeAOT`, `#memory management`, `#compilers`

---

<a id="item-9"></a>
## [Goldman Sachs and Apollo reportedly structure $32B SpaceX bond deal to fund AI chips](https://www.bloomberg.com/news/articles/2026-11-21/goldman-s-spacex-pitch-helps-solve-ai-debt-puzzle-credit-weekly) ⭐️ 6.0/10

Bloomberg reports that Goldman Sachs Group and Apollo are structuring roughly $32 billion in SpaceX bonds intended to finance massive AI chip purchases. According to the report, Goldman spent more than a year designing the arrangement so that the chip spending would not strain corporate balance sheets. If completed, a $32 billion bond package would be one of the largest financing structures ever built around AI hardware, and it points to a shift where AI capex is funded through capital markets rather than operating cash flow. This matters for chip suppliers, credit investors and any company trying to scale AI compute without taking the full depreciation hit on its own books. The available reporting is only a short excerpt, so the bond's coupon, maturity, legal issuer and whether the debt sits off SpaceX's balance sheet are not disclosed. The framing suggests a structured, possibly bankruptcy-remote vehicle rather than a plain vanilla corporate bond, which would shift some risk from SpaceX to creditors and bondholders.

rss · Bloomberg Markets · Nov 21, 15:31

**Background**: AI training and inference require enormous quantities of GPUs and accelerators, and the depreciation of that hardware hits earnings quickly, which is why companies look for ways to spread or externalize the cost. Apollo is a major alternative asset manager that specialises in private credit and structured financing, while Goldman Sachs is a leading underwriter and arranger of large debt deals. SpaceX, the Musk-led rocket and satellite company, is privately held and rarely taps public bond markets, making a multi-tens-of-billions issuance unusual and notable.

**Tags**: `#AI infrastructure`, `#financing`, `#SpaceX`, `#bonds`, `#Goldman Sachs`

---

<a id="item-10"></a>
## [Signal Restricts Mobile Screenshots to Block AI Surveillance](https://techcrunch.com/2026/11/21/signal-restricts-mobile-screenshots-as-it-confronts-existential-threat-of-ai-surveillance/) ⭐️ 6.0/10

Signal has started restricting in-app screenshots on both Android and iOS, aiming to prevent AI assistants such as Gemini and Siri from capturing and reading users’ messages and other on-screen data. This matters because end-to-end encryption protects messages in transit, but not once an operating-system-level AI agent can read the decrypted screen; a major secure messenger acting on that gap could push other apps to follow suit. The change extends Signal’s existing Screen Security protections, which previously kept message previews out of the app switcher, and on Android the app will show users a notice explaining the screenshot-blocking behavior. Client-side screenshot blocks are not absolute, since a separate camera can still photograph the screen.

rss · TechCrunch · Nov 21, 21:37

**Background**: Signal is a widely used end-to-end encrypted messaging app, meaning only the sender and recipient can decrypt message contents. Traditional screenshot protections are implemented by the operating system or app—such as Android’s secure-window flag—to prevent capture of sensitive screens. The rise of AI assistants that can inspect on-screen context has created a new risk: even encrypted messages can be exposed after they are rendered on the display. Signal’s Screen Security setting is the existing control it is now expanding.

<details><summary>References</summary>
<ul>
<li><a href="https://signal.org/blog/protecting-your-privacy/">Signal >> Blog >> Signal is Serious About Protecting Your Privacy</a></li>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/1038390/signal-blocking-ai-agent-screenshots-mobile-app">Signal is blocking Gemini and Siri AI from reading your screen</a></li>
<li><a href="https://support.signal.org/hc/en-us/articles/360043469312-Screen-Security">Screen Security - Signal Support</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#Signal`, `#AI surveillance`, `#mobile security`, `#encryption`

---

<a id="item-11"></a>
## [UN talks pledge to draft 'killer robot' rules by 2028 despite Russian pushback](https://www.scmp.com/news/world/europe/article/3375318/un-talks-pledge-draft-killer-robot-rules-2028-after-russian-pushback) ⭐️ 6.0/10

UN talks on regulating weapons with little or no human oversight ended on Saturday with a pledge to hold further discussions aimed at developing new rules within two years. Around 100 countries had backed legally binding rules on autonomous weapons systems, but the final outcome was weakened by Russia's opposition. This is a key test of whether multilateral AI governance can keep pace with weapons technology, and the weakened pledge signals that consensus on binding limits remains far off. The delay leaves countries and militaries free to develop and potentially deploy increasingly autonomous systems without an international legal framework. Proponents had pushed for legally binding rules on systems that can identify and engage targets with varying degrees of autonomy, but the agreed text only commits to further talks and drafting within two years. Human rights groups criticized the result as disappointing, and several major military powers did not join the roughly 100 states backing binding rules.

rss · SCMP · Nov 21, 06:32

**Background**: Lethal autonomous weapons systems — often called "killer robots" — can select and engage targets without a human deciding to pull the trigger, ranging from loitering munitions to AI-assisted targeting. Because no international treaty specifically covers them, states have debated for over a decade at the UN Convention on Certain Conventional Weapons in Geneva. Human rights and arms-control groups argue that meaningful human control must be preserved, while military powers are wary of limits that could erode perceived advantages.

**Tags**: `#AI governance`, `#autonomous weapons`, `#UN policy`, `#AI ethics`, `#lethal autonomous weapons`

---

<a id="item-12"></a>
## [China's EV share of car sales set to top 70% in November](https://www.scmp.com/business/china-business/article/3375236/chinas-ev-adoption-rate-top-70-petrol-cars-take-brunt-drop-overall-sales) ⭐️ 6.0/10

The China Passenger Car Association (CPCA) said on Thursday that carmakers were expected to deliver 1.15 million electric and plug-in hybrid vehicles to mainland buyers in November, equal to 70.6 per cent of total passenger car sales. That would mark the first time seven out of ten new car buyers in China choose an electrified vehicle, as petrol-only models absorb the decline in overall sales. China is the world's largest auto market, so a 70% electrified share sets a benchmark no other major market is close to and reinforces the country's lead in EV manufacturing and battery supply chains. The shift also pressures global automakers and oil demand, since falling petrol-car volumes in China ripple through export markets and refining economics. The CPCA figure covers both battery-electric vehicles and plug-in hybrids, meaning a substantial portion of the 70.6% still burn petrol when their batteries are depleted. The 1.15 million unit projection is for passenger vehicles delivered to mainland customers in November and comes amid an overall contraction in total car sales.

rss · SCMP · Nov 21, 06:00

**Background**: China's official statistics group battery-electric and plug-in hybrid cars under the label "new energy vehicles" (NEVs), which is why the figures here differ from definitions that count only pure EVs. A plug-in hybrid (PHEV) has both a petrol engine and a larger battery that can be recharged from an outlet, giving limited electric-only range before the engine takes over, whereas a battery-electric vehicle has no petrol engine at all. The CPCA is a Beijing-based industry association whose monthly retail and wholesale data is one of the most closely watched gauges of Chinese auto demand.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/topics/china-passenger-car-association">China Passenger Car Association</a></li>
<li><a href="https://cars.usnews.com/cars-trucks/advice/hybrid-vs-phev-vs-ev">Hybrid vs. Plug-In Hybrid vs. Electric: What's the Difference?</a></li>

</ul>
</details>

**Tags**: `#electric vehicles`, `#China`, `#automotive industry`, `#market adoption`, `#clean energy`

---