如果只看一句发布文案，Gemini Omni 很容易被理解成 Google 又发了一个更强的视频模型。

但把最近几天的报道和案例放在一起看，你会发现这次更新更像是在重新定义一件事，视频生成不再只是「给一句 prompt，吐一个结果」，而是开始变成一套可以持续编辑、持续控制、持续迭代的工作流。

从 AI HOT 最近 7 天收录的相关条目看，Gemini Omni 这一波集中发布发生在 `2026-05-19` 的 Google I/O 2026，`2026-05-22` 又出现了一轮官方创作案例扩散。几条最值得关注的信息，基本都在指向同一个结论，Gemini Omni 的重点不是单次生成，而是多模态输入、世界理解和对话式编辑。

## 这波发布，外面都在怎么讲

先看最核心的几条。

- Google DeepMind 在 [官方博客](https://deepmind.google/blog/introducing-gemini-omni) 里把 Gemini Omni 定义为「从任意输入创造内容」的第一步，起点是视频。
- Sundar Pichai 在 `2026-05-19` 的发帖里强调，Gemini Omni 不只是把场景做得像真的，而是会推理接下来应该发生什么，并且当天就开始在 Gemini App、Google Flow 和 YouTube Shorts 面向 Google AI Plus、Pro、Ultra 用户推出视频生成功能。
- [IT 之家](https://www.ithome.com/0/952/519.htm) 对这次发布的提炼很接地气，一句话总结就是「一句话让 AI 修改视频」，这个说法其实抓得挺准，因为它点出了 Gemini Omni 最重要的交互变化，不再只是生成，而是编辑。
- `2026-05-19` 当天，Google DeepMind 还专门提到 [Gemini Omni 和 Google Flow 的结合](https://x.com/GoogleDeepMind/status/2056804306653794336)，重点放在批量编辑、角色一致性和更电影化的故事表达上。
- 到了 `2026-05-22`，Gemini 官方账号又发了一条 [创意作品汇总](https://x.com/GeminiApp/status/2057616371748651054)，这说明它已经开始从发布会能力展示，进入到「大家真的在拿它做东西」的阶段。

这几条报道拼起来，信号非常明确。

第一，Gemini Omni 是这轮 Gemini 更新里的核心创作能力，不是边角功能。  
第二，它的卖点不是单一模态，而是文本、图片、视频混合输入。  
第三，它真正想打的是「可编辑的视频工作流」，而不是一段一次性的 demo。

## 为什么这件事值得认真看

过去一年，视频模型已经很多了，大家也都见过不少惊艳样片。但真正卡住创作者的，往往不是第一条视频能不能生成出来，而是第二步和第三步，能不能改，能不能延续，能不能保持人物和场景不崩。

Gemini Omni 这次给出的方向，是把视频生成从「出片工具」往「内容制作工具」推了一步。

你不需要每次都从零开始。  
你可以从文本开始，也可以从图片开始，甚至可以直接从已有视频开始。  
然后你再用自然语言继续改它。

这就是为什么外部报道会反复提到 `edit`、`Flow`、`consistency`、`world understanding` 这些词。因为真正稀缺的，不再是模型能不能动，而是模型能不能在你反复修改之后还保持逻辑。

## 如果只看一个官方例子，先看这个

Google DeepMind 的官方展示片，最值得看的地方不是炫，而是它把 Gemini Omni 想解决的问题讲得非常完整。

![](https://cdn.jsdelivr.net/gh/ZeroLu/awesome-gemini-omni@main/promo-assets/gifs/googledeepmind.gif)

这里面传达的信息其实很直接，Gemini Omni 不是只负责出一个短视频，而是负责把创意输入、镜头变化、风格延续和后续编辑串起来。它更像一个创作底座，而不是一个单点功能。

## 案例一，镜头感是不是能被写进去

我最喜欢的一个案例，是这个伦敦眼 prompt。它很短，但测试点非常清楚，镜头突然拉近、轻微来回、重新对焦，而且明确要求没有时间戳、没有对白。

```text
a recording from a capsule on the london eye, a jerky zoom into something in the distance and then refocusing (with a bit of back and forth) (no timestamp or dialog)
```

![](https://cdn.jsdelivr.net/gh/ZeroLu/awesome-gemini-omni@main/promo-assets/gifs/fofr.gif)

这类案例的价值，不在于题材有多花，而在于它能拿来检验一个视频模型到底有没有镜头语言。很多模型能生成画面，但一到这种有明确摄影动作要求的 prompt，就会开始散。

Gemini Omni 至少在这个例子里，说明它已经不是只会做一段「像视频的东西」，而是开始能理解一些更细的镜头意图。

## 案例二，普通场景能不能稳住

另一组我觉得非常有代表性的案例，是白板推导这一类日常场景。它不靠奇观，不靠大特效，真正考验的是人物、动作、文字和机位能不能同时稳定。

这条可恢复的 prompt 片段只有一句开头：

```text
A professor writes out a mathematical proof for
```

但光看三段输出，其实已经能看出测试意图了。

![](https://cdn.jsdelivr.net/gh/ZeroLu/awesome-gemini-omni@main/promo-assets/gifs/tom1.gif)

![](https://cdn.jsdelivr.net/gh/ZeroLu/awesome-gemini-omni@main/promo-assets/gifs/tom2.gif)

![](https://cdn.jsdelivr.net/gh/ZeroLu/awesome-gemini-omni@main/promo-assets/gifs/tom3.gif)

这种例子特别好，因为它逼着你去看一些更实际的问题。

黑板上的信息是不是稳定。  
人物动作是不是自然。  
镜头是不是像一个真的人在拍。  
这些东西如果稳不住，再强的宣传片都没意义。

## 案例三，它已经开始进入对比赛道了

还有一类信号也很重要，就是 Gemini Omni 已经不再只是单独展示，而是被拿去和别的模型正面对比。

![](https://cdn.jsdelivr.net/gh/ZeroLu/awesome-gemini-omni@main/promo-assets/gifs/jsfilmz.gif)

这类对比通常会把重点放在编辑能力、物理表现、水体模拟、动作连续性这些更难的地方。只要一个模型开始频繁进入这种对比环境，就说明行业看它的方式已经变了，不是在问它能不能生成，而是在问它在真实工作流里到底排第几。

## 现在最实际的用法是什么

如果你今天就想试 Gemini Omni，我觉得最现实的路径不是继续刷一堆二手解读，而是直接上手。

Cyberbara 这边已经把 Gemini Omni Video 做成了国内可用入口，文生视频、图生视频、视频转视频都放在同一个工作台里，第一次上手会比很多原生入口直接得多。

![](https://cdn.jsdelivr.net/gh/ZeroLu/awesome-gemini-omni@main/promo-assets/cyberbara-gemini-hero.png)

对普通用户来说，这比「知道模型名」更重要。因为真正阻碍你开始试的，往往不是能力不足，而是入口太远、链路太碎。

## 我顺手整理了一个资料入口

如果你想继续看可复用案例、prompt 片段和对应视频，我把这批公开可验证的内容收进了 `awesome-gemini-omni`，方便后面持续补充。

仓库地址是 `https://github.com/ZeroLu/awesome-gemini-omni`

Cyberbara 页面是 `https://cyberbara.com/zh/gemini-omni`

对我来说，这两个入口刚好解决两件事。

一个负责让你马上开跑。  
一个负责让你回头复盘，看看这个模型到底适合怎么写、怎么测、怎么比较。
