---
layout: default
title: "Horizon Summary: 2026-11-28 (EN)"
date: 2026-11-28
lang: en
---

> From 68 items, 11 important content pieces were selected

---

1. [Google's DeepCrossAttention matches model quality up to 3x faster](#item-1) ⭐️ 8.0/10
2. [WebRTC-Abusing Credit Card Skimmers Found on Popular Shopping Sites](#item-2) ⭐️ 8.0/10
3. [State attorneys general sue SpaceX over Grok generating CSAM and non-consensual images](#item-3) ⭐️ 8.0/10
4. [Convex coding skill accused of silently uploading user app ideas](#item-4) ⭐️ 7.0/10
5. [djb's "False Computer-Checked Proofs" catalogs verifier soundness bugs, sparking trust debate](#item-5) ⭐️ 7.0/10
6. [Washington Signals Readiness to Intervene Aggressively in the U.S.-China AI Race](#item-6) ⭐️ 7.0/10
7. [China ground-tests world's first metal-powder afterburner for jet engines](#item-7) ⭐️ 7.0/10
8. [Hackers Breach US Air Force's Cloud One Platform, Risking Sensitive Military Data](#item-8) ⭐️ 7.0/10
9. [Atari Homebrew Awards Cancelled Over Flood of AI-Generated Entries](#item-9) ⭐️ 6.0/10
10. [Show HN: Bouncemarket, a Prediction Market Game for a Bouncing Ball](#item-10) ⭐️ 6.0/10
11. [Dutch trade minister vows to fight US MATCH Act on chip export controls](#item-11) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Google's DeepCrossAttention matches model quality up to 3x faster](https://research.google/blog/supercharging-transformer-residual-connections/) ⭐️ 8.0/10

Google Research introduced DeepCrossAttention (DCA), a transformer architecture that replaces the standard point-wise summation in residual connections with learnable weights and depth-wise cross-attention over previous layers' outputs. The team reports that DCA reaches comparable model quality while training up to 3x faster, and achieves lower perplexity for a given parameter budget and training time for only a minimal increase in parameters. Residual connections have been essentially unchanged since ResNet and underpin every modern transformer, so a drop-in modification that cuts training time by up to 3x could lower the cost of building large language models across the industry. Because the gain comes from better information flow rather than from a new attention kernel or sparsity scheme, it can in principle be stacked on top of existing efficiency techniques such as FlashAttention or Mixture-of-Experts. The core diagnosis is that a plain residual connection adds a layer's output to its input with equal weight, which dilutes useful earlier representations as networks get deeper; DCA instead learns how much to draw from each prior layer. The paper appeared at ICML 2025, and the reported speedup comes with only a minimal increase in model parameters rather than the large auxiliary networks some competing approaches require.

hackernews · ComputedCamp995 · Nov 27, 23:06 · [Discussion](https://news.ycombinator.com/item?id=50672565)

**Background**: A transformer is built from stacked layers, each containing an attention sub-layer and a feed-forward sub-layer, and each sub-layer is wrapped in a residual (or skip) connection that adds its input directly to its output. These connections were introduced in ResNet for convolutional networks and are what make very deep models trainable at all, since they give gradients a short path back through the network. In a standard transformer that addition is a fixed, parameter-free sum, so every earlier layer's representation contributes equally regardless of relevance.

<details><summary>References</summary>
<ul>
<li><a href="https://research.google/blog/supercharging-transformer-residual-connections/">Supercharging transformer residual connections</a></li>
<li><a href="https://arxiv.org/html/2502.06785">DeepCrossAttention : Supercharging Transformer Residual...</a></li>
<li><a href="https://www.baeldung.com/cs/transformer-networks-residual-connections">Why Are Residual Connections Important in Transformer ...</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News were split between enthusiasm and nitpicking: one reader asked whether DCA could be combined with speculative-decoding techniques like MTP and DFlash that already delivered roughly 10x token throughput gains, while another immediately compared the idea to DenseNet's dense connectivity. A recurring criticism was presentational rather than technical, with users objecting that the benchmark results were plotted as line graphs when bar charts would be more appropriate, and one commenter simply flagged that the post's real title is "Supercharging Transformer Residual Connections."

**Tags**: `#transformers`, `#deep learning`, `#model efficiency`, `#Google Research`, `#residual connections`

---

<a id="item-2"></a>
## [WebRTC-Abusing Credit Card Skimmers Found on Popular Shopping Sites](https://www.infohawk.com/news/2026-11-27-black-friday-webrtc-skimmer) ⭐️ 8.0/10

Security researchers have discovered credit card skimming scripts planted on popular online shopping sites that use WebRTC to send stolen payment data out to attacker-controlled servers. The campaign surfaced around Black Friday, when checkout traffic peaks and skimming implants are hardest to spot. Web skimming already drains payment cards at scale, and routing exfiltration through WebRTC lets attackers slip past the CSP rules and network monitoring that most e-commerce sites rely on for protection. Anyone who runs an online store, or shops on one, is exposed, and the technique is likely to be copied by other Magecart-style groups. WebRTC's data channels and STUN/ICE traffic often fall outside the connect-src directives that content security policies enforce, and it is rarely inspected by the browser extensions and proxies that scan for card-skimmer beacons. As one commenter noted, the abuse is about low monitoring rather than any special capability of WebRTC, and the same exfiltration could be done over plain HTTP if attackers were not worried about detection.

hackernews · scanr · Nov 27, 15:40 · [Discussion](https://news.ycombinator.com/item?id=50668145)

**Background**: Web skimming, often called Magecart after the criminal groups that popularized it, works by injecting JavaScript into the checkout pages of hacked or third-party-supplied storefront code so that card numbers are copied as shoppers type them. Sites commonly defend themselves with Content Security Policy, a browser mechanism that restricts which domains a page may connect to, plus script-integrity checks and client-side monitoring. WebRTC is a browser standard for real-time audio, video and peer-to-peer data transfer that opens connections outside the normal fetch/XHR path, which makes it a convenient and less-watched channel for smuggling data out.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebRTC">WebRTC - Wikipedia</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/hackers-abuse-google-apps-script-to-steal-credit-cards-bypass-csp/">Hackers abuse Google Apps Script to steal credit cards , bypass CSP</a></li>
<li><a href="https://www.zdnet.com/article/inter-a-low-bar-kit-for-magecart-website-credit-card-skimmer-attacks/">Inter: a ‘low bar’ kit for Magecart credit card skimmer ... - ZDNET</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News treated the finding as a vindication for ad and script blocking, arguing that embedding third-party scripts on a site leaves you permanently vulnerable no matter what the script does. Others pushed further, saying the web's model of letting strangers execute arbitrary code in your browser is fundamentally broken, questioning why ad networks and browsers don't sandbox or block JavaScript in ads entirely, and noting that payment still relies on symmetric secrets despite decades of asymmetric cryptography.

**Tags**: `#security`, `#web-security`, `#e-commerce`, `#webrtc`, `#skimming`

---

<a id="item-3"></a>
## [State attorneys general sue SpaceX over Grok generating CSAM and non-consensual images](https://www.oag.state.va.us/media-center/news-releases/jay-jones/3162-attorneys-general-jones-and-rayfield-file-suit-against-spacex-parent-company-of-x-xai-and-grok-over-creation-and-promotion-of-child-exploitation-and-non-consensual-images-on-platform) ⭐️ 8.0/10

A group of state attorneys general, including Virginia's Jay Jones and Oregon's Dan Rayfield, filed suit against SpaceX — the parent company of xAI, X and Grok — alleging that the Grok model created and promoted child sexual abuse material (CSAM) and non-consensual intimate imagery. The action targets the corporate parent rather than only the model developer, and is framed around both the creation and the promotion of such content on the platform. This is one of the first major law-enforcement actions by state AGs against an AI model owner over harmful outputs, which could establish a template for holding AI companies liable for what their models generate. A ruling either way would shape content-moderation obligations for generative AI platforms far beyond Grok itself. The complaint names SpaceX as the defendant because xAI became a SpaceX subsidiary after its 2026 acquisition, so liability questions now run through the corporate structure rather than to a standalone AI startup. A central factual dispute is whether Grok produced such imagery by default or only after users deliberately jailbroke it, and how existing First Amendment carve-outs for material depicting real children apply to synthetic output.

hackernews · DeepLogin · Nov 27, 19:42 · [Discussion](https://news.ycombinator.com/item?id=50670855)

**Background**: Grok is the family of language, image and video models built by xAI, the Elon Musk-founded company whose chatbot is tightly integrated with the X social network. xAI was founded in March 2023, combined with X Corp. in March 2025, and acquired by SpaceX in February 2026 at a reported $250 billion valuation, later rebranded around the SpaceX name. Grok has repeatedly drawn controversy, including for sexual deepfakes and extremist outputs, making it a frequent target for regulators and advocacy groups.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">XAI (company)</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceXAI">SpaceXAI - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were puzzled about how the images were produced, asking whether Grok was simply unusually permissive for all users or whether people had to deliberately trick it. Others asked why the users requesting the material were not the focus, and one commenter argued that Supreme Court precedent protects AI-generated CSAM made for personal consumption, while noting the carve-out requires it not depict or involve real children — a distinction they said likely does not extend to revenge porn.

**Tags**: `#AI safety`, `#generative AI`, `#content moderation`, `#law`, `#policy`

---

<a id="item-4"></a>
## [Convex coding skill accused of silently uploading user app ideas](https://github.com/convex/convex-backend-skill/issues/64) ⭐️ 7.0/10

A GitHub issue (#64) in the convex/convex-backend-skill repository alleges that Convex's official Agent Skill sends the user's app idea — the prompt describing what they want to build — to a remote server without disclosing it. The report drew a direct public reply from Convex CEO Jamie, who confirmed the prompt upload exists and said it powers Convex's "quickstart" feature, the successor to the now-shut-down Convex Chef vibe-coding product. AI coding agents and their skill packages run with broad access to a developer's project and intentions, so undisclosed telemetry on prompts is a trust problem for the whole ecosystem of vendor-supplied agent tooling. Because Convex markets itself as a backend platform that already stores your code and data, developers are now asking where the line is between hosting and quietly harvesting ideas. The allegation concerns a single skill in one repository rather than the Convex backend itself, and no evidence of malicious intent was presented; the CEO framed the upload as a feature-enabling behavior rather than data collection. Commenters noted that uploading prompts is a distinct risk from prompt injection, and that the quickstart path is opt-in only in the sense that installing the skill enables it by default.

hackernews · MickyTheMouse · Nov 27, 18:02 · [Discussion](https://news.ycombinator.com/item?id=50669765)

**Background**: Convex is a reactive backend platform that replaces your database, server functions and file storage with a single TypeScript-centric stack, and it also publishes "Agent Skills" — portable packages of instructions and workflows (SKILL.md files, installed via the npx skills CLI) that teach AI coding agents how to set up auth, design schemas or run migrations. Prompt injection, by contrast, is an attack in which crafted input manipulates a model into unintended behavior, catalogued by OWASP as LLM01:2025. The distinction matters here: this incident is about a vendor's own agent silently exfiltrating context, not an outside attacker hijacking the model.

<details><summary>References</summary>
<ul>
<li><a href="https://www.convex.dev/">Convex | All gas, no breakages</a></li>
<li><a href="https://docs.convex.dev/ai/agent-skills">Convex Agent Skills | Convex Developer Hub</a></li>
<li><a href="https://genai.owasp.org/llmrisk/llm01-prompt-injection/">LLM01:2025 Prompt Injection - OWASP Gen AI Security Project</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread (80 comments) is split between appreciation for the CEO showing up to clarify and lingering unease about defaults: one top commenter concluded that self-hosted open-weight models are "the way to go in the long run," another summarized the mood as "trust is the new attention," and a third noted prompt injection is far more common than models making malicious tool calls on their own. A few commenters also flagged off-topic self-promotion in the thread, and some pushed back that a single bug report is being treated as a field-wide scandal.

**Tags**: `#privacy`, `#AI developer tools`, `#prompt injection`, `#trust & security`, `#hackernews discussion`

---

<a id="item-5"></a>
## [djb's "False Computer-Checked Proofs" catalogs verifier soundness bugs, sparking trust debate](https://cr.yp.to/proofs/falseccp.html) ⭐️ 7.0/10

Daniel J. Bernstein (djb) published a page on cr.yp.to titled "False computer-checked proofs" that catalogs reported soundness bugs in proof checkers for major formal systems including Lean, Coq/Rocq, Isabelle, HOL Light, HOL4, Mizar and Metamath. The page argues that because a checker itself can be buggy, a "computer-checked" proof is not automatically a true proof, and calls for smaller trusted checkers and machine-checked proofs of checker correctness. Formal verification is increasingly used as the gold standard for mathematics (large Lean formalization projects) and for safety-critical software certified under standards such as DO-178C, so questions about the trustworthiness of the checker kernel directly affect how much assurance those results actually provide. The piece reframes trust in formal proofs as a question of toolchain engineering and redundancy rather than an all-or-nothing guarantee. According to coverage of the page, it compiles roughly 199 reports of soundness bugs across these checkers, with Coq/Rocq-related reports accelerating sharply in recent years; a soundness bug means the kernel accepts a proof of something that is not actually provable, as in the Lean 4 kernel bug that accepted a proof of False with no axioms. Bernstein's proposed mitigations are smaller, simpler trusted kernels and formally verified checkers rather than trusting a single large implementation.

hackernews · _tk_ · Nov 27, 15:26 · [Discussion](https://news.ycombinator.com/item?id=50667989)

**Background**: A proof assistant such as Lean, Coq/Rocq, Isabelle or HOL lets mathematicians and engineers write fully formal proofs that a small core program, the kernel, re-checks step by step; the entire assurance of the system rests on that kernel being correct. A soundness bug breaks this foundation: the kernel accepts a derivation it should have rejected, so the checked statement is not actually established. Because kernels are large, hand-written pieces of software, the community has long relied on redundancy — checking the same proof with multiple independently written verifiers — as a practical defense.

<details><summary>References</summary>
<ul>
<li><a href="https://news.lavx.hu/article/d-j-bernstein-catalogs-soundness-bugs-in-seven-proof-checkers">D. J. Bernstein catalogs soundness bugs in seven proof ...</a></li>
<li><a href="https://agihunt.info/en/p/1a1d0b69bfe4cfe1212d6812c41">199 reports of soundness bugs in proof checkers… · AGI Hunt</a></li>
<li><a href="https://essamamdani.com/blog/lean-4-soundness-bug-14576-postmortem">Lean 4 Soundness Bug #14576: What Broke the... | Essa Mamdani</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely pushed back on the practical severity: twotwotwo noted the gap between one faulty verification and actually misleading mathematicians, since an exploit must simultaneously break multiple checkers without the input looking implausible on informal review (a DeepMind researcher once built a "proof" passing Lean and a then-week-old nanoda). dwheeler pointed out that Metamath's main databases require proofs to pass five independently created verifiers in five languages, while gr_norm argued that all known soundness bugs in decades-old systems would fit in a tweet and are more than good enough for 99.9% of software; andai added the deeper worry that a proof can be correct relative to a wrong formalization of the goal.

**Tags**: `#formal-verification`, `#proof-assistants`, `#lean`, `#metamath`, `#soundness-bugs`

---

<a id="item-6"></a>
## [Washington Signals Readiness to Intervene Aggressively in the U.S.-China AI Race](https://www.bloomberg.com/news/articles/2026-11-27/trump-s-ai-gambit-fuels-wild-thanksgiving-week-on-wall-street) ⭐️ 7.0/10

During Thanksgiving week, Washington sent an unmistakable message that the U.S. must do whatever it takes to win the artificial-intelligence race with China, and that the government is prepared to intervene directly to make that happen. The signal drove sharp, volatile moves across Wall Street as investors repriced AI-related assets around the prospect of heavier state involvement. The message marks a shift from the U.S. government acting mainly as a regulator and subsidy provider toward open, aggressive intervention in the AI sector, which could reshape how AI companies are funded, which firms win government backing, and how capital flows into the industry. Because AI stocks now dominate U.S. index performance, any policy signal from Washington now moves markets well beyond the tech sector. The excerpt does not specify which instruments Washington is considering — export controls, direct investment, procurement, antitrust action or subsidies — nor which companies would be affected. The market reaction was described as a "wild" week, indicating high volatility and sensitivity to policy headlines rather than a settled reassessment of fundamentals.

rss · Bloomberg Markets · Nov 27, 18:43

**Background**: The U.S. and China have been locked in a technology competition for years, with Washington using export controls on advanced semiconductors and chipmaking equipment, investment screening, and industrial subsidies to slow China's progress in AI and computing. AI model training depends heavily on high-end GPUs and specialized chips, which makes semiconductor policy a central lever in that competition. In this context, a statement that the government is "prepared to intervene" signals a possible escalation beyond existing tools, and equity markets treat such signals as indicators of future rules, funding, and winners.

**Tags**: `#AI policy`, `#US-China tech competition`, `#government intervention`, `#Wall Street`, `#AI industry`

---

<a id="item-7"></a>
## [China ground-tests world's first metal-powder afterburner for jet engines](https://www.scmp.com/news/china/science/article/3376081/china-test-fires-worlds-first-metal-powder-fuelled-afterburner-fighter-jets) ⭐️ 7.0/10

A research team led by Sun Haijun at Nanchang Hangkong University in Jiangxi has conducted ground tests of a prototype turbojet afterburner that burns metal powder instead of kerosene, with state-run Science and Technology Daily calling it a world first. If validated, metal-powder afterburners could raise thrust and energy density beyond the temperature and thrust-response limits of kerosene, but the work is an early ground-test prototype and its practical impact on fighter propulsion remains unproven. The test involved a turbojet afterburner rather than the main combustor, and the metal powder is reportedly a high-energy material such as aluminum or magnesium; engineering challenges include stable powder feeding, complete combustion, ash deposition, and particle erosion.

rss · SCMP · Nov 27, 13:00

**Background**: An afterburner injects and burns extra fuel in the exhaust stream of a military turbojet or turbofan to produce a short burst of thrust, traditionally using aviation kerosene. Metal powders such as aluminum have high volumetric energy density and have long been studied for ramjets and rocket propellants, but feeding and burning them reliably in a high-speed engine is difficult.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3376081/china-test-fires-worlds-first-metal-powder-fuelled-afterburner-fighter-jets">China test-fires world’s first metal powder-fuelled ... China team ground-tests metal powder afterburner for jet engines China test-fires world’s first metal powder-fuelled ... China tests turbojet engine using metal powder instead of ... Progress and challenges in exploration of powder fueled ... Experimental Investigation of Powdered Metals Fuel Ramjet Combustion Performance and Deposit Characteristics of Boron ...</a></li>
<li><a href="https://en.topwar.ru/294281-kitaj-ispytal-turboreaktivnyj-dvigatel-na-metallicheskom-poroshke-vmesto-kerosina.html">China tests turbojet engine using metal powder instead of kerosene</a></li>
<li><a href="https://piqmarkets.com/story/china-team-ground-tests-metal-powder-afterburner-for-jet-engines">China team ground-tests metal powder afterburner for jet engines</a></li>

</ul>
</details>

**Tags**: `#aerospace propulsion`, `#metal powder fuel`, `#jet engines`, `#afterburner`, `#China research`

---

<a id="item-8"></a>
## [Hackers Breach US Air Force's Cloud One Platform, Risking Sensitive Military Data](https://www.scmp.com/news/world/united-states-canada/article/3376087/hackers-breach-us-air-force-cloud-one-platform-putting-military-data-risk) ⭐️ 7.0/10

Hackers breached the US Air Force's flagship Cloud One cloud computing platform, with the intrusion discovered within roughly the past month during upgrade work on the system, according to three people familiar with the matter. The discovery led to disruption across the platform, and the Air Force declined to comment on security specifics, saying only that it continuously takes measures to protect Department of the Air Force information and systems. Cloud One is one of the largest cloud platforms used by the US military, so a breach there could jeopardize a vast swath of sensitive tactical, personnel and logistics data rather than a single application. The incident also lands just days after reports that a CIA database had been accessed, heightening concern about the resilience of government cloud infrastructure at large. The report is based on anonymous sources rather than an official disclosure, and the Air Force has not confirmed the scope, the attackers, or what data, if any, was actually exfiltrated. Details remain thin on how the intrusion was achieved and exactly which systems or tenants on the shared platform were affected.

rss · SCMP · Nov 27, 12:25

**Background**: Cloud One was initiated in 2017 as a one-stop shop for the Air Force's IT needs, pooling the resources of several commercial cloud operators into a common computing environment with standardized security guardrails. The idea is to let mission teams build and deploy applications on accredited cloud infrastructure without each unit re-solving baseline security and compliance. Because such a platform concentrates many workloads and tenants under one set of controls, a compromise at the platform level can potentially ripple far beyond a single program.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/nov/27/hackers-breach-us-air-force-cloud-computing">Hackers reportedly breach US air force ’s flagship cloud computing...</a></li>
<li><a href="https://nypost.com/2026/11/27/us-news/hackers-breach-us-air-force-flagship-cloud-one-computing-platform/">Hackers breach US Air Force flagship Cloud One computing platform</a></li>
<li><a href="https://www.zerohedge.com/technology/hackers-breach-usafs-critical-cloud-one-platform-insiders-warn-its-big-deal">Hackers Breach USAF 's Critical Cloud One Platform As... | ZeroHedge</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#cloud security`, `#US Air Force`, `#government IT`, `#data breach`

---

<a id="item-9"></a>
## [Atari Homebrew Awards Cancelled Over Flood of AI-Generated Entries](https://forums.atariage.com/topic/394894-atari-homebrew-awards-cancelled/) ⭐️ 6.0/10

The Atari Homebrew Awards, an annual community event honouring new games made by hobbyists for classic Atari hardware, has been suspended for its ninth edition. Organiser James of ZeroPage Homebrew announced the cancellation, stating that with a flood of AI-generated entries he "saw no path forward" and could not determine how much of each submission's work was actually done by a human. The cancellation shows that generative AI is now disrupting even the most insular creative communities — niche retro-computing scenes that were widely assumed to be immune because people write software for obsolete machines purely for fun. It raises hard questions about verification, trust and fair recognition that other game jams, awards and open-source contests will soon face. The core problem is verification: the organiser concluded there is no practical way to audit a submission and quantify how much code, art or design was produced with AI assistance. Rather than run an award he could not judge fairly, he chose to suspend the event entirely, a decision framed as closing the programme rather than merely pausing one cycle.

hackernews · bpierre · Nov 28, 02:03 · [Discussion](https://news.ycombinator.com/item?id=50673688)

**Background**: Homebrew refers to software written by hobbyists for hardware that is long out of production and officially unsupported, such as the Atari 2600 and 7800 consoles. Writing such games requires detailed knowledge of quirky, poorly documented hardware, and the challenge itself is usually the point — people port obscure titles to new machines as an exercise in learning. The Atari Homebrew Awards, run by the ZeroPage Homebrew channel, were an annual showcase that gave these hobbyists public recognition for that work.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gamesradar.com/games/flood-of-new-ai-games-kills-retro-homebrew-competition-this-is-an-extremely-upsetting-conclusion/">"Flood of new AI games" kills retro homebrew ... | GamesRadar+</a></li>
<li><a href="https://dzen.ru/b/awpPbltzf1mXxL5a">Девятую премию за игры для Atari отменили из-за ИИ... | Дзен</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely sympathetic, with several praising the organiser for having the clarity to walk away when the event's founding conditions no longer held. Others expressed surprise that vintage computing — a scene driven by the joy of learning constrained hardware — proved vulnerable to AI submissions at all. The most common counterproposal was to split the awards into separate AI-assisted and fully human categories, so that both could still be celebrated.

**Tags**: `#retro-computing`, `#homebrew`, `#AI-generated-content`, `#game-development`, `#community`

---

<a id="item-10"></a>
## [Show HN: Bouncemarket, a Prediction Market Game for a Bouncing Ball](https://bouncemarket.minhanhday.com/) ⭐️ 6.0/10

A developer released bouncemarket, a browser-based game in which a ball is simulated server-side and players trade shares on where it will land, with the full drop streamed to each client as server-sent events. The post drew 341 points and 115 comments on Hacker News, with the author noting that AI traders run on simple hand-written rules and drop out of any round with more than five human players. The project turns abstract prediction-market mechanics into a fast, playable toy, making questions about arbitrage, liquidity and bot competition tangible for a general audience. It also prompted discussion about whether markets on pure random events could work with real money, an experiment commenters say has not really been tried. Every drop is fully deterministic from the ball's starting position, so rounds can be replayed exactly for later analysis, yet tiny variations in the initial position can flip the final outcome. Players complained that odds can jump from 0.01 to 0.99 in about a tenth of a second, making it hard to react before the ball settles.

hackernews · mday404 · Nov 27, 15:01 · [Discussion](https://news.ycombinator.com/item?id=50667726)

**Background**: Server-sent events (SSE) is a standard browser technology that lets a server push a continuous stream of updates over a single HTTP connection, via the EventSource JavaScript API, which suits real-time feeds like this ball's trajectory. The ball's motion is an example of deterministic chaos: the simulation has no randomness, but because outcomes are extremely sensitive to initial conditions, tiny unknowns make long-term prediction practically impossible — the same butterfly-effect property seen in weather models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Server-sent_events">Server-sent events</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deterministic_chaos">Deterministic chaos</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events">Using server-sent events - Web APIs | MDN - MDN Web Docs</a></li>

</ul>
</details>

**Discussion**: Commenters surfaced strategies the author had not intended: one said simply buying both kinds of cheap shares wins regardless of the outcome, while another reported a +42.21 profit in a single round buying Right shares at an average of 0.19. Others argued the game is really a battle of bots, since a frontier model given only the URL could quickly write an exact solver and exploit the unknown fractional part of the starting position, which the ball's chaotic path gradually reveals.

**Tags**: `#show-hn`, `#prediction-markets`, `#game-design`, `#server-sent-events`, `#chaotic-systems`

---

<a id="item-11"></a>
## [Dutch trade minister vows to fight US MATCH Act on chip export controls](https://www.scmp.com/economy/global-economy/article/3376024/netherlands-will-not-be-dictated-trade-chief-says-fight-against-us-match-act) ⭐️ 6.0/10

Dutch Trade Minister Sjoerd Sjoerdsma told the lower house on Thursday that the cabinet would do "everything in its power" to stop the US Multilateral Alignment of Technology Controls on Hardware (MATCH) Act from being adopted, and conceded that the Nvidia export-control dispute has made that fight harder. His remarks came just days after the Dutch foreign minister delivered a similar message during a visit to China. The Netherlands is home to ASML, the sole supplier of extreme-ultraviolet lithography machines, so Dutch resistance could shape whether Washington can push its chip-equipment export controls onto allied countries. If the MATCH Act advances, it would extend US-style restrictions to Dutch and other allied toolmakers and directly affect semiconductor supply chains serving China. The MATCH Act exists as companion bills — H.R. 8170, introduced in the House on April 2, 2026, and S. 4281, introduced in the Senate and backed by Senators Risch, Ricketts and Kim as bipartisan legislation to stop adversaries from buying "chokepoint" semiconductor manufacturing equipment. The bill text targets export restrictions on certain semiconductor manufacturing equipment and components, meaning Dutch firms such as ASML would be pressed to align with US controls rather than face unilateral American measures.

rss · SCMP · Nov 27, 09:00

**Background**: The United States has for years pressed the Netherlands and Japan to restrict exports of advanced chipmaking tools to China, arguing that controls only work if allied suppliers follow suit. The MATCH Act would formalize that logic by writing multilateral alignment into US law, so foreign equipment makers would have to match American restrictions. The "Nvidia saga" refers to the separate, ongoing controversy over US export controls on Nvidia's AI chips, which has drawn congressional scrutiny of how the Commerce Department administers those rules.

<details><summary>References</summary>
<ul>
<li><a href="https://www.govinfo.gov/app/details/BILLS-119s4281is">S. 4281 (IS) - Multilateral Alignment of Technology Controls ...</a></li>
<li><a href="https://www.foreign.senate.gov/press/rep/release/risch-ricketts-kim-introduce-match-act-level-the-global-playing-field-for-us-tech">[2026-04-08] Risch, Ricketts, Kim Introduce MATCH Act; Level ...</a></li>
<li><a href="https://www.govinfo.gov/app/details/BILLS-119hr8170ih">H.R. 8170 (IH) - Multilateral Alignment of Technology ...</a></li>

</ul>
</details>

**Tags**: `#export controls`, `#semiconductors`, `#US-Netherlands relations`, `#AI hardware`, `#technology policy`

---