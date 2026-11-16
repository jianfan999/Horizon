---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 92 items, 10 important content pieces were selected

---

1. [Anthropic Set for Record IPO, Elevating Dario Amodei as AI Boom's Face](#item-1) ⭐️ 9.0/10
2. [MacBook Pro OLED PWM flicker sparks accessibility debate](#item-2) ⭐️ 8.0/10
3. [Old Bitly Links Hijacked, Including Burger King Tweet](#item-3) ⭐️ 7.0/10
4. [Protomaps Makes Self-Hosting Map Tiles Cheap and Easy](#item-4) ⭐️ 7.0/10
5. [Crows make decisions faster than humans, NYT reports](#item-5) ⭐️ 7.0/10
6. [Microsoft 365 outage silences hotel pool chlorine alarm, sickening 15 guests](#item-6) ⭐️ 7.0/10
7. [2011 Turbo Pascal Size Comparison Resurfaces, Sparking Software Bloat Debate](#item-7) ⭐️ 6.0/10
8. [US Hardware Startups Return to Shenzhen Despite Tariffs](#item-8) ⭐️ 6.0/10
9. [Apple launches app to study AI answers to everyday medical questions](#item-9) ⭐️ 6.0/10
10. [Iran Reportedly Used US Troops' Social Media and Fitness App Data to Target Mideast Bases](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic Set for Record IPO, Elevating Dario Amodei as AI Boom's Face](https://www.bloomberg.com/news/features/2026-11-15/anthropic-s-ipo-makes-dario-amodei-the-new-face-of-the-ai-boom) ⭐️ 9.0/10

Bloomberg reported on November 15, 2026 that Anthropic is set to carry out the largest initial public offering of all time, a listing that would turn its CEO Dario Amodei into a central public figure of the current AI boom. The report frames the offering as the moment when investors' hopes and fears about artificial intelligence become concentrated on a single frontier model maker. If it proceeds at record scale, the IPO would set a public-market valuation benchmark for the entire cohort of private frontier AI labs and give ordinary investors their first large-scale way to bet directly on a pure-play model developer. It also turns a company whose stated mission is managing existential AI risk into a publicly traded entity answerable to quarterly earnings pressure, which could shift how the whole industry talks about safety versus growth. The Bloomberg item is brief and does not disclose a valuation, share count, pricing range, timing or financial figures, so the record-setting claim is reported rather than confirmed with deal terms. Any concrete numbers — and whether the listing actually lands as the largest ever — will only become clear once a formal prospectus is filed.

rss · Bloomberg Markets · Nov 15, 19:00

**Background**: Anthropic is an AI safety and research company that builds what the industry calls frontier models — the most advanced general-purpose AI systems available at any given time, characterized by massive scale and strong multi-step reasoning, multimodal and agentic capabilities. Dario Amodei is its CEO, and the company's culture and outlook are closely associated with his views on AI risk, including the idea that advanced AI could pose an existential threat to humanity. An IPO, or initial public offering, is the process by which a private company first sells shares to public investors and lists on a stock exchange, typically after years of venture funding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/company">Company \ Anthropic</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#IPO`, `#AI industry`, `#Dario Amodei`, `#Bloomberg`

---

<a id="item-2"></a>
## [MacBook Pro OLED PWM flicker sparks accessibility debate](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 8.0/10

A deep-dive article on macanorak.com examines how the new MacBook Pro's tandem OLED panel dims via PWM (pulse-width modulation) at roughly 240 Hz with about 56% flicker depth whenever brightness is set to 99% or below, a measurement originally reported by Notebookcheck's lab testing. The piece, paired with a 429-point Hacker News thread, argues that OLED-sensitive users may experience eye strain, headaches or nausea from a display that is otherwise technically superior. It highlights a trade-off mainstream reviews rarely cover: a display can improve on contrast, black levels and power efficiency while becoming harder to use for people with flicker sensitivity, migraine or post-concussion symptoms. Because PWM dimming is the standard brightness mechanism across most OLED phones, tablets and laptops, the MacBook Pro case feeds a broader accessibility conversation about whether vendors should disclose flicker frequency in spec sheets. The reported figures are roughly 240 Hz flicker frequency and approximately 56% modulation depth, with PWM engaging at essentially all non-maximum brightness levels, so simply turning brightness down does not avoid it. A commenter who re-examined the source data argues the true rate may be higher, since a tandem OLED structure could drive two layers at 480 Hz and 180 degrees out of phase for an effective 960 Hz across most usable brightness levels, and the original article itself notes DC-like dimming behavior at some settings.

hackernews · MacAnorak · Nov 15, 13:15 · [Discussion](https://news.ycombinator.com/item?id=50506719)

**Background**: PWM dimming controls perceived brightness by rapidly switching the display's light emission on and off and varying the duty cycle, rather than by reducing the driving current (DC dimming). It is cheap and preserves color accuracy at low brightness, but the resulting flicker can be perceived by some people — and by the nervous system even below conscious perception — causing eye strain, headaches and nausea; flicker depth and frequency together determine how severe the effect is. OLED panels are especially associated with PWM because per-pixel emission makes low-brightness current control harder, and the MacBook Pro's tandem OLED stacks two emissive layers to boost brightness and longevity. A related accessibility concept is CRI (color rendering index), which describes how evenly a white light source's spectrum covers the visible range compared with sunlight or incandescent bulbs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.appleheadlines.com/macbook-pro-oled-eye-strain-pwm-flicker/">MacBook Pro OLED Eye Strain & PWM Flicker: 7 Moves - AH</a></li>
<li><a href="https://www.oled-info.com/pulse-width-modulation-pwm-oled-displays">Pulse-width modulation (PWM) in OLED displays - OLED-Info</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread mixes technical correction with firsthand experience: one commenter challenges the 240 Hz figure by going back to the source measurements and proposes a tandem-panel 480 Hz-out-of-phase explanation yielding an effective 960 Hz, while others note that humans can perceive flicker well above a display's base rate. Commenters broaden the complaint beyond PWM to LED color rendering, LCD motion blur and individual sensitivity differences, with a post-concussion reader describing how virtually all screens — not only bright OLEDs — became difficult, and several asking for more research into how common PWM sensitivity actually is.

**Tags**: `#displays`, `#OLED`, `#PWM flicker`, `#hardware`, `#accessibility`

---

<a id="item-3"></a>
## [Old Bitly Links Hijacked, Including Burger King Tweet](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 7.0/10

Old Bitly short links, including one used in a Burger King tweet, are reportedly being hijacked and redirected to bizarre or offensive destinations. The scheme appears to target archived corporate social media posts whose shortened links still resolve. The incident shows that URL shorteners create long-lived third-party dependencies: a link can outlive the account, company, or oversight that created it, turning trusted historical posts into attack surface. It matters for brands, archivists, and anyone who relies on short links in published material. The hijacking reportedly involves old bit.ly links embedded in corporate tweets rather than newly created links, and some redirect to unrelated offensive content. URL shorteners concentrate risk because the short domain and code, not the original publisher, control where a click ultimately goes.

hackernews · hspeiser · Nov 15, 22:11 · [Discussion](https://news.ycombinator.com/item?id=50511395)

**Background**: URL shorteners map a short address such as bit.ly/xxxx to a longer destination, making links easier to share but adding a middleman that must keep resolving correctly. Link rot is the related long-term problem in which links stop pointing to their original target because pages move or disappear; short links can suffer both link rot and hijacking when ownership or accounts change. Link hijacking occurs when control of a link’s destination is altered through redirects, compromised accounts, or tampered targets, so a familiar-looking URL can lead somewhere malicious.

<details><summary>References</summary>
<ul>
<li><a href="https://nypost.com/2026/11/15/lifestyle/corporate-social-media-hacked-in-bizarre-bitly-link-hijacking-scheme/">Corporate social media hacked in bizarre Bitly link-hijacking ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Link_rot">Link rot</a></li>
<li><a href="https://nhimg.org/glossary/link-hijacking/">What Is Link Hijacking? Definition & Examples - nhimg.org</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly skeptical of URL shorteners, arguing that outsourced short links accumulate over time and become permanently broken when accounts are deactivated or shortener companies fail. Several said the story reinforced their long-standing opposition to shorteners, while others were surprised that a shortener like Bitly has a Trust and Safety team; one commenter also called for better tracking of abandoned URL ownership.

**Tags**: `#security`, `#URL shorteners`, `#link hijacking`, `#internet infrastructure`, `#link rot`

---

<a id="item-4"></a>
## [Protomaps Makes Self-Hosting Map Tiles Cheap and Easy](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

A blog post argues that self-hosting map tiles with Protomaps has become both affordable and easy, and the write-up reached the front page of Hacker News with 179 points and 43 comments. Commenters added related projects such as OpenFreeMap and PMTiles tooling like gloss and ntmaps, along with real-world side-project use cases. Owning map infrastructure lets developers avoid Mapbox or Google Maps API costs, usage limits, and lock-in, which is especially important for side projects and privacy-sensitive applications. The discussion suggests that the open-source geospatial stack around OpenStreetMap, PMTiles, and MapLibre is now mature enough for practical self-hosting. Protomaps packages a world map as a PMTiles archive, a single static file that can be served from commodity cloud storage such as S3 or Cloudflare R2 using HTTP Range requests. Commenters noted that vector basemaps are small enough to store cheaply, but high-resolution satellite imagery grows rapidly at higher zoom levels, with global coverage potentially reaching hundreds of terabytes.

hackernews · bcye · Nov 15, 19:26 · [Discussion](https://news.ycombinator.com/item?id=50509837)

**Background**: Protomaps is an open-source map of the world designed to be deployed as a single static file on cloud storage, rather than through a traditional tile server. PMTiles is the underlying archive format: it stores a pyramid of map tiles inside one file, similar in spirit to a ZIP archive, and supports low-cost, low-maintenance serving from object storage. In contrast, a conventional self-hosted OpenStreetMap tile stack often involves PostGIS, rendering software, and ongoing server administration.

<details><summary>References</summary>
<ul>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>
<li><a href="https://docs.protomaps.com/pmtiles/">PMTiles Concepts | Protomaps Docs</a></li>
<li><a href="https://github.com/protomaps/PMTiles">GitHub - protomaps/ PMTiles : Pyramids of map tiles in a single file on...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was broadly positive: one commenter pointed to OpenFreeMap as a similar free public-instance project, while another said Protomaps made a Wikipedia walking game with live-rendered street maps affordable enough to build as a side project. Others described running similar setups on Cloudflare R2 for privacy and access control, while also flagging caveats around very large tiles, raster formats, and the storage cost of high-zoom satellite imagery.

**Tags**: `#maps`, `#self-hosting`, `#openstreetmap`, `#pmtiles`, `#geospatial`

---

<a id="item-5"></a>
## [Crows make decisions faster than humans, NYT reports](https://www.nytimes.com/2026/11/15/science/birdbrain-crows-birds-research-decision.html) ⭐️ 7.0/10

A New York Times science article reports research suggesting that crows can reach decisions faster than humans can, and the piece sparked a wide-ranging Hacker News discussion about alternative brain architectures and how intelligence evolves. The coverage highlights that birds achieve flexible, fast cognition without the layered cerebral cortex that mammals rely on. The finding reinforces that complex cognition is not tied to one specific neural blueprint, which matters for how researchers think about the evolution of intelligence and, by extension, for attempts to build intelligent systems on non-biological or non-mammalian architectures. It also reframes the dismissive term "birdbrain" as a misunderstanding of a genuinely sophisticated nervous system. Bird brains are small and lack the layered cortex seen in primates, yet the avian pallium — including the nidopallium and mesopallium — contains densely packed neurons that appear to support comparable cognitive functions; commenters also speculate that shorter physical connection distances could shorten sensorimotor feedback loops and speed up reactions.

hackernews · gumby · Nov 15, 17:53 · [Discussion](https://news.ycombinator.com/item?id=50509023)

**Background**: Corvids such as crows, ravens and jays are classic examples of convergent evolution: they display tool use, mental time travel and rich social cognition despite diverging from mammals hundreds of millions of years ago. Instead of a laminated cerebral cortex, birds have an enlarged pallium organized into distinct nuclei, a fundamentally different wiring plan that nonetheless produces flexible behavior. Earlier work has even found neural correlates of sensory consciousness in corvids, suggesting the foundations of subjective experience may not require a cortex at all.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Avian_brain">Avian brain - Wikipedia</a></li>
<li><a href="https://www.science.org/doi/10.1126/science.1098410">The Mentality of Crows: Convergent Evolution of Intelligence ...</a></li>
<li><a href="https://www.science.org/doi/10.1126/science.abb1447">A neural correlate of sensory consciousness in a corvid bird</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly enthusiastic: one noted that intelligence has evolved independently at least three times — in mammals, corvids and octopuses — with birds using a different neuron design and brain architecture entirely. Others argued that smaller brains mean shorter connection distances and faster feedback loops (comparing it to training the spine rather than the brain when learning piano or dance), pushed back on the "birdbrain" insult by citing magnetoreception, decentralized body clocks and the spatial demands of flight, and recommended Jennifer Ackerman's book "The Genius of Birds."

**Tags**: `#cognitive-science`, `#neuroscience`, `#evolution`, `#animal-intelligence`, `#hacker-news`

---

<a id="item-6"></a>
## [Microsoft 365 outage silences hotel pool chlorine alarm, sickening 15 guests](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 7.0/10

At a hotel in Germany's Rhein-Erft-Kreis (near the Phantasialand theme park), an automatic pool chlorination dosing system overdosed the water with chlorine, and the monitoring system's warning emails — sent through Microsoft Outlook/Microsoft 365 — never reached the operator because of a Microsoft 365 outage. Around 13 guests initially reported airway irritation with two more added later, four were taken to hospital (one classified as a medium injury), and roughly 40 first responders were deployed for triage. The incident is a textbook example of how safety-critical alerting can silently collapse when it depends on a single cloud dependency, turning an ordinary equipment fault into a public-health event. It is likely to sharpen scrutiny of whether commercial facilities need mandatory redundant, non-cloud alert paths for hazardous systems such as pool chemicals, gas detection and fire safety. According to community translations of the original German report, two separate systems failed: the dosing unit itself had a defect that caused it to over-chlorinate, and the monitoring notification path failed because of the M365 outage — the German coverage is notably less dramatic than the English headlines, and most injuries were minor. The hotel's "maintenance safety system" for the sauna/pool area relied on sending emails to operators rather than on an on-site alarm, phone call or SMS.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**Background**: Commercial pools and saunas use closed-loop chlorination controllers: a sensor measures free chlorine in the water and a dosing pump adds chlorine (or acid) to hold the level in range, with the controller sending alerts if readings go out of range. A classic failure mode is that a fouled or failed sensor reads low or zero, so the controller keeps dosing and over-chlorinates the water — which is why operators are expected to verify chemistry manually and why alerting must never hinge on one delivery channel. Emailing alerts through a third-party SaaS like Microsoft 365 adds a dependency on an external service that can be down exactly when the alarm fires.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/data-centers/microsoft-365-outage-leads-to-chlorine-gas-poisoning-of-15-hotel-guests-email-warning-system-fails-40-first-responders-deployed-for-triage-four-hospitalized">Microsoft 365 outage leads to chlorine gas... | Tom's Hardware</a></li>
<li><a href="https://news.ycombinator.com/item?id=50509411">Microsoft 365 outage leads to chlorine gas poisoning of... | Hacker News</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters overwhelmingly blamed the hotel's architecture rather than Microsoft: one commenter who runs a closed-loop chlorination system explained that such controllers commonly fail by reading low and over-dispensing, so a human or an independent sensor design must always provide the safety layer, while another called it "100% fault of the hotel" to have no backup or double-check beyond email. A German-speaking commenter corrected the overheated framing, noting it was a dual failure with 13–15 people affected and mostly minor injuries, and others stressed that anything capable of such harm needs a resilient, redundant alerting architecture.

**Tags**: `#reliability`, `#cloud-dependency`, `#alerting`, `#safety-critical-systems`, `#incident-analysis`

---

<a id="item-7"></a>
## [2011 Turbo Pascal Size Comparison Resurfaces, Sparking Software Bloat Debate](https://prog21.dadgum.com/116.html) ⭐️ 6.0/10

A 2011 blog post titled "Things That Turbo Pascal Is Smaller Than" has resurfaced on Hacker News, using the tiny Turbo Pascal system as a benchmark to show how large modern binaries and software distributions have become. It turns a nostalgic comparison into a concrete critique of software bloat, prompting developers to weigh modern productivity gains against increased binary size, memory use, and layered abstractions. The comparison is qualitative and era-dependent: commenters note that 1986-era PCs had roughly 30,000 times less RAM than today's laptops, so Turbo Pascal was not necessarily leaner relative to its hardware than modern tools like VS Code. The original post is from 2011 and is not a controlled benchmark; its examples illustrate scale rather than prove a specific bloat metric.

hackernews · ksec · Nov 15, 13:44 · [Discussion](https://news.ycombinator.com/item?id=50506894)

**Background**: Turbo Pascal was a Borland development system combining a Pascal compiler and IDE for CP/M and MS-DOS, originally developed by Anders Hejlsberg and known for extremely fast compilation. It became a highly influential PC development tool in the 1980s and early 1990s. "Software bloat" describes successive versions of a program becoming slower or more resource-hungry, often because features are added or efficiency is traded for developer productivity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turbo_Pascal">Turbo Pascal</a></li>
<li><a href="https://en.wikipedia.org/wiki/Software_bloat">Software bloat</a></li>

</ul>
</details>

**Discussion**: Commenters mixed nostalgia with debate: some praised Anders Hejlsberg as one of the best language designers for Turbo Pascal, Delphi, C#, and TypeScript, while others argued that cross-era size comparisons are unfair given the vast RAM differences. Several focused on specific absurdities such as the Unix touch command's binary exceeding Turbo Pascal, and one asked why Pascal declined despite its influence.

**Tags**: `#software engineering`, `#software bloat`, `#Turbo Pascal`, `#binary size`, `#programming history`

---

<a id="item-8"></a>
## [US Hardware Startups Return to Shenzhen Despite Tariffs](https://www.bloomberg.com/news/videos/2026-11-15/pkg-engle-shenzhen-tech-entrepreneurs) ⭐️ 6.0/10

A Bloomberg video segment reported by Stephen Engle documents a renewed wave of US hardware entrepreneurs traveling back to Shenzhen to prototype and manufacture their products, saying the speed and cost cannot be matched elsewhere. The trend is unfolding even as tariffs and political pressure push toward supply-chain diversification away from China. The report suggests that for early-stage hardware, the depth of Shenzhen's supplier and prototyping ecosystem still outweighs tariff costs and policy risk, complicating government efforts to decouple manufacturing. It signals that the practical pull of the region's industrial cluster remains strong for Western startups even as larger firms diversify. The segment is a short news video with limited technical depth, and it highlights speed and cost as the decisive factors rather than any single product or company; Bloomberg does not quantify the size of the returning wave or how much tariffs add to unit costs.

rss · Bloomberg Markets · Nov 15, 23:00

**Background**: Shenzhen, in China's Guangdong province, is often called the world's hardware capital: the Huaqiangbei electronics market and thousands of nearby small factories let teams go from design files to a working prototype in days. That dense supplier network — PCB fabrication, tooling, injection molding, assembly, and components — is hard to replicate quickly elsewhere, which is why hardware founders traditionally treat Shenzhen as a required stop. In recent years, US tariffs on Chinese goods and policy pressure to shift production to Vietnam, Mexico, or India have raised costs and added friction, but have not eliminated the region's prototyping advantage.

**Tags**: `#hardware`, `#shenzhen`, `#manufacturing`, `#supply-chain`, `#innovation`

---

<a id="item-9"></a>
## [Apple launches app to study AI answers to everyday medical questions](https://techcrunch.com/2026/11/15/apple-launches-new-app-to-study-how-people-use-ai-for-health/) ⭐️ 6.0/10

Apple has launched a new app tied to a research study that will examine how people use AI to answer everyday medical questions. The app is positioned as a data-gathering tool for Apple's health-AI research rather than a general-purpose medical product. The study signals that Apple wants first-hand behavioral data on consumer AI health queries, which could shape future health features across iPhone and Apple Watch. Given how many people already turn to chatbots for symptom questions, whatever Apple learns here may influence how the industry designs and constrains medical AI. The available information is thin: Apple has not detailed the study's participant criteria, data-handling practices, or how findings will be published, and the app is described only as answering everyday medical questions. As with any health study, questions about privacy, consent, and whether results translate into shipping features remain open.

rss · TechCrunch · Nov 16, 01:30

**Background**: Apple has spent a decade building health capabilities into its devices, from heart-rate and ECG sensing on Apple Watch to the Health app and its ResearchKit framework for running large-scale medical studies. Meanwhile, general-purpose chatbots such as ChatGPT and Gemini have become common places for people to ask about symptoms and medications, raising concerns among clinicians about accuracy and safety. Apple's move fits both trends: using a research app to gather real-world evidence about AI health behavior before committing to product features.

**Tags**: `#Apple`, `#AI in healthcare`, `#health apps`, `#consumer AI`, `#medical AI`

---

<a id="item-10"></a>
## [Iran Reportedly Used US Troops' Social Media and Fitness App Data to Target Mideast Bases](https://www.scmp.com/news/world/middle-east/article/3374473/how-iran-used-us-troops-digital-footprints-hit-mideast-bases-billions-damage) ⭐️ 6.0/10

According to security experts and US military officials, Iran's military planners mined data from US service members' social media accounts, fitness apps and online advertising to build detailed 'patterns of life' for American bases across the Middle East, then combined that with imagery reportedly supplied by Russian satellites to select targets. The campaign reportedly caused billions of dollars in damage to those bases. The case is a concrete real-world demonstration that everyday commercial data — workout routes, social posts, ad-tech tracking — can be weaponized for military targeting, meaning ordinary service members' personal devices are now a genuine attack surface. It underscores that operational security (OPSEC) failures can translate directly into physical destruction and casualties, with implications for every military and organization whose personnel carry smartphones. The targeting picture was assembled from open sources rather than traditional espionage, reportedly pairing OSINT-derived pattern-of-life analysis with Russian satellite imagery; the article is journalistic reporting rather than a technical deep-dive, and its specific damage figures and Russian imagery claim rest on unnamed security experts and military statements that have not been independently verified in the piece.

rss · SCMP · Nov 15, 05:57

**Background**: Open-source intelligence (OSINT) is intelligence derived from publicly or commercially available information — social media, commercial imagery, ad data — and is increasingly a first resort that guides other collection methods. 'Pattern-of-life' analysis is a surveillance technique that documents habits and routines to predict future behavior, and analysts now fuse ad-tech, signals intelligence and social media data to build such profiles. The risks were famously illustrated in 2018, when Strava's public fitness heatmap revealed the locations of secret US military bases overseas.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Open-source_intelligence">Open-source intelligence - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pattern-of-life_analysis">Pattern-of-life analysis - Wikipedia</a></li>
<li><a href="https://www.theguardian.com/world/2018/jan/28/fitness-tracking-app-gives-away-location-of-secret-us-army-bases">Fitness tracking app Strava gives away location of... | The Guardian</a></li>

</ul>
</details>

**Tags**: `#opsec`, `#osint`, `#privacy`, `#cybersecurity`, `#geopolitics`

---