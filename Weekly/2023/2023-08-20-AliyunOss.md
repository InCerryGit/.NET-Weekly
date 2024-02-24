## 国内主题

### 抓的是周树人，与我鲁迅有什么关系？      

https://www.cnblogs.com/JulianHuang/p/17642511.html

- **问题**：作者看到了一个关于Dictionary.Clear和new Dictionary的问题，想要探究为什么在foreach字典的过程中，这两种操作不会报错。
- **分析**：作者分析了C#字典的源码，发现foreach字典会产生一个迭代器，它有一个指向原字典的字段。如果在外部重新new字典，或者清空字典，都不会影响这个字段，所以不会触发版本检查的异常。

### DateTime 相关的操作汇总【C# 基础】

https://www.cnblogs.com/hnzhengfy/p/DatetimeInCS.html

在日常开发中，日期值当然是不可或缺的，能够清晰的在脑海中梳理出最快捷的实现也非常重要，那么今天就来汇总一下。

### 使用C#创建安装Windows服务程序(干货)

https://www.cnblogs.com/kimiliucn/p/17637533.html

最近在公司要求使用Windows服务作为消息队列的消费者，所以自行研究了一下C#中Windows服务如何创建以及如何使用，以及部署的方式。我是西瓜程序猿，此篇记录一下供大家参考学习。

### 长文本拆分

https://www.cnblogs.com/xbotter/p/17637416.html

> 1. 企业微信消息长度限制为2048个字节，字符长度不等于字节长度
> 2. 使用字节拆分，会导致中文字符被截断
> 3. 使用文本+字节拆分，无法处理emoji表情
> 4. 使用unicode字符拆分，即可解决以上问题

先前在做企业微信的应用接入ChatGPT时遇到一个问题，就是企业微信的消息长度限制为2048个字节，所以遇到超长文本的时候需要拆分成多条消息发送。

###  [MAUI]在.NET MAUI中实现可拖拽排序列表

https://www.cnblogs.com/jevonsflash/p/17631233.html

.NET MAUI 中提供了拖放(drag-drop)手势识别器，允许用户通过拖动手势来移动控件。在这篇文章中，我们将学习如何使用拖放手势识别器来实现可拖拽排序列表。在本例中，列表中显示不同大小的磁贴（Tile）并且可以拖拽排序。

### C# 如何将程序加密隐藏？

https://www.cnblogs.com/hejiale010426/p/17631103.html

下面将介绍如何通过`LiteDB`将自己的程序进行加密，首先介绍一下`LiteDB`。

### WPF如何构建MVVM+模块化的桌面应用

https://www.cnblogs.com/fengjq/p/17630386.html

模块化是一种分治思想，不仅可以分离复杂的业务逻辑，还可以进行不同任务的分工。模块与模块之间相互独立，从而构建一种松耦合的应用程序，便于开发和维护。

### Blazor前后端框架Known-V1.2.12

https://www.cnblogs.com/known/p/17630332.html

Known是基于C#和Blazor开发的前后端分离快速开发框架，开箱即用，跨平台，一处代码，多处运行。

- Gitee： https://gitee.com/known/Known
- Github：https://github.com/known/Known

- 基于C#和Blazor实现的快速开发框架，前后端分离，开箱即用。
- 跨平台，单页应用，混合桌面应用，Web和桌面共享一处代码。
- 包含模块、字典、组织、角色、用户、日志、消息、工作流、定时任务等功能。
- 代码简洁、易扩展，让开发更简单、更快捷！

### .NET Core多线 (5) 常见性能问题

https://www.cnblogs.com/edisonchou/p/dotnet_multithread_learning_notes_chap5.html

去年换工作时系统复习了一下.NET Core多线程相关专题，学习了一线码农老哥的《.NET 5多线程编程实战》课程，我将复习的知识进行了总结形成本专题。

本篇，我们来继续复习一下多线程性能问题的相关知识点，预计阅读时间10分钟。

首先，我们可以明确一下，多线程场景下的常见问题一般为：**高CPU占用**。

## 主题

### 【英文】宣布 .NET 8 预览版 7 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-preview-7/

### 【英文】宣布推出 NuGet 6.7 – 确保您的安全 - NuGet 博客
https://devblogs.microsoft.com/nuget/announcing-nuget-6-7-keeping-you-secure/

### 【英文】.NET Framework 2023 年 8 月安全和质量汇总更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-framework-august-2023-security-and-quality-rollup-updates/

### 【英文】Visual Studio 2022 – 17.7 现已推出 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-7-now-available/

### 【英文】在 .NET 8 Preview 7 中宣布 .NET MAUI：键盘加速器 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-maui-in-dotnet-8-preview-7/

### 【英文】.NET 8 Preview 7 中的 ASP.NET Core 更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/asp-net-core-updates-in-dotnet-8-preview-7/

### 【英文】.NET 2023 年 8 月更新 – .NET 7.0.10、.NET 6.0.21 - .NET 博客
https://devblogs.microsoft.com/dotnet/august-2023-updates/

### 【英文】Visual Studio 2022 17.8 预览版 1 已经到来！ - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-8-preview-1-has-arrived/

### 【英文】SponsorLink 的隐私问题，从版本 4.20 开始 · 问题 #1372 · moq/moq
https://github.com/moq/moq/issues/1372

- [SponsorLink：反馈和前进](https://www.cazzulino.com/sponsorlink-feedback.html)


## 文章、幻灯片等
### 【英文】从 Moq 迁移到 NSubstitute 的备忘单
https://timdeschryver.dev/blog/a-cheat-sheet-to-migrate-from-moq-to-nsubstitute#method-invoked-with-any-arguments

### 【日文】将CsWin32分离为其他项目
https://zenn.dev/shinta0806/articles/cswin32-separation

### 【英文】结构化 ASP.NET 本地化
https://dev.to/giannoudis/structured-aspnet-localization-35bo

### 【英文】.NET 中执行上下文的隐藏工作
https://medium.com/net-under-the-hood/hidden-workings-of-execution-context-in-net-43b491726c65

### 【英文】面向普通受众的多分支图 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/multi-branch-graph-available-for-general-audiences/

### 【英文】使用 NBomber 对 C# 进行 HTTP API 负载测试
https://medium.com/@kostash23lena/load-testing-http-api-on-c-with-nbomber-96939511bdab

### 【英文】如何使用 JetBrains Rider 调试 Docker 和 Docker Compose 解决方案 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/08/16/debugging-docker-and-docker-compose-solutions-with-jetbrains-rider/

### 【日文】在VScode的C#扩展中，继续使用omnisharp-Qiita
https://qiita.com/skitoy4321/items/c6b0873a37fe649f9ca6

### 【C#】使用Spanbyte一点点进行散列值计算（IncrementalHash） - Qiita
https://qiita.com/mitsu_at3/items/438b4c4252947b467ef2

### 【英文】键控服务依赖注入容器支持：探索 .NET 8 预览版 - 第 6 部分
https://andrewlock.net/exploring-the-dotnet-8-preview-keyed-services-dependency-injection-support/

### 【英文】Visual Studio 17.7 中我最喜欢的功能 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/my-favorite-features-in-visual-studio-17-7/

### 【英文】Visual Studio 2022 – 17.7 性能增强 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-7-performance-enhancements/

### 【日文】C# 将自定义记录器合并到通用主机的 DI 中 - Qiita
https://qiita.com/mxProject/items/41f75c057c855c49efd0

### 【日文】如何使用 .NET 8 执行 Blazor 服务器（Blazor 服务器模板消失）
https://zenn.dev/microsoft/articles/blazor-server-on-net8-pre6

### 【英文】在 Kubernetes 上收集 .NET Core 的内存转储
https://cezarypiatek.github.io/post/memory-dump-on-kubernetes/

### 【英文】.NET 迁移的故事 - 简介
https://www.jimmybogard.com/tales-from-the-net-migration-trenches/

### 【英文】介绍 .NET 8 中的新 IHostedLifecycleService 接口 - Steve Gordon - 与 Steve 一起编码
https://www.stevejgordon.co.uk/introducing-the-new-ihostedlifecycleservice-interface-in-dotnet-8

### 【英文】.NET 8 拦截器
https://khalidabuhakmeh.com/dotnet-8-interceptors

### 【日文】[C# 8.0] 通过指定一系列索引器而不是子字符串来提取字符串 - Qiita
https://qiita.com/YouKnow/items/93b4b978ecb113616fae

### 【英文】C# 是否总是具有字符串连接和插值的装箱…
https://pvs-studio.com/en/blog/posts/csharp/1060/

### 【英文】让我们共同创造！您的声音很重要 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/lets-co-create-your-voice-matters/

### 【英文】如何从 Moq 迁移到 NSubstitute
https://itnext.io/how-to-migrate-from-moq-to-nsubstitute-cdb6a80404d

### 【英文】抑制GCTransition
https://minidump.net/suppressgctransition-b9a8a774edbd

### 【日文】通过引用`ImmutableArray<T>`内部数组来加速
https://zenn.dev/benutomo/articles/54083312afca95

### 【英文】Visual Studio 2022 v17.8 预览新的 IntelliTest - Visual Studio 杂志
https://visualstudiomagazine.com/articles/2023/08/14/intellitest-preview.aspx?m=1

### 【日文】从 Moq 迁移到 NSubstitute
https://zenn.dev/masakura/articles/9b97948a11b40d

### 【日文】如何使用 .NET 8 执行 Blazor 服务器（Blazor 服务器模板消失）
https://zenn.dev/microsoft/articles/blazor-server-on-net8-pre6?redirected=1

### 【日文】System.Text.Json 不支持带换行符的 Base64 字符串
https://zenn.dev/shimat/articles/3d319d50b3f0c3

### 【英文】.NET 月刊 | 2023 年 8 月 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/08/07/net-annotated-monthly-august-2023/

### 【英文】.NET 中的 Polyfills 可以简化多目标 - Gérald Barré
https://www.meziantou.net/polyfills-in-dotnet-to-ease-multi-targeting.htm

### 【英文】如何对不同的 .NET 版本进行基准测试
https://steven-giesel.com/blogPost/59cfb6f8-8b87-4707-a99e-e372541b696a

### 【英文】.NET .gcdump 内部结构
https://chnasarre.medium.com/net-gcdump-internals-fcce5d327be7

### 【日文】[C#] 完全理解结构 - Annulus Games
https://annulusgames.com/blog/understanding-struct/

## 库、存储库、工具等

### Giannoudis/TimePeriodLibrary：广泛的时间段计算和单独的日历周期。
https://github.com/Giannoudis/TimePeriodLibrary

- [.NET 时间段库](https://www.codeproject.com/Articles/168662/Time-Period-Library-for-NET)

### PowerRule / PowerRule GitLab

https://gitlab.com/power-rule/power-rule

- [使用PowerRule编写复杂规则](https://zenn.dev/masakura/articles/9253061846d90c)

### le-nn/memento：Blazor/.NET 的简单客户端状态管理容器包括重做/撤消和 ReduxDevTools 支持。
https://github.com/le-nn/memento

- [即使在 Blazor 中我也尝试使用 ReduxDevTools 进行调试](https://zenn.dev/remrem/articles/0768982b3cdc92)
- [我制作了一个在 Blazor 组件之间共享状态的状态管理库](https://zenn.dev/remrem/articles/32ee38e79f4cf0)


## 网站、文档等
### ASP.NET Core 实战，第三版现已出版
https://andrewlock.net/asp-dotnet-core-in-action-third-edition-is-now-in-print/

## 版权声明

* 国内板块由 InCerry 进行整理 : https://github.com/InCerryGit/WeekRef.NET
* 其余内容来自 Myuki WeekRef，由InCerry翻译（已获得授权） : https://github.com/mayuki/WeekRef.NET

**由于笔者没有那么多时间对国内的一些文章进行整理，欢迎大家为《.NET周刊-国内文章》板块进行贡献，需要推广自己的文章或者框架、开源项目可以下方的项目地址提交Issue或者在我的微信公众号私信。**

格式如下：

* 10~50字左右的标题
* 对应文章或项目网址访问链接
* 200字以内的简介，如果太长会影响阅读体验

https://github.com/InCerryGit/.NET-Weekly

## .NET性能优化交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET性能优化经验的群组，主题包括但不限于：

* 如何找到.NET性能瓶颈，如使用APM、dotnet tools等工具
* .NET框架底层原理的实现，如垃圾回收器、JIT等等
* 如何编写高性能的.NET代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET性能问题和宝贵的性能分析优化经验。**目前一群已满，现在开放二群。**

如果提示已经达到200人，可以加我微信，我拉你进群: **ls1075**

另外也创建了**QQ群**，群号: 687779078，欢迎大家加入。 

## 抽奖送书活动预热！！！

感谢大家对我公众号的支持与陪伴！为庆祝公众号一周年，抽奖送出一些书籍，请大家关注公众号后续推文！

![image-20230703203249615](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230703203249615.png)