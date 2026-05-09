---
layout: default
title: "Horizon Summary: 2026-05-09 (EN)"
date: 2026-05-09
lang: en
---

> From 18 items, 6 important content pieces were selected

---

1. [The hypocrisy of cyberlibertarianism](#item-1) ⭐️ 8.0/10
2. [Mathematician Timothy Gowers Tests ChatGPT 5.5 Pro for Problem Solving](#item-2) ⭐️ 8.0/10
3. [GrapheneOS patches Android VPN leak that Google ignored](#item-3) ⭐️ 8.0/10
4. [WebRTC's packet dropping harms LLM audio accuracy](#item-4) ⭐️ 8.0/10
5. [Baidu Launches ERNIE 5.1 with 94% Cost Reduction](#item-5) ⭐️ 8.0/10
6. [NASA JPL Achieves Rotor Breakthrough for Mars Helicopters](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [The hypocrisy of cyberlibertarianism](https://matduggan.com/the-intolerable-hypocrisy-of-cyberlibertarianism/) ⭐️ 8.0/10

Mat Duggan's article critiques cyberlibertarianism, arguing that tech industry leaders and companies have repeatedly abandoned its core principles—such as minimal government regulation and free speech—when it suits their interests, revealing deep hypocrisy. This matters because cyberlibertarianism has profoundly shaped internet governance and tech culture; the critique forces a re-examination of foundational beliefs and the tech industry's accountability, especially as online platforms become central to public life. The article contrasts the rhetoric of early internet figures like John Perry Barlow with later actions of tech giants, such as embracing censorship or surveillance. It highlights the tension between decentralized ideals and the concentrated power that emerged in the industry.

hackernews · ColinWright · May 9, 13:48 · [Discussion](https://news.ycombinator.com/item?id=48074952)

**Background**: Cyberlibertarianism is a political ideology rooted in early internet hacker culture, advocating minimal government regulation, strong privacy, and free expression online. John Perry Barlow's 1996 'Declaration of the Independence of Cyberspace' is a seminal text. Critics argue that as the web commercialized, tech companies adopted these ideals selectively, often prioritizing profit over principles.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyberlibertarianism">Cyberlibertarianism</a></li>
<li><a href="https://en.wikipedia.org/wiki/Technolibertarianism">Technolibertarianism - Wikipedia</a></li>

</ul>
</details>

**Discussion**: A user who knew Barlow agrees with much of the critique, noting that many shelved these principles when inconvenient. Another comment observes that startups often began with legally questionable tactics, then later supported government regulation to entrench themselves. Some readers push back on the article's nostalgia, arguing the pre-internet era was not as bad as depicted.

**Tags**: `#cyberlibertarianism`, `#tech culture`, `#internet ideology`, `#critique`, `#hackernews`

---

<a id="item-2"></a>
## [Mathematician Timothy Gowers Tests ChatGPT 5.5 Pro for Problem Solving](https://gowers.wordpress.com/2026/05/08/a-recent-experience-with-chatgpt-5-5-pro/) ⭐️ 8.0/10

Timothy Gowers, a Fields Medalist, recounts his experience using OpenAI's ChatGPT 5.5 Pro, noting that it can reliably solve 'gentle' mathematical problems and trace its own reasoning, marking a significant advance in AI mathematical capability. This firsthand account from a leading mathematician demonstrates that current LLMs are approaching a level where they can assist in actual mathematical research, potentially shifting how beginners are trained and how research is conducted. GPT-5.5 Pro was released on April 23, 2026, under the codename 'Spud', and is not available to free-tier users. Gowers found that while it still makes mistakes, it can correct itself better than earlier models when given rigid guidance.

hackernews · _alternator_ · May 9, 02:41 · [Discussion](https://news.ycombinator.com/item?id=48071262)

**Background**: ChatGPT 5.5 Pro is a large language model (LLM) developed by OpenAI, building on the GPT-5 architecture. The model is designed to handle complex reasoning tasks, including mathematics, with improved accuracy and self-correction capabilities. Gowers used it to test a variety of 'gentle problems' typically given to beginning PhD students.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT - 5 . 5 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with Gowers' assessment, noting that 5.5 Pro is the first LLM they could wrangle to solve tedious problems correctly, though it remains costly in token usage. Some also highlighted philosophical implications for the value of ideas if AI can generate them easily.

**Tags**: `#AI`, `#LLM`, `#ChatGPT`, `#Mathematics`, `#AI Research`

---

<a id="item-3"></a>
## [GrapheneOS patches Android VPN leak that Google ignored](https://cyberinsider.com/grapheneos-fixes-android-vpn-leak-google-refused-to-patch/) ⭐️ 8.0/10

GrapheneOS has fixed a VPN traffic leak in Android's system_server process that Google acknowledged but declined to patch, allowing VPN-protected devices to expose real IP addresses. This fix addresses a fundamental flaw in Android's VPN implementation that undermines user privacy promises, and it highlights the divergence between stock Android and security-focused alternatives like GrapheneOS. The leak occurs in system_server, a privileged process that bypasses VPN routing restrictions, and was demonstrated on a Pixel 8 running Android 16 with Proton VPN and lockdown mode enabled; GrapheneOS's patch was released after Google authorized public disclosure on April 29, 2025.

hackernews · Georgelemental · May 9, 14:11 · [Discussion](https://news.ycombinator.com/item?id=48075144)

**Background**: GrapheneOS is an open-source, security-hardened Android-based operating system for Pixel devices, built on AOSP. The system_server process operates with elevated networking privileges and is exempt from VPN routing in stock Android, meaning VPN protection is not fully enforced for system traffic. VPN leaks defeat the purpose of using a VPN to hide IP addresses and encrypt traffic.

<details><summary>References</summary>
<ul>
<li><a href="https://cyberinsider.com/grapheneos-fixes-android-vpn-leak-google-refused-to-patch/">GrapheneOS fixes Android VPN leak Google refused to... | CyberInsider</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with Google's decision, with one noting that Android's lockdown mode explicitly promises no traffic bypasses the VPN, making the kernel-level leak particularly egregious. Others discussed the difficulty of obtaining a Pixel for GrapheneOS and shared mixed experiences with the OS's usability compared to LineageOS.

**Tags**: `#security`, `#Android`, `#VPN`, `#GrapheneOS`, `#privacy`

---

<a id="item-4"></a>
## [WebRTC's packet dropping harms LLM audio accuracy](https://simonwillison.net/2026/May/9/luke-curley/#atom-everything) ⭐️ 8.0/10

Luke Curley, in response to OpenAI's low-latency voice AI blog, argues that WebRTC's aggressive audio packet dropping to maintain low latency is fundamentally incompatible with the need for accurate audio prompts in LLM interactions. This critique highlights a critical design conflict between real-time communication protocols and AI voice applications, potentially influencing how companies like OpenAI choose transport protocols for voice-based LLM services. WebRTC's browser implementation hard-codes the inability to retransmit dropped audio packets, as experienced at Discord; users would prefer a 200ms latency increase for accurate prompts rather than degraded audio.

rss · Simon Willison · May 9, 01:03

**Background**: WebRTC (Web Real-Time Communication) is a protocol designed for low-latency audio/video communication, commonly used in video conferencing. It aggressively drops packets during poor network conditions to keep latency low, which is acceptable for human conversations but problematic for AI prompts that require every audio detail for accurate understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://moq.dev/blog/webrtc-is-the-problem/">OpenAI's WebRTC Problem - Media over QUIC</a></li>
<li><a href="https://tldr.tech/dev/2026-05-08">Making Gemma faster, OpenAI’s WebRTC problem, don’t install...</a></li>

</ul>
</details>

**Tags**: `#WebRTC`, `#AI`, `#audio`, `#networking`, `#LLM`

---

<a id="item-5"></a>
## [Baidu Launches ERNIE 5.1 with 94% Cost Reduction](https://mp.weixin.qq.com/s/_I9ziafHheXiJpA-QY2F7A) ⭐️ 8.0/10

Baidu has officially launched ERNIE 5.1, its latest large language model, now available on the Qianfan model plaza and the ERNIE Bot website for enterprise users and developers. The model adopts a 'multi-dimensional elastic pre-training' technique, achieving leading performance with only about 6% of the pre-training cost of comparable models. This release demonstrates that significant efficiency gains can be achieved without sacrificing performance, potentially lowering the barrier for large-scale AI deployment in China. Its competitive rankings on LMArena and claims of surpassing models like DeepSeek highlight the intensifying race among Chinese AI firms. ERNIE 5.1 compresses total parameters to about one-third and active parameters to about half of ERNIE 5.0, using a variable Top-k routing mechanism for dynamic balance between cost and capability. It scores 1223 points on the LMArena search leaderboard, ranking first domestically and fourth globally.

telegram · zaihuapd · May 9, 07:45

**Background**: ERNIE is Baidu's foundational large language model series. 'Multi-dimensional elastic pre-training' is a technique that trains multiple model scales simultaneously, allowing a single training run to produce models of various sizes efficiently. LMArena is a crowdsourced, human-voted leaderboard that ranks AI models based on real user interactions.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.sina.com.cn/tech/digi/2026-05-09/doc-inhxhcxm1651084.shtml">百度发布文心大模型 5.1：搜索能力位居国内首位，预训练成本仅为业界 6%_新浪科技_新浪网</a></li>
<li><a href="https://finance.sina.com.cn/tech/roll/2026-05-09/doc-inhxhqpf1482100.shtml">百度文心大模型5.1发布：登顶多个榜单，预训练成本仅为业界 6%|文心|智能体|百度_新浪科技_新浪网</a></li>
<li><a href="https://www.chinaz.com/2026/0509/1751121.shtml">百度文心大模型5.1正式发布</a></li>

</ul>
</details>

**Tags**: `#Baidu`, `#ERNIE`, `#large language model`, `#AI model`, `#Chinese AI`

---

<a id="item-6"></a>
## [NASA JPL Achieves Rotor Breakthrough for Mars Helicopters](https://arstechnica.com/space/2026/05/engineers-at-nasas-jet-propulsion-lab-make-a-breakthrough-in-rotor-technology/) ⭐️ 8.0/10

NASA JPL engineers successfully tested next-generation rotor blades that reached supersonic speeds (Mach 1.08) in a simulated Mars atmosphere, achieving a 30% improvement in lift efficiency. This breakthrough enables future Mars helicopters to carry heavier payloads and fly longer distances, significantly expanding the scope of aerial exploration on the Red Planet. The test was conducted in JPL's 25-Foot Space Simulator vacuum chamber under Mars-like conditions. The rotor tip speed exceeded Mach 1.0, marking the first supersonic rotor operation on another world.

telegram · zaihuapd · May 9, 14:21

**Background**: Mars has an extremely thin atmosphere, about 1% of Earth's, making it challenging for rotorcraft to generate lift. NASA's Ingenuity helicopter demonstrated flight is possible, but its rotors were limited in speed and lift. The new rotor design uses advanced carbon-fiber materials and refined blade shapes to achieve higher speeds and significantly greater lift.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huxiu.com/article/4856772.html">NASA下一代火星直升机旋翼叶片成功突破音速，马赫1.08</a></li>
<li><a href="https://www.msn.cn/zh-cn/news/other/火星旋翼首破马赫-nasa-开启异星飞行新时代/ar-AA22LmvR">火星旋翼首破马赫，NASA 开启异星飞行新时代 - MSN</a></li>
<li><a href="https://www.cislunarspace.cn/space-news/2026/05/2026-05-07-nasa-mars-helicopter-rotor-mach1/">NASA下一代火星直升机旋翼突破音障 超音速飞行测试取得关键进展 | 地...</a></li>

</ul>
</details>

**Tags**: `#Mars`, `#rotor technology`, `#NASA`, `#space exploration`, `#breakthrough`

---