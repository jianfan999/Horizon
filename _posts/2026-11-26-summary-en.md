---
layout: default
title: "Horizon Summary: 2026-11-26 (EN)"
date: 2026-11-26
lang: en
---

> From 98 items, 17 important content pieces were selected

---

1. [Scott Aaronson Stunned by Claimed 9/4 Matrix Multiplication Proof](#item-1) ⭐️ 9.0/10
2. [1Password Discloses November 2026 Security Incident](#item-2) ⭐️ 8.0/10
3. [Anthropic's GRH Lean proof shrinks to ~76k readable lines](#item-3) ⭐️ 8.0/10
4. [NFS2root: 12-year-old pre-auth remote root bug in Linux kernel NFS server](#item-4) ⭐️ 8.0/10
5. [Google Research Posts 'Cogentic' Papers on Integer Factoring and Discrete Logs](#item-5) ⭐️ 8.0/10
6. [Ubuntu's slow security patching sparks Debian migration debate](#item-6) ⭐️ 7.0/10
7. [New York Times Warns Photographers Against Updating Photoshop Over AI Labeling](#item-7) ⭐️ 7.0/10
8. [FCC approves SpaceX plan to build AI data centers in orbit](#item-8) ⭐️ 7.0/10
9. [New York Bans AI Chatbot Toys for Five Years Over Child Safety Fears](#item-9) ⭐️ 7.0/10
10. [State AGs Challenge Character.AI's Bankruptcy Sale of Private Chats](#item-10) ⭐️ 7.0/10
11. [Foreign AI companion apps spread across Africa without local safeguards](#item-11) ⭐️ 7.0/10
12. [Todoist Confirms 6% of User Data Stolen in Breach](#item-12) ⭐️ 6.0/10
13. [Amazon and Meta in Talks to End Muse AI Agent Blockade](#item-13) ⭐️ 6.0/10
14. [Nvidia and Jensen Huang face unanswered questions over Megaspeed chip flows](#item-14) ⭐️ 6.0/10
15. [UBS: Chinese AI Chips to Capture 88% of Home Market by 2028](#item-15) ⭐️ 6.0/10
16. [PLA embeds AI 'loyal wingman' drone simulations into fighter pilot training](#item-16) ⭐️ 6.0/10
17. [Edward Witten says AI mastering physics could transform the world in unpredictable ways](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Scott Aaronson Stunned by Claimed 9/4 Matrix Multiplication Proof](https://scottaaronson.blog/?p=10379) ⭐️ 9.0/10

Scott Aaronson published a short, profanity-laden blog post expressing sheer astonishment at an apparent AI-driven breakthrough in mathematics, pointing readers to a preprint titled "The Matrix Multiplication Exponent Is Nine Fourths." The preprint, released by OpenAI in a bulk drop of mathematical manuscripts around November 24, 2026, claims both an algorithm achieving n^(9/4+o(1)) field operations and a matching lower bound, with a proof formalized in Lean. If the result holds, it would settle one of the longest-standing open problems in theoretical computer science by pinning down the exact asymptotic complexity of matrix multiplication, a core subroutine in numerical linear algebra and optimization. It is also a dramatic data point in the debate over whether AI systems can produce genuinely novel, machine-verified mathematical results rather than merely assist human mathematicians. The claim has not yet been reviewed by leading mathematicians, and the headline result is a lower bound matching the known upper bound, which would mean no algorithm can achieve a smaller exponent over any field. Notably, algorithms that beat the schoolbook n^3 method are essentially never used in practice because the constant factor hidden in the big-O notation is enormous, so near-term practical impact on real numerical computing is likely minimal.

hackernews · Kotlopou · Nov 25, 19:11 · [Discussion](https://news.ycombinator.com/item?id=50646108)

**Background**: The matrix multiplication exponent, usually written ω, is the smallest real number such that any two n×n matrices can be multiplied using n^(ω+o(1)) field operations; the naive algorithm gives ω = 3, and Strassen's 1969 algorithm was the first to beat it. Finding the true value of ω has been a major open question ever since, with decades of work pushing the best known upper bound down toward roughly 2.37 while rigorous lower bounds remained far weaker. Lean is an interactive proof assistant that lets mathematicians write proofs a computer can mechanically check, so a Lean formalization is a much stronger certificate than an ordinary paper — though it guarantees correctness of the formal proof, not that the formal statement captures the intended mathematics.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Matrix_multiplication_exponent">Matrix multiplication exponent</a></li>
<li><a href="https://xenospectrum.com/en/matrix-multiplication-nine-fourths-lower-bound/">OpenAI Preprint Claims the Matrix Multiplication Exponent Is ...</a></li>
<li><a href="https://mathoverflow.net/questions/518214/what-are-the-practical-implications-of-the-matrix-multiplication-exponent-being">What are the practical implications of the matrix ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters broadly split between awe and skepticism: one argued that AI being good at analytic, axiomatic math does not imply it will "solve" empirical fields or play the sci-fi role of killing us all, while another insisted humans are biologically incapable of freaking out at even a fraction of the appropriate level. Others reached for historical analogies, invoking Bruno Latour's "centers of calculation" and Tycho Brahe's data-gathering work as the precondition for Kepler's laws, and one commenter asked how much of this would have happened with "just" Lean, MathLib, and compute but no LLMs.

**Tags**: `#artificial-intelligence`, `#mathematics`, `#matrix-multiplication`, `#scientific-discovery`, `#AGI`

---

<a id="item-2"></a>
## [1Password Discloses November 2026 Security Incident](https://1password.com/blog/update-on-nov-2026-security-incident) ⭐️ 8.0/10

1Password disclosed a November 2026 security incident, saying it began investigating on November 19, 2026 indications that an attacker gained access; the announcement also referenced malicious code being pushed to backend services. As a widely used password manager, 1Password is a high-value target, and a compromise of its SaaS supply chain can erode trust in cloud-hosted vaults and expose users to follow-on phishing. Commenters reported a follow-on phishing email that included a user's address and fake sharing details—210 items shared with an external Zoho account—but came from a non-1Password domain. The disclosure also drew criticism for not explaining whether branch protection or push-to-main controls were missing or bypassed.

hackernews · lxhrstn · Nov 25, 17:18 · [Discussion](https://news.ycombinator.com/item?id=50644817)

**Background**: 1Password is a password manager that stores encrypted vaults and, in its cloud offering, relies on its own infrastructure and code pipeline to deliver updates. SaaS supply-chain attacks often start with a compromised employee laptop and then move into source control or CI/CD, allowing attackers to push malicious code that reaches production. Users who prefer local-only vaults argue this trust model concentrates risk in the vendor, while 1Password and other cloud providers say they can invest more in security than individuals.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hashicorp.com/en/resources/how-do-client-applications-authenticate-vault">How do client applications authenticate themselves against Vault ?</a></li>
<li><a href="https://pass.pears.com/">PearPass | No Cloud , No Data Centers, Just Your Devices.</a></li>

</ul>
</details>

**Discussion**: HN commenters treated the incident as a textbook SaaS supply-chain risk: tptacek argued that compromised employee laptops leading to production code pushes are the standard breach pattern, while others questioned branch protections and cloud-vault trust. A user also described receiving a convincing phishing email apparently derived from the incident data, reinforcing concerns about follow-on attacks.

**Tags**: `#security`, `#1Password`, `#supply-chain-attack`, `#phishing`, `#SaaS`

---

<a id="item-3"></a>
## [Anthropic's GRH Lean proof shrinks to ~76k readable lines](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

A much shorter, more readable Lean verification of the Generalized Riemann Hypothesis associated with Anthropic has been released, reducing the formalization from roughly 17 million lines to about 76,000 lines and adding human-readable documentation plus a known-math versus new-math split. The reduction makes an enormous machine-checked proof far easier for mathematicians to audit and understand, which could strengthen trust in AI-assisted formal results and set a precedent for documenting large Lean developments. One commenter puts the reduction at 99.56%, while another refers to a separate readable proof of about 300,000 lines, suggesting multiple artifacts or counting conventions. The repository should be consulted for authoritative line counts and for the exact scope of the known-math versus new-math split.

hackernews · nb-t · Nov 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=50648050)

**Background**: Lean is an open-source proof assistant and functional programming language in which proofs are checked mechanically by a small trusted kernel. The Generalized Riemann Hypothesis extends the Riemann Hypothesis from the Riemann zeta function to Dirichlet L-functions and other global L-functions, and it remains unproven in the number-field case. Formal verification translates a mathematical argument into Lean code so that the kernel can confirm every step, but very large proofs can be hard for humans to read or assess for insight. The underlying GRH result has been reported as an AI-assisted proof checked by the Lean and Mathlib communities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://en.wikipedia.org/wiki/Generalized_Riemann_hypothesis">Generalized Riemann hypothesis</a></li>

</ul>
</details>

**Discussion**: Commenters welcomed the improved readability, documentation, and known-versus-new math split, but some questioned whether proof golfing actually answers Terence Tao's critique that huge formal proofs can lack insight. Others said they want a conventional mathematical paper or conference exposition from mathematicians who genuinely understand the argument, not only Lean code.

**Tags**: `#Lean`, `#formal verification`, `#AI for mathematics`, `#theorem proving`, `#Generalized Riemann Hypothesis`

---

<a id="item-4"></a>
## [NFS2root: 12-year-old pre-auth remote root bug in Linux kernel NFS server](https://opensec.in/blog/nfs2root-cve-2026-99362) ⭐️ 8.0/10

Security researchers disclosed CVE-2026-99362, a pre-authentication heap overflow in the Linux kernel's NFS server (nfsd) that lets an unauthenticated remote NFSv4.1/4.2 client overflow a reply-cache slot and leak or corrupt kernel memory, achieving root on hosts that expose TCP port 2049. The flaw went unnoticed for roughly 12 years but has already been fixed upstream in kernel releases 6.12.117, 6.18.61 and 7.3.2, and no proof-of-concept exploit has been published. A pre-authentication remote root bug in a core kernel subsystem is about as severe as Linux vulnerabilities get, and it affects NFSv4.1/4.2 — the default protocol versions on most modern distributions — so any file server reachable by untrusted clients is at risk. It is tempered by the fact that the patch has been available upstream for months, NFS is rarely exposed directly to the public internet, and no exploit code exists publicly, which gives administrators time to patch rather than scramble. The bug is a heap overflow in nfsd's reply cache that can be triggered by a remote NFSv4.1 client before any authentication occurs, meaning Kerberos or other auth layers do not mitigate it. Fixes are in stable kernels 6.12.117, 6.18.61 and 7.3.2; hosts that cannot patch immediately can fall back to disabling 4.1/4.2 via /proc/fs/nfsd/versions or filtering traffic at the network layer.

hackernews · dm · Nov 25, 20:35 · [Discussion](https://news.ycombinator.com/item?id=50647161)

**Background**: NFS (Network File System) is the standard way Unix and Linux machines share files over a network; the server side lives in the kernel as a component called nfsd and listens on TCP port 2049. NFSv4.1 and 4.2 are the modern protocol revisions that add features like sessions, pNFS and server-side copy, and they are what most distributions negotiate by default. A "pre-authentication" vulnerability means the attacker needs no credentials at all, so the only barrier is network reachability — which is why exposing NFS to the internet has always been discouraged.

<details><summary>References</summary>
<ul>
<li><a href="https://opensec.in/blog/nfs2root-cve-2026-99362">NFS 2ROOT (CVE-2026-99362): pre-auth root in Linux nfsd | OpenSec</a></li>
<li><a href="https://www.baeldung.com/linux/nfs-security-over-internet">Security of NFS Over Internet in Linux | Baeldung on Linux</a></li>
<li><a href="https://wiki.archlinux.org/title/NFS">NFS - ArchWiki</a></li>

</ul>
</details>

**Discussion**: Commenters focused on practical mitigation: one shared a ready-made XDP-based L7 firewall rule from the yeet project, another documented disabling 4.1/4.2 at runtime by writing "-4.1 -4.2" to /proc/fs/nfsd/versions (noting it reverts on reboot). Others downplayed the urgency because no PoC exists, NFS was never considered safe on the public internet, and the patch landed months ago, while one used the moment to argue that Linux's growing trusted computing base is why formally verified kernels like seL4 matter.

**Tags**: `#security`, `#linux-kernel`, `#nfs`, `#vulnerability`, `#cve`

---

<a id="item-5"></a>
## [Google Research Posts 'Cogentic' Papers on Integer Factoring and Discrete Logs](https://github.com/google-research/google-research/tree/master/cogentic_research_papers) ⭐️ 8.0/10

Google Research has added a new folder called 'cogentic_research_papers' to its public google-research GitHub repository, containing papers on integer factorization, discrete logarithms and related problems — one visible file is a PDF at cogentic_research_papers/deterministic_factoring_l34/paper.pdf. The upload landed with no abstract, blog post or announcement, so the actual claims and their scope are only inferable from the file names and directory structure. Integer factorization and discrete logarithms are the hard problems underpinning RSA and Diffie-Hellman-style public-key cryptography, so any credible algorithmic advance against them would directly threaten widely deployed encryption. Because the material comes from Google Research rather than an anonymous source, it is being read as a possible sign of serious, AI-assisted cryptanalytic progress. So far only a bare directory of PDFs is public: no peer review, no benchmarks, no stated complexity bounds and no claim about whether any method is classical, quantum or heuristic — details that determine whether RSA-2048 or real-world key sizes are actually at risk. Commenters also stress that a fast factoring algorithm would not automatically imply a fast discrete-log algorithm, and vice versa, since the two problems require separate results.

hackernews · rgwohlbold · Nov 25, 13:33 · [Discussion](https://news.ycombinator.com/item?id=50642086)

**Background**: RSA encryption relies on the assumption that multiplying two large primes is easy while factoring the product back into primes is computationally infeasible; Diffie-Hellman key exchange and elliptic-curve variants rest on the related assumption that discrete logarithms are hard to compute. A polynomial-time algorithm for either problem would break the corresponding deployed systems overnight, which is why progress here is treated as a security event rather than a pure-math curiosity. The 'Cogentic' framing ties into a wider 2025–2026 wave of claims that AI systems are accelerating mathematical discovery, ranging from Erdős problems to reasoning models trained on formal proofs.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50642086">Google releases Cogentic papers on integer factorization , discrete ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Integer_factorization">Integer factorization - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Discrete_logarithm">Discrete logarithm - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread mixes excitement with skepticism: several commenters cite rumors from credible people that this is 'the tip of something bigger,' and others compare it to AlphaGo's exploration of huge search spaces as evidence that AI-driven math results should no longer surprise anyone. Sceptics counter that factoring has been considered shaky for decades — it is why post-RSA alternatives exist — and note the market has kept sliding despite daily 'breakthroughs,' while some commenters say the run of results has overturned their belief that mathematics was immune to being solved by throwing money and compute at it.

**Tags**: `#cryptography`, `#integer-factorization`, `#cryptanalysis`, `#ai-for-mathematics`, `#google-research`

---

<a id="item-6"></a>
## [Ubuntu's slow security patching sparks Debian migration debate](https://www.openwall.com/lists/oss-security/2026/11/25/9) ⭐️ 7.0/10

A late-November 2026 oss-security mailing list post criticized Ubuntu for taking multiple weeks to patch severe vulnerabilities, including a recent remote TCP corruption flaw, and the issue drew a 189-point Hacker News discussion with 95 comments. Ubuntu is one of the most widely deployed Linux server distributions, so slow patching directly affects internet-facing workloads and erodes trust in Canonical's security process; some teams say they are already moving production server images to Debian over the issue. Commenters noted that distributions must balance fast patching with regression testing, and that stable/LTS kernel maintainers warn cherry-picking individual patches can leave systems both insecure and buggy; another user observed fixes sometimes appearing in Ubuntu's -updates pocket before the security repository.

hackernews · gslin · Nov 25, 20:38 · [Discussion](https://news.ycombinator.com/item?id=50647181)

**Background**: A CVE is a publicly cataloged vulnerability, and Linux distributions like Ubuntu and Debian maintain security teams that backport fixes to older package versions rather than forcing full upgrades. Ubuntu's security support varies by repository component: packages in Main and Restricted get Canonical-backed updates, while Universe and Multiverse rely more on community sponsorship. Debian runs its own Security Tracker and advisory process, and comparisons between the two projects often hinge on response speed, QA resources, and how much of the archive is covered.

<details><summary>References</summary>
<ul>
<li><a href="https://www.openwall.com/lists/oss-security/2026/11/25/9">oss- security - Slow Ubuntu security response times</a></li>
<li><a href="https://documentation.ubuntu.com/security/security-updates/">Security updates - Ubuntu security documentation</a></li>
<li><a href="https://www.debian.org/security/">Debian -- Security Information</a></li>

</ul>
</details>

**Discussion**: The Hacker News comments are largely critical: several users report moving server deployments from Ubuntu to Debian because they consider weeks-long security delays unacceptable in 2026. Others push back by stressing regression-testing tradeoffs and Debian's own QA limitations, while one commenter worries that security fixes landing in -updates before the security repo forces a riskier all-updates policy.

**Tags**: `#Ubuntu`, `#Linux security`, `#CVE response`, `#Debian`, `#distro maintenance`

---

<a id="item-7"></a>
## [New York Times Warns Photographers Against Updating Photoshop Over AI Labeling](https://www.theverge.com/ai-artificial-intelligence/1041227/the-new-york-times-warns-photographers-not-to-update-photoshop-over-ai-features) ⭐️ 7.0/10

The New York Times has advised photographers not to update Adobe Photoshop, because the newer versions' AI features can attach provenance metadata that leads social platforms to tag their images as AI-generated. The story, which links to an archived copy of the NYT guidance, sparked a 261-point, 219-comment discussion on Hacker News. Platforms currently cannot reliably distinguish a fully AI-generated image from a photo that received a minor AI-assisted color tweak or cutout, so a blanket "AI-generated" label can damage the credibility of photographers and of brands that position themselves as authoritative sources. This turns a software update decision into a professional reputational and business risk, and pressures Adobe to rethink how AI features are exposed and tagged. The mechanism at issue is Adobe's Content Credentials, cryptographically signed C2PA manifests that record an asset's edit history and any generative AI usage, and which are supported across Photoshop, Lightroom, Premiere and Adobe Stock. Once such metadata is embedded, platforms that read these industry signals can apply labels automatically, and stripping the credentials is awkward and can itself look suspicious.

hackernews · rmason · Nov 25, 21:18 · [Discussion](https://news.ycombinator.com/item?id=50647673)

**Background**: Content Credentials are C2PA manifests — tamper-evident metadata that acts like a nutrition label for digital files, showing what was captured, what was edited, and whether generative AI was involved. Photoshop's generative features are powered by Adobe Firefly, which can fill, expand or replace parts of an image, and Adobe attaches provenance data to outputs from these tools. On the platform side, Meta applies "Made with AI" labels to images and video based on detection of industry-shared AI signals, which is why metadata matters far beyond Adobe's own apps.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Content_Credentials">Content Credentials - Wikipedia</a></li>
<li><a href="https://helpx.adobe.com/photoshop/desktop/save-and-export/metadata-content-credentials/use-content-credentials.html">Content Credentials in Adobe Photoshop</a></li>
<li><a href="https://helpx.adobe.com/creative-cloud/apps/adobe-content-authenticity/content-credentials/overview.html">Content Credentials overview | Creative Cloud - Adobe Inc.</a></li>

</ul>
</details>

**Discussion**: Commenters working in creative tools agreed that separating fully generated images from lightly AI-assisted edits is nearly impossible once the output is a flat image, and warned that an AI label on Instagram or Facebook is a "death blow" to a brand's credibility. Others noted that vanishingly few people actually enjoy encountering generative AI in the wild, framing Adobe's AI push as a liability comparable to Tidal banning AI music, while some used the thread to argue that subscription software is losing ground to one-time-purchase alternatives like Affinity and ArtCraft.

**Tags**: `#AI policy`, `#generative AI`, `#creative tools`, `#Adobe Photoshop`, `#content provenance`

---

<a id="item-8"></a>
## [FCC approves SpaceX plan to build AI data centers in orbit](https://techcrunch.com/2026/11/25/fcc-approves-spacex-plan-to-put-ai-data-centers-in-space/) ⭐️ 7.0/10

On November 25, 2026, the FCC approved SpaceX's application to deploy up to 1 million satellites intended to operate as space-based AI data centers, with Chairman Brendan Carr announcing the decision on Wednesday. The agency dismissed opponents' objections — including potential harm to scientific research — on the grounds that those concerns fall outside its regulatory authority. This is the first major U.S. regulatory green light for orbital computing at megaconstellation scale, potentially upending assumptions about datacenter power, cooling, and latency economics just as terrestrial AI infrastructure runs into grid capacity and land constraints. It also sets a precedent that the FCC will not weigh astronomical or scientific harms when licensing huge satellite fleets, pushing those fights toward other agencies or Congress. The approval covers a fleet of up to 1 million satellites — orders of magnitude beyond any existing constellation — but it is a spectrum and licensing decision, not an endorsement of technical or economic viability. Orbital data centers still have to solve launch cost, radiative heat dissipation in vacuum, and constrained space-to-ground downlink bandwidth, and the FCC's refusal to address scientific-research objections leaves questions about astronomy interference and reentry effects unanswered.

rss · TechCrunch · Nov 25, 20:56

**Background**: Space-based data centers, also called orbital AI infrastructure, are proposed orbital facilities that run AI compute using space-based solar power, typically in sun-synchronous orbit where sunlight is nearly continuous, and shed waste heat by radiating it into space rather than using water cooling. The idea has roots in the 1980s Strategic Defense Initiative's Brilliant Pebbles program, which envisioned autonomous on-orbit data processing, and was revived from 2019 by the Space Development Agency's Proliferated Warfighter Space Architecture. Its economic viability depends heavily on continued reductions in launch costs and on whether ground-based fiber and power infrastructure become the binding constraint for AI growth.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/11/25/spacex-fcc-satellite-approval.html">SpaceX wins FCC approval for 1 million orbital data center satellites</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space-based_data_center">Space-based data center - Wikipedia</a></li>
<li><a href="https://introl.com/blog/orbital-data-centers-space-ai-infrastructure-guide-2025">Orbital Data Centers | Introl Blog</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#space computing`, `#FCC regulation`, `#datacenter policy`, `#satellite networks`

---

<a id="item-9"></a>
## [New York Bans AI Chatbot Toys for Five Years Over Child Safety Fears](https://techcrunch.com/2026/11/25/want-to-buy-your-kid-an-ai-toy-this-christmas-not-in-new-york/) ⭐️ 7.0/10

New York Governor Kathy Hochul signed legislation on Wednesday, November 25, 2026, imposing a five-year moratorium on the manufacture and sale of toys powered by AI chatbots, including talking stuffed animals, dolls, and robots that use the internet to hold conversations with children. The bill, sponsored by State Senator Andrew Gounardes, followed new Common Sense Media research documenting safety failures such as exposure to inappropriate content and risks to children's emotional development. This is one of the first sweeping state-level bans of its kind, and it directly threatens the holiday-season business of AI toy makers in a major market while setting a precedent other states may follow. It signals that regulators are moving from warning about AI companions for children to restricting their sale outright, putting pressure on the fast-growing AI toy category and the vendors behind it. The moratorium covers both manufacture and sale for five years and targets internet-connected toys that converse with children via AI chatbots, not offline electronic toys generally. Common Sense Media's January 2026 assessment recommended that no child age 5 or under use AI toys and urged caution for ages 6 to 12, warning that toys encouraging emotional dependency can undermine healthy social development.

rss · TechCrunch · Nov 25, 18:11

**Background**: AI toy companions are plush toys, dolls, and small robots that connect to the internet and use large language models to hold open-ended spoken conversations with children, often marketed as personalized playmates. Because the model generates responses in real time, the toy can produce content parents never reviewed and can encourage children to confide in it repeatedly. Common Sense Media is a widely cited US nonprofit that rates media and technology for families, and its risk assessments have become influential inputs for policymakers; earlier in 2026 it published a report, "AI in the Toy Box," surveying how parents view these products.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/nov/25/new-york-bans-ai-toys">New York bans AI toys , including those using internet... | The Guardian</a></li>
<li><a href="https://www.nysenate.gov/newsroom/press-releases/2026/andrew-gounardes/sen-gounardes-moratorium-ai-chatbot-toys-passes-state">Sen. Gounardes’ Moratorium on AI Chatbot Toys ... | NYSenate.gov</a></li>
<li><a href="https://www.commonsensemedia.org/press-releases/common-sense-media-warns-against-ai-toy-companions-after-research-reveals-safety-risks">Common Sense Media Warns Against AI Toy Companions After ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#regulation`, `#children's privacy`, `#AI toys`, `#consumer protection`

---

<a id="item-10"></a>
## [State AGs Challenge Character.AI's Bankruptcy Sale of Private Chats](https://techcrunch.com/2026/11/25/state-ags-fight-character-ais-plan-to-auction-off-users-private-chats/) ⭐️ 7.0/10

State attorneys general are challenging Character.AI's proposed bankruptcy sale of user data, saying it includes sensitive personal data from more than 21 million U.S. accounts and 2.1 million accounts registered to minors. The case could set a precedent for whether sensitive conversational data can be treated as a bankruptcy asset and sold to the highest bidder, directly affecting tens of millions of users and raising broader questions about data governance across the AI chatbot industry. The dispute centers on whether private chat logs are part of the bankruptcy estate and whether the company's prior privacy commitments to users survive an asset sale; the proposed sale remains contested and has not been approved.

rss · TechCrunch · Nov 25, 17:35

**Background**: Character.AI is a generative AI chatbot service where users converse with customizable characters. AI chat logs can contain intimate personal details, and research reported by WIRED shows that chatbots can infer a user's personal information from seemingly innocuous conversations. Bankruptcy sales typically involve transferring assets, which raises the question of whether user data and privacy promises transfer along with them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Character.ai">Character.ai - Wikipedia</a></li>
<li><a href="https://character.ai/about">About Character.AI</a></li>
<li><a href="https://www.wired.com/story/ai-chatbots-can-guess-your-personal-information/">AI Chatbots Can Guess Your Personal Information From... | WIRED</a></li>

</ul>
</details>

**Tags**: `#AI privacy`, `#Character.AI`, `#user data`, `#regulation`, `#bankruptcy`

---

<a id="item-11"></a>
## [Foreign AI companion apps spread across Africa without local safeguards](https://restofworld.org/2026/ai-companion-apps-africa-character-ai/?utm_source=rss&utm_medium=rss&utm_campaign=feeds) ⭐️ 7.0/10

A Rest of World report documents how foreign-built AI romance and companion apps — services such as Character.AI that let users hold ongoing romantic or emotional conversations with chatbots — are spreading rapidly among users in Africa. The reporting says the apps arrive with no locally tailored safeguards, and that children in particular are being drawn into addictive, one-sided "synthetic" relationships. The story highlights a consumer-AI risk pattern that regulators in Europe and the US are only beginning to address, now playing out in a region with far weaker oversight and almost no age-verification or local-language moderation. Because these apps shape how young users learn to relate to others, the effects could extend beyond individual screen time to how communal and family-centered social norms are transmitted across generations. The piece is journalistic rather than a technical deep-dive, so it offers few product-specific metrics, but its core concerns are engagement loops designed to maximize daily retention, exposure of minors, and the absence of any local regulatory or parental-control framework. It also notes that the apps are foreign-made, meaning their design choices, content policies, and data practices are set outside the markets where they are being used.

rss · Rest of World · Nov 25, 11:00

**Background**: AI companion apps are chatbots built on large language models and tuned with persona prompts so that users can sustain long, emotionally intimate conversations with a character that remembers prior chats. They have become a large consumer category globally, with the most prominent services developed in the United States and China, and they typically monetize through subscriptions and in-app purchases tied to message limits or premium personas. Most were designed for markets with existing app-store age gating and data-protection rules, and their localization efforts have focused on language support rather than on adapting safety features to local social and legal contexts.

**Tags**: `#AI companions`, `#Africa`, `#youth`, `#AI ethics`, `#consumer AI`

---

<a id="item-12"></a>
## [Todoist Confirms 6% of User Data Stolen in Breach](https://techcrunch.com/2026/11/25/todoist-confirms-6-of-customers-details-were-stolen-in-data-breach/) ⭐️ 6.0/10

Todoist confirmed that a hacker gained access to its production systems and stole customer data belonging to 6% of its users, including email addresses, password hashes, and account creation dates. Because Todoist is a widely used productivity app, the stolen email addresses could fuel targeted phishing, and the password hashes could be cracked if they were stored with fast or unsalted algorithms. Affected users should change their passwords and enable two-factor authentication. The report does not specify how many users 6% represents, which hashing algorithm was used, or whether the hashes were salted, so the actual risk depends on Todoist's password storage practices. Stolen account creation dates can also help attackers craft convincing phishing messages.

rss · TechCrunch · Nov 25, 14:20

**Background**: Password hashing is a one-way process that turns a password into a fixed-length fingerprint so that a leaked database does not directly reveal plaintext passwords. However, fast hashes such as SHA-256 are vulnerable to precomputed rainbow tables and brute-force cracking, which is why security guidance recommends slow, memory-hard algorithms. A unique salt per password ensures that identical passwords produce different hashes, making precomputed tables far less useful to attackers.

<details><summary>References</summary>
<ul>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html">Password Storage - OWASP Cheat Sheet Series</a></li>
<li><a href="https://en.wikipedia.org/wiki/Salt_(cryptography)">Salt (cryptography) - Wikipedia</a></li>
<li><a href="https://webpiki.com/en/blog/hash-algorithms-explained">Hash Algorithms : From SHA-256 to Password Storage | WebPiki</a></li>

</ul>
</details>

**Tags**: `#security`, `#data breach`, `#Todoist`, `#privacy`, `#passwords`

---

<a id="item-13"></a>
## [Amazon and Meta in Talks to End Muse AI Agent Blockade](https://techcrunch.com/2026/11/25/amazon-and-meta-reportedly-in-talks-to-lift-blockade-on-ai-agent-muse/) ⭐️ 6.0/10

Amazon and Meta are reportedly negotiating a deal that would end a two-month blockade preventing Meta's Muse AI agent from operating on Amazon, according to Fortune. The reported talks were disclosed on November 25, 2026, but no agreement has been confirmed. The outcome could set a precedent for how major platforms control AI agents that act on users' behalf, affecting e-commerce, advertising, and the broader AI agent ecosystem. A deal would also signal whether platform blockades or negotiated access will become the norm for agentic commerce. Amazon blocked Muse in September 2026, citing unauthorized access and security concerns, and the current report provides no technical details, timeline, or confirmed terms for lifting the blockade. The discussions are described as preliminary and focused on letting Muse shop on Amazon.

rss · TechCrunch · Nov 25, 14:10

**Background**: Muse is Meta's personal AI agent, announced on September 8, 2026, designed to carry out long-running tasks rather than answer single queries like a chatbot. Amazon blocked it in late September 2026, citing unauthorized access, which highlighted tensions over AI agents accessing third-party platforms. The reported deal would let Muse shop on Amazon, raising questions about platform permissions and AI-assisted commerce.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_(AI_agent)">Muse (AI agent) - Wikipedia</a></li>
<li><a href="https://tech.yahoo.com/ai/meta-ai/articles/amazon-blocks-meta-muse-ai-190958361.html">Amazon Blocks Meta’s Muse AI Agent for Unauthorized Access</a></li>
<li><a href="https://thenextweb.com/news/amazon-and-meta-talks-muse-blockade-ads-fortune">Amazon and Meta in talks to end the Muse blockade , Fortune reports</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#Amazon`, `#Meta`, `#platform policy`, `#tech industry`

---

<a id="item-14"></a>
## [Nvidia and Jensen Huang face unanswered questions over Megaspeed chip flows](https://techcrunch.com/2026/11/25/the-questions-jensen-huang-and-nvidia-will-still-have-to-answer-about-megaspeed/) ⭐️ 6.0/10

TechCrunch reported on November 25, 2026 that Nvidia and CEO Jensen Huang still have to answer what the company knew about where Megaspeed's chips ultimately ended up, and whether Huang's affair with a Megaspeed executive should have made Nvidia doubt Megaspeed's assurances. The piece frames these as open questions for investigators rather than resolved findings. Nvidia is the most consequential supplier of AI accelerators, so any suggestion that it failed to scrutinize a partner's end customers feeds directly into US export-control enforcement and could invite regulatory scrutiny of how cloud partners across Southeast Asia are vetted. The governance angle—whether a personal relationship compromised corporate diligence—also puts pressure on Huang and Nvidia's board, not just on Megaspeed. According to reporting cited in the coverage, Megaspeed bought more than US$4 billion of Nvidia chips, with Alibaba described as both customer and financial backer. TechCrunch's item is a short teaser that presents no new technical evidence, and neither Nvidia nor Megaspeed has confirmed the underlying allegations.

rss · TechCrunch · Nov 25, 13:00

**Background**: Megaspeed is an Nvidia Cloud Partner—a status that lets a company resell GPU cloud capacity built on Nvidia hardware—and it has purchased billions of dollars of Nvidia products for data centers across Southeast Asia, including Malaysia. US export controls restrict sales of advanced AI chips to China, which makes chips routed through third countries such as Malaysia and Singapore a focus for diversion concerns. The allegations matter because cloud partners can, in principle, obscure who the ultimate users of restricted hardware are.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Megaspeed">Megaspeed - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nvidia_alleged_spying_scandal">Jensen Huang scandal - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#export controls`, `#semiconductor industry`, `#corporate governance`, `#AI chips`

---

<a id="item-15"></a>
## [UBS: Chinese AI Chips to Capture 88% of Home Market by 2028](https://www.scmp.com/tech/tech-war/article/3375758/chinese-ai-chips-capture-88-home-market-2028-ubs-says-nvidia-woes-mount) ⭐️ 6.0/10

UBS projects that China's annual shipments of domestically designed AI accelerators will grow nearly sixfold from 1.7 million units in 2025 to more than 10 million units by 2030, with Cambricon Technologies and Biren Technology positioned as the leading vendors. The bank expects local suppliers to hold as much as 88% of the Chinese AI chip market by 2028, a sharp reversal from Nvidia's previous dominance there. The forecast signals that US export controls and Beijing's push for technological self-reliance are reshaping the global AI hardware supply chain, not just delaying Nvidia's China revenue. If borne out, it means Chinese cloud providers and AI labs will increasingly train and serve models on domestic silicon, which affects everything from CUDA ecosystem lock-in to the pricing power of American chipmakers. The numbers are projections rather than confirmed orders, and the ramp depends heavily on domestic foundry capacity, HBM memory supply and maturing software stacks that can substitute for CUDA. For scale, Cambricon reportedly plans to roughly triple output in 2026 to about 500,000 accelerators, while Biren's BR100 chip was launched back in 2022 with claims of performance comparable to Nvidia's H100.

rss · SCMP · Nov 26, 04:00

**Background**: AI accelerators are the specialized processors — GPUs and similar chips — that power training and inference for large models; Nvidia has long supplied the vast majority of China's demand. Successive US export restrictions, culminating in bans on advanced chips such as the H100 and later China-specific parts, pushed Beijing and domestic firms toward locally designed alternatives. Cambricon makes general-purpose AI chips and accelerator cards for data centers and edge devices, while Biren builds GPGPU chips and intelligent computing clusters used by operators such as China Mobile and China Telecom. UBS's forecast is an analyst estimate of how fast that substitution can proceed.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Biren_Technology">Biren Technology - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/cambricon_technologies">Cambricon Technologies — Grokipedia</a></li>
<li><a href="https://ai.g2.com/marketplace/tools/cambricon-technologies">Cambricon Technologies - AI Marketplace | G2</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#semiconductors`, `#China tech`, `#Nvidia`, `#market forecast`

---

<a id="item-16"></a>
## [PLA embeds AI 'loyal wingman' drone simulations into fighter pilot training](https://www.scmp.com/news/china/military/article/3375766/china-embeds-loyal-wingman-drone-simulations-fighter-pilot-training) ⭐️ 6.0/10

PLA Daily reported on Tuesday that an unnamed aviation brigade is incorporating manned-unmanned teaming (MUM-T) simulation systems into routine fighter pilot training, with AI-enabled simulated battle conditions and accompanying 'loyal wingman' drones acting as virtual teammates. This marks an official confirmation that such AI-driven teaming drills have moved from experimental trials into everyday training for frontline units. Embedding loyal-wingman simulations into routine training suggests the PLA is building the human and doctrinal groundwork for fielding collaborative combat aircraft, a capability the US and Australia are also pursuing. If it scales, MUM-T could change how air forces organize sorties, since a single crewed fighter could command multiple uncrewed platforms as force multipliers. The report gives few technical specifics — the aviation brigade is unnamed, and there is no information on the simulation platform, the number of virtual drones per pilot, or how AI agents behave inside the simulated battlespace. Notably, the item describes simulation-based training rather than confirmed operational deployment of real loyal-wingman drones.

rss · SCMP · Nov 25, 14:00

**Background**: A loyal wingman drone — also called a collaborative combat aircraft (CCA) — is a semi-autonomous uncrewed aircraft designed to fly alongside crewed fighters, using AI to hold formation, react to battlefield changes and execute commands without constant manual control. Manned-unmanned teaming (MUM-T) is the broader concept of pairing crewed aircraft with UAVs, typically with a human in the loop directing the unmanned teammate. Countries including the US and Australia (Boeing's MQ-28 Ghost Bat) are developing such systems, and simulation is a common first step before fielding them.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Loyal_wingman_drone">Loyal wingman drone</a></li>
<li><a href="https://www.baesystems.com/en-us/definition/what-is-manned-unmanned-teaming">What is Manned - Unmanned Teaming ( MUM - T )?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_MQ-28_Ghost_Bat">Boeing MQ-28 Ghost Bat - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#military technology`, `#drones`, `#simulation training`, `#manned-unmanned teaming`

---

<a id="item-17"></a>
## [Edward Witten says AI mastering physics could transform the world in unpredictable ways](https://www.scmp.com/news/china/science/article/3375749/edward-witten-i-dont-know-what-world-will-be-when-ai-understands-physics) ⭐️ 6.0/10

Edward Witten, an emeritus professor at the Institute for Advanced Study and the first physicist to win the Fields Medal, suggested that recent AI breakthroughs in solving mathematical problems could mark a turning point in understanding modern physics. He also said he does not know what the world will look like once AI genuinely understands physics. Witten is one of the most influential figures in theoretical and mathematical physics, so his framing of AI as a possible turning point carries weight in how the research community thinks about machine-assisted discovery. If AI tools start contributing to foundational physics rather than just calculation, the pace and style of theoretical work could shift substantially. The remarks were reported in a brief excerpt that offers no technical specifics about which AI systems or results Witten had in mind, and his statement is framed as open uncertainty rather than a concrete prediction. The claim hinges on the distinction between AI solving mathematical problems and AI actually grasping physical meaning.

rss · SCMP · Nov 25, 11:00

**Background**: Edward Witten is an emeritus professor at the Institute for Advanced Study (IAS) in Princeton and a leading figure in theoretical and mathematical physics; in 1990 he became the first physicist to receive the Fields Medal, mathematics' highest honour, for applying ideas from theoretical physics to mathematics. Modern physics, particularly quantum field theory and string-related work, is heavily formulated in advanced mathematics, which is why progress in mathematical problem-solving by AI is seen as potentially relevant to physics. The remark touches on a long-running question of whether machine intelligence can move from pattern-matching and computation to genuine physical understanding.

**Tags**: `#AI`, `#physics`, `#mathematical physics`, `#research commentary`, `#technology impact`

---