真就是毫无预警！`DeepSeek V4` 今天直接掀桌子了！

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/01-hero.png)

全网蹲了几个月的 V4，终于来了！而且一上来就把**百万上下文**做成标配，不加价~

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/02-context.png)

发布之前，大家还在担心：V4 会不会很贵？会不会像 GPT-4 那样用一次肉疼一次？

**这一次，DeepSeek 让担心涨价的人失望了~**

## 01. 两个型号，怎么选？

V4 这次一口气放出两个型号：

| 型号 | 参数量 | 定位 |
|------|--------|------|
| `V4-Pro` | 总参 1.6T / 激活 490 亿 | 旗舰，对标闭源顶尖模型 |
| `V4-Flash` | 总参 2840 亿 / 激活 130 亿 | 经济实惠，日常够用 |

价格方面：
- **Flash**：输入 ¥0.2/百万 tokens，输出 ¥1/百万 tokens
- **Pro**：输入 ¥1/百万 tokens，输出 ¥12/百万 tokens

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/03-pricing.png)

**百万上下文不再加价！** 就问你香不香~

## 02. 性能到底有多强？

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/04-performance.png)

来看 DeepSeek 官方给出的评测：

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/05-benchmark.png)

**Pro 版本**
- 推理能力：追平全球顶尖闭源模型
- 世界知识：开源第一，仅次于 Gemini-3.1-Pro
- 智能体编程：目前开源里的最优解

**Flash 版本**
- 推理能力已经接近 Pro
- 日常任务完全够用，API 价格相当友好

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/06-benchmark-2.png)

更有意思的是，DeepSeek 在官方公告里罕见地主动"认怂"了一句：

> 用 V4-Pro 做 Agentic Coding，实际体验优于 Claude Sonnet 4.5，但和 Opus 4.6 的深度思考模式相比仍有差距。

这种"主动承认差距"的姿态，在国内大厂的发布里确实不多见~

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/07-feedback.png)

手快的网友已经直接上车了。不过可能是之前期待拉得太高，真实体感还需要更多场景去跑——**让子弹飞一会儿~**

## 03. 有什么黑科技？

技术上，V4 这次也整了个新活：**全新的注意力机制**。

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/deepseek-v4/images/08-attention.png)

简单来说：
- 在 token 层面做压缩
- 配合自研的 DSA 稀疏注意力
- 以前百万上下文是"能做，但贵"，现在直接变成"标配，不加价"

这项技术最大的好处是**在超长上下文下依然保持效果稳定**。**从现在开始，1M（百万）上下文是 DeepSeek 所有官方服务的默认配置。**

另外还有两点值得注意：
- 同时兼容 OpenAI 和 Anthropic 两套 API 接口
- 切换只需要改 `model` 参数，迁移成本极低
- 针对 Claude Code、OpenClaw 等主流 Agent 工具做了专门适配

## 04. 怎么用？

现在就能直接体验：

> **网页端**
> [http://chat.deepseek.com](http://chat.deepseek.com)（专家模式 / 即时模式）

> **API**
> [http://api.deepseek.com](http://api.deepseek.com)（已更新）
> 🔹 `base_url` 保持不变，只需将模型名改为 `deepseek-v4-pro` 或 `deepseek-v4-flash` 即可。

特别提醒：V4 针对 Claude Code、OpenClaw 等主流 Agent 工具做了适配优化，**API 同时支持 OpenAI 和 Anthropic 两种接口格式，切换只需改 `model` 参数**。

旧接口还能再用三个月，记得提前迁移：
> ⚠️ `deepseek-chat` 和 `deepseek-reasoner` 将于 **2026 年 7 月 24 日** 停用。

这一波，**百万上下文免费时代**是真的来了！DeepSeek 狠起来，连自己都卷~ 🚀

> 📄 技术报告：[https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro/blob/main/DeepSeek_V4.pdf](https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro/blob/main/DeepSeek_V4.pdf)
>
> 🤗 开源模型权重：[https://huggingface.co/collections/deepseek-ai/deepseek-v4](https://huggingface.co/collections/deepseek-ai/deepseek-v4)
