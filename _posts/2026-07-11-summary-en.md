---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 112 items, 16 important content pieces were selected

---

1. [China's Long March-10B Reusable Rocket Recovery Stirs Space Race Debate](#item-1) ⭐️ 9.0/10
2. [Nvidia's Investments in CoreWeave and Nebius: Circular Financing?](#item-2) ⭐️ 8.0/10
3. [ClickHouse Scales PgBouncer 4x with so_reuseport and Peering](#item-3) ⭐️ 8.0/10
4. [Circle Receives OCC Approval to Establish Trust Bank](#item-4) ⭐️ 8.0/10
5. [CISA forced to improvise incident response playbook on the fly](#item-5) ⭐️ 8.0/10
6. [US Wealth Concentration: Top 10% Hold Vast Majority of Assets (Feb 2025)](#item-6) ⭐️ 8.0/10
7. [Prefer STRICT Tables in SQLite](#item-7) ⭐️ 7.0/10
8. [Chinese team develops wearable dopamine patch for depression, Parkinson's](#item-8) ⭐️ 7.0/10
9. [Southeast Asia’s scammers’ new disguise: your leader’s face](#item-9) ⭐️ 7.0/10
10. [ChangXin IPO, SK Hynix US Listing, OpenAI Agent Launch](#item-10) ⭐️ 6.0/10
11. [AI Flapping-Wing Robot Startup Raises Millions, Targets Consumers](#item-11) ⭐️ 6.0/10
12. [Zhipu CEO Tang Jie's Internal Letter: Focus on AGI Long-Term Goals, Not Short-Term Gains](#item-12) ⭐️ 6.0/10
13. [Phia Accused of Cookie Stuffing Affiliate Fraud](#item-13) ⭐️ 6.0/10
14. [Meta Removes Controversial Instagram AI Feature After Backlash](#item-14) ⭐️ 6.0/10
15. [AI's rising tide may not lift all economies](#item-15) ⭐️ 6.0/10
16. [China Warns Amateur AI Typhoon Forecasts May Be Illegal](#item-16) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [China's Long March-10B Reusable Rocket Recovery Stirs Space Race Debate](https://www.scmp.com/news/china/science/article/3360231/chinas-long-march-10b-rocket-feat-lights-social-media-spacex-set-lose-crown?utm_source=rss_feed) ⭐️ 9.0/10

China successfully recovered the first stage of its Long March-10B rocket during its maiden flight on July 10, 2026, using a sea-based net platform. This marks China as the second nation to achieve controlled recovery of an orbital-class rocket after SpaceX. This breakthrough demonstrates China's rapid progress in reusable rocket technology, potentially reducing launch costs and intensifying competition with SpaceX. It could accelerate commercial space developments, especially for satellite internet constellations. The Long March-10B is a two-stage partially reusable vehicle using kerosene/liquid oxygen for the first stage and methane/liquid oxygen for the second stage. Its first stage recovery employed a net on a ship, similar to some Falcon 9 landing techniques but adapted for sea recovery.

rss · SCMP · Jul 11, 13:00

**Background**: Reusable rockets significantly lower the cost of access to space by recovering and reusing the most expensive part of the launch vehicle. Prior to this, only SpaceX had successfully landed and reused orbital-class rocket stages. The Long March 10B is part of China's next-generation rocket family, which includes the crewed Long March 10 for lunar missions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Long_March_10B">Long March 10B - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Long_March_10">Long March 10 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Falcon_9_first-stage_landing_tests">Falcon 9 first-stage landing tests - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Social media reactions ranged from awe at China's rapid space development to speculation about an intensifying space race with the United States. Many users highlighted the technical achievement while others debated whether SpaceX's lead is under threat.

**Tags**: `#space technology`, `#reusable rockets`, `#China`, `#SpaceX`, `#aerospace`

---

<a id="item-2"></a>
## [Nvidia's Investments in CoreWeave and Nebius: Circular Financing?](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

An analysis reveals that Nvidia's investments in GPU cloud providers CoreWeave and Nebius may represent a circular financing strategy, where Nvidia's equity stakes help fund purchases of its own GPUs, but some argue it is a hedge against hyperscaler dominance. If circular financing is prevalent, it could inflate GPU demand artificially and create financial fragility in the AI infrastructure sector. Conversely, if it's strategic hedging, Nvidia secures alternatives to hyperscalers who are developing their own chips. Nvidia invested $2 billion for a 9% stake in CoreWeave, which plans $35 billion in CapEx in 2026—Nvidia's share is only 5.7% of that year's spending. The analysis also examines Nebius, an AI cloud company spun out of Yandex.

hackernews · adletbalzhanov · Jul 11, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48873836)

**Background**: The GPU boom has led to massive investments in data centers and cloud infrastructure. Nvidia, as the dominant GPU maker, has invested in specialized cloud providers known as 'neoclouds' like CoreWeave and Nebius. Critics raise concerns about circular financing, where Nvidia's investments help clients buy its GPUs, potentially inflating demand. Others view it as a strategic move to reduce reliance on major cloud providers like AWS, Azure, and Google Cloud.

<details><summary>References</summary>
<ul>
<li><a href="https://www.coreweave.com/">The Essential Cloud for AI | CoreWeave</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nebius_Group">Nebius Group - Wikipedia</a></li>
<li><a href="https://news.ycombinator.com/item?id=48873836">Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the...</a></li>

</ul>
</details>

**Discussion**: Commenters are split: some argue the circular financing narrative is overblown given Nvidia's small stake relative to CoreWeave's CapEx. Others focus on the economic profitability of GPU builds, suggesting metrics like token ROI and enterprise budgets are more relevant. There is skepticism about utilization rates and the risk of overbuild, with one commenter noting that capacity constraints may be a blessing if the AI bubble bursts.

**Tags**: `#AI hardware`, `#Nvidia`, `#GPU cloud`, `#financing`, `#market dynamics`

---

<a id="item-3"></a>
## [ClickHouse Scales PgBouncer 4x with so_reuseport and Peering](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse describes how they improved PgBouncer throughput by 4x by using the SO_REUSEPORT socket option to allow multiple PgBouncer processes to share a single port, and implementing peering between processes to handle query cancellations correctly. This optimization turns PgBouncer from a bottleneck into efficient plumbing, enabling database connection pooling to scale linearly with CPU cores. It is particularly valuable for high-throughput PostgreSQL deployments where connection pooler performance becomes the limiting factor. The key techniques are SO_REUSEPORT, which allows multiple sockets to bind to the same port for load distribution across processes, and peering, which forwards query cancellation requests to the correct process. ClickHouse Managed Postgres ships with this setup by default, as described in their blog post from July 1, 2026.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL that manages database connections to improve performance. The SO_REUSEPORT socket option, available since Linux 3.9, allows multiple processes to bind to the same address and port, enabling the kernel to distribute incoming connections across them. Peering in PgBouncer allows processes to share session information so that operations like query cancellation work correctly even when a connection lands on a different process.

<details><summary>References</summary>
<ul>
<li><a href="https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres">How we scale PgBouncer in ClickHouse Managed Postgres</a></li>
<li><a href="https://lwn.net/Articles/542629/">The SO_REUSEPORT socket option [LWN.net]</a></li>
<li><a href="https://www.pgbouncer.org/">PgBouncer - lightweight connection pooler for PostgreSQL</a></li>

</ul>
</details>

**Discussion**: Commenters suggested alternative scalable PgBouncer implementations like Odyssey and pgdog. Some asked about the peering mechanism and whether it is built-in and easy to set up, while others shared their own experiences of running multiple PgBouncer instances via Kubernetes.

**Tags**: `#PostgreSQL`, `#PgBouncer`, `#database`, `#connection pooling`, `#performance`

---

<a id="item-4"></a>
## [Circle Receives OCC Approval to Establish Trust Bank](https://36kr.com/newsflashes/3890740672838404?f=rss) ⭐️ 8.0/10

Circle announced that the U.S. Office of the Comptroller of the Currency (OCC) approved its application to establish a trust bank, named Circle National Trust Bank, allowing it to directly manage reserve assets backing its USDC stablecoin. This regulatory milestone enables Circle to hold and manage USDC reserves directly, reducing reliance on third-party custodians and enhancing transparency, which could strengthen confidence in USDC and set a precedent for stablecoin regulation. The trust bank license does not permit Circle to engage in commercial banking activities such as taking deposits or issuing loans; USDC's circulating supply exceeds $730 billion as of the announcement.

rss · 36氪 · Jul 11, 05:10

**Background**: A trust bank is a financial institution that acts as a trustee, managing assets on behalf of clients according to trust agreements. Previously, Circle relied on third-party banks and custodians to hold the cash and U.S. Treasury assets backing USDC. This approval allows Circle to serve as its own custodian, a significant step in operational independence.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wallstreetmojo.com/trust-bank/">Trust Bank Definition - What Is It, Account, Functions, History</a></li>
<li><a href="https://www.circle.com/blog/how-the-usdc-reserve-is-structured-and-managed">How the USDC Reserve is Structured and Managed | Circle</a></li>

</ul>
</details>

**Tags**: `#stablecoin`, `#regulation`, `#Circle`, `#USDC`, `#cryptocurrency`

---

<a id="item-5"></a>
## [CISA forced to improvise incident response playbook on the fly](https://techcrunch.com/2026/07/10/us-cyber-agency-cisa-had-to-build-its-incident-playbook-during-the-incident-agency-reveals/) ⭐️ 8.0/10

CISA revealed that it had to build its incident response playbook during a data exposure incident caused by a contractor's exposed credentials on a public GitHub repository. This incident exposes significant operational gaps in one of the world's leading cybersecurity agencies, undermining confidence in its preparedness and highlighting the need for more rigorous contractor oversight. The breach was discovered by GitGuardian, a secrets detection firm, and reported by cybersecurity journalist Brian Krebs in May 2026. The exposed repository contained passwords from a CISA contractor, forcing CISA to develop response procedures while handling the incident.

rss · TechCrunch · Jul 11, 01:01

**Background**: CISA (Cybersecurity and Infrastructure Security Agency) is the U.S. federal agency responsible for defending civilian government networks. An incident response playbook is a predefined set of procedures to guide actions during a cybersecurity incident. The fact that CISA lacked a ready playbook for this scenario suggests a failure in preparedness, especially given that contractor credential leaks are common.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cisa.gov/sites/default/files/2024-08/Federal_Government_Cybersecurity_Incident_and_Vulnerability_Response_Playbooks_508C.pdf">TLP:CLEAR Cybersecurity Incident & Vulnerability Response Playbooks</a></li>
<li><a href="https://www.gitguardian.com/">GitGuardian : Secrets Security and NHI Governance</a></li>
<li><a href="https://www.paloaltonetworks.com/cyberpedia/what-is-an-incident-response-playbook">What is an Incident Response Playbook? - Palo Alto Networks</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#incident response`, `#CISA`, `#data exposure`, `#GitHub`

---

<a id="item-6"></a>
## [US Wealth Concentration: Top 10% Hold Vast Majority of Assets (Feb 2025)](https://www.reddit.com/r/Economics/comments/1utkrv8/in_february_2025_the_top_10_owned_87_of_stocks_84/) ⭐️ 8.0/10

As of February 2025, the top 10% of Americans owned 87% of stocks, 84% of private businesses, 44% of real estate, and two-thirds of total wealth. This extreme concentration highlights persistent and growing wealth inequality in the United States, which can fuel policy debates around taxation, social mobility, and economic fairness. The data covers stocks, private businesses, real estate, and overall wealth, but does not include non-wealth measures like income or education.

reddit · r/economics · /u/clonedhuman · Jul 11, 13:54

**Tags**: `#wealth inequality`, `#economics`, `#United States`, `#wealth distribution`

---

<a id="item-7"></a>
## [Prefer STRICT Tables in SQLite](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

The article advocates enabling SQLite's STRICT table mode to enforce static typing, preventing accidental data type corruption. Since SQLite 3.37.0 (2021-11-27), users can declare tables with STRICT to require exact column types. SQLite's default flexible typing can silently store mismatched data, leading to hard-to-find bugs. Using STRICT tables aligns SQLite with other SQL databases' type safety, reducing data integrity risks in production applications. STRICT tables support only five core types: INT, REAL, TEXT, BLOB, and ANY. They also reject unrecognized column types and disallow multi-type affinity assumptions. The feature must be enabled per table, not globally.

hackernews · ingve · Jul 11, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48873940)

**Background**: SQLite traditionally uses dynamic typing, where a column's declared type is just a 'type affinity' that suggests how to store values but does not enforce it. This design choice, explained in SQLite's 'The Advantages Of Flexible Typing', allows flexibility but can lead to silent data corruption. STRICT tables, introduced in version 3.37.0, provide an opt-in rigid typing mode for users who prefer traditional SQL type enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://sqlite.org/flextypegood.html">The Advantages Of Flexible Typing</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>

</ul>
</details>

**Discussion**: Commenters generally support using STRICT tables, with one saying 'CREATE TABLE ... STRICT WITHOUT ROWID is my default.' Another notes they'd like STRICT to be the default, referencing a counterargument from SQLite's documentation about flexible typing. A third comment relates the trade-off to the networking choice between UDP and TCP, where flexibility adds complexity.

**Tags**: `#SQLite`, `#database`, `#type safety`, `#best practices`

---

<a id="item-8"></a>
## [Chinese team develops wearable dopamine patch for depression, Parkinson's](https://www.scmp.com/news/china/science/article/3360202/chinese-teams-wearable-dopamine-patch-could-be-used-track-depression-parkinsons?utm_source=rss_feed) ⭐️ 7.0/10

Scientists from the Shenyang Institute of Automation, Chinese Academy of Sciences, have developed a painless wearable patch that uses microneedles to rapidly and ultrasensitively monitor dopamine levels in interstitial fluid, potentially enabling at-home tracking of Parkinson's disease and depression. This innovation could transform chronic disease management by allowing patients to monitor neurotransmitter levels non-invasively and in real-time, reducing reliance on hospital visits and enabling early intervention for conditions like Parkinson's and depression. The patch employs microscopic needles that penetrate the skin painlessly to sample interstitial fluid, and the sensor demonstrates high sensitivity and rapid response, though it has not yet been validated in clinical settings.

rss · SCMP · Jul 11, 12:00

**Background**: Dopamine is a neurotransmitter crucial for movement, motivation, and reward; its dysregulation is linked to Parkinson's disease and depression. Microneedle-based biosensors are an emerging minimally invasive technology for painless transdermal monitoring, offering a promising alternative to blood draws for continuous biomarker tracking.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3360202/chinese-teams-wearable-dopamine-patch-could-be-used-track-depression-parkinsons">Chinese team’s wearable dopamine patch could be used to track depression</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10898425/">Biopolymer-protected graphene-Fe3O4 nanocomposite based wearable microneedle sensor: toward real-time continuous monitoring of dopamine - PMC</a></li>

</ul>
</details>

**Tags**: `#wearable`, `#dopamine sensor`, `#healthcare`, `#innovation`, `#neuroscience`

---

<a id="item-9"></a>
## [Southeast Asia’s scammers’ new disguise: your leader’s face](https://www.scmp.com/week-asia/economics/article/3360150/southeast-asias-scammers-new-disguise-your-leaders-face?utm_source=rss_feed) ⭐️ 7.0/10

Deepfake of Singapore's prime minister used in a scam that stole US$3.8 million from a victim via a fake Zoom meeting.

rss · SCMP · Jul 11, 00:00

**Tags**: `#deepfake`, `#cybersecurity`, `#fraud`, `#social engineering`

---

<a id="item-10"></a>
## [ChangXin IPO, SK Hynix US Listing, OpenAI Agent Launch](https://36kr.com/p/3890553690192384?f=rss) ⭐️ 6.0/10

ChangXin Memory Technologies, China's first dedicated memory chip IPO, revealed its underwriting syndicate including six major securities firms, with issuance scheduled for July 16. SK Hynix listed on Nasdaq via ADRs, surging nearly 13% on debut. OpenAI released ChatGPT Work, an AI agent powered by GPT-5.6 that can autonomously execute cross-application tasks for hours. ChangXin's IPO marks a milestone for China's domestic memory chip industry, while SK Hynix's US listing provides easier access for global investors to the AI-driven memory market. OpenAI's ChatGPT Work demonstrates significant progress in AI agent capabilities, enabling complex multi-step task automation. ChangXin's IPO is underwritten by CICC, CITIC Securities, Guotai Haitong, Guoyuan Securities, Huatai United, and China Merchants Securities, with several being shareholders. SK Hynix issued 177.9 million ADRs at $149 each, each representing one-tenth of a common share in Seoul. ChatGPT Work is a desktop app integrating chat, work, and Codex, capable of generating tables, slides, documents, and web apps.

rss · 36氪 · Jul 11, 01:24

**Background**: American Depositary Receipts (ADRs) allow non-US companies to trade shares on US exchanges, making it easier for US investors to buy foreign stocks. AI agents are software programs that can autonomously perform tasks by interacting with other applications and data sources, often using large language models. ChangXin is China's leading DRAM manufacturer, aiming to reduce reliance on foreign memory chips.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/美國存託憑證">美国存托凭证 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.221ai.cn/post/14733.html">ChatGPT 智 能 体 Agent - DeepSeek网页版</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#AI`, `#IPO`, `#memory chips`, `#OpenAI`

---

<a id="item-11"></a>
## [AI Flapping-Wing Robot Startup Raises Millions, Targets Consumers](https://36kr.com/p/3889516712065799?f=rss) ⭐️ 6.0/10

Embodied intelligence flapping-wing robot company 'Eagle Eye Smart Wing' has completed tens of millions of yuan in Series A funding, its third round in three months, led by Yuanhe Puhua. The company plans to launch its first consumer product, Eagle X, on Kickstarter in Q3 2025. This development signals a shift from ground-based embodied robots to aerial embodied intelligence, targeting a niche but potentially large consumer market. The use of a proprietary fluid simulation engine for reinforcement learning training could lower development costs and accelerate commercialization of flapping-wing robots. The company's first consumer product, Eagle X, has undergone over 3,000 hours of flight tests and emphasizes modularity with interfaces for user customization. The second industrial-grade product features approximately 15 degrees of freedom, enabling active airflow manipulation rather than passive gliding.

rss · 36氪 · Jul 11, 01:00

**Background**: Embodied AI refers to AI systems that perceive and act in the physical world through a body, often using sensors and actuators. Traditional quadrotor drones hover by fighting airflow with high-speed rotors, but flapping-wing robots mimic birds by leveraging aerodynamics for efficient flight. The startup's Vortrix engine simulates fluid dynamics in a virtual environment, allowing the robot to learn through reinforcement learning before real-world deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Embodied_cognition">Embodied cognition</a></li>
<li><a href="https://journals.sagepub.com/doi/10.1177/02783649251343638">A review on flapping-wing robots: Recent progress and ...</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#embodied AI`, `#flapping-wing`, `#startup`, `#funding`

---

<a id="item-12"></a>
## [Zhipu CEO Tang Jie's Internal Letter: Focus on AGI Long-Term Goals, Not Short-Term Gains](https://36kr.com/newsflashes/3891162734689031?f=rss) ⭐️ 6.0/10

On July 11, Zhipu CEO Tang Jie released an internal letter stating the company will not pursue short-term monetization but instead focus on AGI capabilities such as long-horizon tasks, autonomous agent systems, self-evolution, and extreme safety. The company's market value has entered the trillion-HKD club in June 2026. This signals a strategic commitment to foundational AGI research rather than rapid product deployment, potentially influencing the direction of the Chinese AI industry. It highlights the growing importance of long-horizon task capabilities and autonomous agents as key AGI milestones. Zhipu's open-source model GLM-5.2 has achieved core metrics comparable to or exceeding Claude Opus 4.8 and GPT-5.5, according to search results. The internal letter emphasizes 'Long Horizon Task' capability as the first milestone, drawing on Google DeepMind's report on AGI to ASI.

rss · 36氪 · Jul 11, 11:35

**Background**: AGI (Artificial General Intelligence) refers to AI that can perform any intellectual task that a human can. Long-horizon task capability means an AI can execute complex, multi-step tasks over extended periods. Autonomous agents are AI systems that can act independently to achieve goals. Zhipu AI is a leading Chinese AI company known for its GLM series of large language models.

<details><summary>References</summary>
<ul>
<li><a href="https://36kr.com/p/3891132709206784">独家 | 智 谱 创始人唐杰发内部信：「 GLM ...</a></li>
<li><a href="https://wallstreetcn.com/articles/3776707">智谱创始人唐杰发布内部信：将开启 Touch High...</a></li>
<li><a href="https://tech.ifeng.com/c/8uZA4GGxdfb">别睡了，Anthropic今天凌晨发的东西，可 能 是 AGI 竞赛的分水岭_凤凰网</a></li>

</ul>
</details>

**Tags**: `#AGI`, `#AI战略`, `#智谱AI`, `#行业动态`

---

<a id="item-13"></a>
## [Phia Accused of Cookie Stuffing Affiliate Fraud](https://techcrunch.com/2026/07/10/phia-accused-of-cookie-stuffing-taking-affiliate-credit-on-purchases-it-didnt-earn/) ⭐️ 6.0/10

Phia, a shopping startup co-founded by Bill Gates' daughter Phoebe Gates and Sophia Kianni, has been accused of using 'cookie stuffing' to fraudulently claim affiliate commissions on purchases it did not generate, according to a Bloomberg investigation. This case highlights unethical practices in affiliate marketing and raises questions about governance in high-profile startups, potentially affecting consumer trust in digital advertising and e-commerce platforms. Cookie stuffing involves dropping affiliate tracking cookies onto users' browsers without their knowledge, allowing the fraudster to claim credit for sales they didn't facilitate; Phia allegedly used this technique to earn commissions on purchases made through other affiliates.

rss · TechCrunch · Jul 11, 00:29

**Background**: Affiliate marketing is a performance-based advertising model where publishers earn commissions for driving sales or traffic. Cookie stuffing is a form of affiliate fraud where malicious affiliates drop cookies on users' devices to claim unearned commissions, often via hidden images or scripts. This practice is generally considered illegal and violates terms of most affiliate programs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cookie_stuffing">Cookie stuffing - Wikipedia</a></li>
<li><a href="https://www.crakrevenue.com/blog/cookie-stuffing-affiliate-marketing/">Understanding Cookie Stuffing in Affiliate Marketing | CrakRevenue</a></li>
<li><a href="https://www.anura.io/blog/how-to-fight-cookie-stuffing-within-affiliate-fraud">Combating Cookie Stuffing in Affiliate Fraud : Approaches and...</a></li>

</ul>
</details>

**Tags**: `#affiliate marketing`, `#ethics`, `#startup fraud`, `#cookie stuffing`

---

<a id="item-14"></a>
## [Meta Removes Controversial Instagram AI Feature After Backlash](https://techcrunch.com/2026/07/10/meta-removes-controversial-ai-feature-on-instagram-after-backlash/) ⭐️ 6.0/10

Meta has removed a controversial AI feature on Instagram that allowed users to modify photos from public accounts using AI, after facing widespread user backlash. The company acknowledged the feature 'missed the mark' and discontinued it. This incident highlights growing user concerns over data privacy and consent in AI-driven social media features. It also underscores the fine line platforms must walk between innovation and respecting user autonomy. The feature automatically opted in public Instagram profiles for AI image generation without explicit consent. This follows Meta's earlier admission in 2024 that it scraped public Facebook and Instagram posts since 2007 to train its generative AI model.

rss · TechCrunch · Jul 10, 23:55

**Background**: Generative AI models often require vast amounts of training data, and companies have sometimes used public social media content without clear user permission. This practice has sparked ethical debates about ownership and consent, especially when users are not informed their data could be used for AI training or modification features.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/10/meta-removes-controversial-ai-feature-on-instagram-after-backlash/">Meta removes controversial AI feature on Instagram after ...</a></li>
<li><a href="https://www.msn.com/en-us/news/technology/meta-removes-controversial-instagram-ai-photo-feature-after-social-media-backlash/ar-AA27FzC9">Meta removes controversial Instagram AI photo feature after ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Meta`, `#Instagram`, `#content moderation`, `#backlash`

---

<a id="item-15"></a>
## [AI's rising tide may not lift all economies](https://www.scmp.com/opinion/world-opinion/article/3360068/dont-expect-rising-tide-ai-lift-all-boats?utm_source=rss_feed) ⭐️ 6.0/10

An opinion piece argues that the AI revolution will primarily benefit economies linked to tech supply chains, while leaving others behind and potentially triggering financial crises. This highlights a critical policy challenge for governments, especially in Asia, as they navigate AI-driven growth and financial stability risks, with implications for global inequality. The piece references an International Monetary Fund report that signals potential financial crises alongside AI-driven growth, emphasizing the uneven distribution of benefits.

rss · SCMP · Jul 11, 08:30

**Background**: Artificial intelligence is expected to boost productivity and economic growth, but its benefits are likely concentrated in countries and sectors that produce or heavily use AI technologies. This could widen economic disparities between nations and within societies, while rapid adoption may also create financial instability through job displacement and asset bubbles.

**Tags**: `#AI`, `#economics`, `#technology policy`, `#finance`

---

<a id="item-16"></a>
## [China Warns Amateur AI Typhoon Forecasts May Be Illegal](https://www.scmp.com/news/china/science/article/3360171/typhoon-bavi-nears-chinese-bloggers-warned-amateur-ai-forecasts-may-be-illegal?utm_source=rss_feed) ⭐️ 6.0/10

Chinese state media has warned bloggers that using open-source AI weather models to issue typhoon forecasts on social media may violate the law, as Typhoon Bavi approaches eastern China. This highlights regulatory tensions between accessible AI technology and strict weather forecasting laws in China, potentially affecting the use of open-source AI for public safety communication. State broadcaster China Media Group reported that some 'weather enthusiasts' have been posting forecasts based on data from various open-source AI weather models, which could be illegal under Chinese law that restricts weather forecasting to authorized entities.

rss · SCMP · Jul 11, 00:00

**Background**: China has strict laws regulating weather forecasting, typically allowing only the China Meteorological Administration to issue official forecasts. Recently, open-source AI weather models like those from Microsoft's Aurora and Google DeepMind's WeatherNext have become accessible to the public, enabling amateurs to generate forecasts. This combination of accessible AI and strict regulation creates a potential legal conflict.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/HeQinWill/awesome-WeatherAI">GitHub - HeQinWill/awesome-WeatherAI: A curated list of ...</a></li>
<li><a href="https://blogs.microsoft.com/on-the-issues/2025/11/13/the-next-phase-of-aurora-open-and-collaborative-ai-for-weather-and-climate-forecasting/">The Next Phase of Aurora: Open and Collaborative AI for ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#weather forecasting`, `#China`, `#regulation`

---