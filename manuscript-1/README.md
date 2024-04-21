# 成为一名开源贡献者，从SeaTunnel开始！

## 个人介绍

大家好，我是闫成雨，一名独立开发者。

Github ID: CheneyYin

## 为社区做了哪些贡献

- 增强了Spark引擎和Flink引擎对SeaTunnel数据类型的支持。
- 修复了一些Spark引擎转换层的BUG。
- 完善了Assert连接器支持的数据类型。
- 修复了一些CI相关的BUG。
- 完善了一些文档。

> 贡献记录：https://github.com/apache/seatunnel/pulls?q=is%3Apr+author%3ACheneyYin+is%3Aclosed

## 初识

在2022年～2023年之间，我一直在摸索如何开发一款类似StreamSet和NiFi的可视化数据集成软件，在2023年3月左右，我完成了一个简陋的可视化数据集成软件Metal（已搬运到我的Github仓库）。虽然Metal简陋，但是也达到了验证设计思路、技术栈的目的。

直到我读到《The Evolution of Architecture from ETL to EtLT》这篇发布在devops.dev社区的文章，我了解到许多关于数据集成的新观点，例如小t的意义，使用通用计算引擎的缺陷，数据集成执行引擎存在的价值等等。还有就是Apache SeaTunnel的存在，它建立在这些新的理念之上。在初次体验SeaTunnel之后，我果断放弃了之前思路，转而使用SeaTunnel。

## 提交第一个PR

在一次压测时，我发现Spark抛出OOM异常，然后复现该问题，最后调试定位了原因。Spark转换层的`TransformerProcessor`在内存暂存了输出结果，数据量过大时，造成堆内存不足。

问题分析清楚并找到解决办法后，提交了我在SeaTunnel社区的第一个Issue(#4502)，在Issue中我解释了现象和原因，并且提供了我的解决思路。紧接着，提交了我在SeaTunnel社区的第一个PR(#4503)。

我的第一个PR从提交到合并只用了4天，社区的反馈效率已经相当高了。但对个人而言，很期待，很漫长，尤其在CI环境异常导致测试无法通过后。

## 社区留给我的印象

我对Apache SeaTunnel社区的第一印象是火热、友好。社区对Github Issue和Pull Request反馈也很及时。同时社区对新的贡献者很友好、有耐心，使新的贡献者能方便快捷地参与进来。

