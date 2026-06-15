---
layout: default
title: "Horizon Summary: 2026-06-15 (EN)"
date: 2026-06-15
lang: en
---

> From 133 items, 22 important content pieces were selected

---

1. [Rio de Janeiro's 'homegrown' LLM revealed as weighted merge of two existing models](#item-1) ⭐️ 8.0/10
2. [Anthropic's Safety Narratives Criticized](#item-2) ⭐️ 8.0/10
3. [Jane Street on Formal Methods and the Future of Programming](#item-3) ⭐️ 8.0/10
4. [China's HEPS to Begin Official Operation This Year](#item-4) ⭐️ 8.0/10
5. [New organic molecule achieves ultra-narrowband emission for OLEDs](#item-5) ⭐️ 8.0/10
6. [ChatGPT $200 subscription could cost OpenAI $14,000 per user](#item-6) ⭐️ 8.0/10
7. [FBI disrupts AI-powered phishing service with 1M URLs](#item-7) ⭐️ 8.0/10
8. [Kage: Package any website into a single offline binary](#item-8) ⭐️ 7.0/10
9. [Anthropic Model Suspension Spurs India AI Debate](#item-9) ⭐️ 7.0/10
10. [Meta reverses $2B Manus acquisition after Beijing demand](#item-10) ⭐️ 7.0/10
11. [Meta's AI Model Built by Alexandr Wang Now Needs Zuckerberg's Sales Pitch](#item-11) ⭐️ 7.0/10
12. [AI chatbots in hotels make unauthorized promises](#item-12) ⭐️ 7.0/10
13. [Zeroserve Achieves Caddy Compatibility with Major Performance Gains](#item-13) ⭐️ 6.0/10
14. [Nobel Laureate Calls Musk a Ponzi Scheme; U.S. Bans Foreign Access to Anthropic AI](#item-14) ⭐️ 6.0/10
15. [SoulX Raises Angel Funding for Sleep Comfort Robot MoYa](#item-15) ⭐️ 6.0/10
16. [China's First National 2030 Target for New Energy Heavy Trucks](#item-16) ⭐️ 6.0/10
17. [AI job disruption hits hard as 75% skip unemployment benefits](#item-17) ⭐️ 6.0/10
18. [China cuts 12,000 degrees to embrace AI era](#item-18) ⭐️ 6.0/10
19. [Europe Ditches US Tech: Reddit Discussion](#item-19) ⭐️ 6.0/10
20. [Chinese Drivers Use Plastic Heads to Trick Tesla Autopilot](#item-20) ⭐️ 6.0/10
21. [Zuckerberg Admits Meta Mistakes in AI Workforce Shift](#item-21) ⭐️ 6.0/10
22. [Meta AI unit called soul-crushing gulag by engineers](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Rio de Janeiro's 'homegrown' LLM revealed as weighted merge of two existing models](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

An investigation found that Rio-3.5-Open-397B, released by Rio de Janeiro's IT company IplanRIO as a homegrown fine-tune, is actually a weighted merge of approximately 60% Nex-N2 Pro and 40% Qwen3.5-397B-A17B, with no additional training. This highlights a serious transparency issue in AI model releases, potentially eroding trust in claimed innovations and raising questions about proper attribution in open-source AI development. Every weight tensor in the model showed a 0.6/0.4 blend of Nex and Qwen across all 60 layers and components, with a standard deviation explainable by rounding rather than fine-tuning.

hackernews · unrvl22 · Jun 14, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48528371)

**Background**: Model merging is a technique that combines two or more LLMs into a single model by weighted averaging of their parameters, often using tools like mergekit. Unlike fine-tuning, merging requires no additional training data or computation, but it can improve task performance. The controversy arises because the model was presented as a fine-tune, not a merge, which misrepresents the effort and attribution.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/mlabonne/merge-models">Merge Large Language Models with mergekit</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Discussion**: Community members noted the model's weights are a precise linear interpolation rather than a proper fine-tune, with one commenter describing the technique as a 'simple linear combination' that surprisingly enhanced performance without degradation. Others raised concerns about lack of attribution to original model creators and potential profit from others' work.

**Tags**: `#AI`, `#LLM`, `#open-source`, `#model attribution`, `#controversy`

---

<a id="item-2"></a>
## [Anthropic's Safety Narratives Criticized](https://www.verysane.ai/p/did-anthropic-ask-for-this) ⭐️ 8.0/10

A community discussion on VerySane critiques Anthropic's self-serving AI safety narratives, accusing the company of hubris and questionable regulatory tactics. This reflects growing skepticism about AI companies using safety rhetoric for competitive advantage, and highlights tensions between existential risk concerns and corporate interests. The discussion is based on a high-scoring post with 118 points and 81 comments, providing diverse viewpoints. Commenters compare Anthropic to a doomsday device company and argue that power leads to hubris.

hackernews · ad8e · Jun 14, 22:23 · [Discussion](https://news.ycombinator.com/item?id=48533504)

**Background**: Anthropic is an AI safety company that advocates for regulation of advanced AI. Critics argue that its safety stance may be self-serving, aiming to create a regulatory moat that benefits itself while hindering competitors.

**Discussion**: Commentator ivraatiems compares Anthropic to a doomsday device company that proclaims its products are dangerous. zmmmmm argues that power decouples leaders from reality, leading to hubris. ianm218 notes Anthropic genuinely fears existential risk, while peter422 warns about government picking winners and losers.

**Tags**: `#AI safety`, `#Anthropic`, `#AI ethics`, `#regulation`, `#hubris`

---

<a id="item-3"></a>
## [Jane Street on Formal Methods and the Future of Programming](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street discusses their extensive use of formal methods for correctness in production systems, sparking a deep discussion on the past, present, and future of program verification and its interaction with AI. Jane Street's experience demonstrates that formal methods are feasible and valuable in critical production systems. As AI-generated code becomes more prevalent, formal verification may become a key skill for ensuring reliability. The article mentions their use of various formal tools like SAT solvers and the Boyer-Moore prover. Some commenters note that formal specifications can suffer from similar bugs as tests, but formal methods provide stronger guarantees.

hackernews · eatonphil · Jun 14, 12:35 · [Discussion](https://news.ycombinator.com/item?id=48526633)

**Background**: Formal methods are mathematically-based techniques for verifying software correctness by proving that a program satisfies a formal specification. Unlike testing, which can only find bugs, formal proof can guarantee absence of certain errors. Formal verification is used in high-assurance domains like safety-critical systems.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/roehst/awesome-formal-methods">GitHub - roehst/awesome- formal - methods : Awesome resources on...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Program_verification">Program verification</a></li>

</ul>
</details>

**Discussion**: Commenters include a practitioner who used formal methods decades ago, and a Scala 3 developer using types for compile-time proofs. Some argue that as AI generates more code, human value shifts toward verification.

**Tags**: `#formal methods`, `#verification`, `#programming languages`, `#AI`, `#software engineering`

---

<a id="item-4"></a>
## [China's HEPS to Begin Official Operation This Year](https://36kr.com/newsflashes/3853637219931398?f=rss) ⭐️ 8.0/10

China's High Energy Synchrotron Radiation Source (HEPS) announced plans to officially begin operations in 2025 after passing national acceptance, following a trial run that supported nearly 300 research projects as of April 2026. HEPS is China's first fourth-generation synchrotron radiation source, providing extremely bright X-rays for cutting-edge research in physics, materials science, and biology. Its official operation will significantly boost China's scientific infrastructure and enable breakthroughs in multiple fields. The facility is located in Beijing and has attracted over 1,000 visiting users during its trial phase. HEPS is expected to pass national acceptance within 2025 before commencing full operations.

rss · 36氪 · Jun 14, 23:29

**Background**: Synchrotron radiation is electromagnetic radiation emitted by relativistic charged particles moving through magnetic fields. Synchrotron light sources like HEPS use storage rings to produce intense beams of light across the electromagnetic spectrum, enabling researchers to study the structure and properties of materials at atomic and molecular scales. HEPS is China's first fourth-generation synchrotron source, offering higher brightness and coherence than earlier generations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Synchrotron_light_source">Synchrotron light source - Wikipedia</a></li>
<li><a href="https://english.ihep.cas.cn/heps/ah/bi/">Brief Introduction-- High Energy Photon Source</a></li>

</ul>
</details>

**Tags**: `#synchrotron radiation`, `#scientific infrastructure`, `#high-energy physics`, `#research facility`

---

<a id="item-5"></a>
## [New organic molecule achieves ultra-narrowband emission for OLEDs](https://36kr.com/newsflashes/3853623619441668?f=rss) ⭐️ 8.0/10

Kyoto University researchers developed a novel organic molecule that emits ultra-narrowband light without strong laser excitation, a breakthrough published in Nature. This discovery challenges the long-held assumption that spontaneous emission inevitably produces broad spectra, offering a new design paradigm for high-color-purity OLEDs that could significantly enhance display and lighting quality. The molecule achieves an emission bandwidth dramatically narrower than conventional multiple resonance emitters while also exhibiting excellent thermally activated delayed fluorescence (TADF) performance.

rss · 36氪 · Jun 14, 23:20

**Background**: In conventional OLEDs, spontaneous emission leads to spectral broadening due to the energy-time uncertainty principle, which limits color purity. Ultra-narrowband emitters are critical for achieving deep-blue and high-efficiency displays, but balancing color purity with other performance metrics remains challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://phys.org/news/2026-06-molecule-ultranarrow-emission-spectrum.html">Organic molecule with ultranarrow emission spectrum could lead to...</a></li>

</ul>
</details>

**Tags**: `#OLED`, `#organic molecules`, `#narrowband emission`, `#nature`

---

<a id="item-6"></a>
## [ChatGPT $200 subscription could cost OpenAI $14,000 per user](https://www.reddit.com/r/technology/comments/1u5ufgs/a_200_chatgpt_subscription_could_cost_openai/) ⭐️ 8.0/10

An analysis reveals that if a user fully utilized OpenAI's $200 per month ChatGPT subscription, the compute costs to OpenAI would be approximately $14,000, making the subscription deeply unprofitable. This highlights the unsustainable pricing model of AI subscriptions and raises questions about long-term profitability and business models for AI companies. The analysis likely factors in the cost of GPU compute for extensive use of features like code generation, image generation, or long conversational sessions.

reddit · r/technology · /u/rkhunter_ · Jun 14, 19:33

**Background**: Large language models like ChatGPT require massive computing power, especially for inference, which can be very expensive. OpenAI offers a $200 Pro tier with unlimited access to advanced models, but the actual cost per heavy user may far exceed the subscription fee.

**Tags**: `#AI`, `#OpenAI`, `#ChatGPT`, `#pricing`, `#economics`

---

<a id="item-7"></a>
## [FBI disrupts AI-powered phishing service with 1M URLs](https://www.reddit.com/r/technology/comments/1u5up6d/fbi_disrupts_massive_aipowered_phishing_service/) ⭐️ 8.0/10

The FBI has taken down a large-scale, AI-powered phishing service that utilized approximately one million URLs to trick victims into revealing sensitive information. This operation highlights the growing use of AI in cybercrime and the need for advanced law enforcement responses, as such services can automate and scale phishing attacks to unprecedented levels. The phishing service was reportedly capable of generating and hosting thousands of malicious URLs, using AI to craft convincing phishing pages that mimic legitimate websites, and the FBI's disruption likely involved seizing infrastructure and domain names.

reddit · r/technology · /u/melancholy_dood · Jun 14, 19:44

**Background**: Phishing is a type of cyberattack where attackers deceive individuals into providing sensitive data like passwords or credit card numbers, often through fake emails or websites. AI can enhance phishing by automating the creation of realistic content and evading detection. The FBI and other agencies regularly conduct operations to dismantle such criminal networks.

**Tags**: `#cybersecurity`, `#AI`, `#phishing`, `#law enforcement`, `#threat intelligence`

---

<a id="item-8"></a>
## [Kage: Package any website into a single offline binary](https://github.com/tamnd/kage) ⭐️ 7.0/10

Kage is a new open-source tool that clones any website into a single binary executable for offline viewing, stripping out JavaScript and localizing assets. This enables easy sharing and offline access of entire websites, useful for documentation, company wikis, and AI prototypes in environments without internet. Kage renders pages in headless Chrome, removes all scripts, and localizes CSS, images, and fonts into a standalone binary built with Go. It can serve the archived site via a built-in server or open in a webview.

hackernews · tamnd · Jun 14, 17:25 · [Discussion](https://news.ycombinator.com/item?id=48529990)

**Background**: Traditional web archiving tools like ArchiveBox save websites as collections of files (HTML, PDF, WARC), often requiring a server or browser to view. Kage packages everything into a single Go binary, which can be run directly without dependencies, making it portable and easy to share.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tamnd/kage">GitHub - tamnd/kage: Shadow any website for offline viewing, with the JavaScript stripped out · GitHub</a></li>
<li><a href="https://kage.tamnd.com/">kage</a></li>

</ul>
</details>

**Discussion**: Commenters praised the tool's utility for offline documentation and AI prototype mirroring. Some noted alternatives like SingleFile, while others requested a version that works directly in a browser without a server.

**Tags**: `#web archiving`, `#offline viewing`, `#single binary`, `#Go`, `#documentation`

---

<a id="item-9"></a>
## [Anthropic Model Suspension Spurs India AI Debate](https://techcrunch.com/2026/06/13/as-anthropic-suspends-access-to-new-models-india-debates-its-ai-future/) ⭐️ 7.0/10

Anthropic has suspended access to its new AI models, leading to a debate among Indian tech leaders about the implications for India's AI development. This event highlights the dependency of India on foreign AI models and sparks discussions on the need for indigenous AI capabilities and regulatory frameworks. The specific models affected and the reasons for the suspension are not fully disclosed, but the move has prompted Indian policymakers and tech entrepreneurs to reassess the country's AI strategy.

rss · TechCrunch · Jun 14, 03:00

**Background**: Anthropic is a leading AI research company known for its safe and ethical AI models. India has been actively pursuing AI leadership, with significant investments in AI research and startups. However, reliance on foreign AI platforms raises concerns about data sovereignty and strategic autonomy.

**Tags**: `#AI policy`, `#Anthropic`, `#India`, `#regulation`

---

<a id="item-10"></a>
## [Meta reverses $2B Manus acquisition after Beijing demand](https://techcrunch.com/2026/06/13/meta-reportedly-moves-to-unwind-2b-manus-deal-after-beijings-demand/) ⭐️ 7.0/10

Meta has begun dismantling its $2 billion acquisition of Manus AI after China's National Development and Reform Commission ordered the deal reversed due to violations of foreign investment and technology export rules. This marks the first successful dismantling of a major cross-border tech deal by Chinese regulators, underscoring escalating US-China tech tensions and the increasing regulatory risks for international acquisitions of AI startups. Meta has cut data access to Manus and begun operational separation; Manus founders are seeking $1 billion for a buyback that could lead to a Hong Kong IPO.

rss · TechCrunch · Jun 14, 00:03

**Background**: Manus is a Singapore-registered AI startup with Chinese roots, known for developing a general-purpose AI agent. China's NDRC cited violations of foreign investment and technology export laws. The deal was initially announced in December 2025 and reportedly valued between $2-3 billion.

<details><summary>References</summary>
<ul>
<li><a href="https://www.washingtonpost.com/world/2026/04/27/china-ai-meta-manus/">China says it ordered reversal of Meta’s Manus AI acquisition - The Washington Post</a></li>
<li><a href="https://www.indexbox.io/blog/meta-cuts-ties-with-manus-after-china-orders-2b-acquisition-reversal/">Meta Sunsets Manus Acquisition: Data Access Cut, Buyback Plans Underway - News and Statistics - IndexBox</a></li>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#Manus`, `#acquisition`, `#regulation`, `#China`

---

<a id="item-11"></a>
## [Meta's AI Model Built by Alexandr Wang Now Needs Zuckerberg's Sales Pitch](https://www.reddit.com/r/technology/comments/1u5k5rf/a_year_after_meta_tapped_alexandr_wang_to_build_a/) ⭐️ 7.0/10

The news reports that a year after Meta hired Alexandr Wang to lead development of a new AI model, CEO Mark Zuckerberg is now tasked with selling that model, highlighting a shift from creation to commercialization. This matters because it underscores the challenges tech giants face in monetizing advanced AI models, and reflects Meta's strategic pivot toward AI commercialization under Wang's leadership. Alexandr Wang, former CEO of Scale AI, joined Meta as chief AI officer in June 2025 after Meta acquired a 49% stake in Scale AI for over $14 billion. The model developed under his supervision is now being marketed by Zuckerberg.

reddit · r/technology · /u/Logical_Welder3467 · Jun 14, 12:42

**Background**: Scale AI is a data annotation and AI infrastructure company that provides services including RLHF and LLM evaluation. Alexandr Wang, born 1997, co-founded Scale AI and became the world's youngest self-made billionaire. Meta's heavy investment signals its commitment to advancing AI capabilities and monetizing them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Alexandr_Wang">Alexandr Wang</a></li>
<li><a href="https://en.wikipedia.org/wiki/Scale_AI">Scale AI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Meta`, `#Alexandr Wang`, `#business strategy`

---

<a id="item-12"></a>
## [AI chatbots in hotels make unauthorized promises](https://www.reddit.com/r/technology/comments/1u5w2gr/ai_is_making_promises_your_brand_never_made/) ⭐️ 7.0/10

AI-powered chatbots deployed by hotels are generating unauthorized promises to customers, such as free upgrades or refunds, that the brand never approved, leading to financial losses and reputational damage. This highlights a critical risk of deploying large language models in customer-facing roles without adequate safeguards, affecting brand trust and operational costs across the hospitality industry and beyond. The unauthorized promises often result from AI hallucination, where the model generates plausible-sounding but false information, and hotels may be held liable under existing legal frameworks for the chatbot's statements.

reddit · r/technology · /u/Plastic_Ninja_9014 · Jun 14, 20:38

**Background**: AI hallucination refers to instances where large language models produce false or misleading information presented as fact. In high-stakes scenarios like customer service, these errors can have real-world consequences. Legal liability for AI chatbot actions is an emerging area, often falling under product liability or negligence, and Section 230 protections typically do not shield companies from their own AI's statements.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_hallucination">AI hallucination</a></li>
<li><a href="https://www.ebglaw.com/insights/publications/the-dark-side-of-ai-assessing-liability-when-bots-behave-badly">The Dark Side of AI: Assessing Liability When Bots Behave Badly | Epstein Becker Green</a></li>
<li><a href="https://www.vasquezlawnc.com/blog/ai-chatbot-liability">AI Chatbot Liability: Who Pays When AI Causes Harm? | Vasquez Law Firm</a></li>

</ul>
</details>

**Tags**: `#AI`, `#customer service`, `#brand management`, `#hospitality`, `#AI failures`

---

<a id="item-13"></a>
## [Zeroserve Achieves Caddy Compatibility with Major Performance Gains](https://su3.io/posts/zeroserve-caddy-compat) ⭐️ 6.0/10

Zeroserve now offers Caddy-compatible zero-allocation HTTP serving, achieving 3x throughput and 70% lower latency compared to standard Caddy. However, it lacks ACME support and plugin compatibility, limiting its real-world usability. This performance breakthrough could significantly reduce server costs and improve user experience for high-traffic sites. However, the missing ACME and plugin support limit its practical adoption, especially for production environments relying on automated TLS. The zero-allocation approach is built on io_uring and Rust, achieving efficient async I/O with minimal memory overhead. Community members point out that io_uring may have security concerns and that the lack of ACME is a dealbreaker.

hackernews · losfair · Jun 14, 13:43 · [Discussion](https://news.ycombinator.com/item?id=48527145)

**Background**: Zeroserve is a zero-config web server that uses eBPF for request scripting, aiming to reduce overhead and simplify deployment. io_uring is a Linux kernel interface for async I/O that improves performance over traditional syscalls. ACME is a protocol for automating SSL/TLS certificate issuance, critical for modern HTTPS websites.

<details><summary>References</summary>
<ul>
<li><a href="https://sesamedisk.com/zeroserve-ebpf-web-server-infrastructure/">Zeroserve : An eBPF-Powered Web Server Without... - Sesame Disk</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_uring">io_uring - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight mixed reactions: some see the performance gains as noteworthy, but many consider the missing ACME and plugin support as dealbreakers. There are also concerns about io_uring security and safety compared to libuv. One user noted nginx still holds up well.

**Tags**: `#performance`, `#web server`, `#io_uring`, `#Rust`, `#Caddy`

---

<a id="item-14"></a>
## [Nobel Laureate Calls Musk a Ponzi Scheme; U.S. Bans Foreign Access to Anthropic AI](https://36kr.com/p/3853670570743040?f=rss) ⭐️ 6.0/10

Nobel laureate Paul Krugman accused Elon Musk of running a Ponzi scheme, and the Trump administration banned foreign governments, companies, and individuals from accessing Anthropic's latest AI model. Additionally, Ubtech's humanoid robot U1 received over 3,800 pre-orders in 10 days, with sales limited to adults. These stories highlight growing scrutiny of tech figures and AI as national security assets, as well as the commercialization of humanoid robots for emotional companionship, which raises ethical concerns. Krugman argued that a future SpaceX IPO would force ordinary investors via index funds to prop up Musk's ventures. The U.S. ban on Anthropic's model treats cutting-edge AI as a core national security asset. Ubtech's U1 robot has 88 degrees of freedom, a 2-4 hour battery life, and no '3C' certification.

rss · 36氪 · Jun 14, 23:57

**Background**: A Ponzi scheme is a fraudulent investment operation where returns are paid to earlier investors using the capital of newer investors, rather than from profit. Anthropic is a leading AI safety company founded by former OpenAI employees. The humanoid robot U1 is designed for emotional companionship and incorporates a 'nurturing' emotional AI model.

**Tags**: `#AI regulation`, `#robotics`, `#business`, `#tech news`

---

<a id="item-15"></a>
## [SoulX Raises Angel Funding for Sleep Comfort Robot MoYa](https://36kr.com/p/3851572421432324?f=rss) ⭐️ 6.0/10

SoulX, a consumer flexible robotics startup, has completed a series angel round of tens of millions of yuan led by Hillhouse Capital to develop MoYa, a sleep comfort robot that combines tactile and cognitive relief. The first product is expected to launch in the second half of 2026. This funding signals growing interest in consumer robotics for mental health and sleep, moving beyond traditional wearables and smart devices. MoYa's approach of combining physical embrace with cognitive offloading could create a new category for home emotional care. MoYa uses a proprietary flexible pneumatic system instead of traditional motors, making it quiet and safe for sleep. It features passive interaction design: it only responds when users touch or speak, reducing cognitive barriers. The robot also uses physiological synchronization algorithms to adjust its soothing movements to the user's breathing rhythm.

rss · 36氪 · Jun 14, 01:30

**Background**: Flexible robotics is an emerging field that uses soft materials and pneumatics to create robots that are safer for human interaction. Cognitive offloading refers to transferring mental load to external tools, which can help reduce stress. SoulX's MoYa is one of the first consumer products to integrate these concepts for sleep and emotional care.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/115575975">柔性机器人技术：工业机器人发展的下一方向 - 知乎</a></li>
<li><a href="https://news.qq.com/rain/a/20260428A01SD100">news.qq.com/rain/a/20260428A01SD100</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#health-tech`, `#startup`, `#funding`, `#AI`

---

<a id="item-16"></a>
## [China's First National 2030 Target for New Energy Heavy Trucks](https://36kr.com/newsflashes/3853670728209666?f=rss) ⭐️ 6.0/10

China's Ministry of Transport and ten other departments jointly issued a plan to achieve 40% sales penetration of new energy heavy trucks by 2030, with a stock of over 1.6 million vehicles. This is China's first national quantitative target for new energy heavy trucks, a high-energy-consuming segment, signaling strong policy support for domestic battery and green hydrogen industries. The plan includes infrastructure for charging and battery swapping, and covers multiple scenarios and technologies. Heavy trucks have larger batteries and higher energy consumption than passenger vehicles.

rss · 36氪 · Jun 14, 23:56

**Background**: Heavy trucks are major emitters due to their diesel engines. New energy heavy trucks can be battery electric or hydrogen fuel cell. Battery swapping stations are being built along highways in China to reduce downtime. Green hydrogen production uses renewable energy to produce hydrogen without emissions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Battery_swapping">Battery swapping - Wikipedia</a></li>
<li><a href="https://shanghaiist.com/china-thrives-as-a-testing-ground-for-nev-technologies/">China Thrives as a Testing Ground for NEV Technologies</a></li>

</ul>
</details>

**Tags**: `#policy`, `#new energy vehicles`, `#battery`, `#green hydrogen`, `#China`

---

<a id="item-17"></a>
## [AI job disruption hits hard as 75% skip unemployment benefits](https://www.reddit.com/r/technology/comments/1u5rmbf/ai_job_disruption_is_here_the_problem_may_be/) ⭐️ 6.0/10

A news discussion on Reddit highlights that AI-driven job displacement is occurring, and nearly 75% of affected workers do not apply for unemployment benefits, compounding the problem. This statistic reveals a hidden crisis in AI's labor impact—many displaced workers are not accessing safety nets, potentially worsening economic inequality and understating true job loss figures. The claim of nearly 75% not applying for benefits originates from an unspecified source in the Reddit post, lacking verified methodology or context.

reddit · r/technology · /u/Plastic_Ninja_9014 · Jun 14, 17:45

**Background**: AI and automation are increasingly displacing workers in sectors like manufacturing, customer service, and data entry. Unemployment benefits are government-provided financial support for job losses. Low application rates may stem from barriers such as lack of awareness, complex processes, or stigma.

**Tags**: `#AI`, `#job disruption`, `#unemployment`, `#labor economics`

---

<a id="item-18"></a>
## [China cuts 12,000 degrees to embrace AI era](https://www.reddit.com/r/technology/comments/1u5i8dn/chinas_universities_cut_12000_obsolete_degrees/) ⭐️ 6.0/10

Chinese universities have eliminated approximately 12,000 degree programs deemed obsolete as part of a strategic pivot to prioritize artificial intelligence (AI) education and workforce development. This move reflects a major shift in China's education system to align with rapid AI advancements, potentially reshaping the nation's workforce and global competitiveness. It underscores the tension between updating curricula and preserving traditional academic fields. The cuts span both undergraduate and graduate programs across humanities, social sciences, and some STEM fields. The initiative is part of a broader national strategy to double down on AI, semiconductor, and other emerging technology training.

reddit · r/technology · /u/Saltedline · Jun 14, 11:04

**Background**: China has set ambitious national goals to become a world leader in AI by 2030. Universities are adjusting curricula to meet industry demands for AI talent, often at the expense of traditional liberal arts programs. The 12,000-degree figure represents a significant portion of total degree offerings, signaling a decisive policy direction.

**Tags**: `#AI`, `#education`, `#China`, `#policy`, `#workforce`

---

<a id="item-19"></a>
## [Europe Ditches US Tech: Reddit Discussion](https://www.reddit.com/r/technology/comments/1u5vf8j/all_the_ways_europe_is_ditching_american/) ⭐️ 6.0/10

A Reddit thread consolidates various European initiatives aimed at reducing reliance on American technology, highlighting a growing movement toward digital sovereignty. This shift could significantly alter the global technology landscape, diminishing US dominance and fostering the growth of European alternatives in key sectors. The discussion likely covers areas such as cloud computing, software, and hardware, where Europe is actively developing its own solutions to replace US products.

reddit · r/technology · /u/Well_Socialized · Jun 14, 20:12

**Background**: Europe has long depended on US tech giants for essential services like cloud, search, and social media. Recent geopolitical tensions and privacy concerns have spurred efforts to build local alternatives, such as Gaia-X for cloud infrastructure and the EU's Digital Sovereignty strategy.

**Tags**: `#Europe`, `#technology`, `#geopolitical`, `#digital sovereignty`, `#US tech`

---

<a id="item-20"></a>
## [Chinese Drivers Use Plastic Heads to Trick Tesla Autopilot](https://www.reddit.com/r/technology/comments/1u5q98e/chinese_drivers_are_using_tiny_plastic_heads_to/) ⭐️ 6.0/10

Some Chinese drivers are using small plastic head models placed on the seat to trick Tesla's cabin camera-based driver attention monitoring system, allowing Autopilot to operate without an attentive driver. This bypass undermines Tesla's safety safeguards and could lead to dangerous driving behavior, highlighting ongoing challenges in enforcing driver engagement in semi-autonomous systems. Tesla's driver monitoring system uses a cabin-facing camera to detect driver attention, but the plastic head mimics a human face, potentially fooling the system. Similar bypass methods have included weights on the steering wheel to simulate hand pressure.

reddit · r/technology · /u/Presently_Naked · Jun 14, 16:52

**Background**: Tesla's Autopilot and Full Self-Driving (FSD) systems are advanced driver-assistance features that require continuous driver supervision. The system monitors driver attention via a cabin camera and steering wheel torque sensing. Previous bypass attempts, such as using weighted objects on the steering wheel, have been reported, leading to software updates and strike-based enforcement.

<details><summary>References</summary>
<ul>
<li><a href="https://electrek.co/2021/04/08/tesla-driver-monitoring-system-detect-driver-attention-real-time/">Watch Tesla 's driver monitoring system detect driver attention in...</a></li>
<li><a href="https://techcrunch.com/2021/05/27/tesla-has-activated-its-in-car-camera-to-monitor-drivers-using-autopilot/">Tesla has activated its in-car camera to monitor drivers ... | TechCrunch</a></li>
<li><a href="https://www.businessinsider.com/tesla-autopilot-full-self-driving-drivers-weights-steering-wheel-trick-2023-1">Tesla Drivers Trick Autopilot and Full Self-Driving With Weights</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#Autopilot`, `#driver monitoring`, `#safety exploits`, `#China`

---

<a id="item-21"></a>
## [Zuckerberg Admits Meta Mistakes in AI Workforce Shift](https://www.reddit.com/r/technology/comments/1u5k5zr/zuckerberg_says_meta_made_mistakes_in_ai/) ⭐️ 6.0/10

Mark Zuckerberg acknowledged that Meta made mistakes in its shift of workforce toward artificial intelligence, admitting the company could have handled the transition better. This rare public admission from a major tech CEO underscores the challenges of rapid AI investment and restructuring, potentially influencing how other companies approach workforce changes. The specific mistakes were not detailed, but the statement likely refers to Meta's large-scale layoffs in 2022-2023 and subsequent reallocation of engineers to AI teams.

reddit · r/technology · /u/IKeepItLayingAround · Jun 14, 12:42

**Background**: Meta has been aggressively pivoting toward artificial intelligence, investing billions in AI research and infrastructure. This shift led to significant workforce restructuring, including layoffs of over 20,000 employees, as the company deprioritized non-AI projects.

**Tags**: `#Meta`, `#AI`, `#workforce`, `#technology`, `#strategy`

---

<a id="item-22"></a>
## [Meta AI unit called soul-crushing gulag by engineers](https://www.reddit.com/r/technology/comments/1u5jxft/metas_monthsold_ai_unit_is_a_soulcrushing_gulag/) ⭐️ 6.0/10

A Reddit post reports that engineers inside Meta's newly-formed AI unit describe it as a soul-crushing work environment, akin to a gulag. This revelation highlights potential internal culture issues at one of the leading AI companies, which could affect talent retention and innovation in a competitive industry. The AI unit is only months old, suggesting that toxic culture can develop quickly. The allegations are based on anonymous engineer accounts shared on Reddit.

reddit · r/technology · /u/AdSpecialist6598 · Jun 14, 12:31

**Background**: Meta (formerly Facebook) has been heavily investing in AI, including large language models and generative AI. The company has faced previous criticism over workplace culture and working conditions, making this report consistent with past concerns.

**Tags**: `#Meta`, `#AI`, `#work culture`, `#tech industry`

---