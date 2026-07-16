---
layout: default
title: "Horizon Summary: 2026-07-16 (EN)"
date: 2026-07-16
lang: en
---

> From 143 items, 34 important content pieces were selected

---

1. [Moonshot AI Open-Sources Kimi K3, a 2.8 Trillion Parameter Model](#item-1) ⭐️ 9.0/10
2. [Decoy Font Hides Text from AI, Humans See It](#item-2) ⭐️ 8.0/10
3. [Anthropic Nears IPO, Plans Investor Meetings in Coming Weeks](#item-3) ⭐️ 8.0/10
4. [UK Jails Two Scattered Spider Hackers for Transit Cyberattack](#item-4) ⭐️ 8.0/10
5. [Stardust period tracker shares health data with analytics firm](#item-5) ⭐️ 8.0/10
6. [Shanghai integrates computing centers with power grid for peak load reduction](#item-6) ⭐️ 8.0/10
7. [TSMC commits extra $100 billion to Arizona fabs for AI chips](#item-7) ⭐️ 8.0/10
8. [LM Studio Launches Bionic: Agent Platform for Open Models](#item-8) ⭐️ 7.0/10
9. [Microsoft Comic Chat open sourced](#item-9) ⭐️ 7.0/10
10. [Detecting LLM-Generated Texts with Classical ML](#item-10) ⭐️ 7.0/10
11. [OnePlus Ends New Phone Launches in US and Europe](#item-11) ⭐️ 7.0/10
12. [Interactive Linear Algebra Book Wins Community Praise](#item-12) ⭐️ 7.0/10
13. [AI Empowers Non-Professionals to Create Viral Films, Reshaping Filmmaking](#item-13) ⭐️ 7.0/10
14. [Chinese Aviation Power Startup Raises $14M for 400 kW Engine Platform](#item-14) ⭐️ 7.0/10
15. [Sino Intelligent Driving Raises 300M Yuan in Series C for Autonomous Trucks](#item-15) ⭐️ 7.0/10
16. [Apple AI Approved in China, DeepSeek IPO Plans, Bike Price Hikes](#item-16) ⭐️ 7.0/10
17. [Google Delays Gemini 3.5 Pro to Boost Programming](#item-17) ⭐️ 7.0/10
18. [SF mayor seeks stricter robotaxi rules after Waymo gridlock](#item-18) ⭐️ 7.0/10
19. [Google AI Mode expands to link and interact with apps](#item-19) ⭐️ 7.0/10
20. [AI content moderation fails without consent](#item-20) ⭐️ 7.0/10
21. [US official: Restrict Chinese access to Anthropic AI to keep lead](#item-21) ⭐️ 7.0/10
22. [Chinese Tech Giants Invest in AI-Powered Weight Management](#item-22) ⭐️ 6.0/10
23. [PongBot Aura: Multi-Sport AI Coach Robot Raises $4M on Kickstarter](#item-23) ⭐️ 6.0/10
24. [Microsoft Developing AI Tool Inspired by Mythos for Vulnerability Detection](#item-24) ⭐️ 6.0/10
25. [SpaceXAI Launches Grok 4.5 with Competitive Token Pricing](#item-25) ⭐️ 6.0/10
26. [Coca-Cola suspends Fairlife dairy production after ransomware attack](#item-26) ⭐️ 6.0/10
27. [BP Shuts Down Corporate Venture Arm After 20 Years](#item-27) ⭐️ 6.0/10
28. [X uses Grok AI to combat content theft and engagement bait](#item-28) ⭐️ 6.0/10
29. [Sheryl Sandberg Leads $10M Investment in AI Vehicle Inspection Startup](#item-29) ⭐️ 6.0/10
30. [AMI Labs CEO Rejects AGI, Superintelligence Labels](#item-30) ⭐️ 6.0/10
31. [Space reproduction hurdle: early human cells develop poorly in microgravity](#item-31) ⭐️ 6.0/10
32. [Xpeng aims to mass-produce humanoid robot globally by 2027](#item-32) ⭐️ 6.0/10
33. [Nvidia CEO meets Japanese execs in yakitori summit](#item-33) ⭐️ 6.0/10
34. [China Plans Asteroid Early Warning System](#item-34) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Moonshot AI Open-Sources Kimi K3, a 2.8 Trillion Parameter Model](https://36kr.com/newsflashes/3898931953403522?f=rss) ⭐️ 9.0/10

On July 17, 2025, Moonshot AI officially released Kimi K3, the world's first open-source model at the 3-trillion-parameter scale, featuring 2.8 trillion parameters, Kimi Delta Attention (KDA) hybrid linear attention, Attention Residuals, native vision support, and a 1 million token context window. This breakthrough makes frontier-level AI capabilities openly accessible, enabling researchers and developers to experiment with and deploy a model that rivals top proprietary systems like Claude Fable 5 and GPT-5.6 Sol, potentially accelerating innovation in long-context programming, knowledge work, and reasoning. The model utilizes Kimi Delta Attention (KDA), a linear attention mechanism that scales efficiently to ultra-long contexts, and Attention Residuals, which allow layers to selectively aggregate earlier representations. Full model weights will be released in the coming days along with a technical report.

rss · 36氪 · Jul 16, 23:18

**Background**: Large language models traditionally rely on softmax attention, which has quadratic complexity in context length, making long contexts expensive. Kimi Delta Attention is a linear attention variant that reduces this complexity, while Attention Residuals improve depth-wise information flow. Moonshot AI is a Chinese AI company known for its Kimi chatbot and previous models.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">KIMI LINEAR: AN EXPRESSIVE, EFFICIENT ATTENTION ARCHITECTURE</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>

</ul>
</details>

**Discussion**: Community comments reveal mixed reactions: some users express distrust in Moonshot AI due to unclear credit systems and data training policies on API usage, while others are impressed by K3's benchmark performance—ranked second only to Claude Fable 5 and GPT-5.6 Sol. One user noted the high cost of inference, calling it the most expensive Chinese model tested so far.

**Tags**: `#AI`, `#open-source`, `#large language model`, `#Kimi`, `#machine learning`

---

<a id="item-2"></a>
## [Decoy Font Hides Text from AI, Humans See It](https://www.mixfont.com/experiments/decoy-font) ⭐️ 8.0/10

Mixfont released Decoy Font, a free font based on DejaVu Sans Mono that embeds a hidden message readable by humans but designed to evade AI vision models. This adversarial typography technique exposes a critical limitation in current AI vision systems, highlighting the need for more robust models. It also opens up creative possibilities for CAPTCHAs and hidden communications. The Decoy Font relies on subtle contrast differences—on a light background the hidden text is visible, while on a dark background a different message appears. It is free for personal, commercial, and client use.

hackernews · ray__ · Jul 16, 16:18 · [Discussion](https://news.ycombinator.com/item?id=48936584)

**Background**: Adversarial examples are inputs intentionally perturbed to cause machine learning models to make mistakes, such as classifying a stop sign as a speed limit. Decoy Font applies this concept to typography, creating text that humans can read but AI vision systems misinterpret or fail to detect.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.forgeeks.dev/decoy-font-hides-text-ai/">Decoy Font hides text from AI in plain sight — for(geeks)</a></li>
<li><a href="https://christophm.github.io/interpretable-ml-book/adversarial.html">30 Adversarial Examples – Interpretable Machine Learning</a></li>

</ul>
</details>

**Discussion**: Commenters found the font cool but questioned its practical utility; tests by users showed that GPT, Claude, and Gemini varied in ability to detect the hidden message. One user noted the effect depends on background color, which resolved initial confusion.

**Tags**: `#typography`, `#adversarial AI`, `#font`, `#security`, `#LLM`

---

<a id="item-3"></a>
## [Anthropic Nears IPO, Plans Investor Meetings in Coming Weeks](https://36kr.com/newsflashes/3898921880569737?f=rss) ⭐️ 8.0/10

Anthropic, the AI company behind Claude, is reportedly planning to meet with investors for a potential IPO as early as October, with a valuation exceeding $965 billion after its latest funding round. This IPO would be a landmark event for the AI industry, potentially making Anthropic the most valuable private AI company and signaling strong investor confidence in AI safety-focused firms. The company is arranging meetings with investors through its underwriting banks in the coming weeks, and the IPO could launch as early as October. Anthropic's valuation reached $965 billion in a May funding round, surpassing OpenAI's valuation.

rss · 36氪 · Jul 16, 23:25

**Background**: Anthropic is an AI safety and research company founded in 2021 by former OpenAI employees. Its flagship product is Claude, a large language model chatbot. The company has focused on developing AI systems that are safe and interpretable, using techniques like constitutional AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(chatbot)">Claude (chatbot)</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#IPO`, `#AI`, `#funding`, `#industry news`

---

<a id="item-4"></a>
## [UK Jails Two Scattered Spider Hackers for Transit Cyberattack](https://techcrunch.com/2026/07/16/uk-cops-say-arrest-of-two-young-hackers-disrupted-the-operations-of-an-infamous-hacking-group/) ⭐️ 8.0/10

Two members of the Scattered Spider hacking group, Owen Flowers and Thalha Jubair, were sentenced to five and a half years in prison for hacking Transport for London (TfL) in a 2024 cyberattack that exposed millions of customer records. This sentencing marks a significant victory for law enforcement against a prolific hacking group that has targeted large corporations, highlighting the real-world consequences of cybercrime even for young offenders. The attack occurred between August 31 and September 3, 2024, and the two hackers pleaded guilty last month. They are among the youngest members of Scattered Spider, which is known for social engineering and help-desk attacks.

rss · TechCrunch · Jul 16, 15:37

**Background**: Scattered Spider, also known as UNC3944 or ShinyHunters, is a cybercriminal group composed mainly of teenagers and young adults from the US and UK. They are notorious for targeting large companies via sophisticated social engineering attacks, often compromising IT help desks to gain initial access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Scattered_Spider">Scattered Spider - Wikipedia</a></li>
<li><a href="https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-320a">Scattered Spider | CISA</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#hacking`, `#law enforcement`, `#Scattered Spider`, `#transit hack`

---

<a id="item-5"></a>
## [Stardust period tracker shares health data with analytics firm](https://techcrunch.com/2026/07/16/period-tracker-stardust-shares-users-health-data-with-analytics-firm-says-mozilla-research/) ⭐️ 8.0/10

Mozilla research found that the period tracker app Stardust shares users' health data with an analytics firm, while another app was found to be 'squeaky clean' and respects user privacy. This highlights significant privacy risks for sensitive health data collected by period tracker apps, affecting user trust and potentially exposing intimate information to third parties without consent. The research did not name the analytics firm or the ‘squeaky clean’ app, but it underscores the variability in privacy practices among period tracking apps. Stardust’s website claims it is ‘women-built and data-encrypted.’

rss · TechCrunch · Jul 16, 15:33

**Background**: Period tracker apps are used to log menstrual cycles, ovulation, and pregnancy, often collecting highly personal health data. Mozilla’s ‘Privacy Not Included’ research evaluates consumer products for privacy and security issues, assigning warning labels to products with problems. This finding is part of a broader investigation into how apps handle sensitive data.

<details><summary>References</summary>
<ul>
<li><a href="https://stardust.app/">Stardust</a></li>
<li><a href="https://www.mozillafoundation.org/en/privacynotincluded/about/methodology/">*Privacy Not Included | Shop smart and safe | Mozilla Foundation</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#data-sharing`, `#health-data`, `#period-tracker`, `#Mozilla-research`

---

<a id="item-6"></a>
## [Shanghai integrates computing centers with power grid for peak load reduction](https://www.scmp.com/economy/china-economy/article/3360801/shanghai-synergises-computing-centres-grid-power-infrastructure-upgrade?utm_source=rss_feed) ⭐️ 8.0/10

Shanghai has successfully integrated its computing centers with the power grid in a national first trial, achieving a peak load reduction of 97.8 megawatts within a two-hour period. This milestone demonstrates a new demand-side management approach that can help stabilize the grid amid rising AI infrastructure energy demand, setting a precedent for other cities. It also supports China's broader goals of computing-grid coordination and energy efficiency. Led by State Grid's Shanghai subsidiary, the trial is part of the country's largest single city-level adjustment of computing power load. The city aims to further expand such synergisation as part of its power infrastructure upgrade.

rss · SCMP · Jul 16, 11:00

**Background**: Computing centers, including data centers and AI training facilities, consume enormous amounts of electricity, often straining local grids during peak hours. Demand response programs allow grid operators to temporarily reduce load from such facilities in exchange for compensation. China's 'East-West Computing Transfer' project aims to balance computing resources across regions, while initiatives like the 'Baichuan' computing power grid-connected platform coordinate distributed computing power.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/economy/china-economy/article/3360801/shanghai-synergises-computing-centres-grid-power-infrastructure-upgrade">Shanghai synergises computing centres with grid in power ...</a></li>
<li><a href="https://www.codetd.com/en/article/16567063">The largest in the country! Computing power grid -connected action...</a></li>
<li><a href="https://www.ey.com/en_us/insights/power-utilities/demand-response-and-data-center-growth">Demand response and data center growth | EY - US</a></li>

</ul>
</details>

**Tags**: `#smart grid`, `#computing centers`, `#energy management`, `#AI infrastructure`, `#China`

---

<a id="item-7"></a>
## [TSMC commits extra $100 billion to Arizona fabs for AI chips](https://www.scmp.com/tech/tech-war/article/3360809/tsmc-pledges-extra-us100-billion-arizona-fab-expansion-amid-soaring-ai-chip-demand?utm_source=rss_feed) ⭐️ 8.0/10

TSMC announced an additional $100 billion investment to expand its Arizona fabrication facilities, bringing total US investment to $265 billion, to meet surging AI chip demand. This massive investment underscores the strategic importance of domestic semiconductor manufacturing for AI and signals a major shift in global chip supply chains. It could reduce reliance on Asian foundries and boost US tech sovereignty. TSMC chairman CC Wei said the company would proceed 'as fast as possible' but did not provide a timeline, noting that progress depends on market conditions and customer needs. The investment covers multiple fabs in Arizona.

rss · SCMP · Jul 16, 10:30

**Background**: TSMC is the world's largest dedicated semiconductor foundry, producing chips for companies like Apple, Nvidia, and AMD. The US has been pushing to bring advanced chip manufacturing back home through the CHIPS Act, aiming to secure supply chains amid geopolitical tensions with China. This expansion is part of TSMC's broader strategy to diversify production beyond Taiwan.

**Tags**: `#TSMC`, `#semiconductor`, `#AI chips`, `#manufacturing`, `#investment`

---

<a id="item-8"></a>
## [LM Studio Launches Bionic: Agent Platform for Open Models](https://lmstudio.ai/blog/introducing-lm-studio-bionic) ⭐️ 7.0/10

LM Studio announced Bionic, an AI agent platform that integrates open models with a secure cloud backend, allowing users to run agents locally or via cloud. This bridges local and cloud LLM usage, offering enterprises a secure way to use open models without sacrificing data control, and signals LM Studio's shift from a local tool to a full agent platform. Bionic allows connecting to frontier open models via LM Studio Secure Cloud, with claims of no data retention or training, though community members question whether this applies to the frontier models themselves.

hackernews · minimaxir · Jul 16, 20:18 · [Discussion](https://news.ycombinator.com/item?id=48939662)

**Background**: LM Studio is a popular desktop application for running large language models locally on consumer hardware. Bionic extends this by adding an agent framework and a cloud backend (LM Studio Secure Cloud) that enables users to run larger open models remotely while maintaining a local interface.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/blog">LM Studio Blog | LM Studio</a></li>
<li><a href="https://lmstudio.ai/link">LM Link • Use your local models, remotely. | LM Studio</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some worry about the shift in business model and cloud dependency, while others see value as a polished enterprise wrapper. Questions arise about data privacy when using frontier cloud models.

**Tags**: `#AI`, `#open models`, `#local LLM`, `#agent`, `#LM Studio`

---

<a id="item-9"></a>
## [Microsoft Comic Chat open sourced](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

On July 16, 2026, Microsoft open sourced Comic Chat, a graphical IRC client originally released in 1996 that used comic-style avatars to represent chat participants. This release preserves a piece of internet history and allows developers to study, modify, and run a nostalgic application that influenced early graphical chat interfaces. Comic Chat was originally developed by Microsoft researcher David Kurlander and was bundled with Windows 98 and Internet Explorer 3.0.

hackernews · jervant · Jul 16, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48936426)

**Background**: IRCat (Internet Relay Chat) is a text-based chat protocol for group communication. Comic Chat extended IRC with commands to control character appearance and actions, making conversations look like a comic strip. The project was part of Microsoft's early internet experiments.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://en.wikipedia.org/wiki/IRC">IRC - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members expressed nostalgia and technical curiosity, with one original champion (Robert Standefer) sharing the backstory of the release and another user noting its inspiration for a startup. Some recalled that Comic Chat was controversial in IRC circles due to its non-standard protocol extensions.

**Tags**: `#open source`, `#microsoft`, `#comic chat`, `#irc`, `#history`

---

<a id="item-10"></a>
## [Detecting LLM-Generated Texts with Classical ML](https://blog.lyc8503.net/en/post/llm-classifier/) ⭐️ 7.0/10

A blog post explores using classical machine learning methods like SVM and Naive Bayes to detect LLM-generated texts, presenting a relatively small classifier trained on specific features. As LLM-generated content spreads, reliable detection is crucial for combating misinformation and preserving academic integrity. Classical ML offers a simpler, more interpretable alternative to deep learning detectors, potentially enabling lightweight in-browser tools. The classifier is not large and could potentially run in a browser extension, but skepticism remains high due to the low information density of text, making reliable provenance detection difficult.

hackernews · uneven9434 · Jul 16, 16:41 · [Discussion](https://news.ycombinator.com/item?id=48936880)

**Background**: LLM-generated text refers to content produced by large language models like GPT-4. Classical machine learning methods such as SVM and Naive Bayes have been used for decades in text classification tasks, distinguishing them from modern deep learning approaches that require more data and computation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2666412722000101">Analytics of machine learning-based algorithms for text classification</a></li>
<li><a href="https://chat-test.learnprompting.org/docs/miscl/detect">Detecting AI Generated Text</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some skeptics argue that detection is unreliable and compare it to 'tarot card reading', while others propose alternative metrics like effort-based evaluation. One commenter suggests a browser extension for real-time detection, though many believe the battle is ultimately lost.

**Tags**: `#LLM`, `#AI detection`, `#machine learning`, `#text generation`

---

<a id="item-11"></a>
## [OnePlus Ends New Phone Launches in US and Europe](https://community.oneplus.com/thread/2170715118587871237) ⭐️ 7.0/10

OnePlus has announced it will no longer launch new products in the United States and European markets, while continuing software support for existing devices. This strategic retreat from key Western markets reduces competition and may disappoint loyal users, signaling a shift in the global smartphone landscape as Chinese brands reassess overseas expansion. Only new product rollouts are affected; existing OnePlus devices will receive scheduled updates and security patches backed by parent company Oppo. The announcement does not affect ongoing software support commitments.

hackernews · pilililo2 · Jul 16, 10:14 · [Discussion](https://news.ycombinator.com/item?id=48932539)

**Background**: OnePlus started as a 'flagship killer' brand popular among enthusiasts for its near-stock Android experience, unlockable bootloaders, and competitive pricing. Over time, the brand merged closer with Oppo and lost some of its hacker-friendly identity. This move mirrors a broader trend of Chinese smartphone makers scaling back in Western markets due to regulatory and competitive pressures.

**Discussion**: Commenters quickly corrected the editorialized title, emphasizing that OnePlus is only halting new product launches, not full operations. Some expressed nostalgia for the brand's early enthusiast days, while a former employee praised recent models' battery life but noted the intense 996 work culture.

**Tags**: `#OnePlus`, `#smartphone`, `#business`, `#Europe`, `#USA`

---

<a id="item-12"></a>
## [Interactive Linear Algebra Book Wins Community Praise](https://immersivemath.com/ila/) ⭐️ 7.0/10

An immersive linear algebra book that explains concepts through interactive dynamic figures is gaining renewed attention after being shared on Hacker News, with the community highly praising its educational value. This interactive approach makes abstract linear algebra concepts more intuitive and accessible, potentially improving math education and inspiring similar interactive textbooks for other subjects. The book features dynamic figures that respond to user interaction, tooltips that provide additional explanations, and a clean, section-by-section presentation that guides learners effectively.

hackernews · srean · Jul 16, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48935951)

**Background**: Linear algebra is a core mathematics subject involving vectors, matrices, and linear transformations, often taught with static diagrams. This interactive textbook leverages modern web technologies to create engaging visualizations that help students grasp complex ideas more intuitively.

**Discussion**: Comments were overwhelmingly positive, with users expressing love for the interactive approach and wishing similar resources existed for statistics, probability, and robotics. Some also noted that AI tools like LLMs could make creating such interactive content easier in the future.

**Tags**: `#linear algebra`, `#interactive learning`, `#math education`, `#visualization`

---

<a id="item-13"></a>
## [AI Empowers Non-Professionals to Create Viral Films, Reshaping Filmmaking](https://36kr.com/p/3898151587890824?f=rss) ⭐️ 7.0/10

Vocational school graduate Liu Ziyu created an AI-generated short film 'Zombie Street Cleaner' that amassed over 100 million views, earning him an offer from Hollywood producers. Meanwhile, 20-year-old Meng Ke, a non-professional director, won the Best AI Director award at the Beijing International Film Festival for his AI short film 'Mold'. These cases demonstrate that AI is democratizing filmmaking by dramatically reducing costs and technical barriers, allowing outsiders without traditional industry connections to produce high-quality content. This shift could disrupt the traditional star-driven, high-cost film industry and open doors for a new generation of creators. Liu Ziyu's film cost nearly nothing in terms of production resources, yet achieved mainstream recognition; his English is poor and he can't even use VPNs. The AI short film 'Peony' was made for just 2,000 RMB (membership fees for two AI platforms), while traditional 'low-budget' films cost tens of millions.

rss · 36氪 · Jul 16, 10:07

**Background**: AIGC (AI Generated Content) refers to content automatically created by artificial intelligence, including text, images, audio, and video. Recent advances in AI video generation models (e.g., Alibaba's Wanxiang, Veo 3) have enabled individuals to produce cinematic-quality short films with minimal effort. Traditional filmmaking requires expensive equipment, large crews, and access to star actors, making it nearly impossible for outsiders to break in.

<details><summary>References</summary>
<ul>
<li><a href="https://www.digitaling.com/articles/934226.html">一次性搞懂什么是AIGC！（一篇文章22个基本概念） - 数英</a></li>
<li><a href="https://tongyi.aliyun.com/wan/wanxiang/">万相 | 领先的 AI 视 频 与图像 生 成 模型</a></li>

</ul>
</details>

**Discussion**: One netizen commented on Liu Ziyu's video: 'Awesome, you've boarded the AIGC Noah's Ark. When can us wage laborers turn our lives around?' with a crying emoji. The comment reflects a mix of admiration and hope among ordinary people that AI can provide similar opportunities for career transformation.

**Tags**: `#AI`, `#filmmaking`, `#democratization`, `#AIGC`, `#career transformation`

---

<a id="item-14"></a>
## [Chinese Aviation Power Startup Raises $14M for 400 kW Engine Platform](https://36kr.com/p/3897686922266244?f=rss) ⭐️ 7.0/10

Hanfa Changkong, a Chinese civil aviation power startup, completed a nearly 100 million yuan Pre-A round led by Fangguang Capital to advance its 400 kW class core engine platform. The platform includes turboshaft (S4), turboprop (P4), and turboelectric (H4) variants, with the S4 already in flight testing. This funding addresses a critical gap in China's low-altitude economy: the lack of domestically produced 200-500 kW turbine engines for drones, eVTOLs, and logistics aircraft, which has been dominated by international giants. Hanfa Changkong's platform approach could lower costs and accelerate the commercialization of low-altitude aircraft. The 400 kW core engine completed 60 hours of endurance testing, accumulated 300 starts, and achieved a maximum measured power of 426 kW. The company plans to start turboprop and turboelectric engine ground tests in late 2026, with type certification and mass production targeted by 2027.

rss · 36氪 · Jul 16, 02:12

**Background**: Aircraft turbine engines can be classified into turbofan, turbojet, turboprop, turboshaft, and turbofan types, all sharing a common core (gas generator). Turboshaft engines are used in helicopters, turboprops in fixed-wing aircraft, and turboelectric engines convert shaft power to electricity for distributed propulsion. The 200-500 kW range is a gap in China's domestic supply, as previous development focused on military high-thrust engines.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/108959628">涡喷，涡扇，涡桨，涡轴的区别及航空发动机资讯 - 知乎专栏</a></li>
<li><a href="http://www.camac.org.cn/uploadfile/2411/p10/M5-+航空涡轮发动机（第一次修订）R1版2025年4月7日.pdf">[PDF] 航空涡轮发动机</a></li>

</ul>
</details>

**Tags**: `#aviation`, `#power engines`, `#low-altitude economy`, `#eVTOL`, `#drones`

---

<a id="item-15"></a>
## [Sino Intelligent Driving Raises 300M Yuan in Series C for Autonomous Trucks](https://36kr.com/p/3895721094842249?f=rss) ⭐️ 7.0/10

Sino Intelligent Driving, a Chinese autonomous trucking company, has raised 300 million yuan in Series C funding led by Xingsheng Capital and Yidao Capital to develop its next-generation automotive-grade autonomous driving solutions. This funding round signals continued investor confidence in autonomous heavy-truck commercialization for both closed and open road scenarios, as the sector sees rapid IPO activity and growing demand in logistics. The company's one-stage world model autonomous driving solution and self-developed domain controller are central to its product lineup, which includes unmanned trucks, dump trucks, and flatbed vehicles. The funding will help upgrade the domain controller from non-automotive to automotive-grade to handle open-road challenges such as long distances, wide temperature variations, and strong electromagnetic interference.

rss · 36氪 · Jul 16, 00:00

**Background**: Autonomous heavy-truck companies like Sino Intelligent Driving focus on both closed environments (ports, mines) and open highways. World models in autonomous driving refer to AI systems that can simulate and predict future driving scenarios. Domain controllers serve as the central compute unit processing sensor data and executing driving decisions. Automotive-grade certification ensures reliability under harsh conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2403.02622v3/">World Models for Autonomous Driving : An Initial Survey</a></li>
<li><a href="https://ehfcv.com/tusimple-autonomous-domain-controller-for-commercial-vehicles/">TuSimple Autonomous Domain Controller for Commercial Vehicles</a></li>

</ul>
</details>

**Tags**: `#autonomous driving`, `#autonomous trucking`, `#venture capital`, `#logistics`, `#world model`

---

<a id="item-16"></a>
## [Apple AI Approved in China, DeepSeek IPO Plans, Bike Price Hikes](https://36kr.com/p/3897553391978371?f=rss) ⭐️ 7.0/10

Apple's on-device AI model 'Apple Intelligence' received regulatory approval in China on July 8, 2025, with Alibaba's Qwen providing text and image generation capabilities and Baidu handling AI search features for Chinese iPhones. Separately, three bike-sharing companies—Meituan, Didi Qingju, and Hellobike—raised starting prices to 1.88-1.99 yuan for 60 minutes, and DeepSeek has begun preparing for an IPO, aiming for a 2027 listing in mainland China. Apple's partnership with Alibaba and Baidu marks a significant step for Apple Intelligence to comply with Chinese regulations, potentially boosting iPhone competitiveness in China. DeepSeek's IPO signals growing investor interest in Chinese AI startups, while bike-sharing price hikes reflect industry efforts to achieve profitability after years of subsidies. The approval covers seven on-device generative AI services including Apple Intelligence, Huawei's Xiaoyi, and others. Alibaba's Qwen model powers text and image generation, while Baidu provides AI search for the Chinese version of Siri. DeepSeek is working with an accounting firm to complete financial reports by end of 2025, with IPO timing subject to market conditions.

rss · 36氪 · Jul 15, 23:59

**Background**: On-device AI refers to AI processing that runs locally on a device rather than in the cloud, enhancing privacy and reducing latency. In China, generative AI services require government approval before public deployment. DeepSeek is a Chinese AI company founded in 2023, known for its cost-efficient large language models like DeepSeek-R1, which rival top models from OpenAI and Meta.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="http://www.ce.cn/xwzx/gnsz/gdxw/202607/t20260715_3088731.shtml">ce.cn/xwzx/gnsz/gdxw/202607/t20260715_3088731.shtml</a></li>
<li><a href="https://www.21ic.com/a/1007920.html">端 侧 AI ... - 21ic电子网</a></li>

</ul>
</details>

**Tags**: `#Apple AI`, `#DeepSeek IPO`, `#China Tech`, `#Shared Bikes`, `#AI Regulation`

---

<a id="item-17"></a>
## [Google Delays Gemini 3.5 Pro to Boost Programming](https://36kr.com/newsflashes/3898936840701571?f=rss) ⭐️ 7.0/10

Google has delayed the release of its flagship AI model, Gemini 3.5 Pro, by several months to focus on improving its programming capabilities, according to insiders. This delay highlights the intense competition in the AI industry, as rivals Anthropic and OpenAI have already released models surpassing Gemini, potentially eroding Google's market lead and causing internal unrest among its engineers. The delay has sparked dissatisfaction among ten current and former employees, including engineers and AI researchers, who fear Google is losing its competitive edge against Anthropic and OpenAI.

rss · 36氪 · Jul 16, 23:37

**Background**: Gemini is Google's multimodal AI model series, with the Pro version targeting advanced tasks like coding. Programming ability is a key benchmark for AI models, as it impacts developer adoption and enterprise use. The delay underscores the pressure on Google to match rapid advances from competitors.

**Tags**: `#AI`, `#Google`, `#Gemini`, `#large language models`, `#programming`

---

<a id="item-18"></a>
## [SF mayor seeks stricter robotaxi rules after Waymo gridlock](https://techcrunch.com/2026/07/16/san-francisco-mayor-pushes-for-tougher-rules-after-the-waymo-traffic-fiasco/) ⭐️ 7.0/10

San Francisco Mayor Daniel Lurie has called on state regulators to impose tougher requirements on robotaxi operators like Waymo, following a major hours-long gridlock incident caused by the company's autonomous vehicles. This push for stricter regulation could reshape the operating environment for autonomous vehicle companies in San Francisco and beyond, potentially slowing deployment but improving public safety and trust. The incident involved Waymo robotaxis causing a massive gridlock that lasted hours, highlighting persistent challenges with autonomous vehicle behavior in complex urban settings. Mayor Lurie's statement specifically targeted state regulators at the California Public Utilities Commission (CPUC) and the DMV.

rss · TechCrunch · Jul 16, 23:25

**Background**: Waymo, a subsidiary of Alphabet, operates autonomous taxi services in 10 US metropolitan areas with over 3,800 vehicles. Robotaxis have faced scrutiny for incidents such as blocking roads, failing to yield to emergency vehicles, and safety investigations by federal agencies. The push for regulation comes amid public skepticism, with a 2025 AAA survey showing only 13% trust self-driving vehicles.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo</a></li>
<li><a href="https://en.wikipedia.org/wiki/Robotaxi">Robotaxi</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#regulation`, `#Waymo`, `#San Francisco`

---

<a id="item-19"></a>
## [Google AI Mode expands to link and interact with apps](https://techcrunch.com/2026/07/16/googles-ai-mode-now-lets-you-link-and-interact-with-select-apps/) ⭐️ 7.0/10

Google has updated its AI Mode in Search to allow users to link and interact with select third-party apps, such as Instacart, Canva, and YouTube Music, enabling task completion directly from search results. This update transforms Google Search from a passive answer engine into a proactive assistant that can execute tasks across apps, potentially reshaping user workflows and increasing engagement with Google's ecosystem. The integration currently supports a limited set of apps including Instacart for grocery ordering, Canva for design creation, and YouTube Music for playlist management, with the feature available to Google One AI Premium subscribers in the US via Search Labs.

rss · TechCrunch · Jul 16, 16:00

**Background**: AI Mode is an experimental search feature launched by Google in March 2025, powered by its Gemini model, which handles complex multi-part queries and multimodal inputs. Initially available only to Google One AI Premium subscribers, it represents Google's push to integrate AI deeper into search. This app integration expands AI Mode's capability from answering questions to completing tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_AI_Mode">Google AI Mode</a></li>
<li><a href="https://overcentral.com/en/google-ai-mode-connected-apps/">Google Integrates Third-Party Apps into AI Mode Search</a></li>
<li><a href="https://superintelligencenews.com/applications/ai-mode-app-links-tasks/">AI Mode Adds App Links for Tasks</a></li>

</ul>
</details>

**Tags**: `#Google`, `#AI Mode`, `#app integration`, `#task completion`

---

<a id="item-20"></a>
## [AI content moderation fails without consent](https://restofworld.org/2026/ai-content-moderation-consent-muse/?utm_source=rss&utm_medium=rss&utm_campaign=feeds) ⭐️ 7.0/10

A Rest of World article argues that AI content moderation cannot effectively protect users because it lacks a consent-based framework, using the backlash against Meta's Muse Image as a case study. This highlights a critical flaw in current AI governance approaches, where user consent is often ignored, potentially leading to privacy violations and erosion of trust. It calls for Big Tech to invest in consent-based systems and for governments to regulate accordingly. Meta's Muse Image, an AI image generator with invisible watermarks (Content Seal), faced backlash for using content without consent. The article argues that simply filtering content after creation is insufficient; consent must be incorporated before generation.

rss · Rest of World · Jul 16, 10:00

**Background**: AI content moderation involves using machine learning to detect and filter harmful or inappropriate content on platforms. However, it often operates without explicit user consent for how data is used or generated. Meta's Muse Image, launched in July 2026, is an AI image generator that sparked controversy over its use of celebrity likenesses and other content without permission. The incident underscores the broader challenge of balancing innovation with ethical practices.

<details><summary>References</summary>
<ul>
<li><a href="https://restofworld.org/2026/ai-content-moderation-consent-muse/">AI content moderation has a consent problem - Rest of World</a></li>
<li><a href="https://about.fb.com/news/2026/07/introducing-muse-image-meta-ai/">Introducing Muse Image : Image Generation Built for Your World</a></li>
<li><a href="https://www.linkedin.com/posts/dataconomy-media_meta-ai-bots-used-celebrity-likenesses-without-activity-7369682048480993289-zRxJ">Meta AI bots used celebrity likenesses without consent | Dataconomy...</a></li>

</ul>
</details>

**Tags**: `#AI content moderation`, `#consent`, `#Meta`, `#ethics`, `#AI governance`

---

<a id="item-21"></a>
## [US official: Restrict Chinese access to Anthropic AI to keep lead](https://www.scmp.com/news/china/diplomacy/article/3360833/anthropic-china-and-why-pax-silica-architect-thinks-us-can-keep-ai-lead?utm_source=rss_feed) ⭐️ 7.0/10

US undersecretary Jacob Helberg discusses the ban on foreign access to Anthropic models and argues that the US can maintain its AI lead through initiatives like Pax Silica. This reflects high-level US policy to limit China's access to advanced AI, impacting global tech competition and supply chain security. The interview is part of an exclusive series; Helberg is the architect of Pax Silica, a US-led initiative launched in December 2025 to secure semiconductor and AI supply chains.

rss · SCMP · Jul 16, 15:00

**Background**: Pax Silica is a US-led international initiative focused on securing supply chains for advanced technologies such as semiconductors, artificial intelligence, and rare earth elements, implicitly countering China's dominance in these fields. The US has been in a competitive race with China over AI leadership, with recent measures including restricting Chinese access to advanced AI models from companies like Anthropic.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pax_Silica">Pax Silica</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#US-China competition`, `#AI regulation`, `#Anthropic`

---

<a id="item-22"></a>
## [Chinese Tech Giants Invest in AI-Powered Weight Management](https://36kr.com/p/3896639942592134?f=rss) ⭐️ 6.0/10

Ant Group invested hundreds of millions of yuan in Boohee Health, becoming its largest external shareholder, while JD Health and Tencent Health launched AI-driven weight management programs. These moves signal a strategic shift to boost user engagement in digital health through high-frequency weight management scenarios. Weight management is a high-frequency, sticky use case that can drive user retention for AI health apps, which often suffer from low engagement in serious medical scenarios. This trend could reshape digital health competition in China, with implications for GLP-1 drug integration and personalized nutrition. Boohee Health has over 200 million users, a food database of 1.6 million items, and recently launched an enterprise AI platform 'Boohee Science AI'. Ant Group's health assistant app 'AFU' integrates Boohee's food recognition database, and has 100 million users with 10 million daily consultations.

rss · 36氪 · Jul 16, 02:21

**Background**: AI health apps in China face low user retention because serious medical interactions are infrequent. Weight management combines daily monitoring, dietary tracking, and drug intervention (like GLP-1 agonists), making it an ideal high-frequency scenario. CRO (Contract Research Organization) firms support clinical trials for weight-loss drugs, and GLP-1 drugs have become a booming market in China.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dzwww.com/news/yw/202607/t20260713_17927336.htm">实验猴身价突破20万元，“今年的猴子已被客户订完”_推荐_大众网</a></li>
<li><a href="https://www.rundo-cro.com/newsinfo/8519651.html">rundo- cro .com/newsinfo/8519651.html</a></li>

</ul>
</details>

**Tags**: `#AI in healthcare`, `#weight management`, `#Chinese tech giants`, `#digital health`, `#user engagement`

---

<a id="item-23"></a>
## [PongBot Aura: Multi-Sport AI Coach Robot Raises $4M on Kickstarter](https://36kr.com/p/3896586337978244?f=rss) ⭐️ 6.0/10

Chinese startup PongBot launched Aura, the world's first ultralight AI coach robot for tennis, pickleball, and padel, raising nearly $4 million on Kickstarter within hours. This product shifts smart sports hardware from single-sport tools to a versatile, AI-driven coaching platform, potentially lowering the barrier for beginners to explore multiple racket sports. Aura weighs only 7 kg, features a 120fps dual-camera module (Spotter) with 10 TOPS edge AI, and uses a patented adaptive wheel track to handle different ball types with micron-level precision.

rss · 36氪 · Jul 16, 01:30

**Background**: Traditional ball machines are single-sport devices that cannot adjust for different ball physics. PongBot's previous PACE series focused on high-speed tennis training. Aura's AI Coach system provides real-time form corrections and adaptive ball feeding, unlike post-training analysis tools like SwingVision.

<details><summary>References</summary>
<ul>
<li><a href="https://store.pongbotsports.com/pages/pongbot-aura">PONGBOT Aura - Al Multi - Sport Robot for Tennis, Pickleball & Padel</a></li>
<li><a href="https://www.kickstarter.com/projects/pongbot/aura-the-worlds-first-ultra-light-ai-multi-sport-robot">Pongbot Aura -The First Ultralight AI Coach Multi - Sport Robot</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Sports Hardware`, `#Robotics`, `#Crowdfunding`, `#Consumer Technology`

---

<a id="item-24"></a>
## [Microsoft Developing AI Tool Inspired by Mythos for Vulnerability Detection](https://36kr.com/newsflashes/3898938728924807?f=rss) ⭐️ 6.0/10

Microsoft is reportedly developing an AI-powered tool inspired by Anthropic's Mythos to automatically detect and fix software vulnerabilities, leveraging multiple AI models. This could significantly enhance software security by automating vulnerability discovery and remediation, reducing reliance on manual audits and potentially preventing high-profile breaches. The tool is said to use multiple AI models to not only detect but also fix security flaws, though specific technical details and release timeline remain undisclosed.

rss · 36氪 · Jul 16, 23:42

**Background**: Anthropic's Mythos, built on the Claude Opus 4.6 model, recently demonstrated the ability to find 271 zero-day vulnerabilities in Firefox, highlighting AI's potential in cybersecurity. Traditional vulnerability detection often relies on static analysis or manual code review, which can be time-consuming and miss complex flaws. AI-driven tools like Mythos promise faster, more comprehensive scanning, but validating and patching discovered vulnerabilities without breaking systems remains a challenge.

<details><summary>References</summary>
<ul>
<li><a href="https://kalinga.ai/ai-vulnerability-detection-2026/">AI Vulnerability Detection : Ultimate 2026 Security Shift</a></li>
<li><a href="https://www.periculo.co.uk/cyber-security-blog/claude-mythos-finds-271-zero-days-in-firefox-with-ai">Claude Mythos Finds 271 Zero-Days in Firefox with AI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#vulnerability detection`, `#Microsoft`, `#software security`, `#cybersecurity`

---

<a id="item-25"></a>
## [SpaceXAI Launches Grok 4.5 with Competitive Token Pricing](https://36kr.com/newsflashes/3898893880362882?f=rss) ⭐️ 6.0/10

SpaceXAI announced the launch of Grok 4.5, with pricing set at $2 per million input tokens and $6 per million output tokens. Automation features are now available on the Grok website, iOS, and Android apps, and Grok 4.5 is accessible via Grok Build, Cursor, and the xAI console. This pricing undercuts many competitors like OpenAI and Anthropic, potentially making Grok 4.5 an attractive option for developers and enterprises. The integration with tools like Grok Build and Cursor expands xAI's ecosystem and could accelerate adoption of their models in coding and automation workflows. Grok 4.5 pricing is notably cheaper than GPT-4o (where input is $2.50/$10 per million tokens for different tiers) and Claude 3.5 Sonnet ($3/$15 per million tokens). The model is available through both API and direct use in Grok Build, which is a terminal-first coding agent that plans changes and writes code.

rss · 36氪 · Jul 16, 23:13

**Background**: In AI language models, tokens are units of text (words or fragments) that models process; pricing is based on tokens consumed. Grok Build is a command-line coding agent from xAI that runs in the terminal, plans code changes, and shows diffs before applying. This launch positions xAI competitively in the growing market for AI coding assistants.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.x.ai/build/overview">Grok Build | SpaceXAI Docs</a></li>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>

</ul>
</details>

**Tags**: `#AI`, `#pricing`, `#Grok`, `#language models`

---

<a id="item-26"></a>
## [Coca-Cola suspends Fairlife dairy production after ransomware attack](https://techcrunch.com/2026/07/16/coca-cola-suspended-production-at-its-fairlife-dairy-after-a-ransomware-attack/) ⭐️ 6.0/10

Coca-Cola announced that production at its Fairlife dairy unit in the United States will remain suspended following a ransomware attack. This incident disrupts the supply chain for Fairlife, a popular dairy brand, and highlights the vulnerability of critical food production infrastructure to cyberattacks. Coca-Cola stated that production will 'remain suspended' but did not provide a timeline for resumption or details on the ransom demand.

rss · TechCrunch · Jul 16, 21:22

**Background**: Ransomware is a type of malware that encrypts a victim's files, demanding payment to restore access. Fairlife is a dairy brand owned by Coca-Cola, known for its ultrafiltered milk products. Such attacks can halt production systems and compromise data, leading to operational disruptions.

**Tags**: `#ransomware`, `#cybersecurity`, `#Coca-Cola`, `#Fairlife`

---

<a id="item-27"></a>
## [BP Shuts Down Corporate Venture Arm After 20 Years](https://techcrunch.com/2026/07/16/oil-giant-bp-shutters-its-corporate-venture-arm-after-20-years/) ⭐️ 6.0/10

BP is shutting down its corporate venture arm, BP Ventures, after nearly 20 years of operation, citing lackluster returns. This marks a significant retreat by a major oil company from corporate venture capital, reflecting broader challenges in aligning venture investments with core energy business strategies. BP Ventures was established in the mid-2000s to invest in innovative energy technologies, but reportedly failed to generate satisfactory financial returns.

rss · TechCrunch · Jul 16, 17:37

**Background**: Corporate venture capital (CVC) arms are investment units within large corporations that make equity investments in external startups. They aim to gain strategic insights, access new technologies, and generate financial returns. BP Ventures was one of the early CVCs in the energy sector.

**Tags**: `#corporate venture capital`, `#BP`, `#energy`, `#venture capital`, `#shutdown`

---

<a id="item-28"></a>
## [X uses Grok AI to combat content theft and engagement bait](https://techcrunch.com/2026/07/16/x-cracks-down-on-creators-who-steal-content/) ⭐️ 6.0/10

X announced it will deploy its Grok AI to detect stolen content on the platform, automatically redirect revenue from ads or subscriptions to the original creators, and crack down on engagement bait. This policy update leverages AI to protect creator rights and incentivize original content, potentially shifting the balance of power in the creator economy and setting a precedent for other social platforms. The Grok AI model will analyze content for unauthorized reuse and automatically redirect payouts to verified original creators. Engagement bait, such as misleading prompts to drive interaction, will also be penalized.

rss · TechCrunch · Jul 16, 16:40

**Background**: Grok is a generative AI chatbot developed by SpaceXAI and integrated with X. It has been controversial but is now being applied to content moderation. X has increasingly focused on the creator economy, including ad revenue sharing and subscription-based monetization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Grok_AI">Grok AI</a></li>
<li><a href="https://x.ai/grok">Grok — Truth-seeking AI Chatbot with Voice & Image... | SpaceXAI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#content moderation`, `#social media`, `#X (Twitter)`, `#creator economy`

---

<a id="item-29"></a>
## [Sheryl Sandberg Leads $10M Investment in AI Vehicle Inspection Startup](https://techcrunch.com/2026/07/16/sheryl-sandberg-leads-10-million-investment-in-ai-powered-vehicle-inspection-service/) ⭐️ 6.0/10

Sheryl Sandberg led a $10 million investment round in an AI startup that allows enterprise customers to use smartphones to scan and detect vehicle damage. The company, founded in 2021, uses computer vision to automate vehicle inspections. This investment signals growing confidence in AI-powered vehicle inspection solutions, which can streamline insurance claims, rental car returns, and pre-owned vehicle assessments. It also highlights the potential of smartphone-based systems to democratize access to advanced damage detection. The startup's technology analyzes images captured by a standard smartphone camera to identify dents, scratches, and other exterior damage. The $10 million investment is led by Sheryl Sandberg, former COO of Meta, and will be used to scale the platform.

rss · TechCrunch · Jul 16, 15:00

**Background**: AI-powered vehicle damage detection uses computer vision and machine learning to automatically assess a car's condition from photos. Companies like Hertz are already using similar AI scanning systems to check rental cars for damage upon return. Such systems can reduce human error and speed up inspections.

<details><summary>References</summary>
<ul>
<li><a href="https://inspektlabs.com/blog/top-10-ai-powered-car-damage-inspection-solutions-2/">AI Car Damage Detection Software: 10 Best Tools (2026)</a></li>
<li><a href="https://damagevision.com/">Damage Vision — AI Vehicle Damage Assessment Platform</a></li>
<li><a href="https://www.caranddriver.com/news/a65176049/hertz-ai-scan-rental-car-damage/">caranddriver.com/news/a65176049/hertz-ai- scan -rental-car- damage</a></li>

</ul>
</details>

**Tags**: `#AI`, `#investment`, `#vehicle inspection`, `#computer vision`

---

<a id="item-30"></a>
## [AMI Labs CEO Rejects AGI, Superintelligence Labels](https://techcrunch.com/2026/07/16/why-ami-labs-alexandre-lebrun-wont-call-his-ai-agi-or-superintelligence/) ⭐️ 6.0/10

Alexandre LeBrun, CEO of AMI Labs—a world model startup backed by Yann LeCun—publicly dismissed the terms 'AGI' and 'superintelligence' as misleading hype, advocating for a more grounded approach to AI development. LeBrun's stance challenges the prevalent hype around AGI and superintelligence, promoting a realistic discourse that could influence how the AI community sets expectations and allocates research efforts. AMI Labs focuses on building world models—AI systems that simulate environments to enable planning and reasoning—rather than pursuing the broad goal of AGI. LeBrun's comments come from an opinion piece with limited technical details.

rss · TechCrunch · Jul 16, 14:40

**Background**: World models are AI systems that learn internal representations of environments to predict dynamics and plan actions. Unlike large language models that only generate text, world models simulate physics and causality, enabling autonomous decision-making in robotics and autonomous driving. This makes them a promising but distinct path compared to scaling LLMs toward AGI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#AGI`, `#superintelligence`, `#startup`

---

<a id="item-31"></a>
## [Space reproduction hurdle: early human cells develop poorly in microgravity](https://www.scmp.com/news/china/science/article/3360680/chinese-scientists-have-bad-news-having-babies-space-there-silver-lining?utm_source=rss_feed) ⭐️ 6.0/10

Chinese scientists cultured early-stage human reproductive cells aboard the Tianzhou cargo spacecraft and found that they grew and developed much worse in microgravity compared to Earth. This research highlights a critical barrier for long-term space colonization and human reproduction beyond Earth, emphasizing the need for countermeasures or artificial gravity solutions. The experiments were conducted on two Tianzhou cargo missions, providing direct microgravity exposure for early-stage human reproductive cells, which are the precursors to sperm and eggs.

rss · SCMP · Jul 16, 23:30

**Background**: The Tianzhou is a series of Chinese automated cargo spacecraft used to resupply China's space station, capable of carrying experiments. Microgravity is known to affect biological processes. This study specifically examines the earliest stages of human reproduction.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tianzhou_cargo_spacecraft">Tianzhou cargo spacecraft</a></li>

</ul>
</details>

**Tags**: `#space biology`, `#human reproduction`, `#microgravity`, `#Chinese space program`, `#space colonization`

---

<a id="item-32"></a>
## [Xpeng aims to mass-produce humanoid robot globally by 2027](https://www.scmp.com/business/china-business/article/3360814/race-against-tesla-china-ev-maker-xpeng-launch-viral-humanoid-globally-2027?utm_source=rss_feed) ⭐️ 6.0/10

Chinese EV maker Xpeng announced its next-generation humanoid robot 'Iron' will begin global commercial deliveries in 2027, with monthly production capacity exceeding 1,000 units by the end of 2026. This positions Xpeng as a direct competitor to Tesla in the physical AI race. Xpeng's ambitious timeline marks a significant step in the physical AI race, potentially accelerating the integration of intelligent robotics into manufacturing and services. Success could challenge Tesla's dominance in humanoid robotics and reshape global automation. Xpeng expects to produce over 1,000 humanoid robots per month by the end of 2026, leveraging its existing EV manufacturing capacity for the global launch of the Iron robot in 2027. The company has not disclosed specific technical specs or pricing.

rss · SCMP · Jul 16, 23:00

**Background**: Physical AI refers to the integration of intelligent software with physical hardware like robots and sensors, enabling autonomous interaction with the real world. Xpeng, primarily an electric vehicle maker, is diversifying into robotics, competing with Tesla's Optimus humanoid robot. The company's manufacturing expertise in EVs provides a potential edge in scaling production of complex electromechanical systems.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Physical_AI">Physical AI</a></li>
<li><a href="https://irisdynamics.com/articles/physical-ai-smart-linear-motors">What is Physical AI ? The Role of Smart Linear Motors in Intelligent...</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#humanoid`, `#EV`, `#AI`, `#manufacturing`

---

<a id="item-33"></a>
## [Nvidia CEO meets Japanese execs in yakitori summit](https://www.scmp.com/news/asia/east-asia/article/3360794/nvidia-chief-jensen-huang-seals-japan-robotics-push-after-yakitori-summit?utm_source=rss_feed) ⭐️ 6.0/10

Nvidia CEO Jensen Huang held a "yakitori summit" with Japanese semiconductor executives in Tokyo to strengthen cooperation, particularly in robotics. This signals Nvidia's strategic push to deepen ties with Japan's semiconductor supply chain, which is critical for robotics and AI chip production. The meeting took place at a yakitori restaurant near Kanda Station, involving executives from semiconductor materials and components companies.

rss · SCMP · Jul 16, 08:52

**Background**: Nvidia is a leading AI chipmaker, and Japan is a key player in semiconductor materials and equipment. The "yakitori summit" is an informal business meeting over grilled skewers, common in Japanese corporate culture.

**Tags**: `#Nvidia`, `#Jensen Huang`, `#Japan`, `#semiconductor`, `#robotics`

---

<a id="item-34"></a>
## [China Plans Asteroid Early Warning System](https://www.scmp.com/news/china/science/article/3360783/china-building-early-warning-system-spot-earth-smashing-asteroids?utm_source=rss_feed) ⭐️ 6.0/10

China plans to build an early warning system using ground-based telescopes and a satellite constellation to detect hazardous asteroids, according to scientist Li Mingtao. This initiative adds to global planetary defense efforts, enhancing humanity's ability to protect Earth from potentially catastrophic asteroid impacts. The system will combine multiple ground-based telescopes with an orbital constellation, though specific timetables and technical specifications have not been disclosed.

rss · SCMP · Jul 16, 08:00

**Background**: Asteroids larger than 140 meters can cause devastating regional damage if they strike Earth. NASA's NEO Surveyor and other missions aim to catalog at least two-thirds of such objects. China's proposed system complements these efforts by adding dedicated space-based and ground-based assets.

<details><summary>References</summary>
<ul>
<li><a href="https://www.space.com/china-asteroid-detection-satellite-constellation-idea">Asteroids threatening Earth could be spotted by spacecraft... | Space</a></li>
<li><a href="https://www.jpl.nasa.gov/missions/near-earth-object-surveyor/">Near-Earth Object Surveyor | NASA Jet Propulsion Laboratory (JPL)</a></li>

</ul>
</details>

**Tags**: `#space`, `#asteroids`, `#early warning system`, `#China`, `#planetary defense`

---