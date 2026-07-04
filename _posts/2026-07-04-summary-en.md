---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 125 items, 20 important content pieces were selected

---

1. [Politician investigating spyware hacked with Pegasus](#item-1) ⭐️ 9.0/10
2. [Costco as the Anti-Amazon: Warehouse vs Delivery](#item-2) ⭐️ 8.0/10
3. [SearXNG: A Free Privacy-Focused Metasearch Engine](#item-3) ⭐️ 7.0/10
4. [Jamesob's guide to running SOTA LLMs locally](#item-4) ⭐️ 7.0/10
5. [Factories are just rooms](#item-5) ⭐️ 7.0/10
6. [SiliconFlow Files for HK IPO with Negative Gross Margin](#item-6) ⭐️ 7.0/10
7. [Shengshu Tech Releases Vidu S1 Real-Time Interactive Model](#item-7) ⭐️ 7.0/10
8. [Peng Ding Holdings Plans $1.35B Raise for AI Server and Optical Module PCBs](#item-8) ⭐️ 7.0/10
9. [South Korea Plans 'Korean Starlink' by 2035, Moon Landing by 2030](#item-9) ⭐️ 7.0/10
10. [ByteDance discovers new scaling law for AI agents](#item-10) ⭐️ 7.0/10
11. [Alibaba bans Claude Code over spyware risks](#item-11) ⭐️ 7.0/10
12. [China's satellite engine sets record, surpasses US rival](#item-12) ⭐️ 7.0/10
13. [UN official warns of machine warfare, urges US-China dialogue on military AI](#item-13) ⭐️ 7.0/10
14. [BYD overtakes Tesla to reclaim global EV crown](#item-14) ⭐️ 7.0/10
15. [Li Auto restructures to cut layers, merging product definition into R&D](#item-15) ⭐️ 6.0/10
16. [Qihang Hydrogen Energy Raises Funding for Electric-Hydrogen Coupling](#item-16) ⭐️ 6.0/10
17. [Kleiner Perkins Partner on AI Investing and Lessons from Slack, Figma](#item-17) ⭐️ 6.0/10
18. [AI skills needed for 4 in 10 graduate jobs in China](#item-18) ⭐️ 6.0/10
19. [Experts urge fines for Hong Kong data breaches](#item-19) ⭐️ 6.0/10
20. [Hong Kong employee training hits 14-year high amid AI push](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Politician investigating spyware hacked with Pegasus](https://techcrunch.com/2026/07/02/politician-who-investigated-spyware-abuses-had-his-phone-hacked-with-pegasus-spyware/) ⭐️ 9.0/10

A European politician serving on an EU committee investigating spyware abuses had his iPhone infected with NSO Group's Pegasus spyware in October 2022 and March 2023, according to a forensic analysis by Citizen Lab. This incident demonstrates that even those tasked with investigating spyware are not immune to surveillance, raising serious concerns about the unchecked power of government surveillance and the ethical implications of commercial spyware. The infections were detected by Citizen Lab, which found evidence linking the first infection to a Pegasus campaign targeting Russian- and Belarusian-speaking exiled journalists in Europe. The politician's phone contained both confidential medical information and government documents.

rss · TechCrunch · Jul 3, 05:05

**Background**: Pegasus is spyware developed by Israeli company NSO Group, marketed for crime and terrorism prevention but widely used to target journalists, activists, and politicians. The sale of Pegasus requires approval from the Israeli Ministry of Defense. It can be installed remotely via zero-click exploits and can access messages, calls, passwords, and device sensors.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/NSO_Group">NSO Group</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the infection timeline overlaps with a known Pegasus campaign in Europe, and some pointed out that Greece and Poland have been implicated in spyware abuse. Others questioned why the politician used a single device for both personal and government work, highlighting poor security practices.

**Tags**: `#cybersecurity`, `#Pegasus`, `#NSO Group`, `#surveillance`, `#privacy`

---

<a id="item-2"></a>
## [Costco as the Anti-Amazon: Warehouse vs Delivery](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 8.0/10

A new analysis article contrasts Costco's warehouse club model with Amazon's home delivery model, highlighting the logistical and societal trade-offs between bulk store purchases and single-item door delivery. This comparison challenges the dominance of on-demand delivery by re-evaluating the hidden costs of last-mile logistics, such as increased vehicle trips and packaging waste, and raises questions about the social value of extreme convenience. The article notes that Costco deliberately avoids the last-mile shipping problem by having customers transport goods themselves, while Amazon relies on a complex delivery network for individual packages. This difference leads to entirely different cost structures and environmental impacts.

hackernews · bookofjoe · Jul 3, 15:14 · [Discussion](https://news.ycombinator.com/item?id=48776044)

**Background**: Costco operates as a membership-only warehouse club where customers buy in bulk at low prices and transport items home themselves. Amazon, on the other hand, offers vast product selection with rapid home delivery, often of single items. The article argues that the convenience of home delivery comes with hidden logistical complexity and social costs.

**Discussion**: Comments offer diverse perspectives: some compare the environmental efficiency of a single delivery truck vs individual car trips; others praise Costco's avoidance of the last-mile problem as wise engineering. One commenter notes that in the UK, Costco membership is technically restricted to businesses and certain professions. The discussion is largely US-centric but includes international viewpoints.

**Tags**: `#retail`, `#logistics`, `#Amazon`, `#Costco`, `#engineering philosophy`

---

<a id="item-3"></a>
## [SearXNG: A Free Privacy-Focused Metasearch Engine](https://github.com/searxng/searxng) ⭐️ 7.0/10

SearXNG is a free and open-source metasearch engine that aggregates results from multiple search services and databases while ensuring users are neither tracked nor profiled. It has gained significant attention as a self-hostable alternative for privacy-conscious users and as a backend for AI agents. SearXNG provides a practical solution for users seeking to reduce dependency on single search engines and improve privacy by distributing queries across multiple providers. It also enables integration with local AI models and RAG applications, extending its utility beyond simple web search. It is a fork of the discontinued Searx project and supports JSON output for programmatic use, making it suitable for integration with tools like TinySearch and YaCY. Users may experience slower results and occasional CAPTCHAs from certain backends like DuckDuckGo.

hackernews · theanonymousone · Jul 3, 20:15 · [Discussion](https://news.ycombinator.com/item?id=48779454)

**Background**: A metasearch engine acts as an aggregator, sending a single query to multiple underlying search engines (like Google, Bing, DuckDuckGo) and combining their results. Unlike traditional search engines, metasearch engines typically do not maintain their own index or collect user data, offering enhanced privacy. SearXNG is server-side software that can be hosted on a local network or public instance, giving users full control over their search data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SearXNG">SearXNG - Wikipedia</a></li>
<li><a href="https://github.com/searxng/searxng">GitHub - searxng/searxng: SearXNG is a free internet metasearch engine which aggregates results from various search services and databases. Users are neither tracked nor profiled. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metasearch_engine">Metasearch engine</a></li>

</ul>
</details>

**Discussion**: The community shows mixed sentiment: asciimoo, the original Searx creator, points out limitations of the metasearch concept and promotes his new project Hister—a full-text indexer. Others comment on privacy trade-offs (sending queries to many engines) and practical issues like speed and CAPTCHAs. Several users highlight its usefulness as a search backend for local AI agents and RAG applications.

**Tags**: `#metasearch`, `#privacy`, `#open-source`, `#search-engine`

---

<a id="item-4"></a>
## [Jamesob's guide to running SOTA LLMs locally](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob published a comprehensive guide on running state-of-the-art large language models (LLMs) locally, detailing build configurations ranging from $3,000 to $40,000 and beyond. This guide is valuable for enthusiasts and developers seeking to run LLMs privately without cloud reliance, but the high costs and quantization trade-offs revealed in community discussion underscore that local setups remain impractical for most users compared to cloud subscription services. The flagship ~$40K build includes four $12K GPUs, but commenters note the actual cost is more like $50-55K, and running models like 'almost Opus' may require $400K in H200s; alternatives like 2x RTX 3090s ($3K) or Apple M5 Max with 48GB unified memory ($3K) can run capable quantized models.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Local LLM inference requires significant GPU VRAM to store model weights and handle context. Quantization techniques reduce model memory footprint by converting 32-bit parameters to 8-bit or 4-bit integers, enabling larger models to fit on consumer hardware with minor quality loss. The guide and comments explore trade-offs between cost, quality, and hardware complexity.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@nageshchauhanc4/quantization-in-large-language-models-llms-8850b0b0395a">Quantization in Large Language Models (LLMs) | Medium</a></li>
<li><a href="https://overchat.ai/ai-hub/llm-hardware-requirements">Local LLM Hardware Requirements in 2026 | AI Hub</a></li>
<li><a href="https://llm-stats.com/blog/research/hardware-requirements-running-llms-locally">How to Calculate Hardware Requirements for Running LLMs Locally</a></li>

</ul>
</details>

**Discussion**: Commenters express caution: Aurornis warns about hidden costs and reliance on quantization; GTP suggests 128GB unified memory setups as a mid-range compromise; jacobgold calculates $40K equals 16.8 years of Claude Opus subscription, calling local models wildly expensive and possibly dangerous; datadrivenangel recommends cloud hosting over expensive builds.

**Tags**: `#local-llm`, `#hardware`, `#cost`, `#quantization`, `#alternatives`

---

<a id="item-5"></a>
## [Factories are just rooms](https://interconnected.org/home/2026/07/03/factories) ⭐️ 7.0/10

The article reflects on the idea that factories can be simple, room-like spaces, sharing personal anecdotes about hands-on manufacturing. It challenges the assumption that manufacturing requires large-scale infrastructure, potentially inspiring more individuals to engage in small-scale production. The post received high engagement with 178 points and 73 comments, indicating strong community interest in the topic.

hackernews · arbesman · Jul 3, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48776035)

**Background**: The maker movement and hacker culture have long promoted the idea that individuals can create physical goods in small workshops, echoing the 'factory as a room' concept discussed in the article.

**Discussion**: Commenters shared mixed experiences: some found joy in small-scale manufacturing, while others noted business sustainability challenges (e.g., rm445's company struggled to win consistent business).

**Tags**: `#manufacturing`, `#entrepreneurship`, `#hacker-culture`, `#discussion`

---

<a id="item-6"></a>
## [SiliconFlow Files for HK IPO with Negative Gross Margin](https://36kr.com/p/3879814941437956?f=rss) ⭐️ 7.0/10

SiliconFlow, a Chinese AI token supply platform founded in August 2023, filed for an IPO on the Hong Kong Stock Exchange under Chapter 18C for pre-commercial companies. Despite rapid user growth reaching over 10 million registered users, its gross margin turned negative at -24% in 2025, meaning it costs 1.24 yuan to generate 1 yuan of token revenue. As the largest independent token supplier in China by 2025 throughput, SiliconFlow's IPO reveals the intense price war and profitability challenges in AI inference infrastructure. Its negative gross margin highlights the difficulty of monetizing rapidly growing token traffic, which could influence investor sentiment toward AI infrastructure startups. In 2025, SiliconFlow's revenue was 55.33 million yuan while cost of sales was 68.63 million yuan, resulting in a gross loss of 13.30 million yuan. Computing resource rental accounted for 86.9% of sales costs, and R&D expenses were 209 million yuan, or 378% of revenue.

rss · 36氪 · Jul 3, 11:12

**Background**: SiliconFlow operates as an AI inference infrastructure company that aggregates heterogeneous computing resources (NVIDIA, AMD, Huawei Ascend, etc.) and supplies standardized token services via a self-built inference engine and orchestration system. The Hong Kong Stock Exchange's Chapter 18C listing rules, introduced in 2023, provide a pathway for specialist technology companies that may not yet meet traditional financial eligibility tests, allowing pre-commercial firms to list.

<details><summary>References</summary>
<ul>
<li><a href="https://app.dealroom.co/news/note/siliconflow-raises-2b-yuan-series-b-for-its-ai-token-factory">SiliconFlow raises 2B+ yuan Series B for its AI 'token factory' | Dealroom.co</a></li>
<li><a href="https://www.hkex.com.hk/Listing/Rules-and-Resources/Guidance/IPO/Listing-of-Specialist-Technology-Companies?sc_lang=en">Listing of Specialist Technology Companies - HKEX</a></li>
<li><a href="https://www.hkexgroup.com/Media-Centre/Insight/Insight/2026/HKEX-Insight/18C-Explained?sc_lang=en">18C, Explained - hkexgroup.com</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#IPO`, `#token supply`, `#startup`, `#SiliconFlow`

---

<a id="item-7"></a>
## [Shengshu Tech Releases Vidu S1 Real-Time Interactive Model](https://36kr.com/newsflashes/3879857819201798?f=rss) ⭐️ 7.0/10

Shengshu Technology has officially released the Vidu S1 real-time interactive model, enabling live video calls and voice-controlled video generation. Users can quickly create personalized interactive characters based on real humans, anime, and other initial images. This marks a significant step toward real-time interactive video generation, moving beyond static or pre-rendered AI video. It could revolutionize applications in virtual avatars, customer service, and entertainment by allowing natural conversational interaction. Vidu S1 supports 540P (960x540) resolution at 25 FPS (up to 42 FPS), and uses an autoregressive diffusion model (AR + Diffusion) to continuously predict and generate video content based on historical frames and voice commands. It also supports personalized voice cloning for consistent character identity.

rss · 36氪 · Jul 3, 11:55

**Background**: Traditional video generation models like Sora or Runway produce short clips offline with no user interaction during generation. Vidu S1 breaks this paradigm by enabling real-time, interactive video generation where the model responds to voice commands and can generate infinite-length continuous streams. Shengshu Technology is a Chinese AI startup focused on multimodal generative models, and Vidu is their video generation series.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/L0UPP1210511AQHO.html">刚刚，Vidu S1 重磅来袭，视频生成迈入实时交互时代！|全模态|vidu_网易订阅</a></li>
<li><a href="https://www.163.com/dy/article/L0URU4RA05118HA4.html">生数科技发布 Vidu S1，推动视频生成迈向“实时交互”新时代|大模型|vidu_网易订阅</a></li>

</ul>
</details>

**Tags**: `#AI视频生成`, `#实时交互`, `#多模态`, `#生数科技`

---

<a id="item-8"></a>
## [Peng Ding Holdings Plans $1.35B Raise for AI Server and Optical Module PCBs](https://36kr.com/newsflashes/3879823039901697?f=rss) ⭐️ 7.0/10

Peng Ding Holdings (鹏鼎控股) announced a private placement to raise up to 9.6 billion yuan (approximately $1.35 billion) for its Qing Ding AI server and high-speed optical module high-density interconnect (HDI) build-up board project. This significant investment highlights the growing demand for advanced PCB substrates critical for AI servers and high-speed optical communication, reflecting the industry's shift toward high-performance computing and data transmission infrastructure. The funds will be used specifically for the Qing Ding project, which focuses on HDI build-up boards—a key technology enabling miniaturization and high-speed signal integrity in AI servers and 800G/1.6T optical modules.

rss · 36氪 · Jul 3, 11:20

**Background**: High-Density Interconnect (HDI) PCBs use finer lines and spaces, smaller vias, and sequential lamination to pack more circuitry into a smaller footprint. HDI build-up boards are essential for AI servers that require high-speed data processing and for high-speed optical modules used in data centers. As AI and cloud computing drive demand for faster, denser interconnects, PCB manufacturers like Peng Ding are scaling up advanced substrate production.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pcbonline.com/blog/high-density-interconnect-pcb-for-ai-high-speed.html">High - Density Interconnect PCB for AI, High -Speed Network, etc.</a></li>
<li><a href="https://www.linkedin.com/pulse/high-density-interconnect-hdi-printed-circuit-boards-antti-rayming-mamwc">High - Density Interconnect ( HDI ) Printed Circuit Boards</a></li>

</ul>
</details>

**Tags**: `#AI servers`, `#optical modules`, `#PCB`, `#semiconductor`, `#fundraising`

---

<a id="item-9"></a>
## [South Korea Plans 'Korean Starlink' by 2035, Moon Landing by 2030](https://36kr.com/newsflashes/3879815486025993?f=rss) ⭐️ 7.0/10

South Korea announced plans to build a low-Earth orbit satellite communication network consisting of hundreds of satellites by 2035, and to advance its lunar landing target from 2032 to 2030. This initiative aims to enhance South Korea's national security and communication sovereignty while supporting the 6G era, positioning the country as a competitive player in global space technology. The low-orbit satellite network is considered core infrastructure for national security and the 6G era, and will also boost South Korea's satellite and launch vehicle development capabilities.

rss · 36氪 · Jul 3, 11:12

**Background**: South Korea established the Korea AeroSpace Administration (KASA) on May 27, 2024, to lead space policy and foster a private-sector-driven space industry. The country has been accelerating its space ambitions, including previous plans for a moon landing by 2032 and a Mars mission by 2045. Low-Earth orbit satellite constellations, like SpaceX's Starlink, are already commercially deployed for global broadband, and South Korea aims to create its own version to ensure independent communication infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://readhub.cn/topic/8ZvVm4MoK42">韩 国 宇 宙 航 空 厅 正式成立 将打造以民间为主的太 空 产业生态圈</a></li>
<li><a href="https://www.163.com/dy/article/J3SBNP9V05566R1T.html">163.com/dy/article/J3SBNP9V05566R1T.html</a></li>

</ul>
</details>

**Tags**: `#satellite communication`, `#6G`, `#space technology`, `#South Korea`, `#low-earth orbit`

---

<a id="item-10"></a>
## [ByteDance discovers new scaling law for AI agents](https://www.scmp.com/tech/big-tech/article/3359373/chinas-bytedance-discovers-new-scaling-law-could-sustain-ai-boom?utm_source=rss_feed) ⭐️ 7.0/10

ByteDance's Seed AI team published a paper revealing a new scaling law for AI agents, showing they can double their learning speed every three months through real-world task interaction. This discovery could sustain AI progress as traditional scaling laws based on model size and data are hitting limits, offering a new direction for continued improvement in AI capabilities. The scaling law was derived using a new benchmark called EdgeBench, which includes 134 tasks lasting 12 to 72 hours, with over 38,000 hours of agent runtime logged across five frontier models.

rss · SCMP · Jul 3, 22:00

**Background**: Scaling laws in AI are empirical rules that predict how model performance improves with increased compute, data, or parameters. OpenAI's 2020 scaling law showed that larger models consistently perform better. ByteDance's new law applies to AI agents, which are autonomous systems that perform tasks on behalf of humans, and focuses on learning from interaction rather than static training.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/tech/big-tech/article/3359373/chinas-bytedance-discovers-new-scaling-law-could-sustain-ai-boom">China’s ByteDance discovers new scaling law that could sustain AI ...</a></li>
<li><a href="https://researchaudio.io/p/test-time-compute-as-a-scaling-dimension">Test-time compute as a scaling dimension</a></li>
<li><a href="https://digg.com/tech/7gby8q0r">ByteDance - Seed releases EdgeBench, showing AI agent ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#scaling laws`, `#ByteDance`, `#AI agents`

---

<a id="item-11"></a>
## [Alibaba bans Claude Code over spyware risks](https://www.scmp.com/tech/big-tech/article/3359375/alibaba-bans-staff-using-claude-code-over-anthropic-spyware-concerns?utm_source=rss_feed) ⭐️ 7.0/10

Alibaba Group has banned its employees from using Anthropic's Claude Code for work, citing security risks related to hidden code that tracks users. This policy decision highlights growing security concerns in AI tool adoption by large enterprises, potentially influencing industry-wide usage restrictions. Claude Code was added to Alibaba's list of high-risk software after being discovered to carry backdoor vulnerabilities. The ban follows Anthropic's alleged prior use of hidden code to track Chinese users.

rss · SCMP · Jul 3, 14:15

**Background**: Claude Code is an AI coding agent developed by Anthropic that reads codebases, edits files, and runs commands in terminals and IDEs. The tool has faced scrutiny after allegations that its code included hidden tracking features targeting Chinese users, which raised concerns about backdoor risks and data privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#corporate policy`, `#Anthropic`, `#Claude`

---

<a id="item-12"></a>
## [China's satellite engine sets record, surpasses US rival](https://www.scmp.com/news/china/science/article/3359363/chinas-satellite-engine-smashes-record-leaves-us-rival-far-behind?utm_source=rss_feed) ⭐️ 7.0/10

China tested an upgraded satellite engine that fired for 11,617 seconds (3.2 hours) across five orbit-raising maneuvers, a record-breaking operating life that surpasses a US rival. This achievement demonstrates China's progress in electric propulsion technology, which is critical for efficient station-keeping and orbit-raising of large communications, military, and deep-space spacecraft. The engine, developed by the China Academy of Aerospace Propulsion Technology, produces 750 newtons of thrust and was tested in multiple maneuvers totaling over 3 hours of continuous operation.

rss · SCMP · Jul 3, 14:00

**Background**: Electric propulsion uses electrical power to ionize and accelerate propellant, offering higher efficiency than chemical rockets but lower thrust. Orbit-raising maneuvers use such engines to gradually change a satellite's altitude, reducing fuel consumption and enabling longer missions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spacecraft_electric_propulsion">Spacecraft electric propulsion - Wikipedia</a></li>
<li><a href="https://control.asu.edu/Classes/MAE462/462Lecture08.pdf">Spacecraft Dynamics and Control - Lecture 8: Impulsive Orbital ...</a></li>
<li><a href="https://economictimes.indiatimes.com/news/science/chandrayaan-3-a-timeline-and-all-the-milestones/orbit-raising-maneuvers/slideshow/102983654.cms">Orbit - raising maneuvers - Chandrayaan-3: A timeline and all the...</a></li>

</ul>
</details>

**Tags**: `#aerospace`, `#satellite`, `#propulsion`, `#China`, `#technology`

---

<a id="item-13"></a>
## [UN official warns of machine warfare, urges US-China dialogue on military AI](https://www.scmp.com/news/china/diplomacy/article/3359277/machine-warfare-coming-us-china-urged-address-military-ai-global-rules-stall?utm_source=rss_feed) ⭐️ 7.0/10

Robin Geiss, director of the United Nations Institute for Disarmament Research (UNIDIR), warned that machine warfare is imminent and called on the US and China to engage in pragmatic dialogue on military artificial intelligence, as global efforts to regulate lethal autonomous weapons systems (LAWS) remain stalled. This warning highlights the urgent need for international regulation of autonomous weapons, especially as the US and China are leaders in AI development. The lack of global rules increases the risk of an unregulated arms race in military AI. Geiss made the remarks during a lecture at Tsinghua University in Beijing. He emphasized the need for industry and the international community to shift from stalled multilateral convention talks to concrete dialogue on the safe and ethical use of AI in warfare.

rss · SCMP · Jul 3, 11:00

**Background**: The United Nations Institute for Disarmament Research (UNIDIR) is a research institute focused on disarmament and international security. Lethal autonomous weapons systems (LAWS) are weapon systems that can identify and engage targets without human control. The UN Secretary-General has called for a legally binding instrument to prohibit LAWS by 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UNIDIR">UNIDIR</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lethal_autonomous_weapon">Lethal autonomous weapon - Wikipedia</a></li>
<li><a href="https://disarmament.unoda.org/en/our-work/emerging-challenges/lethal-autonomous-weapon-systems">Lethal Autonomous Weapon Systems | United Nations Office for Disarmament Affairs</a></li>

</ul>
</details>

**Tags**: `#AI`, `#military`, `#regulation`, `#geopolitics`, `#ethics`

---

<a id="item-14"></a>
## [BYD overtakes Tesla to reclaim global EV crown](https://www.scmp.com/business/china-business/article/3359287/chinas-byd-surpasses-tesla-regain-lead-global-ev-race?utm_source=rss_feed) ⭐️ 7.0/10

BYD has surpassed Tesla to become the world's largest EV manufacturer, fueled by strong overseas shipments despite an 8.2% year-on-year drop in domestic deliveries. This signals China's growing dominance in the EV market and increasing global recognition of Chinese EV brands, challenging Tesla's leadership and reshaping the competitive landscape. BYD's achievement is driven by a surge in overseas shipments, while its domestic deliveries saw an 8.2% decline year-on-year. Tesla reported lower-than-expected deliveries in the same period.

rss · SCMP · Jul 3, 10:00

**Background**: BYD, a Chinese automaker, has been a major player in the EV market, previously holding the top spot before Tesla overtook it. The EV industry is highly competitive, with both companies vying for global leadership amid shifting market dynamics.

**Tags**: `#EV`, `#automotive`, `#BYD`, `#Tesla`, `#business`

---

<a id="item-15"></a>
## [Li Auto restructures to cut layers, merging product definition into R&D](https://36kr.com/p/3877919172047111?f=rss) ⭐️ 6.0/10

Li Auto is splitting its product department's core functions—electric vehicle definition and autonomous driving terminal product teams—and merging them into the R&D departments led by Liu Liguo and Zhan Kun, respectively, to shorten product decision cycles. This move streamlines decision-making, reducing three-layer approvals to two, which could accelerate product iteration and help Li Auto regain competitiveness in the increasingly crowded EV market. The reorganization specifically dismantles the platform product definition layer previously headed by Fan Haoyu, merging its core teams into the vehicle R&D and foundation model R&D groups, while the product line department under Liu Jie remains focused on commercial success.

rss · 36氪 · Jul 3, 10:45

**Background**: Li Auto had adopted a three-layer product decision structure inspired by Huawei in 2022, but this led to slow decision-making. CEO Li Xiang acknowledged the efficiency problem in late 2024, vowing to return to a startup management style. The restructuring is part of a series of organizational changes in 2025–2026 aimed at boosting agility amid intense competition from NIO, Xpeng, and Xiaomi.

<details><summary>References</summary>
<ul>
<li><a href="https://m.21jingji.com/article/20260703/herald/094484a41c67c2623d8f17a4418f5b74.html">理想汽车“ 动 刀”产品部 - 21财经</a></li>
<li><a href="https://36kr.com/p/3728358954564999">36kr.com/p/3728358954564999</a></li>

</ul>
</details>

**Tags**: `#Li Auto`, `#organizational restructuring`, `#automotive`, `#product development`, `#smart driving`

---

<a id="item-16"></a>
## [Qihang Hydrogen Energy Raises Funding for Electric-Hydrogen Coupling](https://36kr.com/p/3879274157928449?f=rss) ⭐️ 6.0/10

Xiamen Qihang Hydrogen Energy Technology Co., Ltd., spun off from Jiageng Innovation Laboratory, completed a new funding round led by Xiamen Gaoxin Investment. The funds will support R&D on key electric-hydrogen coupling equipment and off-grid hydrogen production technologies. This investment highlights growing interest in electric-hydrogen coupling solutions that can improve the efficiency and cost of green hydrogen production, a critical enabler for integrating variable renewable energy into the energy system. Qihang Hydrogen Energy has developed three product lines: IGBT hydrogen production power supplies, off-grid/microgrid hydrogen production solutions, and fuel cell inverters. Its power supplies span 30 kW to 20 MW, covering liquid-cooled and air-cooled routes, and it has partnered with over 50 electrolyzer manufacturers.

rss · 36氪 · Jul 3, 02:02

**Background**: Electric-hydrogen coupling refers to the integration of power electronics and electrolysis to efficiently convert renewable electricity into hydrogen. Off-grid hydrogen production systems operate independently from the main grid, using renewable sources and storage to produce hydrogen locally, which is especially useful in remote areas or for reducing grid dependency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.researchgate.net/publication/383444047_Hydrogen_Energy_in_Electrical_Power_Systems_A_Review_and_Future_Outlook">(PDF) Hydrogen Energy in Electrical Power Systems: A Review and...</a></li>
<li><a href="https://arxiv.org/pdf/2203.13951">Research on Flexibility Margin of Electric - Hydrogen Coupling Energy</a></li>
<li><a href="https://www.hovogen.com/post/off-grid-hydrogen-production-systems-powering-the-future-with-industrial-hydrogen-generators">Off - Grid Hydrogen Production Systems: Powering the Future with...</a></li>

</ul>
</details>

**Tags**: `#hydrogen energy`, `#power electronics`, `#green hydrogen`, `#startups`, `#renewable energy`

---

<a id="item-17"></a>
## [Kleiner Perkins Partner on AI Investing and Lessons from Slack, Figma](https://www.bloomberg.com/news/videos/2026-07-03/masters-in-business-with-mamoon-hamid-video) ⭐️ 6.0/10

In a Bloomberg interview, Kleiner Perkins partner Mamoon Hamid shares his approach to early-stage AI investing and reflects on his successful investments in Slack and Figma. This interview provides valuable insights into how a top venture capital firm evaluates AI startups, which is crucial for entrepreneurs and investors navigating the AI revolution. Hamid discusses both the investments Kleiner Perkins made and those they missed, offering a candid look at the decision-making process in early AI investing.

rss · Bloomberg Markets · Jul 3, 21:13

**Background**: Kleiner Perkins is a prominent Silicon Valley venture capital firm. Mamoon Hamid is a partner known for early investments in companies like Slack and Figma. This interview explores his perspective on AI as the next major technological shift.

**Tags**: `#AI`, `#venture capital`, `#investing`, `#Kleiner Perkins`

---

<a id="item-18"></a>
## [AI skills needed for 4 in 10 graduate jobs in China](https://www.scmp.com/economy/china-economy/article/3359328/ai-skills-required-4-out-10-graduate-jobs-china-says-recruitment-portal?utm_source=rss_feed) ⭐️ 6.0/10

According to Maimai, a Chinese recruitment portal, nearly 40% of job postings for fresh graduates in the first five months of 2025 mentioned AI skills, up from about 30% in the same period of 2024. This trend reflects the rapid integration of AI into Chinese businesses, making AI literacy a critical differentiator for new graduates entering the job market and reshaping hiring priorities across industries. Maimai, the platform that reported this data, has 120 million users in mainland China and is often compared to LinkedIn. The data covers job postings from January to May 2025.

rss · SCMP · Jul 3, 12:00

**Background**: Maimai is a professional networking and recruitment platform in China, similar to LinkedIn, with over 110 million verified professionals. As AI adoption accelerates across sectors such as manufacturing, finance, and tech, employers increasingly seek graduates who can work with AI tools, leading to a surge in job postings requiring AI-related skills.

<details><summary>References</summary>
<ul>
<li><a href="https://teamedupchina.com/maimai-the-closest-thing-to-linkedin-in-china/">Maimai (脉脉): The Closest Thing to LinkedIn in China - TeamedUp China</a></li>
<li><a href="https://www.octoplusmedia.com/china-linkedin-maimai-advertise-b2b-social-network-app/">Maimai: Market on China Version of Linkedin, Career and Social Networking Platform for B2B Collaboration</a></li>

</ul>
</details>

**Tags**: `#AI`, `#job market`, `#China`, `#skills`, `#recruitment`

---

<a id="item-19"></a>
## [Experts urge fines for Hong Kong data breaches](https://www.scmp.com/news/hong-kong/society/article/3359358/fine-firms-data-breaches-hong-kong-cybersecurity-experts-urge?utm_source=rss_feed) ⭐️ 6.0/10

Cybersecurity experts in Hong Kong have called for authorities to impose fines on companies that suffer data breaches, following a ransomware attack that encrypted personal data of over 1 million individuals linked to Shun Hing Group, a major appliance distributor. This push for financial penalties could lead to stronger data protection regulations in Hong Kong, potentially setting a precedent for holding companies accountable for security failures and better protecting consumer privacy. The breach was initially reported by Shun Hing Group on March 23, and the Office of the Privacy Commissioner for Personal Data has launched an investigation. The experts made their comments on Friday, the day after the investigation was announced.

rss · SCMP · Jul 3, 11:50

**Background**: Data breach fines are common in other jurisdictions like the EU under GDPR, but Hong Kong currently lacks such penalties. The call from experts highlights gaps in the city's data protection framework, which relies on voluntary compliance and corrective actions rather than punitive measures.

**Tags**: `#data breach`, `#cybersecurity`, `#regulation`, `#Hong Kong`, `#privacy`

---

<a id="item-20"></a>
## [Hong Kong employee training hits 14-year high amid AI push](https://www.scmp.com/news/hong-kong/hong-kong-economy/article/3359315/employee-training-hours-hong-kong-hit-14-year-high-amid-ai-push-survey?utm_source=rss_feed) ⭐️ 6.0/10

According to a survey by the Hong Kong Institute of Human Resource Management, average annual training hours per employee reached 19.4 in 2023, a 6.8% increase from the previous year and the highest in 14 years. The rise reflects a strategic push by Hong Kong companies to upgrade employee skills in AI and technology, signaling a response to rapid digital transformation. This trend could enhance workforce competitiveness and adaptability in a changing economy. The survey, conducted by the Hong Kong Institute of Human Resource Management, recorded 19.4 average annual training hours per employee, marking the second consecutive year of increase and the highest since at least 2010.

rss · SCMP · Jul 3, 08:54

**Background**: Hong Kong, as a global financial hub, is increasingly emphasizing technology adoption to maintain its competitive edge. The push for AI skills is part of wider efforts to reskill workers for the digital economy. The survey highlights the tangible impact of these initiatives on training investment.

**Tags**: `#AI`, `#training`, `#workforce`, `#Hong Kong`

---