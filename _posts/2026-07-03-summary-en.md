---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 155 items, 30 important content pieces were selected

---

1. [Virginia Bans Sale of Geolocation Data](#item-1) ⭐️ 8.0/10
2. [Linux 6.9 Regression: LUKS Suspend Fails to Wipe Encryption Keys from Memory](#item-2) ⭐️ 8.0/10
3. [Podman v6.0.0 Released with Networking Overhaul and Quadlet](#item-3) ⭐️ 8.0/10
4. [Nadkai Quantum Secures Funding for Neutral Atom Quantum Computer](#item-4) ⭐️ 8.0/10
5. [AI's energy hunger threatens tech giants' net-zero goals](#item-5) ⭐️ 8.0/10
6. [Anthropic Discusses Custom AI Chip with Samsung](#item-6) ⭐️ 8.0/10
7. [OpenAI Proposes 5% Equity Donation to US Sovereign Wealth Fund](#item-7) ⭐️ 8.0/10
8. [US government hacked again via Homeland Security network](#item-8) ⭐️ 8.0/10
9. [Microsoft launches AI deployment company with $2.5B commitment](#item-9) ⭐️ 8.0/10
10. [Exapunks (2018) discussion on Zachtronics legacy](#item-10) ⭐️ 7.0/10
11. [PeerTube: Decentralized Open Source Video Platform](#item-11) ⭐️ 7.0/10
12. [Guide to Asking Strangers for Help Effectively](#item-12) ⭐️ 7.0/10
13. [Former DJI Scientist's Startup SPARO Raises Hundreds of Millions in Four Rounds](#item-13) ⭐️ 7.0/10
14. [China Accelerates Small Modular Reactors for AI Data Centers](#item-14) ⭐️ 7.0/10
15. [Are Stablecoins Money? Policymakers Seek Safety and Utility](#item-15) ⭐️ 7.0/10
16. [Private space pilots fly orbital missions for US Space Force](#item-16) ⭐️ 7.0/10
17. [IQM goes public, admits quantum tech uncertainty](#item-17) ⭐️ 7.0/10
18. [China AI drug-design deals surge despite US scrutiny](#item-18) ⭐️ 7.0/10
19. [India orders WhatsApp to freeze username rollout](#item-19) ⭐️ 7.0/10
20. [Keldian Tech Raises Funding for AI Elderly Care Robots](#item-20) ⭐️ 6.0/10
21. [Meitu CEO on AI Product Strategy Driving Overseas Growth](#item-21) ⭐️ 6.0/10
22. [South Korea Considers $4B+ Tax Windfall for AI Models](#item-22) ⭐️ 6.0/10
23. [Spotify Asks Prediction Markets to Remove Logo After Chart Rigging](#item-23) ⭐️ 6.0/10
24. [Economist Uses AI to Assess Its Forecast Accuracy](#item-24) ⭐️ 6.0/10
25. [Meta quietly releases vibe-coded gaming app Pocket](#item-25) ⭐️ 6.0/10
26. [Boeing-owned Wisk Aero accused of firing safety whistleblower](#item-26) ⭐️ 6.0/10
27. [Indian entrepreneur invests $30M in AI office suite](#item-27) ⭐️ 6.0/10
28. [India Hackathon Challenges Silicon Valley AI Model](#item-28) ⭐️ 6.0/10
29. [Cyberattack on Shun Hing Group exposes 1M people's data](#item-29) ⭐️ 6.0/10
30. [CXMT's $4.3B IPO: AI boom meets US export threat](#item-30) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Virginia Bans Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

Virginia has enacted a ban on the sale of geolocation data, becoming one of the first states to specifically prohibit this practice to protect consumer privacy. This regulation directly targets data brokers who collect and sell location information without consent, potentially curbing abuses such as tracking visits to sensitive locations like Planned Parenthood. It sets a precedent for other states to follow, strengthening privacy protections. The law applies to the sale of geolocation data collected in Virginia, but enforcement may face challenges with out-of-state companies. The ban does not affect data collection for legitimate services like navigation, only its sale to third parties.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data refers to information that identifies the physical location of a device or person, often collected by apps and websites. Data brokers are companies that aggregate such personal data from various sources and sell it to third parties for marketing, risk assessment, or other purposes. In the US, there is no comprehensive federal privacy law, so state-level regulations like Virginia's are important steps toward protecting consumer privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Data_broker">Data broker</a></li>

</ul>
</details>

**Discussion**: Commenters generally support the ban, citing real-world examples of location data misuse, such as tracking at Planned Parenthood for anti-abortion ads and car insurance companies using driving behavior data. Some express concerns about enforcement and whether the law will effectively target bad actors without loopholes.

**Tags**: `#privacy`, `#geolocation`, `#data regulation`, `#law`, `#Virginia`

---

<a id="item-2"></a>
## [Linux 6.9 Regression: LUKS Suspend Fails to Wipe Encryption Keys from Memory](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

A regression in Linux kernel 6.9 caused the LUKS suspend functionality to stop wiping disk-encryption master keys from memory when the system is suspended to RAM. This security regression undermines the protection of full-disk encryption, as an attacker with physical access to a sleeping device could extract the master key from memory. The issue affects systems using cryptsetup's luksSuspend command, which relies on the kernel to wipe the dm-crypt key from memory; it was introduced in Linux 6.9 and has since been fixed.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a standard for disk encryption on Linux. When a LUKS-encrypted volume is unlocked, the master key is held in kernel memory. The cryptsetup luksSuspend command suspends the encrypted volume and typically wipes the master key from RAM to prevent exposure during sleep. The regression in Linux 6.9 broke this key wiping step.

<details><summary>References</summary>
<ul>
<li><a href="https://askubuntu.com/questions/95625/suspend-to-ram-and-encrypted-partitions">encryption - Suspend to RAM and encrypted partitions - Ask Ubuntu</a></li>
<li><a href="https://github.com/nailfarmer/debian-luks-suspend">GitHub - nailfarmer/debian- luks - suspend : Lock encrypted root volume...</a></li>

</ul>
</details>

**Discussion**: Commenters had mixed reactions: some considered the title clickbait since luksSuspend is a Debian-specific extension not widely tested, while others noted that such silent security regressions are easy to overlook. A few users were not particularly worried, as they rely on disk encryption mainly for data protection when disposing of hardware.

**Tags**: `#Linux`, `#security`, `#kernel`, `#encryption`, `#LUKS`

---

<a id="item-3"></a>
## [Podman v6.0.0 Released with Networking Overhaul and Quadlet](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 introduces significant networking improvements, including rootless networking without pause processes on Kernel 6.18+, and the stable integration of Quadlet for running containers as systemd services. The import path has moved to go.podman.io/podman/v6 as part of the CNCF transition. This release strengthens Podman's position as a leading Docker alternative by improving compatibility and security while reducing overhead. Quadlet simplifies container management for systemd users, potentially accelerating enterprise adoption. Networking enhancements include deterministic multi-network ordering and default network isolation for better Docker compatibility. Quadlet allows defining containers, pods, and volumes in systemd unit files, generating services automatically. Deprecated components like slirp4netns are replaced by Pasta.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is a daemonless container engine that can run containers rootlessly, often used as a Docker alternative. Quadlet is a tool that generates systemd unit files from container definitions, enabling integration with systemd for lifecycle management. This release marks a major version bump, indicating breaking changes like import path migration and removal of deprecated code.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/podman-container-tools/podman/releases/tag/v6.0.0">Release v6.0.0 · podman-container-tools/podman</a></li>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet</a></li>
<li><a href="https://fedoraproject.org/wiki/Changes/Podman6">Changes/Podman6 - Fedora Project Wiki</a></li>

</ul>
</details>

**Discussion**: Commenters praised Podman's ease of migration and Quadlet's utility, with some noting Docker's popularity despite Podman's technical superiority. However, concerns were raised about minor incompatibilities that could cause issues for projects expecting Docker-specific behavior. Overall sentiment is positive but cautious about compatibility.

**Tags**: `#podman`, `#containers`, `#docker-alternative`, `#devops`, `#container-runtime`

---

<a id="item-4"></a>
## [Nadkai Quantum Secures Funding for Neutral Atom Quantum Computer](https://36kr.com/p/3877814169530630?f=rss) ⭐️ 8.0/10

Nadkai Quantum, a Beijing-based startup founded by Peking University PhDs, completed its first round of financing of several million yuan led by GL Ventures, with participation from Inno, Changshi, and Feitu. The funds will be used to develop next-generation neutral atom quantum computers and ultracold atom quantum simulators. This marks the first Chinese company to achieve engineering-level neutral atom quantum computing at the nanokelvin scale, a promising path to scalable quantum computers. The strong academic background and early commercial traction signal potential impact on China's quantum computing ecosystem. The team can cool nine types of atoms (including rubidium, potassium, cesium, lithium, etc.) to below 10 nanokelvin, the widest range of atom species at such temperatures in China. They operate a dual-track business model: delivering dedicated quantum simulation systems to research institutions while developing general-purpose neutral atom quantum computers.

rss · 36氪 · Jul 2, 01:16

**Background**: Neutral atom quantum computers use lasers to trap and manipulate individual neutral atoms as qubits. Unlike superconducting qubits, neutral atoms are naturally identical, offering high scalability and low error correction overhead. Ultracold atoms at temperatures near absolute zero exhibit pronounced quantum effects, enabling precise control and high-fidelity operations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Neutral_atom_quantum_computer">Neutral atom quantum computer</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ultracold_atom">Ultracold atom - Wikipedia</a></li>
<li><a href="https://www.quera.com/neutral-atom-platform">Building Quantum Computers with Neutral Atoms | QuEra</a></li>

</ul>
</details>

**Tags**: `#quantum computing`, `#neutral atom`, `#startup funding`, `#quantum technology`, `#China`

---

<a id="item-5"></a>
## [AI's energy hunger threatens tech giants' net-zero goals](https://techcrunch.com/2026/07/02/a-warning-sign-about-ais-real-cost-courtesy-of-google-and-amazon/) ⭐️ 8.0/10

Tech giants like Google and Amazon are struggling to meet their net-zero emission targets due to the rapidly increasing energy demands of AI systems. This highlights a critical tension between AI advancement and corporate sustainability pledges, potentially forcing companies to choose between technological progress and environmental commitments. The massive computational power required for training and running large AI models significantly increases electricity consumption, making it harder for companies to offset their carbon footprints.

rss · TechCrunch · Jul 2, 19:14

**Background**: AI models, especially large language models, require immense amounts of energy for training and inference. This energy often comes from non-renewable sources, contributing to carbon emissions. Many tech companies have pledged to reach net-zero emissions by 2030 or 2040, but the growth of AI is making those targets more difficult to achieve.

**Tags**: `#AI`, `#sustainability`, `#net-zero`, `#energy consumption`, `#tech industry`

---

<a id="item-6"></a>
## [Anthropic Discusses Custom AI Chip with Samsung](https://techcrunch.com/2026/07/02/anthropic-is-discussing-a-new-custom-chip-with-samsung/) ⭐️ 8.0/10

Anthropic is reportedly in discussions with Samsung to develop a custom AI chip, mirroring OpenAI's recent partnership with Broadcom for its Jalapeño inference chip. This signals a growing trend among leading AI companies to invest in custom hardware to reduce dependence on NVIDIA GPUs and optimize performance and cost for AI inference. It could intensify competition in the AI chip market. The news comes about a week after OpenAI unveiled its custom AI inference chip named Jalapeño, built with Broadcom. Anthropic's discussions with Samsung are reportedly at an early stage, and no specific chip specifications have been disclosed.

rss · TechCrunch · Jul 2, 18:31

**Background**: Custom AI chips, known as ASICs (application-specific integrated circuits), are designed specifically for AI workloads like inference, offering higher efficiency than general-purpose GPUs. While NVIDIA GPUs dominate AI training, companies are increasingly turning to custom chips for inference to lower costs and power consumption. OpenAI's Jalapeño chip is a recent example of this trend.

<details><summary>References</summary>
<ul>
<li><a href="https://www.itechpost.com/articles/236458/20260625/openai-unveils-custom-ai-chip-openai-jalapeno-chip-built-broadcom-strengthen-ai-infrastructure.htm">OpenAI Unveils Custom AI Chip : OpenAI Jalapeño Chip Built With...</a></li>
<li><a href="https://www.nextpcb.com/blog/what-is-ai-asic-tpu-vs-gpu-comparison">What Is an AI ASIC ? TPU vs GPU vs ASIC for Machine Learning...</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#custom chip`, `#Anthropic`, `#Samsung`, `#industry trend`

---

<a id="item-7"></a>
## [OpenAI Proposes 5% Equity Donation to US Sovereign Wealth Fund](https://techcrunch.com/2026/07/02/openai-proposed-donating-5-of-its-equity-to-a-us-sovereign-wealth-fund/) ⭐️ 8.0/10

OpenAI CEO Sam Altman has proposed donating 5% of the company's equity to a U.S. sovereign wealth fund, aiming to share AI's financial gains with the public. This proposal could fundamentally shift AI governance by linking private AI profits to public wealth, potentially setting a precedent for other AI companies and addressing inequality concerns. The donation would consist of equity, not cash, and the sovereign wealth fund would be a state-owned investment fund. The proposal revives discussions about public participation in AI's economic benefits.

rss · TechCrunch · Jul 2, 15:20

**Background**: A sovereign wealth fund (SWF) is a state-owned investment fund that invests in assets like stocks, bonds, real estate, and alternative investments. Most SWFs are funded by commodity exports or foreign exchange reserves. The United States does not currently have a federal sovereign wealth fund, though proposals have been made by politicians including Donald Trump and Bernie Sanders.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sovereign_wealth_fund">Sovereign wealth fund</a></li>
<li><a href="https://www.investopedia.com/terms/s/sovereign_wealth_fund.asp">investopedia.com/terms/s/ sovereign _ wealth _ fund .asp</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI governance`, `#sovereign wealth fund`, `#AI equity`, `#public benefit`

---

<a id="item-8"></a>
## [US government hacked again via Homeland Security network](https://techcrunch.com/2026/07/02/us-government-says-it-got-hacked-again/) ⭐️ 8.0/10

A top Democrat on the Senate Intelligence Committee warned that a hack on the Homeland Security Information Network (HSIN) may risk national security. This incident highlights persistent vulnerabilities in government intelligence-sharing systems, potentially exposing sensitive but unclassified information to adversaries and undermining interagency collaboration. HSIN is a secure web-based platform used by federal, state, local, and tribal agencies to share Sensitive But Unclassified (SBU) information. The network has been hacked at least twice before in 2009.

rss · TechCrunch · Jul 2, 14:22

**Background**: The Homeland Security Information Network (HSIN) is a web-based platform launched in February 2004 by the Department of Homeland Security. It enables trusted sharing of Sensitive But Unclassified (SBU) information among government agencies. HSIN provides tools like SharePoint portals, Jabber chat, and a situational awareness application. Previous security breaches in 2009 show that the network has been a target for years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Homeland_Security_Information_Network">Homeland Security Information Network</a></li>
<li><a href="https://www.linkedin.com/pulse/understanding-dhs-networks-hsin-beyond-gary-ramah-o6awc">Understanding DHS Networks : HSIN and Beyond</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#government`, `#hacking`, `#national security`, `#intelligence`

---

<a id="item-9"></a>
## [Microsoft launches AI deployment company with $2.5B commitment](https://techcrunch.com/2026/07/02/microsoft-launches-its-own-ai-deployment-company-with-2-5-billion-commitment/) ⭐️ 8.0/10

On July 2, 2026, Microsoft announced the formation of the Microsoft Frontier Company, a new operating business dedicated to enterprise AI deployment, backed by a $2.5 billion investment and staffed with 6,000 engineers. This move follows similar initiatives by Amazon, OpenAI, and Anthropic, signaling that AI deployment has become a strategic priority for major tech firms and could accelerate enterprise adoption of artificial intelligence. The Microsoft Frontier Company will be led by Rodrigo Kede Lima and will embed engineers directly inside customer organizations to build and run AI systems, supported by the $2.5 billion commitment and a workforce of 6,000 industry and engineering experts.

rss · TechCrunch · Jul 2, 13:53

**Background**: AI deployment refers to integrating AI models into real-world systems to deliver value through automation, insights, or decision support. Microsoft already offers various AI tools, but the Frontier Company is specifically chartered to ensure successful large-scale deployments by providing hands-on engineering support.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/02/microsoft-launches-its-own-ai-deployment-company-with-2-5-billion-commitment/">Microsoft launches its own AI deployment company with $2.5 billion commitment | TechCrunch</a></li>
<li><a href="https://thenextweb.com/news/microsoft-frontier-company-2-5-billion-ai-deployment">Microsoft launches a $2.5 billion AI deployment business with 6,000 engineers</a></li>
<li><a href="https://www.geekwire.com/2026/microsoft-announces-2-5b-frontier-company-to-embed-ai-engineers-inside-customers/">Microsoft unveils $2.5B 'Frontier Company' to embed AI engineers inside customers – GeekWire</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#AI`, `#deployment`, `#investment`

---

<a id="item-10"></a>
## [Exapunks (2018) discussion on Zachtronics legacy](https://www.zachtronics.com/exapunks/) ⭐️ 7.0/10

A Hacker News post about Exapunks (2018) gained 207 points and 73 comments, focusing on the game's impact and Zachtronics' legacy in programming puzzle games. The discussion underscores how Zachtronics games demystify low-level programming and inspire careers, highlighting the enduring appeal of programming puzzles in the gaming community. Zach Barth continues game development under Coincidence Games with a new spacecraft engineering puzzle game UVS Nirmana. Exapunks features an in-game handheld console called Redshift for creating and sharing homebrew games.

hackernews · yu3zhou4 · Jul 2, 18:41 · [Discussion](https://news.ycombinator.com/item?id=48765663)

**Background**: Zachtronics is known for assembly-language puzzle games like TIS-100 and SHENZHEN I/O. Exapunks, released in 2018, challenges players to hack networks using a fictional assembly language in a retro computing environment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Exapunks">Exapunks - Wikipedia</a></li>
<li><a href="https://thinkygames.com/games/exapunks/">Exapunks · Thinky Games</a></li>
<li><a href="https://www.zachtronics.com/exapunks/">Zachtronics | EXAPUNKS</a></li>

</ul>
</details>

**Discussion**: Commenters express nostalgia for Exapunks and Shenzhen I/O, noting how they capture programming fun. One mentions Zach Barth's new studio Coincidence Games and UVS Nirmana, while another discusses developing a hybrid Zachtronics-Starcraft game.

**Tags**: `#programming games`, `#zachtronics`, `#puzzle games`, `#exapunks`, `#game design`

---

<a id="item-11"></a>
## [PeerTube: Decentralized Open Source Video Platform](https://github.com/Chocobozzz/PeerTube) ⭐️ 7.0/10

PeerTube is a free, decentralized, and federated video platform that uses peer-to-peer technology to distribute video content. However, it struggles with monetization and attracting a broad audience. PeerTube represents an alternative to centralized platforms like YouTube, offering greater control and privacy. Its success could reshape online video hosting, but monetization issues deter professional creators. PeerTube uses ActivityPub for federation, allowing instances to communicate. It also uses WebTorrent for peer-to-peer streaming to reduce server load. However, content discovery and audience size remain limited.

hackernews · doener · Jul 2, 11:17 · [Discussion](https://news.ycombinator.com/item?id=48759634)

**Background**: PeerTube is part of the Fediverse, a network of interconnected servers running federated software. It was developed by Framasoft in 2018 as an alternative to YouTube. Unlike centralized platforms, each PeerTube instance is independently operated, and content can be shared across instances via the ActivityPub protocol. This design promotes decentralization and user control.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ActivityPub">ActivityPub - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fediverse">Fediverse - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight monetization as a major barrier for professional creators, with one YouTuber noting the high production costs. Others point to the lack of audience and content in popular categories like gaming and music. Some users appreciate the open-source and privacy aspects but acknowledge social factors limit adoption.

**Tags**: `#decentralized`, `#video hosting`, `#federation`, `#open source`, `#peer-to-peer`

---

<a id="item-12"></a>
## [Guide to Asking Strangers for Help Effectively](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 7.0/10

A practical guide titled 'How to ask for help from people who don't know you' has been published, emphasizing proof of work, concise messaging, and setting realistic expectations. This guide provides actionable advice for professionals seeking to expand their network and receive assistance, addressing a common pain point in career development and collaboration. The author advises demonstrating proof of work upfront to show seriousness, keeping requests brief, and understanding that most strangers are more willing to help than assumed.

hackernews · FigurativeVoid · Jul 2, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48761118)

**Background**: When reaching out to strangers for help, common mistakes include long, unspecific requests and failing to show prior effort. The concept of 'proof of work' means demonstrating that you have already tried to solve the problem yourself, which increases the likelihood of a positive response.

**Discussion**: Commenters shared personal experiences, noting that over-investing in proof of work can backfire; short, targeted emails often work better. Others highlighted misjudging how often people are asked for help, and emphasized that proof of work must be substantive, not just surface-level.

**Tags**: `#networking`, `#career advice`, `#communication`, `#professional development`

---

<a id="item-13"></a>
## [Former DJI Scientist's Startup SPARO Raises Hundreds of Millions in Four Rounds](https://36kr.com/p/3877830625046535?f=rss) ⭐️ 7.0/10

SPARO (Silicon Feather Technology), founded by former DJI senior scientist Zhang Fu, has completed four consecutive funding rounds totaling hundreds of millions of yuan within six months, backed by investors including Yao Capital, Jinqiu Capital, Alibaba, and Hony Capital. SPARO's rapid funding signals strong market confidence in general aerial intelligence, a field that aims to evolve drones from remote-controlled tools into autonomous agents capable of understanding, reasoning, and manipulating environments — a potential paradigm shift for the low-altitude economy and embodied AI. SPARO claims centimeter-level localization without GPS, obstacle avoidance latency under 5 milliseconds, and a World Navigation Model that understands spatial semantics and dynamics. It has already accumulated dozens of seed customers including drone and logistics companies.

rss · 36氪 · Jul 2, 01:33

**Background**: SPARO is building a full-stack aerial intelligence system including multimodal perception, an end-to-end 'cerebellum' for low-latency control, and a 'World Navigation Model' brain that predicts how spaces behave. The company aims to enable drones to operate in GPS-denied, low-light, or dynamic environments and perform tasks like repair or cleaning. Its founder Zhang Fu is a top robotics researcher globally, previously at DJI and now a tenured associate professor at the University of Hong Kong.

<details><summary>References</summary>
<ul>
<li><a href="https://m.sohu.com/a/1044642804_118792?scm=10001.325_13-325_13.0.0-0-0-0-0.5_1334">全明星资本押注，半年四轮融资：硅羽科技定义“空中智能体”_搜狐网</a></li>
<li><a href="https://hub.baai.ac.cn/view/50075">全球首个「导航大脑」上线！一句话让机器人自己找路回家 - 智源社区</a></li>

</ul>
</details>

**Tags**: `#drones`, `#autonomous systems`, `#robotics`, `#AI`, `#venture capital`

---

<a id="item-14"></a>
## [China Accelerates Small Modular Reactors for AI Data Centers](https://36kr.com/newsflashes/3879130252636162?f=rss) ⭐️ 7.0/10

Chinese energy authorities recently held a meeting to accelerate the development of small modular nuclear reactors (SMRs), with experts and officials discussing their potential to power AI data centers as a stable zero-carbon energy source. As AI compute loads surge, intermittent renewables like wind and solar struggle to provide stable power, making SMRs a promising solution for data center energy needs. If successful, this could significantly reduce carbon emissions while supporting the AI boom. SMRs are nuclear reactors under 300 MWe that can be factory-built and scaled modularly. The recent meeting, reported by Shanghai Securities News, featured experts analyzing the integration path of SMRs with AI data centers, and the authorities urged rapid progress on demonstration projects.

rss · 36氪 · Jul 2, 23:35

**Background**: Small modular reactors (SMRs) are advanced nuclear reactors with a power capacity of up to 300 MW per unit, designed for modular construction and passive safety. AI data centers face soaring electricity demand, with Gartner predicting up to 160% growth in data center power consumption over two years. SMRs offer stable, zero-carbon power that can be located behind the meter, bypassing grid limitations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Small_modular_nuclear_reactor">Small modular nuclear reactor</a></li>
<li><a href="https://www.iaea.org/newscenter/news/what-are-small-modular-reactors-smrs">What are Small Modular Reactors (SMRs)? | IAEA</a></li>
<li><a href="https://colinmcnamara.netlify.app/energy-challenges-for-ai-data-centers-bridging-the-gap-between-demand-and-sustainability/">Energy Challenges for AI Data Centers : Bridging the Gap Between...</a></li>

</ul>
</details>

**Tags**: `#small modular reactors`, `#AI infrastructure`, `#data center energy`, `#nuclear power`, `#zero-carbon`

---

<a id="item-15"></a>
## [Are Stablecoins Money? Policymakers Seek Safety and Utility](https://www.economist.com/finance-and-economics/2026/07/02/are-stablecoins-money) ⭐️ 7.0/10

The Economist published an article questioning whether stablecoins qualify as money, emphasizing that policymakers should ensure both safety and utility. This debate shapes future stablecoin regulation and could influence their adoption in global finance, affecting monetary policy and financial stability. The article does not take a definitive stance but highlights the dual obligation of regulators to foster innovation while protecting consumers.

rss · The Economist · Jul 2, 09:37

**Background**: Stablecoins are cryptocurrencies designed to maintain a stable value, typically pegged to fiat currency like the US dollar. They come in various types: fiat-collateralized, crypto-collateralized, algorithmic, and hybrid. Their classification and regulatory treatment are critical as they bridge traditional finance and crypto.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gemini.com/cryptopedia/what-are-stablecoins-how-do-they-work">What Are Stablecoins and How Do They Work ? | Gemini</a></li>
<li><a href="https://web3.gate.com/learn/articles/2026-stablecoin-classification-deep-dive-from-fiat-collateralized-to-algorithmic-stablecoins-market-landscape-and-future-trends/15457">Stablecoin Classification 2026: Fiat -Backed, Crypto - Collateralized ...</a></li>

</ul>
</details>

**Tags**: `#stablecoins`, `#cryptocurrency`, `#monetary policy`, `#regulation`

---

<a id="item-16"></a>
## [Private space pilots fly orbital missions for US Space Force](https://techcrunch.com/2026/07/02/private-space-pilots-are-flying-orbital-missions-for-the-us-space-force/) ⭐️ 7.0/10

True Anomaly and Rocket Lab are conducting orbital satellite inspections for the US Space Force, marking a significant integration of private space capabilities into military operations. This demonstrates growing trust in commercial space companies for national security missions, potentially accelerating private-sector involvement in space defense and surveillance. The missions involve 'Top Gun-style' satellite fly-bys, where private spacecraft approach and inspect other satellites in orbit, gathering data on their condition and behavior.

rss · TechCrunch · Jul 2, 23:01

**Background**: Orbital satellite inspections are maneuvers where one spacecraft approaches another to assess its health, spin rate, surface conditions, or potential hazards. Traditionally conducted by government agencies, private companies like True Anomaly (focused on space defense) and Rocket Lab (end-to-end space services) are now offering these capabilities to the military.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Satellite">Satellite - Wikipedia</a></li>
<li><a href="https://www.trueanomaly.space/">True Anomaly - Delivering Decisive Capabilities for Space Superiority.</a></li>
<li><a href="https://rocketlabcorp.com/">Rocket Lab | The Space Company | Rocket Lab</a></li>

</ul>
</details>

**Tags**: `#space`, `#defense`, `#private aerospace`, `#satellite operations`

---

<a id="item-17"></a>
## [IQM goes public, admits quantum tech uncertainty](https://techcrunch.com/2026/07/02/iqm-europes-first-public-quantum-company-admits-the-future-of-the-tech-is-uncertain/) ⭐️ 7.0/10

IQM, Europe's first public quantum computing company, listed on Nasdaq at a valuation of approximately $1.9 billion and acknowledged the uncertain future of quantum technology. This IPO marks a significant milestone for the quantum computing industry in Europe, but the admission of uncertainty reflects the speculative nature of the technology, which could temper investor enthusiasm and set realistic expectations. IQM is a full-stack quantum computing company based in Finland, and its listing on Nasdaq gives it a valuation of $1.9 billion, making it Europe's first publicly traded quantum firm.

rss · TechCrunch · Jul 2, 20:42

**Background**: Quantum computing aims to leverage quantum mechanics to perform certain calculations much faster than classical computers. While it promises breakthroughs in cryptography, drug discovery, and optimization, the technology is still in early development and faces significant technical hurdles. IQM's IPO highlights growing commercial interest, but its candid acknowledgment of uncertainty underscores the long road ahead.

**Tags**: `#quantum computing`, `#IPO`, `#IQM`, `#technology uncertainty`

---

<a id="item-18"></a>
## [China AI drug-design deals surge despite US scrutiny](https://www.scmp.com/business/china-business/article/3359182/china-ai-drug-design-deals-swell-us-scrutiny-mounts?utm_source=rss_feed) ⭐️ 7.0/10

Chinese AI-driven drug-design firms have seen out-licensing deals with global pharmaceutical companies surge to $75 billion in the first five months of 2026, from nearly zero before 2020. This boom indicates Chinese AI biotech firms are becoming key players in global drug discovery despite rising geopolitical tensions and US scrutiny of Chinese biotech. The data, reported by HSBC's Linda Shu, shows a rapid increase from zero before 2020 to $75 billion in just five months of 2026, reflecting a transformative shift in cross-border dealmaking.

rss · SCMP · Jul 2, 11:00

**Background**: AI-driven drug design uses machine learning to accelerate the discovery and development of new drugs by predicting molecular properties and optimizing candidates. Out-licensing deals allow Chinese biotech firms to partner with global pharmaceutical companies to commercialize their innovations, while US scrutiny refers to heightened regulatory and investment reviews on Chinese biotech due to national security concerns.

**Tags**: `#AI`, `#drug discovery`, `#biotech`, `#China`, `#business`

---

<a id="item-19"></a>
## [India orders WhatsApp to freeze username rollout](https://www.scmp.com/news/asia/southeast-asia/article/3359148/india-orders-whatsapp-halt-username-feature-over-anonymity-concerns?utm_source=rss_feed) ⭐️ 7.0/10

The Indian government has ordered WhatsApp to halt the rollout of its new username feature, citing concerns that it could enable anonymity and facilitate cybercrime. This action escalates India's crackdown on messaging anonymity after similar moves against Telegram, and could affect over 500 million WhatsApp users in India, with implications for privacy and cybersecurity debates. WhatsApp's username feature lets users be contacted without sharing their phone number, which the Indian government argues could be exploited by scammers and cybercriminals. The government has asked WhatsApp to freeze the rollout until it can address these concerns.

rss · SCMP · Jul 2, 07:23

**Background**: WhatsApp traditionally uses phone numbers as user identifiers, which ties identity to a verified number. The username feature was designed to offer more privacy by allowing users to communicate without revealing their phone number. India has been increasingly regulating messaging platforms, citing the need to trace malicious actors. Earlier in 2026, India also cracked down on Telegram for similar anonymity features.

<details><summary>References</summary>
<ul>
<li><a href="https://www.devdossier.in/blog/whatsapp-username-feature-explained">WhatsApp Username Feature Explained: Hide Your Phone Number...</a></li>
<li><a href="https://www.bitdefender.com/en-us/blog/hotforsecurity/whatsapp-usernames-explained-how-to-reserve">WhatsApp usernames explained</a></li>
<li><a href="https://www.cfr.org/podcasts/why-it-matters/whatsapp-india">WhatsApp With India? | Council on Foreign Relations</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#regulation`, `#whatsapp`, `#cybersecurity`

---

<a id="item-20"></a>
## [Keldian Tech Raises Funding for AI Elderly Care Robots](https://36kr.com/p/3877863381741577?f=rss) ⭐️ 6.0/10

Shenzhen-based Keldian Technology completed a strategic funding round led by Leaguer Innovation, with plans to develop rehabilitation transport and home companion robots for elderly care. The company's GR-150 rehabilitation robot, co-developed with West China Hospital, uses SLAM and multi-sensor fusion for autonomous navigation. As China's aging population grows, the elderly care robotics market is expected to reach 30 trillion yuan by 2035. Keldian's focus on both institutional and home scenarios positions it to address critical care gaps and potentially lead the emerging sector. The GR-150 robot targets medical and care facilities for transporting disabled patients, while the second-generation home companion robot integrates health monitoring, emotional companionship, and fall detection. The company expects to finalize products by Q3 2026 and begin mass production in Q1 2027.

rss · 36氪 · Jul 2, 02:07

**Background**: SLAM (Simultaneous Localization and Mapping) enables a robot to build a map of an unknown environment while tracking its own location in real time. Multi-sensor fusion combines data from various sensors (e.g., cameras, LiDAR, IMU) to improve accuracy and robustness. These technologies are critical for autonomous navigation in elderly care robots.

<details><summary>References</summary>
<ul>
<li><a href="https://www.yumpu.com/en/document/view/28324385/slamsimultaneous-localization-and-mapping">SLAM : Simultaneous Localization And Mapping</a></li>
<li><a href="https://blogs.curiositytech.in/day-18-autonomous-robots-navigation-slam-techniques/">Day 18 – Autonomous Robots: Navigation & SLAM Techniques...</a></li>

</ul>
</details>

**Tags**: `#elderly care`, `#robotics`, `#AI`, `#healthcare`, `#funding`

---

<a id="item-21"></a>
## [Meitu CEO on AI Product Strategy Driving Overseas Growth](https://36kr.com/p/3877112973733895?f=rss) ⭐️ 6.0/10

Meitu CEO Wu Xinhong revealed in an interview that AI-reconstructed imaging and design products now account for 76.6% of revenue, up from 35% a year ago, driving 2025 net profit up 64.7% to 965 million yuan. Overseas MAU returned to 100 million, fueled by AI tools like Wink and RoboNeo. This shows how a traditional Chinese tech company successfully pivoted to AI, achieving profitable growth through organizational agility and a bottom-up product innovation model. It offers a roadmap for other consumer-tech firms navigating the AI wave. Meitu set up small AI innovation studios with up to 10 million yuan per team, built a middle platform for imaging and growth, and enforces a strict product validation cadence: from idea to launch within one month, and ARR must reach $100,000 within six months. The company also forbids legacy apps from aggressively cross-promoting new products.

rss · 36氪 · Jul 2, 00:30

**Background**: Meitu, once known for its photo-editing app MeituXiuxiu, struggled with monetization until subscriptions became mainstream. The company has since pivoted to AI products targeting overseas markets, leveraging tools like Wink (AI video enhancer) and a middle-platform strategy to accelerate development and reuse components across products.

<details><summary>References</summary>
<ul>
<li><a href="https://wink.ai/">Wink AI - Video and Image Enhancer & Editor for All Scenes</a></li>

</ul>
</details>

**Tags**: `#AI strategy`, `#business transformation`, `#overseas expansion`, `#generative AI`

---

<a id="item-22"></a>
## [South Korea Considers $4B+ Tax Windfall for AI Models](https://36kr.com/newsflashes/3879140914753795?f=rss) ⭐️ 6.0/10

South Korea is considering using approximately 5 trillion won (about $3.8 billion) in incremental tax revenue from the semiconductor boom to fund the development of its own AI models, including purchasing 10,000 Nvidia Vera Rubin GPUs and recruiting AI talent. This substantial government investment signals South Korea's ambition to reduce reliance on foreign AI models and strengthen its AI ecosystem. If realized, it could accelerate the country's AI capabilities and set a precedent for other nations seeking to build sovereign AI infrastructure. The plan is reported to involve the Ministry of Science and ICT using the windfall tax revenue to procure around 10,000 Nvidia Vera Rubin GPU modules, which are next-generation AI accelerators expected to ship in the second half of 2026. The initiative also includes recruiting AI talent to support the development.

rss · 36氪 · Jul 2, 23:46

**Background**: South Korea's semiconductor industry, led by Samsung and SK Hynix, has generated significant tax revenue due to high demand for memory chips. The government sees an opportunity to reinvest part of that windfall into AI development. Nvidia's Vera Rubin is the successor to the Blackwell architecture, designed for massive AI workloads, and is expected to deliver tenfold improvements in token cost and bandwidth.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pcgamer.com/hardware/graphics-cards/nvidias-new-six-trillion-transistor-vera-rubin-superchip-for-ai-makes-the-92-billion-transistor-rtx-5090-gaming-gpu-look-positively-puny/">Nvidia 's new six-trillion transistor Vera Rubin 'superchip... | PC Gam...</a></li>
<li><a href="https://www.networkworld.com/article/3848394/nvidia-details-its-gpu-cpu-and-system-roadmap-for-the-next-three-years.html">Nvidia details its GPU , CPU, and system roadmap for... | Network World</a></li>

</ul>
</details>

**Tags**: `#AI`, `#government funding`, `#Nvidia`, `#GPU`, `#South Korea`

---

<a id="item-23"></a>
## [Spotify Asks Prediction Markets to Remove Logo After Chart Rigging](https://www.bloomberg.com/news/articles/2026-07-02/spotify-challenges-prediction-markets-after-song-chart-rigging) ⭐️ 6.0/10

Spotify has requested that prediction markets Kalshi and Polymarket remove its logo and clarify that they have no partnership with Spotify, after identifying users manipulating song chart rankings tied to prediction market bets. This highlights the vulnerability of streaming charts to manipulation when linked to financial incentives, and raises questions about the integrity of prediction markets and their impact on real-world platforms. The manipulation involved users artificially inflating song streams on Spotify to influence outcomes of prediction market contracts on Kalshi and Polymarket, which likely offered odds on chart positions.

rss · Bloomberg Markets · Jul 2, 19:58

**Background**: Prediction markets like Kalshi (regulated) and Polymarket (crypto-based) allow users to bet on future events, including song chart positions. Spotify's charts are based on streaming counts, which can be gamed. The company is now protecting its brand by distancing itself from these platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://kalshi.com/">Kalshi - Prediction Market for Trading the Future</a></li>
<li><a href="https://en.wikipedia.org/wiki/Polymarket">Polymarket - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Spotify`, `#prediction markets`, `#chart manipulation`, `#streaming`, `#Kalshi`

---

<a id="item-24"></a>
## [Economist Uses AI to Assess Its Forecast Accuracy](https://www.economist.com/interactive/finance-and-economics/2026/07/02/is-the-economist-always-wrong) ⭐️ 6.0/10

The Economist has published an interactive article using artificial intelligence to systematically test the accuracy of its own forecasts over the years. This self-reflection by a reputable publication provides a novel look at media forecasting reliability, potentially influencing how readers and journalists evaluate predictions. The AI-driven analysis likely examined a range of economic and political predictions, comparing them against actual outcomes to measure accuracy.

rss · The Economist · Jul 2, 14:22

**Background**: The Economist is a weekly magazine known for its analysis of global affairs, including frequent forecasts on economics, politics, and technology. This project leverages AI to conduct a large-scale audit of its own past predictions, which is unusual for established media outlets.

**Tags**: `#AI`, `#forecasting`, `#journalism`, `#data analysis`

---

<a id="item-25"></a>
## [Meta quietly releases vibe-coded gaming app Pocket](https://techcrunch.com/2026/07/02/meta-quietly-launches-vibe-coded-gaming-app-pocket/) ⭐️ 6.0/10

Meta has quietly launched Pocket, an experimental AI app that generates interactive mini games from text prompts using a technique known as 'vibe coding'. This marks a major tech company's first foray into AI-powered text-to-game creation, potentially democratizing game development for non-programmers and signaling a new trend in AI-assisted content creation. Pocket is described as an 'experimental' app by Meta, and it relies on the 'vibe coding' paradigm where users describe a game in natural language and the AI generates the corresponding code and assets automatically.

rss · TechCrunch · Jul 2, 18:44

**Background**: Vibe coding is a software development practice where developers use AI to generate code from high-level prompts, often requiring minimal manual intervention. The term gained popularity in 2025 as large language models became capable of producing functional code snippets. Pocket applies this concept to game creation, allowing users to generate interactive experiences simply by describing them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#AI`, `#gaming`, `#text-to-game`

---

<a id="item-26"></a>
## [Boeing-owned Wisk Aero accused of firing safety whistleblower](https://techcrunch.com/2026/07/02/boeing-owned-wisk-aero-accused-of-firing-manager-who-raised-safety-concerns/) ⭐️ 6.0/10

A former software manager at Boeing-owned Wisk Aero has alleged that the company rushed software testing ahead of a crucial 2025 flight test and was subsequently fired for raising safety concerns. This allegation highlights potential risks in the development of autonomous eVTOL air taxis, where software reliability is critical to passenger safety. It also raises questions about whistleblower protection in the fast-paced advanced air mobility industry. The former manager claims the rush occurred before a key flight test in 2025, though the specific test and aircraft generation (likely Generation 6) have not been confirmed. Wisk Aero has not publicly responded to the allegations.

rss · TechCrunch · Jul 2, 17:30

**Background**: Wisk Aero, a Boeing-backed company, is developing autonomous, electric vertical takeoff and landing (eVTOL) aircraft for air taxi services. The company's sixth-generation eVTOL is intended to be the first certified autonomous passenger aircraft in the U.S. Aviation software must meet rigorous safety standards set by the FAA and industry guidelines to ensure reliability in safety-critical systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aerotime.aero/articles/wisk-aero-boeing-autonomous-flight-oshkosh">First-ever public demo of autonomous eVTOL aircraft : video</a></li>
<li><a href="https://www.robotics247.com/article/wisk_aero_lands_450m_boeing_advancing_autonomous_air_taxis/Drones">Wisk Aero Lands $450M From Boeing to Advance... - Robotics 24/7</a></li>
<li><a href="https://www.jploft.com/blog/aviation-software-testing-guide">Aviation Software Testing Guide: All You Need to Know</a></li>

</ul>
</details>

**Tags**: `#software testing`, `#safety`, `#whistleblower`, `#aviation`, `#Boeing`

---

<a id="item-27"></a>
## [Indian entrepreneur invests $30M in AI office suite](https://techcrunch.com/2026/07/01/indian-tech-tycoon-bets-30m-to-build-an-ai-alternative-to-microsoft-office/) ⭐️ 6.0/10

Bhavin Turakhia, a serial Indian tech entrepreneur, has committed $30 million of his own money to launch Neo, an AI-native office suite that competes with Microsoft Office and Google Workspace. Neo was introduced on July 2, 2026, from Bengaluru, built entirely around autonomous agents. This move challenges the long-standing dominance of Microsoft and Google in the productivity software market, potentially forcing incumbents to accelerate AI integration. If successful, Neo could offer businesses a powerful, AI-first alternative that redefines how office work is done. Neo is Turakhia's fifth venture and the first enterprise software project he has personally funded at this scale. The suite is built on an 'agent architecture,' leveraging autonomous AI agents to automate tasks across documents, spreadsheets, and communication tools.

rss · TechCrunch · Jul 2, 05:30

**Background**: Bhavin Turakhia is a well-known Indian entrepreneur who previously co-founded successful tech companies including Directi, Radix, and Zeta. Microsoft Office and Google Workspace have dominated the office productivity space for decades, with few serious challengers. Neo represents a bet that AI can fundamentally reshape these tools, similar to how cloud-based suites disrupted traditional desktop software.

<details><summary>References</summary>
<ul>
<li><a href="https://windowsforum.com/threads/neo-by-bhavin-turakhia-ai-native-office-suite-built-on-agent-architecture.433258/">Neo by Bhavin Turakhia: AI-Native Office Suite Built on Agent Architecture | Windows Forum</a></li>
<li><a href="https://windowsnews.ai/article/bhavin-turakhias-neo-takes-aim-at-microsoft-office-with-30m-ai-native-agent-suite.433258">Bhavin Turakhia’s Neo Takes Aim at Microsoft Office with $30M AI-Native Agent Suite - Windows News</a></li>
<li><a href="https://cryptobriefing.com/neo-turakhia-30m-microsoft-office-competitor/">Neo founder Bhavin Turakhia invests $30M to compete with Microsoft Office</a></li>

</ul>
</details>

**Tags**: `#AI`, `#enterprise software`, `#office productivity`, `#startup`

---

<a id="item-28"></a>
## [India Hackathon Challenges Silicon Valley AI Model](https://restofworld.org/2026/india-bhashini-open-source-offline-ai-hackathon/?utm_source=rss&utm_medium=rss&utm_campaign=feeds) ⭐️ 6.0/10

India is hosting a hackathon that invites developers to build offline, multilingual AI tools, promoting an alternative to the dominant Silicon Valley AI playbook centered on large, cloud-based models. This initiative could democratize AI development by enabling regions with limited internet access to create and use AI tools, reducing dependence on Western tech giants and their infrastructure. The hackathon focuses on building tools that run entirely offline, using local processing power rather than cloud servers, and supports multiple Indian languages to address linguistic diversity.

rss · Rest of World · Jul 2, 10:00

**Background**: The Silicon Valley AI playbook typically relies on massive cloud computing resources, large datasets, and centralized model deployment. Offline AI tools, by contrast, run locally on devices, enabling use in low-connectivity environments. India's hackathon aims to foster an alternative ecosystem that is open source, multilingual, and accessible to a broader population.

<details><summary>References</summary>
<ul>
<li><a href="https://www.forbes.com/sites/ronschmelzer/2026/04/30/ai-is-breaking-silicon-valleys-global-playbook/">AI Is Breaking Silicon Valley’s Global Playbook</a></li>
<li><a href="https://modelfit.io/guides/run-ai-offline/">Does Ollama Work Offline ? Yes: Full 2026 Guide</a></li>
<li><a href="https://promptandskills.com/learn/local-ai/run-ai-offline-india">Run AI Completely Offline in India — India Guide... | PromptAndSkills</a></li>

</ul>
</details>

**Tags**: `#AI`, `#India`, `#multilingual`, `#open source`, `#offline`

---

<a id="item-29"></a>
## [Cyberattack on Shun Hing Group exposes 1M people's data](https://www.scmp.com/news/hong-kong/law-and-crime/article/3359218/cyberattack-hong-kongs-shun-hing-group-affects-data-1-million-people?utm_source=rss_feed) ⭐️ 6.0/10

A cyberattack on Hong Kong's Shun Hing Group compromised the personal data of approximately 1.05 million people, prompting an investigation by the Office of the Privacy Commissioner for Personal Data. This breach highlights the vulnerability of large retailers in Hong Kong and underscores the need for stronger cybersecurity measures to protect massive amounts of consumer data. The company reported the breach to the privacy watchdog on March 23, and the investigation is ongoing. The exact nature of the compromised data has not been fully disclosed yet.

rss · SCMP · Jul 2, 16:22

**Background**: Shun Hing Group is a major appliance distributor in Hong Kong, handling extensive customer data including personal information. Cyberattacks on such companies can lead to identity theft and fraud. The privacy watchdog's investigation aims to assess the breach's impact and ensure compliance with data protection laws.

**Tags**: `#cybersecurity`, `#data breach`, `#Hong Kong`, `#privacy`

---

<a id="item-30"></a>
## [CXMT's $4.3B IPO: AI boom meets US export threat](https://www.scmp.com/tech/big-tech/article/3359168/inside-cxmts-us43b-ipo-soaring-profits-meet-us-export-threat-and-high-stakes-hbm-race?utm_source=rss_feed) ⭐️ 6.0/10

China's leading DRAM maker, ChangXin Memory Technologies (CXMT), is preparing a 29.5 billion yuan ($4.3 billion) IPO on Shanghai's STAR Market, capitalizing on an AI-driven memory upcycle while facing potential US export restrictions. This IPO is significant because it highlights China's push to achieve semiconductor self-sufficiency amid escalating US-China tech tensions, and its success could reshape the global DRAM and HBM market dominated by Samsung, SK Hynix, and Micron. The IPO is on the STAR Market, China's Nasdaq-style board for tech firms, and comes as CXMT benefits from a global memory shortage fueled by AI demand for HBM chips. However, US export controls threaten its access to advanced equipment and technology.

rss · SCMP · Jul 2, 08:46

**Background**: DRAM (Dynamic Random-Access Memory) is a type of volatile memory widely used in computers and servers. HBM (High Bandwidth Memory) is a 3D-stacked DRAM technology that provides high bandwidth for AI accelerators and graphics cards. The Shanghai STAR Market is a Chinese stock exchange board designed for high-tech and innovative companies, with looser listing rules. CXMT is China's largest DRAM manufacturer and a key player in the nation's effort to reduce dependence on foreign chips.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.hawksford.com/insights-and-guides/china-business-guides/launch-of-star-market">Shanghai STAR Market : China’s NASDAQ for Tech... | Hawksford</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#semiconductors`, `#AI`, `#IPO`, `#US-China trade`

---