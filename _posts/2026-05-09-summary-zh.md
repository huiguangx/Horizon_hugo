---
layout: default
title: "Horizon Summary: 2026-05-09 (ZH)"
date: 2026-05-09
lang: zh
---

> From 32 items, 16 important content pieces were selected

---

1. [Triton v3.7.0 发布，新增 scaled BMM 和 FP8 常量](#item-1) ⭐️ 8.0/10
2. [互联网档案馆瑞士成立为独立实体](#item-2) ⭐️ 8.0/10
3. [研究显示：让 LLM 处理文档会导致内容损坏](#item-3) ⭐️ 8.0/10
4. [Google reCAPTCHA 对去谷歌化安卓用户失效](#item-4) ⭐️ 8.0/10
5. [网络自由主义的虚伪曝光](#item-5) ⭐️ 8.0/10
6. [数学家体验 ChatGPT 5.5 Pro，突出推理能力提升](#item-6) ⭐️ 8.0/10
7. [GrapheneOS 修复了被谷歌忽略的安卓 VPN 泄露漏洞](#item-7) ⭐️ 8.0/10
8. [人工智能打破两种漏洞文化](#item-8) ⭐️ 8.0/10
9. [WebRTC 设计损害 LLM 提示准确性](#item-9) ⭐️ 8.0/10
10. [Claude Code：HTML 输出为何胜过 Markdown](#item-10) ⭐️ 8.0/10
11. [Anthropic 拟募数百亿美元，估值逼近万亿美元](#item-11) ⭐️ 8.0/10
12. [美国怀疑英伟达芯片经泰国走私至阿里巴巴](#item-12) ⭐️ 8.0/10
13. [DeepSeek 首轮融资估值据称达 450 亿美元](#item-13) ⭐️ 8.0/10
14. [苹果拟打破台积电独家代工，或采用英特尔 18A](#item-14) ⭐️ 8.0/10
15. [ChatGPT Android 版 APK 拆解发现 Codex 远程桌面控制功能](#item-15) ⭐️ 8.0/10
16. [研究：AI 回答常偏向日本或美国视角](#item-16) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Triton v3.7.0 发布，新增 scaled BMM 和 FP8 常量](https://github.com/triton-lang/triton/releases/tag/v3.7.0) ⭐️ 8.0/10

Triton v3.7.0 新增了缩放批量矩阵乘法 (scaled BMM)、前端直接创建 FP8 常量的支持，以及 tl.squeeze 和 tl.unsqueeze 等新的方言操作。 此版本增强了 Triton 更高效地处理现代 AI 工作负载的能力，特别是低精度推理和训练，并通过新的方言操作扩展了编译器的灵活性。 Scaled BMM 允许对矩阵乘法输入进行分块缩放，提高低精度格式的数值稳定性。FP8 常量允许在 Triton 内核中直接声明 FP8 值，减少开销。

github · atalman · May 7, 22:19

**背景**: Triton 是一种用于编写高性能 GPU 内核的领域特定语言和编译器，广泛应用于 PyTorch 等深度学习框架。块缩放矩阵乘法中的缩放因子有助于缓解低比特计算中的精度损失。FP8 是一种 8 位浮点格式，越来越多地被用于高效的 AI 推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://triton-lang.org/main/getting-started/tutorials/10-block-scaled-matmul.html">Block Scaled Matrix Multiplication — Triton documentation</a></li>
<li><a href="https://pytorch.org/blog/accelerating-llama3/">Accelerating Llama3 FP8 Inference with Triton Kernels – PyTorch</a></li>
<li><a href="https://github.com/parca-dev/proton">GitHub - parca-dev/ proton</a></li>

</ul>
</details>

**标签**: `#triton`, `#compiler`, `#AI`, `#ML`, `#release`

---

<a id="item-2"></a>
## [互联网档案馆瑞士成立为独立实体](https://blog.archive.org/2026/05/06/internet-archive-switzerland-expanding-a-global-mission-to-preserve-knowledge/) ⭐️ 8.0/10

2026 年 5 月 6 日，互联网档案馆宣布成立瑞士分支机构作为独立实体，与互联网档案馆、加拿大互联网档案馆和欧洲互联网档案馆一起，共同构建一个分布式、有弹性的数字图书馆。 此次扩展通过创建去中心化的档案馆网络，降低了单点故障或法律脆弱性的风险，从而加强了全球数字保存。它以更具弹性的基础设施推进了“普及所有知识”的使命。 互联网档案馆瑞士由执行董事 Roman Griesfelder 领导，他是一名奥地利公民，自 1998 年起居住在瑞士。该组织计划结合 2026 年 11 月在巴黎举行的联合国教科文组织会议，探索如何保护濒危档案。

hackernews · hggh · May 9, 12:00 · [社区讨论](https://news.ycombinator.com/item?id=48074265)

**背景**: 数字保存确保数字信息长期可访问和可用，但集中式档案馆面临法律挑战、审查和物理灾难的风险。分布式数字图书馆隐藏了实际服务器架构，允许用户与最近的节点交互，从而提高了弹性和性能。互联网档案馆长期倡导知识的普及访问，而瑞士实体是迈向联邦化、独立图书馆网络的关键一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.archive.org/2026/05/06/internet-archive-switzerland-expanding-a-global-mission-to-preserve-knowledge/">Internet Archive Switzerland : Expanding a Global Mission to...</a></li>
<li><a href="https://internetarchive.ch/">Internet Archive Switzerland</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_preservation">Digital preservation - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，互联网档案馆需要一种类似 Usenet 的对等互联模型，其中独立组织共享内容但不共享 DMCA 删除请求，以在法律上保护网络。有人对瑞士实体的实际独立性表示怀疑，指出其与美国的互联网档案馆共享董事会成员和基础设施。

**标签**: `#internet-archive`, `#digital-preservation`, `#decentralization`, `#resilience`, `#libraries`

---

<a id="item-3"></a>
## [研究显示：让 LLM 处理文档会导致内容损坏](https://arxiv.org/abs/2604.15597) ⭐️ 8.0/10

一项涉及 19 个大语言模型（包括 Gemini 3.1 Pro、GPT 5.4 等前沿模型）的大规模实验表明，将文档任务委托给 LLM 会导致长期工作流程结束时平均 25%的内容被损坏。 这一发现挑战了 LLM 能够可靠处理 AI 代理系统中文档维护任务的假设，凸显了一个可能影响自动化工作流程的生产力和信任度的根本局限性。 即使配备了工具使用能力，内容损坏仍然存在，表明问题根源在于模型的统计特性，而非实现不佳。作者将这种退化称为“语义消融”（semantic ablation），即独特的见解被通用标记所取代。

hackernews · rbanffy · May 9, 08:44 · [社区讨论](https://news.ycombinator.com/item?id=48073246)

**背景**: 大型语言模型通过基于训练数据预测最可能的下一词元来生成文本，这天然使得输出偏向常见模式。当迭代使用时——例如编辑或总结文档——每次处理都会倾向于移除罕见、高熵的信息，并用更通用的语言替换。这种现象称为“语义消融”（semantic ablation），意味着 LLM 逐渐剥离细微差别和精确性，实质上损坏了原始意图。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2604.15597">[2604.15597] LLMs Corrupt Your Documents When You Delegate</a></li>
<li><a href="https://www.theregister.com/2026/02/16/semantic_ablation_ai_writing/">Semantic ablation: Why AI writing is boring and dangerous • The Register</a></li>
<li><a href="https://huggingface.co/papers/2604.15597">Paper page - LLMs Corrupt Your Documents When You Delegate</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍认同内容损坏的现象，有评论者将其比作 JPEG 退化，另一位则创造了“语义消融”一词。部分质疑存在：simonw 对工具使用实验的设计提出疑问，认为更好的代理模式可以减轻损坏。其他人则提出变通方法，例如将知识存储为独立的事实文件，仅将 LLM 用于最终渲染。

**标签**: `#LLMs`, `#document corruption`, `#semantic ablation`, `#AI agents`, `#tool use`

---

<a id="item-4"></a>
## [Google reCAPTCHA 对去谷歌化安卓用户失效](https://reclaimthenet.org/google-broke-recaptcha-for-de-googled-android-users) ⭐️ 8.0/10

Google 最新的 reCAPTCHA 更新要求 Play Integrity 认证，导致没有 Google Play 服务的去谷歌化安卓设备无法使用该服务。 这一变化迫使去谷歌化安卓用户在隐私与访问数百万依赖 reCAPTCHA 的网站之间做出选择，并标志着行业向远程认证作为守门机制的趋势。 Play Integrity 通过验证设备是否运行已认证的安卓版本并安装了 Google Play 来检查设备真实性，而像 GrapheneOS（即使使用沙盒版 Play Services）等替代操作系统可能无法完全满足要求。

hackernews · anonymousiam · May 8, 18:45 · [社区讨论](https://news.ycombinator.com/item?id=48067119)

**背景**: 去谷歌化安卓指的是避免使用谷歌专有服务以增强隐私的自定义 ROM 或设备。reCAPTCHA 是广泛使用的机器人检测系统。Play Integrity 是一种谷歌 API，通过硬件支持的认证来验证应用和设备的完整性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/google/play/integrity/overview">Overview of the Play Integrity API | Android Developers</a></li>
<li><a href="https://tech.yahoo.com/phones/articles/googling-android-simpler-think-no-193119747.html">De - Googling Android is simpler than you think—no special phone...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Remote_attestation">Remote attestation</a></li>

</ul>
</details>

**社区讨论**: 社区评论揭示了深层担忧：一位用户解释了远程认证如何通过 EK->AIK 密钥将设备与身份绑定，认为这损害了隐私。另一位指出，即使是沙盒版 Play Services 也可能无法通过 Play Integrity，还有一位感叹网络正转向强制性的类似 KYC 的验证。

**标签**: `#Android`, `#reCAPTCHA`, `#privacy`, `#Google Play Integrity`, `#remote attestation`

---

<a id="item-5"></a>
## [网络自由主义的虚伪曝光](https://matduggan.com/the-intolerable-hypocrisy-of-cyberlibertarianism/) ⭐️ 8.0/10

一篇文章批判了网络自由主义理念的虚伪，尤其在版权问题上，当人工智能威胁到他们的经济利益时，科技内部人士改变了立场。 这一批判意义重大，因为它揭示了科技行业对自由市场与反监管理念的选择性应用，影响着人工智能和版权政策的辩论。 文章运用网络自由主义独立宣言的历史案例以及当前人工智能的争议，展示了这种不一致性，并指出富有的权势人物忽视了这些争论。

hackernews · ColinWright · May 9, 13:48 · [社区讨论](https://news.ycombinator.com/item?id=48074952)

**背景**: 网络自由主义是一种植根于早期互联网黑客和密码朋克文化的政治意识形态，主张政府最少监管和信息自由流动。文章认为，当自身利益受到威胁时，其支持者就会抛弃这些原则，尤其是在人工智能时代的版权问题上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyberlibertarianism">Cyberlibertarianism</a></li>
<li><a href="https://en.wikipedia.org/wiki/Technolibertarianism">Technolibertarianism - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论指出人们对版权态度的转变，用户观察到企业此前利用版权打压开源，现在却声称用版权保护其人工智能生成内容。部分评论者同意该批判，但也指出例外情况，并质疑这种虚伪的普遍性。

**标签**: `#cyberlibertarianism`, `#copyright`, `#AI`, `#tech criticism`, `#ethics`

---

<a id="item-6"></a>
## [数学家体验 ChatGPT 5.5 Pro，突出推理能力提升](https://gowers.wordpress.com/2026/05/08/a-recent-experience-with-chatgpt-5-5-pro/) ⭐️ 8.0/10

菲尔兹奖得主 Timothy Gowers 分享了他使用 OpenAI 的 ChatGPT 5.5 Pro 的体验，称赞其推理和解决问题的能力相比早期模型有了显著提升。他指出，该模型现在能够解决他所谓的“温和问题”，而这些问题以前被认为适合初入博士阶段的学生。 这位顶尖数学家的反思表明，先进的 LLM 正在接近能够处理真正数学研究问题的水平，可能改变研究进行的方式以及博士生的培养模式。这一讨论引发了关于人类思维价值以及学术教育未来的紧迫问题。 ChatGPT 5.5 Pro 于 2026 年 4 月 23 日由 OpenAI 发布，代号为“Spud”，不向免费用户提供。Gowers 强调，虽然该模型功能强大，但仍会犯很多错误，需要严格的引导才能正确执行，但它在自我纠正和推理跟踪方面表现出色。

hackernews · _alternator_ · May 9, 02:41 · [社区讨论](https://news.ycombinator.com/item?id=48071262)

**背景**: ChatGPT 5.5 Pro 是 OpenAI 大型语言模型系列的最新版本，在 GPT-4 的基础上改进了推理和多模态能力。Timothy Gowers 是著名数学家、菲尔兹奖得主，他发表的博文将模型的能力与博士级别的问题解决能力相比较，在学术界和 AI 社区引发了广泛讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT - 5 . 5 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍认同 Gowers 的观察，用户注意到模型自我纠正能力的提升，但也指出其成本高昂且容易犯概念性错误。一些评论者（如物理学家 ziotom78）分享了使用类似模型检查论文的积极体验，而其他人则就原创思维和研究训练的价值展开了更深入的讨论。

**标签**: `#ChatGPT`, `#LLM`, `#AI research`, `#mathematics`, `#education`

---

<a id="item-7"></a>
## [GrapheneOS 修复了被谷歌忽略的安卓 VPN 泄露漏洞](https://cyberinsider.com/grapheneos-fixes-android-vpn-leak-google-refused-to-patch/) ⭐️ 8.0/10

GrapheneOS 发布了一个更新，修复了安卓系统中的 VPN 绕过漏洞，该漏洞允许 system_server 进程在始终开启 VPN 和阻止非 VPN 连接保护启用时泄露用户的真实 IP 地址。谷歌承认了该问题但拒绝修复，GrapheneOS 在 4 月 29 日公开披露后自行实施了修复。 此修复意义重大，因为它恢复了安卓系统上 VPN 的隐私保证，恶意应用或网络观察者可能利用该漏洞揭露用户的真实 IP 地址。这也凸显了谷歌的安全优先级与社区期望之间的分歧，进一步巩固了 GrapheneOS 作为注重隐私的替代方案的地位。 该漏洞源于 system_server 拥有更高的网络权限，使其能够绕过 VPN 路由限制。GrapheneOS 实现了网络权限检查，以确保 system_server 的流量通过 VPN。谷歌拒绝修复该问题，称需要不兼容的更改，但 GrapheneOS 在不破坏兼容性的情况下成功修复。

hackernews · Georgelemental · May 9, 14:11 · [社区讨论](https://news.ycombinator.com/item?id=48075144)

**背景**: GrapheneOS 是一个基于安卓的注重隐私和安全性的开源操作系统，主要面向 Google Pixel 设备。安卓的 system_server 是一个核心进程，托管许多系统服务并以高权限运行。VPN 泄露是指流量绕过了 VPN 隧道，暴露了用户的真实 IP 地址。该漏洞允许 system_server 直接访问网络，即使在启用了“阻止非 VPN 连接”的情况下也能绕过 VPN 路由。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberinsider.com/grapheneos-fixes-android-vpn-leak-google-refused-to-patch/">GrapheneOS fixes Android VPN leak Google refused to... | CyberInsider</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://stackoverflow.com/questions/34651015/what-is-systemserver-for-android">What is SystemServer for Android ? - Stack Overflow</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映了不同的反应：一些用户讨论了运行 GrapheneOS 所需的 Pixel 手机的成本和可用性，而另一些用户则将其用户体验与 LineageOS 进行了不利比较。一位评论者表示惊讶，谷歌竟然尊重了禁售期直到 4 月 29 日，而不是立即发布修复。总体而言，讨论显示出兴趣，但也存在采用 GrapheneOS 的实际担忧。

**标签**: `#security`, `#Android`, `#GrapheneOS`, `#VPN`, `#privacy`

---

<a id="item-8"></a>
## [人工智能打破两种漏洞文化](https://www.jefftk.com/p/ai-is-breaking-two-vulnerability-cultures) ⭐️ 8.0/10

AI 工具正在加速漏洞的发现与利用，削弱了开源与闭源软件在漏洞处理上的传统区别，这是 Jeff Kaufman 提出的观点。 这种转变缩小了防御者修补漏洞的时间窗口，尤其是对闭源软件而言，可能增加行业范围内零日攻击的频率和影响。 催化剂来自开源采用增加和逆向工具改进带来的软件透明度提升，而不仅仅是 LLM；这一趋势在 AI 出现之前很久就被预测到了。

hackernews · speckx · May 8, 17:55 · [社区讨论](https://news.ycombinator.com/item?id=48066524)

**背景**: 传统上，开源软件的漏洞发现和修补更加透明，而闭源软件依赖于保密性。AI 现在能够更快地生成利用代码，模糊了这一界限。

**社区讨论**: 评论者争论 AI 是否是真正的驱动因素，有人指出对比补丁差异早已是常见做法。其他人强调，更低的利用生成成本使得协调披露更加重要，而非更不重要。

**标签**: `#AI`, `#vulnerability disclosure`, `#cybersecurity`, `#open source`, `#LLMs`

---

<a id="item-9"></a>
## [WebRTC 设计损害 LLM 提示准确性](https://simonwillison.net/2026/May/9/luke-curley/#atom-everything) ⭐️ 8.0/10

Luke Curley 指出，WebRTC 为了低延迟而激进地丢弃数据包，这损害了发送给 LLM 的提示的准确性，用户宁愿等待可靠传输也不愿收到快速但已损坏的输入。 WebRTC 的设计目标与 LLM 交互需求之间的这种不匹配可能导致 AI 响应质量下降，影响基于语音的 AI 应用的用户体验。这凸显了随着 AI 从人人通信转向人机通信，协议需要相应调整。 WebRTC 使得在浏览器中无法重传音频数据包，正如 Discord 尝试实现该功能时所经历的那样。Curley 指出，用户愿意接受额外 200 毫秒的延迟来获得准确的提示，但协议的实现被硬编码为优先保证实时延迟。

rss · Simon Willison · May 9, 01:03

**背景**: WebRTC 是一种为低延迟音频和视频通话设计的实时通信协议。在恶劣网络条件下，它会激进地丢弃数据包以保持流畅播放和唇同步，因为重传会增加延迟。这种权衡适用于人类对话，但对于传输像 LLM 提示这样的精确数据则存在问题，因为每个数据包都对准确性至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bloggeek.me/webrtcglossary/packet-loss/">Packet Loss in WebRTC: Causes, Effects & How to Fix It • BlogGeek.me</a></li>
<li><a href="https://www.digitalsamba.com/blog/packet-loss-in-webrtc">Understanding and Preventing Packet Loss in WebRTC: A Guide</a></li>

</ul>
</details>

**标签**: `#WebRTC`, `#LLMs`, `#real-time communication`, `#audio streaming`, `#protocol design`

---

<a id="item-10"></a>
## [Claude Code：HTML 输出为何胜过 Markdown](https://simonwillison.net/2026/May/8/unreasonable-effectiveness-of-html/#atom-everything) ⭐️ 8.0/10

Anthropic 的 Claude Code 团队成员 Thariq Shihipar 建议在提示 Claude Code 时使用 HTML 而非 Markdown 作为输出格式，并展示了 HTML 能够提供更丰富的交互式解释，包括嵌入 SVG 图表和小部件。该建议附有示例提示和 HTML 制品集合。 这一技术改变了在 LLM 输出中使用 Markdown 的常见做法，从 AI 编程助手中解锁出更有效且视觉更吸引人的响应。开发者现在可以获得更丰富、自包含的 HTML 解释，其中包含交互元素，从而改善代码审查和学习体验。 Shihipar 提供了提示示例，例如要求 Claude 创建包含内联边距注释和按严重程度颜色编码的代码审查 HTML 制品。Simon Willison 用 GPT-5.5 在 Linux 漏洞解释上测试了该方法，生成了样式良好的交互式 HTML 页面，但他指出需要更强调漏洞本身而非封装代码。

rss · Simon Willison · May 8, 21:00

**背景**: Claude Code 是 Anthropic 的代理式编码工具，在终端中运行，允许开发者将工程任务委托给 AI 并借助 AI 探索代码库。传统上，Markdown 因其 token 效率而成为 LLM 的默认输出格式，但 HTML 允许在单个自包含文件中实现更丰富的格式、嵌入式视觉效果和交互元素。Simon Willison 此前曾撰写关于构建用于交互式工具的 HTML 工具的文章。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://digitalthoughtdisruption.com/2025/08/19/offline-html-productivity-artifact-generator-prompt/">Offline HTML Productivity Artifact Generator: Field-Ready AI Prompt</a></li>

</ul>
</details>

**标签**: `#LLM`, `#prompting`, `#HTML`, `#Claude Code`, `#technical-deep-dive`

---

<a id="item-11"></a>
## [Anthropic 拟募数百亿美元，估值逼近万亿美元](https://www.ft.com/content/a40cafcc-0fa4-4e70-9e24-90d826aea56d) ⭐️ 8.0/10

Anthropic 正计划今年夏天筹集数百亿美元的新资金，以扩容其算力基础设施，此举可能将其估值推高至近 1 万亿美元，从而超越其最大竞争对手 OpenAI。 这标志着 AI 行业竞争格局的重大转变，Anthropic 可能在估值上超越 OpenAI，吸引大量资本投资，从而加速 AI 发展并重塑市场格局。 在 Forge Global 等私募二级市场交易平台上，Anthropic 的隐含估值已达 1 万亿至 1.2 万亿美元，超过了 OpenAI 约 8800 亿美元的估值。今年 2 月，Anthropic 刚刚完成一轮 300 亿美元融资，投后估值 3800 亿美元，得益于企业客户爆发式增长，短短数月其估值预期已翻倍逾两倍。

telegram · zaihuapd · May 8, 11:15

**背景**: Anthropic 是一家领先的人工智能公司，以开发 Claude 系列大语言模型而闻名，是 OpenAI 的主要竞争对手。AI 行业投资激增，各公司竞相构建更大规模的模型和数据中心，需要海量资金。二级市场估值通常反映了正式融资轮次完成前的投资者预期。

**标签**: `#Anthropic`, `#Funding`, `#Valuation`, `#OpenAI`, `#AI Industry`

---

<a id="item-12"></a>
## [美国怀疑英伟达芯片经泰国走私至阿里巴巴](https://www.bloomberg.com/news/articles/2026-05-08/us-said-to-suspect-nvidia-chips-smuggled-to-alibaba-via-thailand) ⭐️ 8.0/10

美国检方怀疑泰国公司 OBON Corp. 将价值 25 亿美元的 Super Micro 服务器（内含先进英伟达芯片）走私至中国，阿里巴巴被指为终端客户之一。 此案可能加剧美中技术出口管制紧张局势，影响两国 AI 能力发展，并可能导致美国对泰国的芯片出口限制更加严格。 OBON 曾参与创建泰国主权 AI 云 Siam AI，后者获得了英伟达合作伙伴地位；阿里巴巴否认与 Super Micro 或 OBON 有任何业务关系，Siam AI 的 CEO 声称已离开 OBON 且公司未涉及走私。

telegram · zaihuapd · May 8, 13:23

**背景**: 英伟达的先进 AI 芯片（如 H100 和 A100）受美国出口管制，以防止中国获得用于军事或监控的尖端技术。主权 AI 云是由政府控制的数字基础设施，旨在将国家数据和计算能力保留在境内。泰国 Siam AI Cloud 由英伟达支持，旨在为泰国开发主权 AI 生态系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://siam.ai/">Siam ai corporation co., ltd.</a></li>
<li><a href="https://www.linkedin.com/company/siam-ai">SIAM . AI Cloud | 513 followers on LinkedIn. Thailand 's Leading...</a></li>

</ul>
</details>

**标签**: `#NVIDIA`, `#AI chips`, `#export controls`, `#smuggling`, `#Alibaba`

---

<a id="item-13"></a>
## [DeepSeek 首轮融资估值据称达 450 亿美元](https://t.me/zaihuapd/41289) ⭐️ 8.0/10

据称，DeepSeek 正在寻求首轮外部融资，估值可能达到 450 亿美元，中国国家集成电路产业投资基金正洽谈领投。 这将是 DeepSeek 首次大规模外部融资，标志着国资更深介入中国 AI 核心公司，可能在芯片出口限制背景下加速开发低成本高效 AI 模型。 估值约 450 亿美元，使 DeepSeek 成为全球最具价值的 AI 初创公司之一。领投方为国家集成电路产业投资基金（'大基金'），该基金通常投资半导体企业。

telegram · zaihuapd · May 8, 14:59

**背景**: DeepSeek 是一家成立于 2023 年的中国 AI 公司，以其开源权重的大语言模型闻名，训练成本仅为竞争对手（如 OpenAI 的 GPT-4）的一小部分。该公司的成功挑战了美国在 AI 领域的主导地位，并引发了全行业对成本效率的重新评估。国家集成电路产业投资基金由中国政府设立，旨在提升国内半导体自给率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://en.wikipedia.org/wiki/China_Integrated_Circuit_Industry_Investment_Fund">China Integrated Circuit Industry Investment Fund - Wikipedia</a></li>
<li><a href="https://www.scmp.com/tech/enterprises/article/2145422/how-chinas-big-fund-helping-country-catch-global-semiconductor-race">How China ’s ‘Big Fund ’ is helping the country catch up in chip race</a></li>

</ul>
</details>

**标签**: `#AI融资`, `#DeepSeek`, `#中国AI`, `#产业基金`

---

<a id="item-14"></a>
## [苹果拟打破台积电独家代工，或采用英特尔 18A](https://t.me/zaihuapd/41292) ⭐️ 8.0/10

据报道，苹果正考虑结束台积电自 2014 年以来的独家代工地位，最早可能在 2027 年将部分中低端处理器交由英特尔的 18A 工艺生产。 这一潜在转变可能降低苹果对单一供应商的依赖，实现芯片供应链多元化，同时在 AI 芯片需求增长背景下为英特尔的代工业务带来重大提振。 英特尔的角色仅限于代工制造，不涉及芯片设计；合作最初将针对 Mac、iPad 或 iPhone 的中低端处理器。

telegram · zaihuapd · May 8, 17:18

**背景**: 自 2014 年以来，台积电一直是苹果的独家芯片制造商，负责生产所有 A 系列和 M 系列处理器。英特尔的 18A 工艺（相当于 2 纳米）是其代工复兴战略的一部分，旨在与台积电和三星竞争。此举正值台积电优先满足英伟达等 AI 芯片客户产能需求之际，促使苹果寻求供应链多元化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.comss.ru/page.php?id=19090">Новые процессоры Intel Core Ultra 300 (Panther Lake) на Intel ...</a></li>
<li><a href="https://hardwareand.co/actualites/breves/intel-18a-est-maintenant-pret-nous-dit-intel">" Intel 18 A est maintenant prêt", nous dit Intel ! - Hardware & Co</a></li>

</ul>
</details>

**标签**: `#Apple`, `#TSMC`, `#Intel`, `#chip manufacturing`, `#supply chain`

---

<a id="item-15"></a>
## [ChatGPT Android 版 APK 拆解发现 Codex 远程桌面控制功能](https://www.androidauthority.com/codex-smartphone-control-3665256/) ⭐️ 8.0/10

对 ChatGPT Android 版 1.2026.125 的 APK 拆解发现了字符串，显示 OpenAI 正在为 Codex 开发远程桌面控制功能，使用户能够从智能手机管理桌面会话。 这一发展可能改变 AI 代理交互范式，实现无缝的跨设备控制，并有可能将 Codex 从编码助手扩展为桌面环境的通用遥控器。 该功能仍在开发中，没有预览或发布日期；它要求桌面端登录同一账号，并支持查找和重新连接远程会话。

telegram · zaihuapd · May 9, 02:18

**背景**: APK 拆解涉及反编译 Android 应用的安装文件，检查未发布的代码和字符串，从而揭示即将推出的功能。OpenAI Codex 是一个大型语言模型，可将自然语言转换为代码；新功能旨在将 Codex 的能力扩展到从智能手机远程控制桌面会话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model ) - Wikipedia</a></li>
<li><a href="https://medium.com/commencis/apk-teardown-in-a-nutshell-7701c3628bf5">APK Teardown in a Nutshell. In short, converting/decompiling | Medium</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#remote control`, `#Android`, `#AI`

---

<a id="item-16"></a>
## [研究：AI 回答常偏向日本或美国视角](https://cybernews.com/ai-news/every-ai-answer-japan/) ⭐️ 8.0/10

巴斯克大学和卡迪夫大学的一项研究发现，八个主流 AI 模型在 24 种语言中经常将答案锚定到日本或美国的视角，其中五个模型偏向日本，两个偏向美国。 这凸显了广泛使用的 AI 模型中的系统性文化偏见，引发了对公平性和全球适用性的担忧，特别是对于来自代表性不足地区的用户。 这种偏见主要是在监督微调阶段形成，而非预训练阶段，且低资源语言更容易输出指向模型本国（日本或美国）的答案。

telegram · zaihuapd · May 9, 10:02

**背景**: 监督微调（SFT）是一个训练阶段，模型使用标注数据适应特定任务，往往会强化训练数据中的偏见。低资源语言缺乏足够数据，因此更容易受到此类偏见的影响。该研究在八个模型和 24 种语言中测试了 31,680 个文化问题，揭示了锚定效应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/from-prompting-precision-why-supervised-fine-tuning-future-hussain-ujzpf">From Prompting to Precision: Why Supervised Fine - Tuning is the...</a></li>
<li><a href="https://www.igi-global.com/book/empowering-low-resource-languages-nlp/324158">Empowering Low - Resource Languages With NLP Solutions</a></li>

</ul>
</details>

**标签**: `#AI bias`, `#cultural bias`, `#machine learning fairness`, `#NLP research`, `#language models`

---