大家好～

最近在 GitHub 上挖到一个宝藏项目——`Awesome-AI4Med`，目前已经拿下 **2.7k stars**！

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/images/01-home.png)

这项目干了件啥事呢？**把医疗 AI 领域零散的资源，整理成了一张完整的地图**——从`医疗大模型`到`多模态模型`，从`评测基准`到`开源数据集`，全给你归置得明明白白~

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/images/02-overview.png)

搞过医疗 AI 研究的兄弟应该都懂，光是"找资料、比模型、挑数据"这三步，就能把人耗掉一两周。知乎搜一圈、arxiv 翻几遍、HuggingFace 再跑一遍，结果还没开始写代码就累了~

现在好了，一份清单直接搞定~

> 项目地址：
> **https://github.com/FreedomIntelligence/Awesome-AI4Med**

## 核心资源

先整体扫一眼，这张地图上都覆盖了什么：

> 🏥 医疗大模型：HuatuoGPT、LLaVA-Med 等
> 🖼️ 多模态大模型：影像、病理、基因组全覆盖
> 📊 评测基准：MedQA、USMLE、临床诊断任务
> 📁 海量数据集：各种医疗场景的真实数据

你说这些东西要自己一个一个找，那真叫一个费劲。每家项目散落在不同地方，格式还不统一，对比起来脑壳疼~

下面挑 **3 个最值得看的部分** 展开说一下：

### 1、医疗大模型

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/images/03-medical-llms.png)

目前收录了主流的医疗垂直和多模态大模型，**一口气列了 20 多个**：

- HuatuoGPT 系列（华佗，中文医疗问诊）
- Apollo、MMedLM（多语种医疗）
- MediTron、Med42、BioMistral（英文医疗）
- MedGemma、Baichuan-M1/M2（最近的新模型）
- …… 等等

每个模型都配了论文、HuggingFace 权重、Github 代码的**三件套链接**，省掉你满网找仓库的功夫~

### 2、评测基准

做医疗 AI，躲不开"效果评估"这关。这里把主流基准整理了一遍：

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/images/05-benchmarks.png)

- **MedEvalKit**：一个框架打包了 30+ 基准，多模态 + 纯文本都能跑
- **MedBench**：中文医疗测评，覆盖 Med-Exam、MedHC、MedMC、CMeEE 等
- **LiveClin**：临床任务评测

训完模型直接跑这几套基准做对比，比自己拍脑袋下结论靠谱多了~

### 3、数据集

想训模型但没数据？这里有现成的，**分文本和多模态两大类**：

![](https://cdn.jsdelivr.net/gh/yukuifang/tech-posts@master/images/04-datasets.png)

文本类：
- Huatuo-26M（**2600 万条**中文医疗问答）
- medical-o1-reasoning-SFT（医疗推理微调集）
- Multilingual-Medical-Corpus（多语种医疗语料）

多模态类：
- PubMedVision（**129 万**医学影像-文本对）
- MedTrinity（**2500 万**）
- SLAKE、OmniMedVQA（医学视觉问答）

每个数据集都标了来源链接和样本量，不用自己从论文附录里一行行抠链接~

## 最后

说实话，这种项目的 stars 不会像那些"花活"爆款一样冲上 100k，但**对真正在做事的人来说，它省下的是最贵的资源——时间**~

你想想：做医疗 AI 项目的第一步是干什么？**找资料、对数据、选模型**。这几步自己走，一两周就过去了~现在好了，有人把地图画好了，你只管按图索骥~

而且医疗 AI 这个赛道，说大也大说小也小。大方向确实有人在卷，但**细分场景里还有一堆空地**——问诊、影像辅诊、病历结构化、用药提醒……每一个都够一个独立的小项目。

这种资源汇总的仓库，**帮的就是那些想入局、但一直不知道从哪下手的兄弟**~
