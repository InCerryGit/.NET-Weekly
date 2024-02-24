## 国内文章

### 2023成都.NET线下技术沙龙圆满结束

https://www.cnblogs.com/edisonchou/p/2023_chengdu_dotnet_club_activity_review.html

2023年4月15日周六，由MASA技术团队和成都.NET俱乐部共同主办的2023年成都.NET线下技术沙龙活动在成都市世纪城新会展中心知域空间举行，共计报名人数90多人，**实际到场60多人**，13:30~18:00四个半小时的现场交流氛围极好，到场的童鞋也满载而归，我们看到了成都.NET社区小伙伴的**激情**，也让我们更加相信.NET社区的**明天会更好**！

### C#中使用CAS实现无锁算法

https://www.cnblogs.com/eventhorizon/p/17338890.html

本文主要介绍了C#中使用CAS实现无锁算法的方法和原理。文章首先解释了CAS的基本概念和优势，然后介绍了C#中使用Interlocked类的CompareExchange方法来实现CAS操作的方式，最后给出了两个算法示例：计数器和队列，分别展示了如何使用CAS操作来实现线程安全的数据结构和算法。

### .NET无侵入自动化探针原理和主流实现

https://www.cnblogs.com/InCerry/p/about-dotnet-auto-apm-instru-impl.html

本文介绍了.NET无侵入自动化探针的原理和主流实现，主要包括以下内容：

- APM探针的概念和作用，以及如何采集平台相关指标和组件相关指标。
- .NET方法注入的方式和原理，包括静态注入和动态注入，以及各自的优缺点。
- 基于CLR Profile API实现APM探针的原理，包括Profiler注册、JIT编译拦截、代码修改插桩、上下文传播和数据收集等步骤。
- CLR Profile API提供的事件和接口，以及如何使用ILRewriter工具类进行IL代码的分析和修改。
- RequestReJIT方法的介绍和优势，以及如何使用它实现动态地重新编译方法。

本文旨在帮助开发者深入理解.NET无侵入自动化探针的技术细节和实现方式，为.NET应用程序的性能监测和优化提供参考。

### ASP.NET Core Web API 流式返回，逐字显示

https://www.cnblogs.com/cplemom/p/17269789.html

本文主要介绍了ASP.NET Core Web API 流式返回的方法和效果。文章分别用C#和js代码示例展示了如何使用流式响应返回文本和图片内容，以及如何在客户端实时捕获返回的信息。文章还简要介绍了Websocket、SSE和长轮询等网页和服务端通信的技术。

### 使用ServiceSelf解决.NET应用程序做服务的难题

https://www.cnblogs.com/kewei/p/17346228.html

本文主要介绍了ServiceSelf项目，它是一个为.NET泛型主机的应用程序提供自安装为服务进程的能力的工具，支持windows和linux平台。文章分别介绍了ServiceSelf的功能、自我服务安装、自我服务卸载和自我服务日志监听等特点，并给出了相关的代码示例。文章还对比了其他的服务生命周期包和日志提供者，并指出了ServiceSelf的优势和精炼的api设计。

### 记一次 .NET 某外贸ERP 内存暴涨分析

https://www.cnblogs.com/huangxincheng/p/17345889.html

本文主要介绍了.NET高级调试训练营的一次案例分析，涉及到.NET内存暴涨的原因和解决方法。文章通过WinDbg工具，分析了一个.NET5的外贸ERP系统的内存dump文件，发现了托管堆上有大量的无根对象和临时对象，导致内存分配区域和提交区域相差过大。文章进一步定位了问题SQL语句和ORM框架FreeSql的映射机制，给出了优化建议和原理解释。

### 一个可用于生产项目 基于 .NET 6 自研ORM

https://www.cnblogs.com/China-Mr-zhong/p/17342895.html

本文主要介绍了基于.NET 6自研的轻量级ORM框架Fast Framework的特点和用法。文章从项目明细、核心对象、增删改查、Lambda表达式、数据库日志、事务和多租户等方面，详细说明了该框架的优点和缺点，以及如何使用不同的方法和对象进行数据库操作。文章还给出了开源地址和作者的联系方式，以及一些亮点功能和注意事项。

### .NET实现解析字符串表达式

https://www.cnblogs.com/Z7TS/p/17339894.html

本文主要介绍了如何使用System.Linq.Dynamic.Core库来解析字符串表达式并生成Lambda表达式树。文章首先说明了功能需求和构建字符串表达式的两种方式，然后介绍了System.Linq.Dynamic.Core库的功能、用法和文档地址，最后浅析了该库的源码实现和原理，以及一些相关的类和方法。

### 如何在 .NET Core WebApi 中处理 MultipartFormDataContent 中的文件

https://www.cnblogs.com/hippieZhou/p/17316146.html

本文主要介绍了如何在.NET Core WebApi中处理MultipartFormDataContent中的文件。文章分析了一个由于前端APP发送的文件缺少fileName字段导致后端无法解析的问题，给出了后端的兼容性处理方案，以及前端的优化建议。文章还提供了相关的代码示例和注意事项。

### LangChain vs Semantic Kernel

https://www.cnblogs.com/shanyou/p/17338785.html

这篇文章是从开发人员的角度比较了两个用于构建与AI集成的应用程序的库：Semantic Kernel（SK）和LangChain。文章介绍了这两个库的背景、特点、优势和不足，并给出了一些相关链接。文章的主要观点是：

- SK和LangChain都是为了简化开发人员使用OpenAI等大型语言模型（LLM）的过程，提供了一些协调业务流程、管理对话历史记录、实现链接等功能的工具。
- SK是由微软创立的，主要面向C#开发人员，也支持Python，它被称为轻量级SDK，可帮助开发人员将代码组织到内置于Planner中的技能、记忆和连接器中。SK有一个官方的支持页面和LinkedIn学习课程，还有一个MS Graph连接器工具包，适用于需要与日历、电子邮件、OneDrive等集成的方案。
- LangChain是由Harrison Chase创立的，他是一个ML工程师，它支持Python和TypeScript，其中Python具有更多功能。LangChain主要是为习惯于使用笔记本的ML工程师构建的，它不把自己称为SDK，而是Model as a Service粘合剂。LangChain有一个大型的开源社区，目前已经有29k star。
- 文章认为选择使用哪一个库主要取决于开发人员的技能，LLM已经将机器学习的门槛降低到普通开发人员就可以开发AI应用，SK在帮助应用开发人员开发AI方面的帮助会比LangChain更大，作者会选择采用SK来构建AI应用。

### ASP.NET Core - 缓存之分布式缓存

https://www.cnblogs.com/wewant/p/17114119.html

本文是基于 ASP.NET Core 框架的分布式缓存的介绍，主要包括以下几个方面：

- 分布式缓存的概念和优势，以及与内存缓存的区别。
- 分布式缓存的使用方法，基于 IDistributedCache 接口的抽象和扩展。
- 分布式缓存的接入方式，以内存缓存和 Redis 缓存为例，介绍了如何配置和切换不同的缓存实现。
- 分布式缓存的性能测试，比较了内存缓存、Redis 缓存和内存缓存结合 Redis 缓存的效率和消耗。

### 【译】ConfigureAwait FAQ

https://www.cnblogs.com/MeteorSeed/p/17327465.html

本文是关于 .NET 中 async/await 的 ConfigureAwait 方法的常见问题解答，主要涵盖了以下内容：

- SynchronizationContext 和 TaskScheduler 的概念和作用，以及它们如何影响 await 的行为。
- ConfigureAwait 方法的含义和用法，以及它如何通过传入一个布尔值来控制是否在原始上下文或调度器上执行回调。
- 使用 ConfigureAwait(false) 的好处，包括性能提升和死锁避免，以及使用 ConfigureAwait(true) 的场景。
- 使用 ConfigureAwait(false) 的指导原则，即在通用库代码中使用，在应用程序级代码中不使用。
- 使用 ConfigureAwait(false) 的局限性和注意事项，例如它不会影响 ExecutionContext 和 AsyncLocal 的流动，它不会保证回调不会在原始上下文中运行，它需要在每个 await 处使用等。
- 使用其他技巧来替代或辅助 ConfigureAwait(false) 的可能性和风险，例如使用 Task.Run, SynchronizationContext.SetSynchronizationContext, Task.GetAwaiter().GetResult 等。

### 记一次 .NET某医疗器械清洗系统 卡死分析

https://www.cnblogs.com/huangxincheng/p/17328225.html

本文是一篇关于.NET程序卡死分析的技术博客，作者分享了一个.NET某医疗器械清洗系统卡死的案例，介绍了如何使用windbg工具观察内核态和用户态的线程栈，定位到卡死的原因是非主线程创建了一个用户控件，导致内核态在某种情况下给它发消息。作者提供了解决办法，并总结了这个案例的经验教训。

### C# 如何设计一个好用的日志库？【架构篇】

https://www.cnblogs.com/czzj/p/JGP_MyLog.html

本文介绍了C#如何设计一个好用的日志库，分别介绍了日志的简单记录、通过开源库HslCommunication和NLog实现不同级别和选项的日志记录，以及使用TextAnalysisTool.NET进行日志查看和分析的方法。本文旨在帮助开发者提高日志记录的技能和效率，提高程序的稳定性和可维护性。

## 主题

### 【英文】Windows 社区工具包 2023 更新 - #ifdef Windows

https://devblogs.microsoft.com/ifdef-windows/the-windows-community-toolkit-2023-update/

关于 Windows 社区工具包更新。

它引入了新的 WCT Lab 组件、下一个版本中的组件以及命名空间的统一。

## 文章、幻灯片等
### 【日文】我尝试创建一个可以使用 Azure Functions 和 LINE Messaging API 与 ChatGPT 通信的服务

https://zenn.dev/takunology/articles/linebotandazure-gpt

了解如何使用 Azure Functions 和 OpenAI 的 ChatGPT API 实现 LINE 机器人。

### 【日文】使用 SetWindowSubclass 的自定义窗口过程 (C# / WinUI 3)

https://zenn.dev/shinta0806/articles/de27f23a0c3684

如何在 WinUI 3 应用程序中执行自定义窗口过程（子类化窗口）。

### 【日文】如何轻松调试 Windows 服务 - Qiita

https://qiita.com/TheParkSider/items/dc0aa0a03c02cec462e6

如何在实施 Windows 服务时简化调试。

### 【英文】改进 Visual Studio 中 JavaScript 的语法突出显示 - Visual Studio 博客

https://devblogs.microsoft.com/visualstudio/improving-the-syntax-highlighting-of-javascript-in-visual-studio/

在 Visual Studio 2022 v17.6 及更高版本中引入了对 JavaScript 语法突出显示的改进。

### 【英文】如何在 Rider 中使用 Aqua Web Inspector 进行 ASP.NET Core 开发 | .NET 工具博客

https://blog.jetbrains.com/dotnet/2023/04/20/jetbrains-rider-and-aqua-for-aspnetcore-development/

如何使用 IDE 的内置 Web 检查器通过 Rider 中提供的 JetBrains Aqua 插件进行 ASP.NET Core 开发。

### 【英文】Git 工具预览功能以提高生产力 - Visual Studio 博客

https://devblogs.microsoft.com/visualstudio/git-tooling-preview-features-to-enhance-productivity/

Visual Studio（预览版）中与 Git 相关的增强功能汇总。

### 【英文】使用 ReSharper 减少集合查找 | .NET 工具博客

https://blog.jetbrains.com/dotnet/2023/04/18/reduce-lookups-in-hashset-dictionary-and-other-collections-with-resharper/

关于 ReSharper 指出在操作 Dictionary 和 HashSet 等集合之前调用 ContainsKey 和 Contains 的不必要情况的能力。

### 【英文】.NET Web 视图控件中的 Chrome 扩展

https://dev.to/dotnetbrowser/chrome-extensions-in-net-web-view-controls-11lm

关于DotNetBrowser、WebView2、CefSharp等WebView中Chrome扩展的支持情况。

### 【英文】使用 Serilog 格式化 .Net 应用程序日志并将其发送到 Elasticsearch

https://medium.com/@ingrid.jardillier/format-and-send-net-application-logs-to-elasticsearch-using-serilog-9819742cf806

配置 Serilog 以将日志发送到 Elasticsearch 的说明。

### 【日文】从内存转储中检查 .NET 应用程序用于 HTTP 通信的代理设置 - Qiita

https://qiita.com/nishiseki/items/fe3e4795df9f790831f7

如何获取 .NET 应用程序的内存转储并从内存转储中解析 HTTP 代理配置信息。

### 【英文】使用 Kubernetes 运行非 root .NET 容器 - .NET 博客

https://devblogs.microsoft.com/dotnet/running-nonroot-kubernetes-with-dotnet/

它通过示例介绍了 .NET 8 支持的 Kubernetes 上非根容器的使用。它也应该与 dotnet-monitor 一起工作。

### 【日文】[Xamarin/C#] 在智能手机上创建一个VR照片展示应用

https://zenn.dev/daddy_yukio/articles/a70e04b8896f15

关于用Xamarin.Forms显示360度球面图像的实现。

### 【英文】为 .NET SDK 项目设置绝对输出路径

https://weblog.west-wind.com/posts/2023/Apr/21/Setting-an-Absolute-Output-Path-for-NET-SDK-Projects

关于构建时如何指定输出目标路径，以及如何通过AppendTargetFrameworkToOutputPath指定不将目标框架添加到路径中。

### 【英文】使用自定义集合调查 Enumerable.LastOrDefault 中的崩溃 - Gérald Barré

https://www.meziantou.net/investigating-a-crash-in-enumerable-lastordefault.htm

讨论在自定义集合上使用 LINQ LastOrDefault 方法时非线程安全操作引发异常的情况。

### 【英文】.NET 8 性能版

https://steven-giesel.com/blogPost/f6504300-7bf0-48d2-8a14-ba4e2bbea02e

.NET 8 和更早版本在枚举、LINQ、反射和列表等领域的基准性能比较。

### 【日文】用于 Azure OpenAI 服务的 C# SDK（也可用于 ChatGPT）

https://zenn.dev/microsoft/articles/azure-openai-service-csharpsdk

一篇关于开始使用 Azure OpenAI 服务的 .NET SDK（包括 ChatGPT）的文章。

### 【日文】在 C# 中创建带有 QR 图像的 Excel（NPOI、ZXing）

https://zenn.dev/junnuj/articles/a68409f9e18fd0

如何使用 ZXing.NET 生成二维码并使用 NPOI 在 Excel 中嵌入图像。

### 【日文】使用语义内核轻松链接 GPT 和外部工具 - 技术主题的味道

https://acro-engineer.hatenablog.com/entry/2023/04/18/120000

如何使用 Semantic Kernel 集成 ChatGPT API 和外部工具 Elasticsearch。

### 【杂记】清除赋值规则 |不明航班C博客

https://ufcpp.net/study/csharp/start/definiteassignment/

关于避免未初始化的显式分配规则。它还提到了 C# 10 中的改进。


## 库、存储库、工具

### microsoft/Tokenizer：用于 OpenAI LLM 的 BPE 标记器的 .NET 实现。

https://github.com/microsoft/Tokenizer

OpenAI 的 tiktoken 令牌计数库的 .NET 实现。

- [使用 C# 计算 Azure OpenAI 服务令牌](https://zenn.dev/microsoft/articles/azure-openai-count-token)


### CalvinAllen/vs4mac-super-clean：Super Clean 是 Visual Studio for Mac 的一个扩展，当它被触发时，会完全清除解决方案中所有项目的 bin 和 obj 目录

https://github.com/CalvinAllen/vs4mac-super-clean

用于删除所有 obj 和 bin 目录的 Visual Studio for Mac 扩展。

### bUnit-dev/bUnit：bUnit 是 Blazor 组件的测试库，它使测试看起来、感觉起来和运行起来都像常规单元测试。bUnit 使呈现和控制被测组件的生命周期、传递参数和将服务注入其中，触发事件处理程序，并使用内置的语义 HTML 比较器验证从组件呈现的标记。

https://github.com/bUnit-dev/bUnit

使 Blazor 组件更易于测试的库。

- [Blazor 组件测试：原始标记的基本验证](https://medium.com/@longeardev/blazor-component-testing-basic-verification-of-a-raw-markup-670bf91c1d90)

## 版权声明

* 国内板块由 InCerry 进行整理 : https://github.com/InCerryGit/WeekRef.NET
* 其余内容来自 Myuki WeekRef，由InCerry翻译（已获得授权） : https://github.com/mayuki/WeekRef.NET

**由于笔者没有那么多时间对国内的一些文章进行整理，欢迎大家为《.NET周报-国内文章》板块进行贡献，需要推广自己的文章或者框架、开源项目可以下方的项目地址提交Issue或者在我的微信公众号私信。**

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