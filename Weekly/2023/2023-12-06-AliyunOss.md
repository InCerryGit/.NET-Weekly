## 国内文章

### .NET 与 OpenEuler 共展翅，昇腾九万里

https://www.cnblogs.com/shanyou/p/17858385.html

本文介绍了openEuler操作系统，它支持多处理器架构，包括X86、ARM等，并计划支持更多芯片架构。openEuler社区正通过场景化的特别兴趣小组（SIG）扩展应用范围，覆盖服务器、云计算、边缘计算到嵌入式等多个场景。作者曾推广欧拉运行.NET Core，因其对ARM的优秀支持获得华为云MVP。同时，文章提到微软.NET Framework的开源历程，.NET Core遵循ECMA标准，现已成为全场景开发平台。中国.NET社区的发展需要优质开源社区支持，openEuler为合作伙伴提供了机会。2023中国.NET开发者峰会将展示科技进步，openEuler作为赞助商参与，邀请更多赞助者加入。

### MAUI Blazor 如何通过url使用本地文件

https://www.cnblogs.com/Yu-Core/p/17855661.html

本文提出了在MAUI Blazor应用中显示本地媒体文件的新方法。文章首先指出了之前方案的不足，如不同平台URL不统一、音视频文件无法播放、Windows上大文件显示限制和iOS/Mac的跨域问题。随后，文章介绍了如何通过修改项目文件和添加处理ContentType的静态类来完善方案。具体包括在.csproj文件中配置基于文件名的多目标，以及创建StaticContentProvider.cs来获取文件ContentType。这样，可以在前端统一使用特定格式的URL来显示或播放本地的图片和视频文件。

### 【译】Visual Studio 2022 - 17.8 的性能改进

https://www.cnblogs.com/MeteorSeed/p/17851304.html

Visual Studio 2022 17.8版本带来了性能提升，包括异步文件打开、改进Razor/Blazor响应性、加速F5、优化C++虚幻引擎智能感知和加快非SDK风格.NET项目构建。这些更新提高了编码效率，特别是在处理大文件和复杂项目时。用户可通过设置特定属性来启用非SDK项目的构建加速。微软鼓励用户反馈，以进一步优化Visual Studio体验。

### .NET中有多少种定时器

https://www.cnblogs.com/czwy/p/17862702.html

本文介绍了.NET中的六种定时器，分为UI定时器和UI无关定时器。UI定时器包括WinForm、WPF和WebForm的定时器，它们在UI线程上执行，简化了线程安全问题。WinForm定时器简单易用，但精度不高；WPF定时器基于Dispatcher，精度不准确，可能延迟；WebForm定时器通过Javascript和服务端回调实现，保证单一异步回调。UI无关定时器适用于后台任务，不涉及UI操作，从.NET 6开始有三种。每种定时器根据应用场景选择，以满足不同的精度和线程安全需求。

### .net下功能强大的HTML解析库HtmlAgilityPack，数据抓取必备

https://www.cnblogs.com/hanbing81868164/p/17856515.html

本文介绍了HtmlAgilityPack，这是一个.NET平台的HTML解析库，能将HTML转换为DOM对象，支持XPath查询并提供API进行HTML操作。安装HtmlAgilityPack需通过Visual Studio的NuGet包管理器。使用时，先加载HTML到HtmlDocument对象，再通过XPath获取DOM节点，可进行节点修改，如改属性或内容。还能将DOM对象转换回HTML文本。文中举例说明了如何获取页面标题、所有图片和链接。

### ASP.NET Core Web API设置响应输出的Json数据格式的两种方式

https://www.cnblogs.com/Can-daydayup/p/17860547.html

本文讲述了在ASP.NET Core Web API中设置Json响应格式的方法。介绍了两种JSON序列化库：内置的System.Text.Json和功能强大的Newtonsoft.Json。文章指出，可以全局配置Json属性名称序列化方式和日期格式，以满足前端需求。通过示例展示了未配置前的API输出Json数据，并介绍了如何使用System.Text.Json进行全局配置，以自定义时间输出格式。

### 一篇学会cron表达式

https://www.cnblogs.com/goodtimeggb/p/17862867.html

本文介绍了Cron表达式，这是一种在Unix系统中用于定时任务的字符串格式，包含六个字段，用空格分隔。通过数字和特殊字符定义执行时间，如"*"代表所有值，"-"定义范围。文中提供了Cron表达式的示例，并介绍了在.NET中使用NCrontab和Quartz库来解析和执行Cron表达式的方法。NCrontab不支持秒级，而Quartz支持，适合需要精确控制的任务。

### 编程技巧 --- VS如何调试.Net源码

https://www.cnblogs.com/pandefu/p/17860440.html

本文讲述了在VS2022中调试.Net源码的方法。首先，需要在"工具"-"选项"-"文本编辑器"-"C#"-"高级"-"转到定义"中勾选所有选项以查看源码。其次，要启用源代码单步执行，包括取消选择"启用仅我的代码"，选择"启用源链接支持"，并在"符号"下选择"Microsoft 符号服务器"。配置后，首次启动应用时会有符号加载时间。通过这些设置，可以在"调用堆栈"窗口中下载和加载符号进行源码调试。文章还建议通过实践提升调试技巧，以便更好地理解框架工作原理和提高解决BUG的效率。

### 小心C#中的只读结构体成员

https://www.cnblogs.com/broadm/p/17862169.html

本文讲述了C#中结构体的只读属性对代码行为的影响。通过示例展示了将结构体成员设为只读后，尝试修改其字段值时，编译器不报错但修改不成功，因为只读机制会导致字段值在堆栈上拷贝。这种隐蔽的行为可能引发BUG，如自旋锁示例中的计数错误。文章建议在结构体或字段需要只读时，使用readonly关键字直接修饰，以避免潜在问题。

### C# 泛型编译特性对性能的影响

https://www.cnblogs.com/tansm/p/CSharp-Generic-Performance.html

本文探讨了C#中泛型的编译行为，特别是结构和类作为泛型参数时对性能的不同影响。结构作为值类型，存储在栈上，泛型参数为结构时编译器生成特定实现，提升性能，减少装箱拆箱。类作为引用类型，存储在堆上，泛型参数为类时编译器生成通用实现，可能导致性能下降。性能测试显示结构类型泛型参数性能较高，类类型泛型参数性能略低。

### 中间件IIS监控指标、配置和Windbg调试分析

https://www.cnblogs.com/tianqing/p/17864122.html

本文介绍了中间件IIS的监控指标和配置最佳实践。关键性能计数器包括Web服务的当前连接数、每秒请求数等，ASP.NET的请求执行时间、请求排队数等，以及CPU和内存的使用情况。最佳实践建议定期回收应用程序池，合理设置工作进程数，启用输出和静态内容缓存，以及压缩以提升性能。监控和日志记录需适度，安全设置要定期更新。IIS请求队列是处理前临时存放请求的地方，监控请求队列的性能计数器有助于优化队列设置，如增加工作进程数、优化代码和调整队列长度，以减少等待时间，确保请求快速处理。通过这些措施，可以优化IIS服务器性能。

### 设计模式（十五）解释器

https://www.cnblogs.com/WinterSir/p/17506255.html

本文介绍了解释器模式，这是一种用于构建语言解释器的设计模式，包含抽象表达式、终结符表达式、非终结符表达式和环境类四个角色。通过这些角色，可以解释和执行用户根据特定文法编写的代码。文中以X公司开发的字符界面格式化指令为例，展示了如何使用解释器模式处理指令并输出格式化内容。环境类存储指令，抽象节点类负责解释语句和执行命令。

### C#简化工作之实现网页爬虫获取数据

https://www.cnblogs.com/mingupupu/p/17860491.html

本文介绍了使用C#编写网页爬虫来获取网站上的气象信息。网站共有67页气象数据，手动复制粘贴效率低下。通过构建每一页的URL并发送GET请求，成功抓取并存储了4万多条数据到数据库。

## 主题

### C# 日历 | 降临节日历 2023 - Qiita
https://qiita.com/advent-calendar/2023/csharplang

2023 年 C# 降临节日历目前正在进行中。

### NUnit 4.0.1 | 框架版本 | NUnit 文档
https://docs.nunit.org/articles/nunit/release-notes/framework.html#nunit-401---december-2-2023

NUnit 4.0.0/4.0.1 已发布。

它包括许多改进和修复，例如对 TestCaseSource 的异步支持、对 .NET 6 目标的支持和测试取消 (CancelAfter)，以及删除 .NET Framework 3.5、4.0、4.5 和 .NET Core 2.1 等目标.ing.

### 宣布 ML.NET 3.0 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-ml-net-3-0/

ML.NET 3.0已发布。

此版本包括对象检测 API、问答 (QA) 和命名实体提取 (NER)、Intel oneDAL 硬件训练加速、AutoML 改进、DataFrame 更新、Tensor 原语集成等。

### 发布 v2.5.140 · MessagePack-CSharp/MessagePack-CSharp
https://github.com/MessagePack-CSharp/MessagePack-CSharp/releases/tag/v2.5.140

MessagePack v2.5.140 已发布。

此版本修复了 Mono 运行时中的错误。

### 2023 年的开发者生态系统：C# 的主要趋势 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/11/30/the-developer-ecosystem-in-2023-key-trends-for-csharp/

JetBrains 的 C# 开发者生态系统趋势研究。

ASP.NET Core使用的功能、C#版本、开发目标、IDE/编辑器、插件的使用等

### ReSharper 2023.3 候选版本现已推出 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/11/29/the-resharper-2023-3-rc/

ReSharper 2023.3 候选版本已发布。

AI 助手增强功能、C# 12 支持、实体框架探索和图表绘制、UI 改进、改进的 Razor 格式化引擎、用于单元测试的 AI 生成、新语法和拼写检查器等等。

### Rider 2023.3 候选版本现已推出 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/11/29/the-rider-2023-3-rc/

Rider 2023.3 候选版本已发布。

包括各种新功能，例如 AI Assistant 增强功能、对 .NET 8 SDK（包括 C# 12 和 F# 8）的支持、改进的多项目启动、类型依赖关系图、预测调试、单元测试的 AI 生成等等。

### 六项工作：发布 ImageSharp 3.1.0
https://sixlabors.com/posts/announcing-imagesharp-310/

ImageSharp 3.1.0 已发布。

此版本包括对动画 WebP 和 PNG 的支持、对 Quite Ok (Qoi) 的支持、改进的解码器可靠性以及各种性能改进。


## 文章、幻灯片等
### 最少使用 Blazor Web App 的 OAuth 身份验证 (ASP.NET Core 8.0)
https://zenn.dev/tetr4lab/articles/1946ec08aec508

了解如何在 .NET 8 中的 Blazor Web App 中实现 Google OAuth 身份验证。

### 从 BitmapSource 转换为 Bitmap 的最佳实践
https://zenn.dev/nuits_jp/articles/2023-12-03-convert-bitmapsource-to-bitmap

介绍一个在WPF中从BitmapSource转换为Bitmap的好方法。

### [无需 Mac] 轻松调试 .NET MAUI iOS 应用程序并将其部署到 iPhone 的步骤 - Qiita
https://qiita.com/kami_teru/items/b2a6bd77f7c836ae3d1e

如何在实际设备（例如 iPhone）上从仅在 Windows 上的 Visual Studio 调试和执行 .NET MAUI iOS 应用程序。

### 如何使用 .Net8 Blazor WASM 创建 ASP.Net Core 托管配置
https://zenn.dev/vigilanteyu/articles/d7a47dff63e8e2

如何在 .NET 8 中实现与 Blazor WebAssembly 的 ASP.NET Core Hosted 等效的配置，该配置一直存在于 .NET 7 中。

### Visual Basic 2023 回顾 - Qiita
https://qiita.com/yaju/items/97c7d6ae94a303bdbb5b

今年 Visual Basic 主题的综述，包括 Visual Basic .NET。

### 使用 IndexedDB 在 .NET MAUI Blazor 混合应用程序中存储本地数据 - 第 1 部分

https://dev.to/icebeam7/storing-local-data-in-a-net-maui-blazor-hybrid-app-using-indexeddb-part-1-3hn2

了解如何使用 IndexedDB 在 .NET MAUI Blazor 混合应用中存储本地数据。

### 我评估了 ImageMagick、ImageSharp 和 System.Drawing 的性能
https://zenn.dev/nuits_jp/articles/2023-12-01-imagemagic-imagesharp-benchmarks

图像处理库 Magick.NET (ImageMagick)、ImageSharp 和 System.Drawing 的性能比较。
本文比较了 .NET Framework 和 .NET 8 之间的解码、裁剪和二值化处理。

### .NET 8.0 如何将 AIS.NET 性能提升 27% | endjin
https://endjin.com/blog/2023/11/how-dotnet-8-boosted-ais-dotnet-performance-by-27-percent-for-free

了解在 .NET 8 中运行 AIS.NET（一个用于分析 AIS 解码器（AIS 是船舶无线电消息）的库）时的显着性能改进。

### Visual Studio 17.8 中我最喜欢的功能 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/my-favorite-features-in-visual-studio-17-8/

介绍 Mads Kristensen 推荐的 Visual Studio 2022 版本 17.8 的新功能。

本文重点介绍了保留大小写的搜索和替换以及丰富的拉取请求体验等功能。

### [LogProperties] 和新的遥测日志源生成器背后
https://andrewlock.net/behind-logproperties-and-the-new-telemetry-logging-source-generator/

.NET 8 提供的 Microsoft.Extensions.Telemetry.Abstractions 中包含的“LogProperties”属性的说明，该属性将属性值保留在日志中。

### [All] LINQ，这种情况下会发生什么？ [空数组怎么办？ ] - 奇塔
https://qiita.com/RyotaMurohoshi/items/bf45f4e7d52e6aad8ef7

C# 降临节日历 2023 年第 1 天文章。解释极端情况，例如在空数组上执行 LINQ All 的结果以及存在绑定元素时 OrderBy 的结果。

### 在 VSCode 2023 中的 C# 中更改块 {} 之前和之后的换行符 | Aqua Ware Tweet 博客
https://aquasoftware.net/blog/?p=1975

C# 2023 年降临节日历第 2 天文章。如何在 C# 代码格式设置中设置大括号之前和之后的开口。

### C# 标记在跨平台开发中的兴起
https://platform.uno/blog/the-rise-of-c-markup-for-cross-platform-development/

C#标记介绍，是Uno Platform的UI描述方法在C#中。

### C# 开发套件热重载
https://www.poppastring.com/blog/hot-reload-for-c-dev-kit

如何在 Visual Studio Code 的扩展 C# 开发工具包中启用实验性功能热重载。

### 使用 OmniSharp-Vim 显示代码风格分析结果，例如 IDE0001 - Qiita
https://qiita.com/lx-sasabo/items/4ceb7be5e2721e4e52f8

如何使用 OmniSharp-Vim 显示来自分析器等的代码分析结果。

### 如何在 .NET 8 中的 Blazor 中将 JavaScript 与静态服务器渲染 (SSR) 结合使用
https://zenn.dev/microsoft/articles/aspnetcore-blazor-dotnet8-jsinterop

了解如何在 .NET 8 中将静态服务器渲染 (SSR) 与 Blazor 结合使用时实现和运行自定义 JavaScript。

### .NET 的 HttpClient Timeout 指的是什么超时？ | @jsakamoto
https://devadjust.exblog.jp/29756261/

解释可以在 HttpClient 上设置的超时实际上如何工作。

### 将最小的 ASP.NET Web 服务器嵌入到桌面应用程序中
https://weblog.west-wind.com/posts/2023/Nov/27/Embed-a-minimal-ASPNET-Web-Server-into-a-Desktop-Application

如何在桌面应用程序中包含最小的 ASP.NET Core 服务器。

### [C#] 尝试 FakeTimeProvider 和 FakeLogger - TekuMemo
https://aneuf.hatenablog.com/entry/2023/11/27/210000

引入“FakeTimeProvider”，它是 .NET 8 中引入的“ITimeProvider”的伪造实现，以及“FakeLogger”，它是新引入的“ILogger”的伪造实现。

### [C#] 集合表达式：尝试使用具有唯一类型的集合表达式（CollectionBuilder 属性） - TekuMemo
https://aneuf.hatenablog.com/entry/2023/11/24/210000

关于“CollectionBuilderAttribute”，它用自己的类型实现 C# 12 集合表达式，以及如何使用它来实现它。

### [C#] 什么是依赖注入？ - Annulus Games
https://annulusgames.com/blog/dependency-injection/

关于依赖注入的说明。服务定位器及其问题、使用 Microsoft.Extensions.DependencyInjection 作为 DI 容器的各种示例、除 M.E.DI 之外的 .NET/Unity DI 容器的介绍等。

## 库、存储库、工具等。

### thomhurst/ModularPipelines：用 C# 编写管道！
https://github.com/thomhurst/ModularPipelines

一个框架，它组合模块来创建用于某种处理/工作的管道。

- [使用 ModularPipelines 在 C# 中编写管道](https://medium.com/@thomhurst/write-your-pipelines-in-c-using-modularpipelines-226de1a24bb7)


### nenoNaninu/AspNetCore.SignalR.OpenTelemetry：这是一个检测库，用于检测 ASP.NET Core SignalR 并收集有关 SignalR 集线器方法调用的指标和跟踪。
https://github.com/nenoNaninu/AspNetCore.SignalR.OpenTelemetry

用于将 SignalR 指标流式传输到 OpenTelemtry 的库。

https://x.com/nenomake/status/1730229080455303389?s=12


### 调试输出过滤器 - Visual Studio Marketplace
https://marketplace.visualstudio.com/items?itemName=GrantDavies.NiahTextFilter2022

Visual Studio 扩展允许您历史记录和过滤调试输出。

## 网站、文档等
### 推文

故事是我能够使用 Avalonia XPF（Avalonia 的跨平台 WPF 兼容性套件）在浏览器中运行 PerfView。

https://twitter.com/AvaloniaUI/status/1729403695392059887

![image-20231212220751740](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231212220751740.png)

---

定义空类或接口时，使用“;”声明它而不使用主体会很方便。

https://x.com/sergiopedri/status/1730233715345826173?s=12

![image-20231212220825932](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231212220825932.png)

---


关于在分析时启动应用程序时暂停分析的功能。

https://x.com/vs_debugger/status/1730647909279166974?s=12

![image-20231212220904913](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231212220904913.png)

---


一个关于使用 Ghidra 脚本使本机 AOT 字符串搜索成为可能的故事。

https://x.com/washi_dev/status/1725270583011688726?s=12

![image-20231212220937562](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231212220937562.png)

---


PolySharp 现已提供适用于 C# 12 的新 polyfill。

https://x.com/sergiopedri/status/1729878697824698514?s=12

![image-20231212221030184](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231212221030184.png)

---

`[InlineArray]` 的最大值为 1MB

https://x.com/hypeartistmusic/status/1728123597968011688?s=12&t=ggvrrZ7oLogHyNoIGNgjbw

![image-20231212221115138](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231212221115138.png)

![Image](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/F_uG_wEWsAAsNC8.jpeg)

![Image](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/F_uHOazWUAAVjyX.jpeg)

## 深入探索
### [API 提案]：引入新的内存缓存库 · 问题 #4766 · dotnet/extensions
https://github.com/dotnet/extensions/issues/4766

提议引入一种名为 RCache 的新型内存高效内存缓存。

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

![image-20230703203249615](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230703203249615.png)