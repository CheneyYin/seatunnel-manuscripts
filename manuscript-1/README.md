# 成为一名开源贡献者，从SeaTunnel开始！

## 个人介绍

大家好，我是闫成雨，目前是一名独立开发者。专注于数据开发、机器学习、资源调度算法和分布式系统。

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

在2022年到2023年期间，我一直在尝试开发一款类似于StreamSet和NiFi的可视化数据集成软件。直到2023年3月左右，我完成了一个简陋的可视化数据集成软件Metal，并将其迁移到了我的GitHub仓库。尽管Metal功能简单，但它成功验证了设计思路和技术栈的可行性。

直到我阅读了发布在devops.dev社区的文章《The Evolution of Architecture from ETL to EtLT》，我才了解到许多关于数据集成的新观点，如小t的概念、使用通用计算引擎的局限性以及数据集成执行引擎的价值等等。同时，这也是我首次接触到Apache SeaTunnel，它是建立在这些新理念之上的。在第一次尝试SeaTunnel后，我毅然放弃了之前的方向，转而选择了SeaTunnel。

## 提交第一个PR


在一次压测中，我注意到Spark引擎抛出了OOM（Out Of Memory）异常。我首先复现了这个问题，然后进行了调试并定位了原因。发现是Spark转换层的`TransformerProcessor`在内存中临时存储了输出结果，导致处理大数据量时堆内存不足。

在对问题进行深入分析并找到解决方案后，我向SeaTunnel社区提交了我的第一个Issue(#4502)。在这个Issue中，我解释了问题的现象和原因，并提出了解决方案。随后，我提交了我的第一个PR(#4503)。

我的第一个PR从提交到合并仅用了4天，这显示了社区高效的反馈速度。但对我个人来说，这个过程充满了期待和漫长，特别是在CI环境出现异常导致测试无法通过时。不过，社区的资深成员及时提供了帮助，最终成功合并了PR。

## 持续参与

在过去的一年里，我一直积极参与社区活动，阅读技术大咖们的分享内容，关注并回复社区的Issue，同时持续跟踪Pull Request列表。

另外，我也为社区做出了一些代码贡献。例如，为Spark引擎添加了对SeaTunnel的Time类型的支持(#5188)，为Flink引擎增加了可配置precision和scale的Decimal类型支持(#5419)，还增强了Hocon风格的泛型声明(#6187)，以及完善了Assert连接器覆盖全部数据类型(#6275)等。这些Pull Request大多旨在改善用户的使用体验。

## 社区留给我的印象

我对Apache SeaTunnel社区的第一印象是热情而活跃。社区对Issue和Pull Request的反馈速度很快，同时也对新的贡献者非常友好和耐心，使得新贡献者能够轻松快速地参与进来。

## 对SeaTunnel未来的期望

- 希望社区能够进一步壮大，吸引更多的开发者加入，共同推动SeaTunnel的发展。
- 希望SeaTunnel的用户群体能够不断增长，让更多人受益于其强大的功能和便捷的数据集成解决方案。
- 希望SeaTunnel的用户体验能够持续改善。
- 希望SeaTunnel能够在稳定性方面取得新的突破。
- 希望SeaTunnel的文档能够更加详实完善，提供全面而清晰的使用指南和技术文档，方便用户快速上手和解决问题。
