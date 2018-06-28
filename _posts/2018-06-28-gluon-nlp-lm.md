---
title: GluonNLP V0.3 语言模型
author: 王晨光 Amazon Applied Scientist
---

## 语言模型篇

![](img/kaibuliaokou.png){:width="500px"}

当时年幼无知的你看到杰伦唱:“*<span style="color:gray">就是开不了口，让她知道</span>*”，心里的潜台词一定是这样的：

![](img/gewhat.jpg){:width="300px"}

就是：*<span style="color:blue">杰伦究竟为啥开不了口？</span>*不行我来，我们感到很生气（暴露了年龄orz）。现在做了GluonNLP的我终于明白，原来是杰伦的*语言模型*不行。如果您也有*类似症状*😀新版本GluonNLP V0.3提供了最先进的治疗方案，即目前市面上表现最佳的*Cache语言模型*，了解一下。

*<span style="color:orange">啥是语言模型?</span>*说人话的解释就是：让计算机模拟人能听懂、读懂的语言。*<span style="color:orange">那语言模型能干啥？</span>*基本上自然语言处理涉及到的领域都离不开语言模型，例如机器翻译，最近很火的问答系统，聊天机器人；还能有一些比较上档次的人工智能大新闻，比如常听到的人工智能写诗，写歌词啥的，其实背后的大佬就是语言模型。

于是患有类似症状的我，感觉再不学习语言模型就玩完了的我，几个月前上了船，GluonNLP几个小伙伴Sheng Zha ([@szha](https://github.com/szha) [@home](https://www.linkedin.com/in/shengzha))，Xingjian Shi ([@sxjscience](https://github.com/sxjscience) [@home](https://home.cse.ust.hk/~xshiab/))就跟我([@cgraywang](https://github.com/cgraywang) [@home](https://sites.google.com/site/raychenguangwang))造了各种语言模型。

这次新发布的Cache语言模型为啥用过的都说好？因为效果好，能把PPL从之前最优的 *<span style="color:orange">69.74 提升到 54.51</span>*（PPL是公认的语言模型评价指标，越低越好）。本质上Cache语言模型是*记性更好的深度循环神经网络*。类似于水浒武松在跟咱们聊他打虎猛准狠的故事，Cache语言模型能够更好的记住武松刚提到的*老虎*，咱们也会接着跟武松聊*老虎*，而不是*老鼠*（==避免被武松大哥削）。

![](img/laohulaoshu.png){:width="500px"}

于是自从有了GluonNLP语言模型后的杰伦，不再开不了口，而是变身诗人（*LAOSIJI*）：

![](img/qinghuaci.png){:width="500px"}

想要了解更多的语言模型技术细节，请参考[这里](https://gluon-nlp.mxnet.io/scripts/index.html#language-model)和持续关注我们的公众号哦~
