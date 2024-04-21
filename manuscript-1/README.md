# 从SeaTunnel开始，成为一名开源贡献者！

## 个人介绍

大家好，我是闫成雨，目前是一名独立开发者。工作内容和兴趣集中于数据开发、机器学习、资源调度算法、分布式系统。

> GitHub ID: CheneyYin
>
> 个人主页：https://cheneyyin.github.io/

## 为社区做了哪些贡献

- 加强了Spark引擎和Flink引擎对SeaTunnel数据类型的支持。
- 修复了一些Spark引擎转换层的BUG。
- 完善了Assert连接器支持的数据类型。
- 修复了一些CI相关的BUG。
- 完善了一些文档。

> 贡献记录：https://github.com/apache/seatunnel/pulls?q=is%3Apr+author%3ACheneyYin+is%3Aclosed

## 初识

在2022年到2023年之间，我一直在摸索如何开发一款类似StreamSet和NiFi的可视化数据集成软件。到了2023年3月左右，我完成了一个简陋的可视化数据集成软件Metal（已搬运到我的GitHub仓库）。虽然Metal简陋，但也达到了验证设计思路、技术栈的目的。

直到我读到《The Evolution of Architecture from ETL to EtLT》这篇发布在devops.dev社区的文章，我了解到许多关于数据集成的新观点，例如小t的意义，使用通用计算引擎的缺陷，数据集成执行引擎存在的价值等等。还有就是首次接触到Apache SeaTunnel，它建立在这些新的理念之上。在初次体验SeaTunnel之后，我果断放弃了之前的思路，转而使用SeaTunnel。

## 提交第一个PR

在一次压测时，我发现Spark抛出OOM异常。首先我复现该问题，最后调试定位了原因。Spark转换层的`TransformerProcessor`在内存暂存了输出结果，数据量过大时，造成堆内存不足。

问题分析清楚并找到解决办法后，提交了我在SeaTunnel社区的第一个Issue(#4502)，在Issue中我解释了现象和原因，并且提供了我的解决思路。紧接着，提交了我在SeaTunnel社区的第一个PR(#4503)。

我的第一个PR从提交到合并只用了4天，可见社区的反馈效率相当高。但这个过程对个人而言，很期待，很漫长，尤其在CI环境异常导致测试无法通过后。不过社区大佬及时提供了帮助了，最终合并了PR。

## 社区留给我的印象

我对Apache SeaTunnel社区的第一印象是热情、活跃。社区对Issue和Pull Request反馈很快。同时社区对新的贡献者很友好、有耐心，让新的贡献者能方便快捷地参与进来。

## 对SeaTunnel的期望

- 社区更加壮大。
- 用户越来越多。
- 用户体验越来越好。
- SeaTunnel的稳定性有新的突破。
- 文档更加详实完善。
