## 国内文章

### LRU缓存替换策略及C#实现

https://www.cnblogs.com/eventhorizon/p/17290125.html

这篇文章讲述了缓存替换策略，特别是LRU算法。LRU算法基于这样一个假设：如果数据最近被访问过，那么将来被访问的几率也更高。通常我们会用双向链表来实现这个数据结构，每次访问数据的时候，就将数据移动到链表的尾部。但如果数据的访问模式不符合LRU算法的假设，那么LRU算法就会失效。文章还提到了LFU和LFRU算法，可以有效的解决这个问题。最后，文章介绍了如何优化算法，降低链表的删除操作的时间复杂度。

### Semantic Kernel 入门系列：🔥Kernel 内核和🧂Skills 技能 

https://www.cnblogs.com/xbotter/p/semantic_kernel_introducation_kernel_and_skills.html

这篇文章讨论了如何使用语义内核（SK）构建结合LLM AI和原生代码能力的应用程序。SK的基本能力由技能组成，技能由语义函数（LLM AI能力）和本地函数（代码能力）组成。需要一个内核来组织和管理技能并提供基础服务配置。该页面还提供了如何设置应用程序环境和安装SK nuget包的说明。它还讨论了如何在SK中使用语义和本地函数。

### ASP.NET Core如何知道一个请求执行了哪些中间件？

https://www.cnblogs.com/Ax0ne/p/17300692.html

这篇文章介绍了如何使用 `Microsoft.AspNetCore.MiddlewareAnalysis` 和 `Microsoft.Extensions.DiagnosticAdapter` 两个 Nuget 包来分析和记录中间件。文章提供了一个适配器的代码实现，用来把从 `DiagnosticSource` 接收到的日志对象输出到控制台。文章还介绍了如何使用 `DiagnosticListener` 对象的 `SubscribeWithAdapter` 方法来订阅日志。最后，文章提供了一种方法来查看一个请求执行了哪些中间件。

### .NET Core MongoDB数据仓储和工作单元模式封装

https://www.cnblogs.com/Can-daydayup/p/17157135.html

这篇文章介绍了如何使用.NET Core应用程序连接MongoDB并封装MongoDB数据仓储和工作单元模式。文章详细讲解了仓储模式和工作单元模式的好处，以及如何在MongoDB中实现它们。文章还提到，MongoDB单机服务器不支持事务，只有在集群情况下才支持事务。最后，文章给出了一些示例代码，展示了如何定义MongoDB DBContext上下文类，以及如何使用仓储和工作单元模式进行数据操作。

### .Net Core后端架构实战【2-实现动态路由与Dynamic API】

https://www.cnblogs.com/zhangnever/p/17131504.html

这篇博客讲述了如何在.Net Core 7.0 WebApi后端架构中实现动态路由与Dynamic API。作者提到了使用过ABP vNext和Furion框架的可能都会对它们的动态API感到好奇。文章详细介绍了动态路由的实现方式，以及WebApplicationBuilder在不同版本中的变化。此外，作者还详细解释了UseRouting和UseEndpoints的源码。最后，作者提到了MapControllers方法的作用，即将controller里面的action映射为我们的终结点。总之，这篇博客为我们提供了关于.Net Core后端架构实战的宝贵经验。

### Semantic Kernel 知多少 | 十行代码开发一个AI应用

https://www.cnblogs.com/sheng-jie/p/17294842.html

这篇文章介绍了Semantic Kernel (SK) ，它是一个轻量级的SDK，可以轻松地将传统编程语言与最新的大型语言模型 (LLM) AI "提示"相结合。SK提供了多种能力，包括提示链、递归推理、总结、zero/few-shot（零样本和少量样本）学习、上下文记忆、长期记忆、嵌入、语义索引、 规划，以及访问外部知识库和您自己的数据。文章还提供了一个简单的AI应用示例：使用SK开发专属AI外教应用。总之，这篇文章为我们提供了关于如何使用SK进行面向AI编程的宝贵经验。

### 记一次 .NET 某设备监控系统 死锁分析

https://www.cnblogs.com/huangxincheng/p/17292169.html

上周看了一位训练营朋友的dump，据朋友说他的程序卡死了，看完之后发现是一例经典的死锁问题，蛮有意思，这个案例算是学习 `.NET高级调试` 入门级的案例，这里和大家分享一下。

### C#泛型的逆变协变(个人理解) 

https://www.cnblogs.com/CollapseNav/p/17285595.html

这篇文章讲述了C#泛型里的逆变协变。作者通过举例说明了逆变协变的概念和使用方法。例如，`IEnumerable<object> list = new List<string> ();`体现的是协变，符合一般直觉，整体上看起来就像是将子类赋值给基类。而`IFace<string> item = new Face<object> ();`则体现了逆变。作者还解释了什么时候可以用逆变，什么时候可以用协变，以及这两个东西用起来有什么限制。简单来说，有关泛型输入的用逆变，关键词是in；有关泛型输出的用协变，关键词是out；如果接口中既有输入又有输出，就不能用逆变协变。总之，这篇文章为我们提供了关于C#泛型里的逆变协变的宝贵经验。

### 聊一聊如何使用Crank给我们的类库做基准测试

https://www.cnblogs.com/catcher1994/p/17291228.html

这篇文章介绍了如何使用 Crank 工具来进行基准测试。Crank 是一个 client-server 架构的工具，由控制器和代理组成。它可以用来在多个环境下运行基准测试，也可以针对 Pull Request 进行基准测试。文章中还提供了一个简单的入门示例，以及如何在不同机器上执行基准测试的方法。总之，Crank 是一个非常不错的工具，可以结合 BenchmarkDotNet 来做类库的基准测试，也可以结合其他压测工具进行 api/grpc 框架和应用的测试。

### NetCore 使用 Swashbuckle 搭建 SwaggerHub

https://www.cnblogs.com/calvinK/p/netcore-buiding-swaggerhub.html

本文介绍了SwaggerHub，一种集中管理和展示公司API信息的工具。为减少沟通成本并实现全局视野，可选用成熟商业产品如https://swagger.io/tools/swaggerhub/。此外，文章提供了在.Net Core环境中使用Swashbuckle.AspNetCore搭建自定义SwaggerHub的方法。只需一行代码配置Urlsoption，即可添加多个swagger.json文件。SwaggerUIOptions对象的更改实时生效，而URL可以配置为endpoint或任意位置的文件。

### ASP.NET Core - 缓存之内存缓存(上)

https://www.cnblogs.com/wewant/p/17114036.html

本文介绍了缓存技术，特别是在.NET Core框架中的内存缓存。缓存通过存储数据副本降低了生成内容所需的工作，提高应用性能和可伸缩性。注意事项包括：使用缓存适用于不常更改且成本高的数据；始终设有回退选项；应考虑缓存失效的情况；限制缓存增长。

### 我没能实现始终在一个线程上运行 task

https://www.cnblogs.com/newbe36524/p/0x029-I-can-not-manage-to-always-run-task-on-one-thread.html

这篇文章讨论了如何在处理带有异步代码的常驻任务时确保代码在同一个线程上运行。作者提出了几种解决方案，包括增加线程池容量，使用同步重载方法，以及自定义任务调度程序。但是，这些方法都有其局限性和困难。作者建议读者可以通过 UniTask 项目来了解如何实现全套自定义。

### 记一次 .NET 某手术室行为信息系统 内存泄露分析

https://www.cnblogs.com/huangxincheng/p/17282019.html

昨天有位朋友找到我，说他的程序内存存在泄露导致系统特别卡，大地址也开了，让我帮忙看一下怎么回事？今天上午看了下dump，感觉挺有意思，在我的分析之旅中此类问题也蛮少见，算是完善一下体系吧。

## 主题

### 【英文】WiX v4.0.0 | 发行说明 | WiX 工具集
https://wixtoolset.org/docs/releasenotes/#v4

WiX v4.0.0 已经发布。

此版本包括各种改进，例如 ARM64 支持和 NuGet 提供的工具。

### 【英文】ReSharper 2023.1 带有增强的 C# 支持、令人兴奋的 C++ 更新等！| .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/04/05/resharper-2023-1/

ReSharper 2023.1 已发布。

此版本包括修复集合中多个查找的 QuickFix、引入空检查模式的语法样式、改进快捷方式和更新对话框等。

此外，从此版本开始，不再支持 Visual Studio 2010 和 2012。

### 【英文】dotCover、dotMemory、dotPeek 和 dotTrace 2023.1 发布！| .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/04/05/dottools-2023-1-release/

dotCover、dotMemory、dotPeek、dotTrace 2023.1 已发布。

dotTrace 现在作为 Linux 和 macOS 的独立测试版提供，并进行了多项改进。

### 【英文】ASP.NET Core 8 中身份验证和身份的改进 - .NET 博客
https://devblogs.microsoft.com/dotnet/improvements-auth-identity-aspnetcore-8/

了解 .NET 8 中 ASP.NET Core 中的身份验证和身份管理。

它提到从 .NET 8 SPA 模板中删除了 IdentityServer 依赖项并改进了自托管身份验证。

### 【英文】.NET 8 中的 ASP.NET Core 路由工具增强功能 - .NET 博客
https://devblogs.microsoft.com/dotnet/aspnet-core-route-tooling-dotnet-8/

.NET 8 中 ASP.NET Core 路由的工具增强。

- 根语法突出显示
- 完成参数和路由名称
- 完成路线限制
- 根分析器和 CodeFix
- 最小的 API 和 Web API，Blazor 支持

### 【英文】发布 ILSpy 8.0 预览版 4 icsharpcode/ILSpy
https://github.com/icsharpcode/ILSpy/releases/tag/v8.0-preview4

ILSpy 8.0 Preview 4 已经发布。

此版本添加了新主题并修复了各种错误。


## 文章、幻灯片等
### 【英文】在 ASP.NET Core 最小 API 中接收和测试传入的 Webhook：综合指南
https://www.christianfindlay.com/blog/asp-dotnet-core-minimal-webhooks

描述实现和测试使用 ASP.NET Core 的最小 API 接收请求的 webhook 的过程。

### 【英文】Visual Studio 工具箱：使用并行堆栈调试线程和任务 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-toolbox-debug-threads-tasks-with-parallel-stacks/

线程和并行堆栈调试工具的介绍视频。

### 【英文】如何为桌面和移动开发创建 NuGet 包
https://dev.to/yushulx/how-to-create-a-nuget-package-for-both-desktop-and-mobile-development-5e61

如何创建一个 NuGet 包，其中除了桌面之外还包括适用于 Android 和 iOS 的绑定库。

### 【日文】[C#11] 使用通用数学模拟 OpenCV 的 saturate_cast
https://zenn.dev/shimat/articles/daab88eea9c41f

一篇关于使用通用数学实现类似 OpenCV 的 saturate_cast 函数的方法的文章。

### 【日文】[C#] dotnet user-jwts 很好  - 尼诺的花园
https://blog.neno.dev/entry/2023/04/07/165241

引入 user-jwts 工具，它允许您在使用 ASP.NET Core 开发时使用 JWT 时轻松生成可以在本地开发环境中使用的 JWT。

### 【英文】.NET 注释月刊 | 2023 年 4 月 | .NET 工具博客

https://blog.jetbrains.com/dotnet/2023/04/06/net-annotated-monthly-april-2023/

JetBrains 4 月发行的 .NET 相关信息。

### 【英文】ArrayPool深入
https://medium.com/@epeshk/arraypool-t-ea90cb24b87f

ArrayPool 内部实现的描述。

- [(C#) ArrayPool<T>.Shared Kaitai Shinsho - 猫的钟声](https://ikorin2.hatenablog.jp/entry/2020/07/25/113904)

### 【英文】使用 MSAL.NET 改进了 Windows Broker 支持 | Microsoft Entra Identity 开发人员博客
https://devblogs.microsoft.com/identity/improved-windows-broker-support-with-msal-net/

在 MSAL.NET 中改进 Windows 环境中的代理支持。

### 【日文】在 C# 中使用 SonarQube 显示覆盖范围 - Qiita
https://qiita.com/YoshijiGates/items/e1055e14c9960228726b

如何覆盖 C# 项目并使其在 SonarQube 中可见。

### 【英文】向 ASP.NET Core 添加客户端验证，无需 jQuery 或非侵入式验证
https://andrewlock.net/adding-client-side-validation-to-aspnet-core-without-jquery-or-unobtrusive-validation/

如何在没有 jQuery 或 ASP.NET Core 中的非侵入式验证的情况下添加客户端验证。

文章介绍了如何使用 npm 的 aspnet-client-validation 包并对其进行自定义。

### 【日文】微软宣布将 LLM 集成到应用程序开发中的 OSS“语义内核”——Qiita
https://qiita.com/nohanaga/items/430b59209b02c298ef2a

语义内核简介，这是一个用于将诸如 ChatGPT 之类的 LLM 集成到您的应用程序中的框架。

### 【英文】迭代器基准测试结果令人震惊 - 开发负责人
https://www.devleader.ca/2023/03/17/shocking-results-from-collection-and-iterator-benchmarks/

在针对产生意外结果的列表和迭代器对 LINQ 进行基准测试时，对我忽略的事情的思考。

### 【英文】在 C# 中使用 iText7 拆分和合并 PDF 文件 - Qiita
https://qiita.com/nekohei/items/9a2e8b1e9dfc922592ea

如何使用 iText 7 拆分和合并 PDF 文件。

### 【英文】C# 的主要构造函数
https://csharp.christiannagel.com/2023/03/28/primaryctors/

将在 C# 12 中引入的主要构造函数的讨论。

### 【日文】使用 Lambda 和 AWS Lambda Web Adapter 运行 .NET WEB API
https://zenn.dev/junnuj/articles/c2ba888670bc8e

了解如何使用 Lambda Web Adaptor 在 Lambda 上运行纯 ASP.NET Core 应用程序。

## 库、存储库、工具

### ufcpp/ScribanSourceGenerator

https://github.com/ufcpp/ScribanSourceGenerator

ScribanSourceGenerator 使用 Scriban（模板引擎）生成源代码。

- [[C#] 使用 ScribanSourceGenerator 生成编译时代码 - Qiita](https://qiita.com/thinva/items/6ae7e295dabe417645cf)


### Visual Studio Marketplace 发布者 - GitHub Marketplace
https://github.com/marketplace/actions/visual-studio-marketplace-publisher

要发布到 Visual Studio Marketplace 的 GitHub 操作。

- [介绍“Visual Studio Marketplace Publisher”GitHub Action](https://dev.to/calvinallen/introducing-the-visual-studio-marketplace-publisher-github-action-1nme)

### Visual Studio VSIX 签名者 - GitHub 市场
https://github.com/marketplace/actions/visual-studio-vsix-signer

用于签署 Visual Studio VSIX 的 GitHub 操作。

- [介绍“Visual Studio VSIX Signer”GitHub 操作](https://dev.to/calvinallen/introducing-the-visual-studio-vsix-signer-github-action-3iog)

### drasticactions/Drastic.InAppSettingsKit
https://github.com/drasticactions/Drastic.InAppSettingsKitInAppSettingsKit 的绑定库，用于在 iOS 应用程序中创建设置屏幕。

https://twitter.com/dramaticactions/status/1642778859992154114?s=20

![image-20230410202553139](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230410202553139.png)

## 站点、文档等
### 推文

**关于 Java 和 .NET 堆栈跟踪之间的区别。**
https://twitter.com/matarillo/status/1643864714466951168?s=12

![image-20230410203021882](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230410203021882.png)



---

**MFractor 现在支持 Visual Studio for Mac v17.5。**

https://twitter.com/matthewrdev/status/1642281174793068544?s=12

![image-20230410203110672](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230410203110672.png)

## 深入探索

### 在 DateTime、DateTimeOffset、DateOnly、TimeOnly、TimeSpan、Char、Rune 上实现 IUtf8SpanFormattable by stephentoub Pull Request #84469 dotnet/runtime
https://github.com/dotnet/runtime/pull/84469

为 DateTime 等值类型实现“IUtf8SpanFormattable”的 PR。

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