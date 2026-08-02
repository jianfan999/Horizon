---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 114 items, 10 important content pieces were selected

---

1. [IBM Achieves Verifiable Quantum Advantage in Three Experiments](#item-1) ⭐️ 8.0/10
2. [Karpathy's Pelican Tweet Sparks Debate on 3D Benchmarks](#item-2) ⭐️ 7.0/10
3. [Show HN: Kakehashi – Experimental userspace to run macOS binaries on Linux ARM](#item-3) ⭐️ 7.0/10
4. [F* Showcases Proof-Oriented Programming for Verified Software](#item-4) ⭐️ 7.0/10
5. [eBay Harassment Campaign Leads to $56M Payout, Executives Sentenced](#item-5) ⭐️ 7.0/10
6. [AI Scheduler Takes Over Telescope for Autonomous Observing](#item-6) ⭐️ 7.0/10
7. [Sam Altman Calls for Slower AI, Igniting 'Decel' Debate](#item-7) ⭐️ 7.0/10
8. [Chinese scientists propose burying nuclear bomb to deflect asteroids](#item-8) ⭐️ 7.0/10
9. [Wang Hong's Fields Medal win sparks debate on China's education system](#item-9) ⭐️ 7.0/10
10. [China’s First Buyers Embrace UBTech’s U1 Pro Consumer Humanoid Robot](#item-10) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [IBM Achieves Verifiable Quantum Advantage in Three Experiments](https://36kr.com/newsflashes/3922984685022857?f=rss) ⭐️ 8.0/10

IBM and its partners demonstrated and verified quantum advantage in three independent experiments using the Quantum Heron R3 superconducting system and new error mitigation techniques. This is a major milestone for quantum computing, proving that quantum systems can deliver verifiable advantages over classical methods in practical tasks, potentially accelerating adoption in science and industry. The three experiments were all based on IBM's latest Quantum Heron R3 processor, which features 156 qubits and improved coherence, gate fidelity, and readout performance, combined with advanced error mitigation to make results reliable.

rss · 36氪 · Aug 2, 23:13

**Background**: Quantum advantage refers to a quantum computer achieving a meaningful, verifiable speedup or better result on a task that is classically intractable or impractical. Error mitigation techniques reduce the impact of noise in quantum computations without requiring full error correction. IBM's Heron series is the company's latest family of superconducting quantum processors, with the r3 revision released in July 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IBM_Heron">IBM Heron - Wikipedia</a></li>
<li><a href="https://quantum.cloud.ibm.com/docs/en/guides/processor-types">Processor types | IBM Quantum Documentation</a></li>
<li><a href="https://www.ibm.com/quantum/hardware">IBM Quantum Computing | Hardware and roadmap</a></li>

</ul>
</details>

**Tags**: `#quantum computing`, `#IBM`, `#quantum advantage`, `#error mitigation`

---

<a id="item-2"></a>
## [Karpathy's Pelican Tweet Sparks Debate on 3D Benchmarks](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Andrej Karpathy posted an AI-generated 3D scene of a pelican on a bicycle, prompting a community debate about whether such outputs should be used as benchmarks for models' physical world understanding. The tweet drew 400 points and 311 comments. This discussion highlights a growing trend of evaluating AI models beyond text and images, toward physical world reasoning. It could influence how future benchmarks are designed and how model capabilities are judged. Community members noted that some models may be specifically fine-tuned to generate three.js code, making such outputs less indicative of general physical understanding. Others argued the benchmark is deliberately qualitative and subjective, and expressed concern about lowered quality expectations due to AI content saturation.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**Background**: Physical world understanding benchmarks aim to test AI systems' grasp of object properties, relationships, and dynamics. Recent efforts include PhysBench with 10,002 entries and PAI-Bench covering real-world cases, reflecting a shift from generation quality to world modeling. Karpathy, a founding member of OpenAI and former Tesla AI director, frequently shares experimental AI outputs and insights.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2501.16411v2">[2501.16411v2] PhysBench: Benchmarking and Enhancing Vision-Language Models for Physical World Understanding</a></li>
<li><a href="https://arxiv.org/html/2512.01989v1">PAI-Bench: A Comprehensive Benchmark For Physical AI</a></li>

</ul>
</details>

**Discussion**: Reactions were mixed: some defended the benchmark as a useful qualitative measure of physical understanding, while others warned that models may be overfitted to three.js generation. Some commenters also questioned whether a janky pelican indicates solved problems, noting lowered quality expectations. A few shared practical experiences using LLMs to build 3D animations.

**Tags**: `#AI`, `#ML`, `#Benchmarking`, `#3D Generation`, `#Karpathy`

---

<a id="item-3"></a>
## [Show HN: Kakehashi – Experimental userspace to run macOS binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 7.0/10

Kakehashi is an experimental userspace project to run macOS CLI binaries natively on Linux ARM, currently demonstrating functional 7-Zip, curl, and Xcode Git with active community interest.

hackernews · vlad_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**Tags**: `#macOS`, `#Linux`, `#ARM`, `#binary-compatibility`, `#emulation`

---

<a id="item-4"></a>
## [F* Showcases Proof-Oriented Programming for Verified Software](https://fstar-lang.org/) ⭐️ 7.0/10

The F* homepage presents the language as a general-purpose, proof-oriented programming language supporting both purely functional and effectful programming. The Hacker News discussion highlights the community's interest in its syntax and practical applications, though the announcement itself is not tied to a specific release. F* is a prominent example of a proof-oriented language that aims to make formal verification practical for everyday software. As interest grows in machine-checked correctness, especially with AI-assisted verification, F*'s approach could influence how developers integrate proof obligations into real-world codebases. The language blends functional programming with effectful features, letting programmers express and verify properties within a single system. The F* homepage and community examples emphasize writing specifications alongside code, so that compiling a program is essentially checking its correctness assertions.

hackernews · ducktective · Aug 2, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49143925)

**Background**: Formal verification uses machine-checkable mathematical proofs to guarantee that software behaves exactly as intended, making it valuable for security-critical and safety-critical systems. Proof-oriented programming languages like F* aim to lower the barrier by integrating proofs and code in one language, rather than using separate verification tools. F* has been developed over many years with applications in verified cryptography and protocol implementations. Some observers predict that AI advances will push formal verification from a niche practice into mainstream software engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://fstar-lang.org/">F*: A Proof-Oriented Programming Language</a></li>
<li><a href="https://en.wikipedia.org/wiki/F*_(programming_language)">F* (programming language) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed opinions: one criticized the F* homepage for lacking inline code examples, while another praised F*'s ability to call external libraries during incremental migration of C codebases. Others asked about industry adoption and use cases, with a tutorial link shared in response. A minor joke suggested that even responsive stylesheets cannot be implemented without side effects.

**Tags**: `#proof-oriented programming`, `#formal verification`, `#functional programming`, `#programming languages`, `#software correctness`

---

<a id="item-5"></a>
## [eBay Harassment Campaign Leads to $56M Payout, Executives Sentenced](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 7.0/10

eBay executives were sentenced for orchestrating a harassment campaign against a critical couple, resulting in a $56 million payout. Former Senior Director Jim Baugh received 57 months in prison, while other team members received fines or time served. This case underscores how corporate security teams can abuse power and target private citizens, raising serious ethical and legal questions for tech companies. It also signals that courts are willing to hold senior executives personally accountable for such misconduct. Sentencing details include Brian Gilbert, former Senior Manager of Special Operations, receiving time served, one year supervised release, and a $20,000 fine. Prosecutors said seven members of eBay's security team, including former police captains, worked together to harass and intimidate the Steiners.

hackernews · JumpCrisscross · Aug 2, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49147435)

**Background**: The campaign targeted David and Ina Steiner, who ran a newsletter critical of eBay. Security team members sent threatening messages, made unwanted deliveries, and conducted surveillance, leading to the couple's fears for their safety. eBay later agreed to pay $56 million to settle the case, and the criminal convictions highlight a disturbing pattern of corporate security overreach.

**Discussion**: Commenters questioned whether the harassment stopped at just one couple, suggesting other critics may have been targeted and hoping for broader investigations. Others referenced the Behind the Bastards podcast series and a quote from Scott Adams about unsupervised people misbehaving when they believe they won't be caught.

**Tags**: `#eBay`, `#corporate misconduct`, `#legal`, `#cybersecurity`, `#accountability`

---

<a id="item-6"></a>
## [AI Scheduler Takes Over Telescope for Autonomous Observing](https://36kr.com/newsflashes/3923005684379008?f=rss) ⭐️ 7.0/10

A U.S.-based research team from Northwestern University, the University of Chicago, and Fermilab has developed an AI scheduling system that can take over a telescope and decide where to point it. The system has been deployed on the Víctor M. Blanco 4-meter Telescope in Chile, where it now directs the 570-megapixel Dark Energy Camera, and its decision-making is said to be comparable to human schedulers. This is a significant milestone on the road to fully autonomous observatories, where AI can handle rapid, time-critical observing decisions without humans in the loop. By optimizing how telescope time is allocated, such systems could increase the scientific yield of major observatories and are already being explored for facilities like the Vera C. Rubin Observatory. The AI system controls the Dark Energy Camera (DECam), a 570-megapixel wide-field instrument mounted on the Blanco Telescope at the Cerro Tololo Inter-American Observatory (CTIO) in Chile. DECam was originally built for the Dark Energy Survey between 2013 and 2019 and remains a key tool for cosmology, dark energy, and general astronomy.

rss · 36氪 · Aug 2, 23:49

**Background**: Telescope scheduling is a complex optimization problem because observatories must balance weather conditions, target visibility, scientific priorities, and instrument constraints. Automated scheduling systems such as Spike, developed for the Hubble Space Telescope in the 1980s, have long helped plan observations, and AI-based schedulers now promise to adapt dynamically to changing conditions. Similar AI-augmented scheduling approaches are also being designed for next-generation facilities like the Vera C. Rubin Observatory, which will need highly automated operations to handle enormous data volumes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dark_Energy_Camera">Dark Energy Camera</a></li>
<li><a href="https://aipromptshow.com/telescope-scheduling-can-ai-unlock-even-more-discoveries/">Telescope Scheduling: Can AI Unlock Even More Discoveries?</a></li>
<li><a href="https://fr4nc3.medium.com/ai-augmented-telescope-scheduling-at-the-vera-c-rubin-observatory-a-systems-engineering-approach-7b9934f9c122">AI-Augmented Telescope Scheduling at the Vera C. Rubin Observatory: A Systems Engineering Approach | by Francia Riesco | Medium</a></li>

</ul>
</details>

**Tags**: `#AI`, `#天文观测`, `#调度系统`, `#自动化`, `#科学仪器`

---

<a id="item-7"></a>
## [Sam Altman Calls for Slower AI, Igniting 'Decel' Debate](https://techcrunch.com/2026/08/02/sam-altman-and-ais-decel-debate/) ⭐️ 7.0/10

TechCrunch's Equity podcast, published August 2, 2026, covered Sam Altman's recent plea for the AI industry to 'pace the rate of AI development.' The episode frames the request as part of the broader decelerationist ('decel') side of AI discourse. As CEO of OpenAI, Altman is one of the most influential figures in AI, so a public call for slower development could shift industry sentiment and shape regulatory debates. Supporters see it as prudent caution, while critics view it as either alarming or as a potential brake on innovation. The term 'decel' is often used dismissively by accelerationists, many of whom identify with the e/acc community, and the accel/decel divide was a central theme in the 2023 OpenAI leadership conflict. Altman's current comments may strike some as a contrast with OpenAI's rapid rollout of products like GPT-4.

rss · TechCrunch · Aug 2, 20:54

**Background**: The AI world is split between accelerationists, who argue AI should advance as fast as possible because the benefits outweigh the risks, and decelerationists, who favor guardrails, regulation, and slower deployment. The debate gained mainstream attention after OpenAI's leadership crisis in November 2023. 'Decel' is shorthand for decelerationism, and the e/acc movement has popularized the pro-acceleration viewpoint. This context helps explain why Altman's statement carries such symbolic weight.

<details><summary>References</summary>
<ul>
<li><a href="https://quillette.com/2023/12/18/to-accelerate-or-decelerate-ai-that-is-the-question/">To Accelerate or Decelerate AI : That is the Question</a></li>
<li><a href="https://www.yahoo.com/news/decel-term-encapsulates-dueling-ideologies-082425752.html">What is a decel ? The term that encapsulates the dueling ideologies in AI</a></li>
<li><a href="https://michaelparekh.substack.com/p/ai-origin-stories-of-ai-accel-vs">AI : Origin stories of AI 'accel' vs ' decel '</a></li>

</ul>
</details>

**Tags**: `#AI`, `#policy`, `#Sam Altman`, `#ethics`, `#tech industry`

---

<a id="item-8"></a>
## [Chinese scientists propose burying nuclear bomb to deflect asteroids](https://www.scmp.com/news/china/science/article/3362361/chinese-rocket-scientists-find-most-effective-way-nuke-doomsday-asteroid?utm_source=rss_feed) ⭐️ 7.0/10

Researchers at the China Academy of Launch Vehicle Technology proposed a two-spacecraft method to deflect or destroy an Earth-threatening asteroid: first a penetrator digs a deep hole, then a second spacecraft detonates a nuclear bomb inside that hole. Their simulations indicate a 3-megaton subsurface explosion is highly effective. Subsurface nuclear detonation could deliver energy into an asteroid far more efficiently than surface or standoff bursts, potentially enabling deflection of large doomsday asteroids. This adds a new option to planetary defense portfolios, complementing kinetic impactors like NASA's DART mission. The proposed mission uses a metal penetrator to create the hole, then a second spacecraft drops the nuclear device into it. The simulation uses a 3-megaton explosion; the approach remains unvalidated experimentally and not yet published in a peer-reviewed venue.

rss · SCMP · Aug 2, 14:00

**Background**: Asteroid deflection is an active area of planetary defense research, with methods including kinetic impactors, gravity tractors, and nuclear explosions that can be detonated standoff, on the surface, or subsurface. A NASA analysis noted that non-nuclear kinetic impactors are the most mature approach, while a subsurface nuclear explosion, even at a shallow burial depth of 3 to 5 meters, can deliver enough energy to likely disrupt the target asteroid.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Asteroid_impact_avoidance">Asteroid impact avoidance - Wikipedia</a></li>
<li><a href="https://ntrs.nasa.gov/api/citations/20150022454/downloads/20150022454.pdf">Strategy Against the Asteroid Impact</a></li>
<li><a href="https://bigthink.com/hard-science/scientists-test-how-to-deflect-asteroids-with-nuclear-blasts/">Scientists test how to deflect asteroids with nuclear blasts - Big Think</a></li>

</ul>
</details>

**Tags**: `#asteroid deflection`, `#nuclear explosive`, `#planetary defense`, `#space technology`, `#China`

---

<a id="item-9"></a>
## [Wang Hong's Fields Medal win sparks debate on China's education system](https://www.scmp.com/news/china/politics/article/3362551/discouraged-university-maths-star-wang-hong-spurs-chinese-education-debate?utm_source=rss_feed) ⭐️ 7.0/10

Wang Hong, a 35-year-old mathematician, became the first Chinese woman to win the Fields Medal, but her candid remarks about feeling discouraged during her early years at an elite Chinese university have ignited a nationwide debate on education and student support. This news shines a spotlight on whether China's intense academic environment adequately supports students, especially women in STEM fields. It could influence education policy and public conversation about mental health and mentorship in universities. Wang Hong is the first Chinese woman to receive the Fields Medal, often described as mathematics' most prestigious prize. Her remarks about feeling 'discouraged' were made during interviews after the award, and they struck a chord with many young Chinese students.

rss · SCMP · Aug 2, 12:00

**Background**: The Fields Medal is awarded every four years to mathematicians under 40, and it is considered one of the highest honors in mathematics. Chinese education is known for its rigorous, exam-oriented approach, which fosters outstanding performance but may also create stress and insufficient emotional support for students. Wang Hong's experience highlights the tension between academic excellence and personal well-being in such systems.

**Tags**: `#mathematics`, `#education`, `#Fields Medal`, `#China`, `#gender in STEM`

---

<a id="item-10"></a>
## [China’s First Buyers Embrace UBTech’s U1 Pro Consumer Humanoid Robot](https://www.scmp.com/tech/tech-trends/article/3362557/first-impressions-count-chinese-buyers-open-their-homes-ubtechs-consumer-humanoids?utm_source=rss_feed) ⭐️ 6.0/10

UBTech Robotics has begun selling its U1 Pro consumer humanoid in China, and early buyers like 39-year-old Beijing investor Song are sharing why they purchased the 159,800 yuan (US$23,680) companion robot. The robot marks one of the first consumer-facing humanoid offerings from the Shenzhen-based company. This signals early consumer enthusiasm for humanoid home robots, a market long dominated by industrial and commercial uses. UBTech’s push into homes could help normalise humanoid ownership and shape expectations for AI-powered companions in China. The U1 Pro, sold under UBTech’s UWORLD consumer brand, is a lifelike companion humanoid featuring emotional AI, 88 degrees of freedom, and a launch price around US$25,000. Buyer Song noted the robot won’t cook or clean, and said 'the happiest part is often the waiting'.

rss · SCMP · Aug 2, 06:00

**Background**: Humanoid robots have historically been confined to factory floors and highly structured environments, used mostly for industrial tasks. UBTech Robotics, a Shenzhen-based company known for humanoid and smart service robots, is now trying to bring such machines into homes as companions, supported by AI technologies and realistic design.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/UBtech_Robotics">UBtech Robotics</a></li>
<li><a href="https://humanoid.guide/product/u1-pro/">UBTECH U 1 Pro Specs & Price | Humanoid .guide</a></li>
<li><a href="https://www.ubtrobot.com/en/?keyword=">UBTECH : Humanoid Robot | AI Education Robot | Commercial Robot ...</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#consumer electronics`, `#humanoid robots`, `#China tech`, `#AI`

---