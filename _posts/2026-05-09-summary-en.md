---
layout: default
title: "Horizon Summary: 2026-05-09 (EN)"
date: 2026-05-09
lang: en
---

> From 32 items, 16 important content pieces were selected

---

1. [Triton v3.7.0 Released with Scaled BMM, FP8 Constants](#item-1) ⭐️ 8.0/10
2. [Internet Archive Switzerland Launches as Independent Entity](#item-2) ⭐️ 8.0/10
3. [LLMs corrupt documents when delegated tasks, study finds](#item-3) ⭐️ 8.0/10
4. [Google reCAPTCHA Breaks for De-Googled Android Users](#item-4) ⭐️ 8.0/10
5. [Hypocrisy of Cyberlibertarianism Exposed](#item-5) ⭐️ 8.0/10
6. [Mathematician’s Experience with ChatGPT 5.5 Pro Highlights Improved Reasoning](#item-6) ⭐️ 8.0/10
7. [GrapheneOS patches Android VPN leak ignored by Google](#item-7) ⭐️ 8.0/10
8. [AI cracks the two vulnerability cultures](#item-8) ⭐️ 8.0/10
9. [WebRTC design degrades LLM prompt accuracy](#item-9) ⭐️ 8.0/10
10. [Claude Code: Why HTML Output Beats Markdown](#item-10) ⭐️ 8.0/10
11. [Anthropic plans tens of billions in new funding, valuation nears $1T](#item-11) ⭐️ 8.0/10
12. [US suspects Nvidia chips smuggled to Alibaba via Thailand](#item-12) ⭐️ 8.0/10
13. [DeepSeek Reportedly Seeks $45B Valuation in First Funding Round](#item-13) ⭐️ 8.0/10
14. [Apple May End TSMC Exclusivity, Consider Intel 18A](#item-14) ⭐️ 8.0/10
15. [ChatGPT Android APK reveals Codex remote desktop control feature](#item-15) ⭐️ 8.0/10
16. [Study: AI answers often lean toward Japanese or US views](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Triton v3.7.0 Released with Scaled BMM, FP8 Constants](https://github.com/triton-lang/triton/releases/tag/v3.7.0) ⭐️ 8.0/10

Triton v3.7.0 adds scaled batched matrix multiplication (scaled BMM), support for direct FP8 constants in the frontend, and new dialect operations like tl.squeeze and tl.unsqueeze. This release enhances Triton's ability to handle modern AI workloads more efficiently, particularly for low-precision inference and training, and broadens the compiler's flexibility with new dialect operations. Scaled BMM enables block-wise scaling of matrix multiplication inputs, improving numerical stability for low-precision formats. FP8 constants allow direct declaration of FP8 values in Triton kernels, reducing overhead.

github · atalman · May 7, 22:19

**Background**: Triton is a domain-specific language and compiler for writing high-performance GPU kernels, widely used in deep learning frameworks like PyTorch. Scaling factors in block-scaled matmul help mitigate precision loss in low-bit computations. FP8 is an 8-bit floating-point format increasingly adopted for efficient AI inference.

<details><summary>References</summary>
<ul>
<li><a href="https://triton-lang.org/main/getting-started/tutorials/10-block-scaled-matmul.html">Block Scaled Matrix Multiplication — Triton documentation</a></li>
<li><a href="https://pytorch.org/blog/accelerating-llama3/">Accelerating Llama3 FP8 Inference with Triton Kernels – PyTorch</a></li>
<li><a href="https://github.com/parca-dev/proton">GitHub - parca-dev/ proton</a></li>

</ul>
</details>

**Tags**: `#triton`, `#compiler`, `#AI`, `#ML`, `#release`

---

<a id="item-2"></a>
## [Internet Archive Switzerland Launches as Independent Entity](https://blog.archive.org/2026/05/06/internet-archive-switzerland-expanding-a-global-mission-to-preserve-knowledge/) ⭐️ 8.0/10

On May 6, 2026, the Internet Archive announced the establishment of Internet Archive Switzerland as an independent entity, joining Internet Archive, Internet Archive Canada, and Internet Archive Europe to build a distributed, resilient digital library. This expansion strengthens global digital preservation by creating a decentralized network of archives, reducing the risk of a single point of failure or legal vulnerability. It advances the mission of Universal Access to All Knowledge with a more resilient infrastructure. Internet Archive Switzerland is led by Executive Director Roman Griesfelder, an Austrian citizen living in Switzerland since 1998. The organization plans to explore how endangered archives can be protected in conjunction with a UNESCO conference scheduled for November 2026 in Paris.

hackernews · hggh · May 9, 12:00 · [Discussion](https://news.ycombinator.com/item?id=48074265)

**Background**: Digital preservation ensures that digital information remains accessible and usable over the long term, but centralized archives face risks from legal challenges, censorship, and physical disasters. A distributed digital library hides the actual server architecture and allows users to interact with the nearest node, improving resilience and performance. The Internet Archive has long advocated for universal access to knowledge, and this Swiss entity represents a key step toward a federated, independent network of libraries.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.archive.org/2026/05/06/internet-archive-switzerland-expanding-a-global-mission-to-preserve-knowledge/">Internet Archive Switzerland : Expanding a Global Mission to...</a></li>
<li><a href="https://internetarchive.ch/">Internet Archive Switzerland</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_preservation">Digital preservation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Internet Archive needs a Usenet-style peering model where independent organizations share content but not DMCA takedown requests, to legally protect the network. Some expressed skepticism about the actual independence of the Swiss entity, pointing out shared board members and infrastructure with the US-based Internet Archive.

**Tags**: `#internet-archive`, `#digital-preservation`, `#decentralization`, `#resilience`, `#libraries`

---

<a id="item-3"></a>
## [LLMs corrupt documents when delegated tasks, study finds](https://arxiv.org/abs/2604.15597) ⭐️ 8.0/10

A large-scale experiment with 19 LLMs, including frontier models like Gemini 3.1 Pro and GPT 5.4, shows that delegating document tasks to LLMs corrupts an average of 25% of content by the end of long workflows. This finding challenges the assumption that LLMs can reliably handle document maintenance in AI agent systems, highlighting a fundamental limitation that could affect productivity and trust in automated workflows. Even when equipped with tool use capabilities, the corruption persisted, suggesting the issue is rooted in the model's statistical nature rather than poor implementation. The authors term this degradation 'semantic ablation,' where unique insights are replaced by generic tokens.

hackernews · rbanffy · May 9, 08:44 · [Discussion](https://news.ycombinator.com/item?id=48073246)

**Background**: Large language models generate text by predicting the most probable next token based on training data, which inherently biases outputs toward common patterns. When used iteratively—such as editing or summarizing a document—each pass tends to remove rare, high-entropy information and replace it with more generic language. This phenomenon, known as semantic ablation, means that LLMs gradually strip away nuance and precision, effectively corrupting the original intent.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2604.15597">[2604.15597] LLMs Corrupt Your Documents When You Delegate</a></li>
<li><a href="https://www.theregister.com/2026/02/16/semantic_ablation_ai_writing/">Semantic ablation: Why AI writing is boring and dangerous • The Register</a></li>
<li><a href="https://huggingface.co/papers/2604.15597">Paper page - LLMs Corrupt Your Documents When You Delegate</a></li>

</ul>
</details>

**Discussion**: Community members largely agree corruption occurs, with one commenter likening it to JPEG degradation and another coining 'semantic ablation.' Some skepticism arises: simonw questions the tool-use experiment's design, suggesting better agent patterns could mitigate corruption. Others propose workarounds, like storing knowledge as separate fact files and using LLMs only for final rendering.

**Tags**: `#LLMs`, `#document corruption`, `#semantic ablation`, `#AI agents`, `#tool use`

---

<a id="item-4"></a>
## [Google reCAPTCHA Breaks for De-Googled Android Users](https://reclaimthenet.org/google-broke-recaptcha-for-de-googled-android-users) ⭐️ 8.0/10

Google's latest reCAPTCHA update now requires Play Integrity attestation, rendering the service inaccessible on de-googled Android devices without Google Play Services. This change forces de-googled Android users to choose between privacy and access to millions of websites that rely on reCAPTCHA, and signals a broader industry trend toward remote attestation as a gatekeeping mechanism. Play Integrity checks device authenticity by verifying that the device runs a certified Android build with Google Play installed, which alternative OSes like GrapheneOS (even with sandboxed Play Services) may not fully satisfy.

hackernews · anonymousiam · May 8, 18:45 · [Discussion](https://news.ycombinator.com/item?id=48067119)

**Background**: De-googled Android refers to custom ROMs or devices that avoid Google's proprietary services to enhance privacy. reCAPTCHA is a widely used bot detection system. Play Integrity is a Google API that verifies app and device integrity through hardware-backed attestation.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/google/play/integrity/overview">Overview of the Play Integrity API | Android Developers</a></li>
<li><a href="https://tech.yahoo.com/phones/articles/googling-android-simpler-think-no-193119747.html">De - Googling Android is simpler than you think—no special phone...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Remote_attestation">Remote attestation</a></li>

</ul>
</details>

**Discussion**: Community comments reveal deep concerns: one user explains how remote attestation can tie devices to identities via EK->AIK keys, arguing it compromises privacy. Another notes that even sandboxed Play Services may not pass Play Integrity, and a third laments the web's shift toward forced KYC-like verification.

**Tags**: `#Android`, `#reCAPTCHA`, `#privacy`, `#Google Play Integrity`, `#remote attestation`

---

<a id="item-5"></a>
## [Hypocrisy of Cyberlibertarianism Exposed](https://matduggan.com/the-intolerable-hypocrisy-of-cyberlibertarianism/) ⭐️ 8.0/10

An essay critiques the hypocrisy of cyberlibertarian ideals, particularly regarding copyright, as tech insiders shift positions when AI threatens their economic interests. This critique is significant because it reveals the selective application of free-market and anti-regulation ideologies in tech, influencing policy debates on AI and copyright. The essay uses historical examples from the Cyberlibertarian Declaration of Independence and current AI controversies to illustrate the inconsistency, noting that wealthy and powerful players ignore these debates.

hackernews · ColinWright · May 9, 13:48 · [Discussion](https://news.ycombinator.com/item?id=48074952)

**Background**: Cyberlibertarianism is a political ideology rooted in the early internet hacker and cypherpunk culture, advocating minimal government regulation and free information flow. The essay argues that its proponents abandon these principles when their own interests are at stake, especially regarding copyright in the age of AI.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyberlibertarianism">Cyberlibertarianism</a></li>
<li><a href="https://en.wikipedia.org/wiki/Technolibertarianism">Technolibertarianism - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments note the shift in attitudes toward copyright, with users observing that corporations previously used copyright against open source but now claim it to protect their AI-generated content. Some agree with the critique but point out exceptions and question the universality of the hypocrisy.

**Tags**: `#cyberlibertarianism`, `#copyright`, `#AI`, `#tech criticism`, `#ethics`

---

<a id="item-6"></a>
## [Mathematician’s Experience with ChatGPT 5.5 Pro Highlights Improved Reasoning](https://gowers.wordpress.com/2026/05/08/a-recent-experience-with-chatgpt-5-5-pro/) ⭐️ 8.0/10

Field Medalist Timothy Gowers shared his experience with OpenAI's ChatGPT 5.5 Pro, praising its significantly improved reasoning and problem-solving abilities compared to earlier models. He noted that the model can now solve what he calls 'gentle problems' that were previously considered appropriate for beginning PhD students. This reflection from a leading mathematician signals that advanced LLMs are approaching a level where they can handle genuine mathematical research problems, potentially transforming how research is conducted and how PhD students are trained. The discussion highlights urgent questions about the value of human thinking and the future of academic education. ChatGPT 5.5 Pro was released by OpenAI on April 23, 2026, under the codename 'Spud,' and is not available to free-tier users. Gowers emphasized that while the model is powerful, it still makes many mistakes and requires rigid guidance to perform correctly, but it excels at self-correction and reasoning tracing.

hackernews · _alternator_ · May 9, 02:41 · [Discussion](https://news.ycombinator.com/item?id=48071262)

**Background**: ChatGPT 5.5 Pro is the latest in OpenAI's series of large language models, building on GPT-4 with improved reasoning and multimodal capabilities. Timothy Gowers is a renowned mathematician and Fields Medalist, and his blog post comparing the model's abilities to PhD-level problem-solving has sparked widespread discussion in academic and AI communities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT - 5 . 5 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments generally align with Gowers' observations, with users noting the model's improved self-correction but also its high cost and tendency to make conceptual errors. Some commenters, like physicist ziotom78, share positive experiences using similar models for checking papers, while others debate the deeper implications for the value of original thinking and research training.

**Tags**: `#ChatGPT`, `#LLM`, `#AI research`, `#mathematics`, `#education`

---

<a id="item-7"></a>
## [GrapheneOS patches Android VPN leak ignored by Google](https://cyberinsider.com/grapheneos-fixes-android-vpn-leak-google-refused-to-patch/) ⭐️ 8.0/10

GrapheneOS released an update fixing a VPN bypass vulnerability in Android that allowed the system_server process to leak a user's real IP address even when Always-On VPN and Block connections without VPN were enabled. Google acknowledged the issue but refused to patch it, and GrapheneOS implemented its own fix after public disclosure on April 29. This fix is significant because it restores the privacy guarantee of VPNs on Android, which could be exploited by malicious apps or network observers to unmask a user's real IP address. It also highlights a divergence between Google's security priorities and the community's expectations, reinforcing GrapheneOS's role as a privacy-focused alternative. The vulnerability stemmed from system_server having elevated networking privileges that exempted it from VPN routing restrictions. GrapheneOS implemented network permission checks to ensure system_server traffic goes through the VPN. Google declined to patch the issue, stating it required an incompatible change, but GrapheneOS managed to fix it without breaking compatibility.

hackernews · Georgelemental · May 9, 14:11 · [Discussion](https://news.ycombinator.com/item?id=48075144)

**Background**: GrapheneOS is a privacy- and security-focused open-source operating system based on Android, targeting Google Pixel devices. The Android system_server is a core process that hosts many system services and runs with elevated privileges. A VPN leak occurs when traffic bypasses the VPN tunnel, exposing the user's actual IP address. This vulnerability allowed system_server to directly access the network, bypassing VPN routing even with Block connections without VPN enabled.

<details><summary>References</summary>
<ul>
<li><a href="https://cyberinsider.com/grapheneos-fixes-android-vpn-leak-google-refused-to-patch/">GrapheneOS fixes Android VPN leak Google refused to... | CyberInsider</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://stackoverflow.com/questions/34651015/what-is-systemserver-for-android">What is SystemServer for Android ? - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: Community comments reflected mixed reactions: some users discussed the cost and availability of Pixel phones for running GrapheneOS, while others compared its user experience unfavorably to LineageOS. One commenter expressed surprise that Google honored the embargo until April 29 instead of releasing the fix immediately. Overall, the discussion showed interest but also practical concerns about adopting GrapheneOS.

**Tags**: `#security`, `#Android`, `#GrapheneOS`, `#VPN`, `#privacy`

---

<a id="item-8"></a>
## [AI cracks the two vulnerability cultures](https://www.jefftk.com/p/ai-is-breaking-two-vulnerability-cultures) ⭐️ 8.0/10

AI tools are accelerating vulnerability discovery and exploitation, undermining the traditional distinction between how open-source and closed-source software handle vulnerabilities, as argued by Jeff Kaufman. This shift reduces the time window for defenders to patch vulnerabilities, especially for closed-source software, potentially increasing the frequency and impact of zero-day attacks across the industry. The catalyst is increased software transparency from open source adoption and improved reversing tools, not just LLMs; the trend was predicted long before AI.

hackernews · speckx · May 8, 17:55 · [Discussion](https://news.ycombinator.com/item?id=48066524)

**Background**: Traditionally, vulnerabilities in open-source software were discovered and patched more transparently, while closed-source relied on secrecy. AI now enables faster exploit generation, blurring this divide.

**Discussion**: Commenters debated whether AI is the real driver, with some noting that diffing patches was already common. Others emphasized that cheaper exploit generation makes coordinated disclosure more important, not less.

**Tags**: `#AI`, `#vulnerability disclosure`, `#cybersecurity`, `#open source`, `#LLMs`

---

<a id="item-9"></a>
## [WebRTC design degrades LLM prompt accuracy](https://simonwillison.net/2026/May/9/luke-curley/#atom-everything) ⭐️ 8.0/10

Luke Curley argues that WebRTC's aggressive packet dropping for low latency harms the accuracy of prompts sent to LLMs, as users prefer waiting for reliable delivery over fast but corrupted input. This mismatch between WebRTC's design goals and the needs of LLM interactions could lead to degraded AI responses, affecting user experience in voice-based AI applications. It highlights the need for protocol adaptations as AI shifts from human-to-human to human-to-machine communication. WebRTC makes it impossible to retransmit audio packets within browsers, as Discord experienced when attempting to implement such functionality. Curley notes that users would gladly accept an extra 200ms delay for accurate prompts, but the protocol's implementation is hard-coded for real-time latency.

rss · Simon Willison · May 9, 01:03

**Background**: WebRTC is a real-time communication protocol designed for low-latency audio and video calls. It drops packets aggressively under poor network conditions to maintain smooth playback and lip synchronization, as retransmission would increase delay. This trade-off is suitable for human conversation but problematic for transmitting precise data like LLM prompts, where each packet matters for accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://bloggeek.me/webrtcglossary/packet-loss/">Packet Loss in WebRTC: Causes, Effects & How to Fix It • BlogGeek.me</a></li>
<li><a href="https://www.digitalsamba.com/blog/packet-loss-in-webrtc">Understanding and Preventing Packet Loss in WebRTC: A Guide</a></li>

</ul>
</details>

**Tags**: `#WebRTC`, `#LLMs`, `#real-time communication`, `#audio streaming`, `#protocol design`

---

<a id="item-10"></a>
## [Claude Code: Why HTML Output Beats Markdown](https://simonwillison.net/2026/May/8/unreasonable-effectiveness-of-html/#atom-everything) ⭐️ 8.0/10

Thariq Shihipar from Anthropic's Claude Code team recommends using HTML instead of Markdown as the output format when prompting Claude Code, demonstrating that HTML enables richer interactive explanations with embedded SVG diagrams and widgets. This advice is accompanied by example prompts and a collection of HTML artifacts. This technique shifts the common practice of using Markdown for LLM outputs, unlocking more effective and visually engaging responses from AI coding assistants. Developers can now get richer, self-contained HTML explanations that include interactive elements, improving code review and learning experiences. Shihipar provides prompt examples like asking Claude to create an HTML artifact for code review with inline margin annotations and color-coded findings. Simon Willison tested the approach with GPT-5.5 on a Linux exploit explanation, producing a well-styled interactive HTML page, though he notes the need to emphasize the exploit over the harness.

rss · Simon Willison · May 8, 21:00

**Background**: Claude Code is Anthropic's agentic coding tool that runs in the terminal, allowing developers to delegate engineering tasks and explore codebases with AI assistance. Traditionally, Markdown has been the default output format for LLMs due to its token efficiency, but HTML allows for richer formatting, embedded visuals, and interactive elements within a single self-contained file. Simon Willison has previously written about building HTML tools for interactive utilities.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://digitalthoughtdisruption.com/2025/08/19/offline-html-productivity-artifact-generator-prompt/">Offline HTML Productivity Artifact Generator: Field-Ready AI Prompt</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#prompting`, `#HTML`, `#Claude Code`, `#technical-deep-dive`

---

<a id="item-11"></a>
## [Anthropic plans tens of billions in new funding, valuation nears $1T](https://www.ft.com/content/a40cafcc-0fa4-4e70-9e24-90d826aea56d) ⭐️ 8.0/10

Anthropic is planning to raise tens of billions of dollars in new funding this summer to expand its computing infrastructure, potentially pushing its valuation to nearly $1 trillion and surpassing OpenAI. This signals a major shift in the AI industry's competitive landscape, with Anthropic potentially overtaking OpenAI in valuation and attracting massive capital investment, which could accelerate AI development and reshape market dynamics. On secondary markets like Forge Global, Anthropic's implied valuation has already reached $1-1.2 trillion, surpassing OpenAI's ~$880 billion. Just in February, Anthropic completed a $30 billion funding round at a $380 billion valuation, meaning its expected valuation has more than doubled in a few months thanks to explosive enterprise customer growth.

telegram · zaihuapd · May 8, 11:15

**Background**: Anthropic is a leading AI company known for developing the Claude series of large language models and is a major competitor to OpenAI. The AI industry has seen a surge in investment, with companies racing to build larger models and data centers, requiring massive capital. Secondary market valuations often reflect investor expectations before official funding rounds close.

**Tags**: `#Anthropic`, `#Funding`, `#Valuation`, `#OpenAI`, `#AI Industry`

---

<a id="item-12"></a>
## [US suspects Nvidia chips smuggled to Alibaba via Thailand](https://www.bloomberg.com/news/articles/2026-05-08/us-said-to-suspect-nvidia-chips-smuggled-to-alibaba-via-thailand) ⭐️ 8.0/10

US prosecutors suspect Thai company OBON Corp. smuggled $2.5 billion worth of Super Micro servers containing advanced Nvidia chips to China, with Alibaba identified as one of the end customers. This case could escalate tensions over technology export controls between the US and China, potentially impacting the development of AI capabilities in both countries and leading to stricter restrictions on chip exports to Thailand. OBON was involved in creating Thailand's sovereign AI cloud, Siam AI, which gained Nvidia partner status; Alibaba denies any business relationship with Super Micro or OBON, and Siam AI's CEO claims to have left OBON and denies involvement.

telegram · zaihuapd · May 8, 13:23

**Background**: Nvidia's advanced AI chips, such as the H100 and A100, are subject to US export controls to prevent China from accessing cutting-edge technology for military or surveillance purposes. Sovereign AI clouds are government-controlled digital infrastructures designed to keep national data and computing power within a country's borders. Thailand's Siam AI Cloud, backed by Nvidia, aims to develop a sovereign AI ecosystem for Thailand.

<details><summary>References</summary>
<ul>
<li><a href="https://siam.ai/">Siam ai corporation co., ltd.</a></li>
<li><a href="https://www.linkedin.com/company/siam-ai">SIAM . AI Cloud | 513 followers on LinkedIn. Thailand 's Leading...</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#AI chips`, `#export controls`, `#smuggling`, `#Alibaba`

---

<a id="item-13"></a>
## [DeepSeek Reportedly Seeks $45B Valuation in First Funding Round](https://t.me/zaihuapd/41289) ⭐️ 8.0/10

DeepSeek is reportedly seeking a $45 billion valuation in its first external funding round, with China's National Integrated Circuit Industry Investment Fund in talks to lead the investment. This would mark the first major external investment in DeepSeek and signal deeper state involvement in China's AI sector, potentially accelerating the development of cost-efficient AI models amid ongoing chip export restrictions. The valuation is around $45 billion, making DeepSeek one of the most valuable AI startups globally. The funding round is led by the state-backed 'Big Fund' for integrated circuits, which typically invests in semiconductor companies.

telegram · zaihuapd · May 8, 14:59

**Background**: DeepSeek is a Chinese AI company founded in 2023, known for its open-weight large language models trained at a fraction of the cost of competitors like OpenAI's GPT-4. The company's success has challenged U.S. dominance in AI and sparked industry-wide reassessments of cost efficiency. The National Integrated Circuit Industry Investment Fund, established by the Chinese government, aims to boost domestic semiconductor self-sufficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://en.wikipedia.org/wiki/China_Integrated_Circuit_Industry_Investment_Fund">China Integrated Circuit Industry Investment Fund - Wikipedia</a></li>
<li><a href="https://www.scmp.com/tech/enterprises/article/2145422/how-chinas-big-fund-helping-country-catch-global-semiconductor-race">How China ’s ‘Big Fund ’ is helping the country catch up in chip race</a></li>

</ul>
</details>

**Tags**: `#AI融资`, `#DeepSeek`, `#中国AI`, `#产业基金`

---

<a id="item-14"></a>
## [Apple May End TSMC Exclusivity, Consider Intel 18A](https://t.me/zaihuapd/41292) ⭐️ 8.0/10

Apple is reportedly considering ending TSMC's exclusive chip manufacturing and may use Intel's 18A process for some lower-end processors as early as 2027. This potential shift could reduce Apple's reliance on a single supplier, diversify chip supply chains, and provide a major boost to Intel's foundry business amid growing AI chip demand. Intel's role would be limited to manufacturing, not chip design, and the partnership would initially target lower-end processors for Macs, iPads, or iPhones.

telegram · zaihuapd · May 8, 17:18

**Background**: TSMC has been Apple's exclusive chip manufacturer since 2014, producing all A-series and M-series processors. Intel's 18A process (equivalent to 2 nm) is part of its foundry revival strategy, aiming to compete with TSMC and Samsung. The move comes as TSMC prioritizes capacity for AI chip customers like Nvidia, prompting Apple to seek supply chain diversification.

<details><summary>References</summary>
<ul>
<li><a href="https://www.comss.ru/page.php?id=19090">Новые процессоры Intel Core Ultra 300 (Panther Lake) на Intel ...</a></li>
<li><a href="https://hardwareand.co/actualites/breves/intel-18a-est-maintenant-pret-nous-dit-intel">" Intel 18 A est maintenant prêt", nous dit Intel ! - Hardware & Co</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#TSMC`, `#Intel`, `#chip manufacturing`, `#supply chain`

---

<a id="item-15"></a>
## [ChatGPT Android APK reveals Codex remote desktop control feature](https://www.androidauthority.com/codex-smartphone-control-3665256/) ⭐️ 8.0/10

An APK teardown of ChatGPT Android version 1.2026.125 has revealed strings indicating OpenAI is developing a remote desktop control feature for Codex, enabling users to manage desktop sessions from their smartphones. This development could shift AI agent interaction paradigms, allowing seamless cross-device control and potentially expanding Codex's utility from coding assistant to a universal remote control for desktop environments. The feature is still under development with no preview or release date; it requires the desktop to be logged into the same account and supports finding and reconnecting to remote sessions.

telegram · zaihuapd · May 9, 02:18

**Background**: An APK teardown involves decompiling an Android app's installation file to inspect unreleased code and strings, revealing upcoming features. OpenAI Codex is a large language model that translates natural language into code; the new feature aims to extend Codex's capabilities to control desktop sessions remotely from a smartphone.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model ) - Wikipedia</a></li>
<li><a href="https://medium.com/commencis/apk-teardown-in-a-nutshell-7701c3628bf5">APK Teardown in a Nutshell. In short, converting/decompiling | Medium</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#remote control`, `#Android`, `#AI`

---

<a id="item-16"></a>
## [Study: AI answers often lean toward Japanese or US views](https://cybernews.com/ai-news/every-ai-answer-japan/) ⭐️ 8.0/10

A study by the University of the Basque Country and Cardiff University found that eight major AI models frequently anchor their answers to Japanese or US cultural perspectives across 24 languages, with five models biased toward Japan and two toward the US. This highlights systemic cultural bias in widely used AI models, raising concerns about fairness and global applicability, especially for users from underrepresented regions. The bias primarily emerges during supervised fine-tuning, not during pre-training, and low-resource languages are more likely to receive answers anchored to the model's own country.

telegram · zaihuapd · May 9, 10:02

**Background**: Supervised fine-tuning (SFT) is a training stage where models are adapted to specific tasks using labeled data, often reinforcing biases in the training data. Low-resource languages lack sufficient data, making them more susceptible to such biases. This study tested 31,680 cultural questions across eight models and 24 languages, revealing anchoring effects.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/from-prompting-precision-why-supervised-fine-tuning-future-hussain-ujzpf">From Prompting to Precision: Why Supervised Fine - Tuning is the...</a></li>
<li><a href="https://www.igi-global.com/book/empowering-low-resource-languages-nlp/324158">Empowering Low - Resource Languages With NLP Solutions</a></li>

</ul>
</details>

**Tags**: `#AI bias`, `#cultural bias`, `#machine learning fairness`, `#NLP research`, `#language models`

---