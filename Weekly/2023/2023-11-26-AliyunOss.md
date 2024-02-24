## 国内文章

### 万字长文：从 C# 入门学会 RabbitMQ 消息队列编程

https://www.cnblogs.com/whuanle/p/17837034.html

如题，详细的介绍RabbitMQ以及C#的使用。

### CPF C#跨平台UI框架开源了

https://www.cnblogs.com/dskin/p/17849896.html

本文介绍了C#的跨平台UI框架CPF，它支持.NETStandard2.0和net4，可在Windows、Mac、Linux等系统上运行，不依赖系统控件，实现了窗体和控件的透明、异形等效果。CPF采用动画、数据绑定、Mvvm模式和CSS简化开发，支持国产CPU平台。框架使用Skia图形库和平台适配器，保证了控件的自绘和一致性。CPF提供了C#和CSS描述UI和样式的方式，无需Xaml，且考虑了国内系统兼容性。CPF是开源的，可通过克隆或下载编译，还有扩展库如浏览器和视频播放控件。作者鼓励大家参与开源社区，共同完善CPF。

### 一套开源、强大且美观的WPF UI控件库 - HandyControl

https://www.cnblogs.com/Can-daydayup/p/17850568.html

本文介绍了HandyControl，一套开源的WPF UI控件库，它提供了80多种自定义控件，重写了所有原生样式，帮助开发者轻松创建美观且交互性强的应用程序。文章还指导如何安装WPF的Vs开发环境，运行HandyControl项目源码，并展示了项目运行截图。最后，提供了项目的GitHub和Gitee开源地址，并提到该项目已被收录到C#/.NET/.NET Core优秀项目和框架精选中。

### C#/.NET/.NET Core推荐学习书籍（已分类）

https://www.cnblogs.com/Can-daydayup/p/17855099.html

本文介绍了DotNetGuide技术社区和一系列C#/.NET/.NET Core学习书籍。DotNetGuide是.NET开发者的开源社区，提供学习资料、技术分享、项目推荐等。文章还推荐了多本C#相关书籍，涵盖CLR、C#语言特性、编程技巧等内容，适合不同层次的读者学习。

### Avalonia 实现跨平台的IM即时通讯、语音视频通话（源码，支持信创国产OS，统信、银河麒麟）

https://www.cnblogs.com/shawshank/p/17817414.html

本文介绍了基于Avalonia框架的跨平台即时通讯(IM)软件开发，该软件支持文字、表情聊天，文件传输，语音视频通话和远程桌面功能。开发环境包括Visual Studio 2022、.NET Core 3.1、C#语言和Avalonia UI框架。作者还分享了自定义消息类型的核心代码，并建议使用Avalonia的0.10.*版本。

### 自研 Fast.ORM 已全面支持AOT编译

https://www.cnblogs.com/China-Mr-zhong/p/17852177.html

本文介绍了Fast Framework，这是一个基于.NET 6.0的轻量级ORM框架，支持多种数据库，具有简单API、高性能等优点，但目前只支持数据库先行模式。作者分享了AOT编译的经验，包括避免动态获取方法、不使用Emit和dynamic关键字等。项目包含ORM核心、文件日志、依赖注入等模块，还有控制台测试、单元测试和Web测试项目。核心对象包括Ado、DbContext和DbOptions，支持多租户和主从分离配置。项目开源地址提供了源代码和AOT编译示例。

### 记一次在线客服系统用户遭勒索，索要茶水费事件的 Windbg 分析与应对

https://www.cnblogs.com/sheng_chao/p/17848742.html

本文记录了客户使用在线客服系统时遭受勒索攻击的事件。通过监测服务器CPU使用率，发现并解决了后台服务的异常占用问题。使用WinDbg工具分析Dump文件，确定攻击者通过TCP端口发送垃圾数据导致服务器负载过高。最终通过增强端口安全措施，成功识别并拉黑攻击IP，确保了系统安全稳定运行。同时，文章展示了客服系统的强大功能，如不丢消息、支持所有浏览器和移动端，以及开源社区的贡献精神。

### 龙芯发布 .NET 8 SDK 8.0.100-ea1(试用版)

https://www.cnblogs.com/shanyou/p/17855570.html

龙芯.NET团队发布了基于LoongArch64架构的.NET 8 SDK试用版，自2019年研发以来，已与.NET社区同步开发。新版SDK在生命周期内将持续更新，支持多种64位操作系统，提供性能优化和安全更新。用户可通过官方网站下载SDK和相关资源，享受社区最新特性和专业团队支持。

### ConfigureAwait in .NET8

https://www.cnblogs.com/ms27946/p/ConfigureAwait_in_NET8_CN.html

本文讨论了.NET中的ConfigureAwait，它通过布尔参数控制异步方法是否在原上下文中继续执行。默认情况下，异步方法会在捕获的上下文中恢复，但使用ConfigureAwait(false)可以在任意线程池线程上恢复。过去，建议在库中广泛使用ConfigureAwait(false)，但这一做法已逐渐放弃。文章还纠正了对ConfigureAwait(false)的几个误解，比如它并非避免死锁的好方法，也不意味着方法后续部分一定在线程池线程上运行。最后，介绍了.NET8中新增的ConfigureAwait(ConfigureAwaitOptions)，它是一个枚举类型，提供了更多配置awaitables的方法，但目前仅适用于Task和`Task<T>`。

### .net 温故知新【14】：Asp.Net Core WebAPI  缓存

https://www.cnblogs.com/SunSpring/p/17848185.html

本文讨论了缓存的概念、作用和实现方式。缓存是一种性能优化手段，通过存储数据来加快数据检索速度。RFC9111规定了缓存控制的标准，特别是`Cache-Control`响应头的作用。在Asp.net Core中，通过`ResponseCacheAttribute`设置`max-age`可以控制浏览器缓存。服务器缓存通过响应缓存中间件实现，但如果客户端禁用缓存或发送`no-cache`请求，服务器缓存将不起作用。内存缓存是另一种缓存方式，它使用IMemoryCache在服务器内存中存储数据。

### 对 .NET程序2G虚拟地址紧张崩溃 的最后一次反思

https://www.cnblogs.com/huangxincheng/p/17853851.html

本文讲述了如何在32位操作系统上通过配置3G开关，解决程序因2G虚拟地址空间限制而频繁崩溃的问题。文章首先指出，医疗行业常用的老旧系统如XP和Windows7 x86，因用户态和内核态各占2G内存，导致程序容易崩溃。解决方案包括开启程序的Large Address Aware和机器级别的3G开关，使程序能使用更多内存。验证是否成功开启3G，可以通过观察地址空间或使用windbg工具检查。

### 一个基于.NET Core开源、跨平台的仓储管理系统

https://www.cnblogs.com/Can-daydayup/p/17857794.html

本文介绍了ZEQP.WMS，一个基于.NET Core的开源跨平台仓储管理系统，支持MSSQL/MySQL数据库。该系统提供全面的仓库操作管理，如物品跟踪、存储、拣选等，旨在提升自动化和效率。系统采用Colder.Admin.AntdVue框架开发，功能包括仓库、货架、客户、供应商管理等。项目源码可在GitHub获取，同时该项目也被收录在C#/.NET/.NET Core优秀项目和框架精选中。另外，文章推荐了DotNetGuide技术社区，为.NET开发者提供学习资料、技术分享和交流机会。

### 一个NET8 AOT编译的辅助项目，让你的任何可执行应用快速部署为服务

https://www.cnblogs.com/Start201505/p/17857565.html

本文介绍了如何将应用程序转换为服务，无需重新编码。作者分享了基于.NET 8的快速开发框架Simple Framework，以及使用WinSW将应用封装为服务的方法。WinSW依赖.NET环境，而NSSM不依赖，但作者选择了WinSW。文章还详细介绍了如何构建一个.NET 8 AOT编译的辅助工具，通过简单的指令菜单来生成配置文件和管理服务，使得服务的启停变得方便快捷。

### 你所不知道的ASP.NET Core进阶系列（三）

https://www.cnblogs.com/CreateMyself/p/17830637.html

本文讨论了模型绑定的细节问题，作者在长时间未更新博客后继续探讨此话题。文中通过实例代码展示了在.NET中使用FromQuery特性进行模型绑定时遇到的问题，即新增属性后值无法绑定。作者分析可能的原因，提出属性名与参数名或URL键名相同（不区分大小写）可能导致问题，并建议读者通过分析源码来找出根本原因。最后，作者鼓励读者不要怀疑自己，因为找到问题源码是一个必经的学习过程。

### 在ASP.NET Core 中使用 .NET Aspire 消息传递组件

https://www.cnblogs.com/powertoolsteam/p/17850840.html

本文介绍了如何使用.NET Aspire组件在ASP.NET Core应用中实现与Azure服务总线的消息传递。首先需安装.NET 8.0、.NET Aspire工作负载、Docker桌面和IDE。然后在Azure中设置服务总线账户，并选择无密码身份验证或连接字符串进行身份验证。接着创建ASP.NET Core项目和Worker Service项目，最后将.NET Aspire Azure服务总线组件添加到API。通过这些步骤，可以将消息发送到服务总线主题供订阅者使用。

### C#12中的Collection expressions（集合表达式语法糖）

https://www.cnblogs.com/chenyishi/p/17843378.html

C#12新增了创建集合的语法糖，支持数组、Span<T>和泛型集合等类型。通过集合表达式，可简化集合初始化，还能用".."解构集合，将元素内联到其他集合。自定义类型也可支持集合表达式，需实现Create方法和应用CollectionBuilderAttribute。

### 【ASP.NET Core】MVC过滤器：运行流程

https://www.cnblogs.com/tcjiaan/p/17855411.html

本文解释了MVC中的过滤器，它们是在MVC操作方法调用前后进行处理的类型，如授权检查、数据源修改等。ASP.NET Core的MVC框架中，过滤器通过实现IFilterMetadata接口来标识，而具体的过滤功能则通过实现不同的接口如IAuthorizationFilter、IResourceFilter等来完成。过滤器可以形成调用管道，按顺序执行。作者通过代码示例展示了过滤器的运行过程。

### 在Linux平台下使用.NET Core访问Access数据库读取mdb文件数据

https://www.cnblogs.com/VAllen/p/access-mdb-files-in-linux.html

本文介绍了如何在Linux系统下使用C#访问Access数据库。作者分享了在Ubuntu 22.04.3 LTS上，通过安装依赖库如unixodbc和mdbtools，并配置ODBC来实现数据库访问。文章还提供了配置文件示例和一个简单的C#项目代码，展示了跨平台数据库访问的实现方法。

## 主题

### Cake v4.0.0 发布
https://cakebuildnet.medium.com/cake-v4-0-0-released-475ce3ddd987

Cake v4.0.0 已发布。

此版本包括对 C# 12 和 .NET 8 的支持、文件 API 增强功能等。

### 发布 NATS.Net v2.0.0 · nats-io/nats.net.v2
https://github.com/nats-io/nats.net.v2/releases/tag/v2.0.0

NATS.Net v2.0.0 已发布。

它是 NATS 的 .NET 客户端库，自 v2.0.0 起它已成为基于 AlterNats 的现代实现。该版本包括核心 NATS 命令支持、JetStream 支持、NATS 服务 API 支持、本机 AOT 支持等。

### Npgsql 8.0 发行说明 | Npgsql 文档
https://www.npgsql.org/doc/release-notes/8.0.html

Npgsql 8.0 已发布。

此版本包含新功能，例如对本机 AOT 和 Trimming 的支持、通过 Metrics API 支持 OpenTelemetry 指标以及注册为密钥服务。它还包括其他几个重大更改。

8.0 版本是支持 .NET Framework（.NET Standard 2.0）的最后一个版本，从 9.0 开始将不再支持。

### 宣布 .NET Chiseled 容器 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-chiseled-containers/

.NET Chiseled Containers 的发布公告。

Chiseled镜像是一个包含Ubuntu发布的最小组件的容器镜像，基于此，我们发布了包含.NET运行时的镜像。

文章阐述了 Chiseled 在容量、依赖关系、漏洞处理等方面的优势，以及采用 Distroless 时的差异。

### 宣布 NuGet.exe 和 NuGet 客户端 SDK 包支持政策：让您了解情况并确保安全 - NuGet 博客
https://devblogs.microsoft.com/nuget/announcing-nuget-exe-and-nuget-client-sdk-packages-support-policy-keeping-you-informed-and-secure/

关于 NuGet.exe 和 NuGet 客户端 SDK 包的支持策略。

本文介绍了对 NuGet.exe 和 NuGet Client SDK 的未来支持。一般来说，更新只会提供给当前版本以及对 Visual Studio 和 .NET SDK 的 LTS 支持，易受攻击的 NuGet 版本将从 tools.json 中删除，并且软件包将被弃用。

### Visual Studio 2022 – 17.8 性能增强 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-8-performance-enhancements/

解释 Visual Studio 2022 版本 17.8 中的性能改进。

文章包括提高打开文件时的响应能力、提高 Razor/Blazor 中的响应能力、加快 F5（调试执行）、优化虚幻引擎 C++ 中的 IntelliSense 以及构建非 SDK 风格的 .NET 项目。

### Azure Pipelines 和 GitHub Actions 的托管映像运行程序现已完成推出，包括 .NET 8 SDK（*-最新）和 Visual Studio 17.8（windows-最新）
https://github.com/actions/runner-images/blob/main/images/ubuntu/Ubuntu2204-Readme.md

Azure Pipelines 和 GitHub Actions 的运行器映像现在包括 .NET 8 SDK 和 Visual Studio 2022 17.8 (Windows)。

https://x.com/timheuer/status/1727006190306287773?s=12&t=ggvrrZ7oLogHyNoIGNgjbw

### ServiceStack v8
https://docs.servicestack.net/releases/v8_00

ServiceStack v8 已发布。

此版本包括 Blazor 和身份验证等各种项目的模板更新，以及 PHP 的端到端类型化 API 支持等各种改进。

https://x.com/servicestack/status/1726603790453989682?s=12
### 版本 2.1.0 · microsoft/reverse-proxy
https://github.com/microsoft/reverse-proxy/releases/tag/v2.1.0

Yarp 2.1.0 已发布。

此版本包括多项错误修复和改进。

### Tye 实验的结束 · 问题 #1622 · dotnet/tye
https://github.com/dotnet/tye/issues/1622Tye 旨在成为本地微服务开发工具，随着 .NET Aspire 的发布而存档。

## 文章、幻灯片等
### tannergooding (@tannergooding@dotnet.social)
https://dotnet.social/@tannergooding/111423937700237917

.NET 中硬件内在函数的简史和演示等。

### 主要构造函数 – 在 Rider 和 ReSharper 中使用 C# 12 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/11/23/primary-constructors-using-csharp-12-in-rider-and-resharper/

介绍 Rider 和 ReSharper 中的 C# 12 主构造函数支持。

支持哪些转换/简化、双捕获警告、参数突出显示、代码风格等。

### 使用 .NET 8 构建 Arm64 Docker 镜像：快速解决方案
https://medium.com/medialesson/building-arm64-docker-images-with-net-8-a-quick-solution-5491a94eb507

创建 Arm64 Docker 镜像时，您可以通过在“FROM”中指定“--platform=$BUILDPLATFORM”来确定构建时的平台。

### 我想在 .NET 8 Blazor 中尽可能避免使用 InteractiveWebAssembly 进行预渲染
https://zenn.dev/microsoft/articles/aspnetcore-blazor-dotnet8-wasmloading

如何在 Blazor 中使用 InteractiveWebAssembly，同时尽可能减少预渲染。

### 为 .NET 8 应用程序设置 GitHub Codespaces
https://dev.to/this-is-learning/set-up-github-codespaces-for-a-net-8-application-5999

如何为 .NET 8 应用程序创建 GitHub Codespaces 环境。

### ASP.NET Core 8.0 中的新 Minimal API 功能
https://medium.com/abp-community/new-minimal-apis-features-in-asp-net-core-8-0-683d8a79b18d

快速介绍 .NET 8 中 ASP.NET Core 最小 API 的新功能。

### 在 ReSharper 2023.3 中可视化实体框架关系和附加查询分析 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/11/20/visualize-entity-framework-relationships-and-additional-query-analysis-in-resharper-2023-3/

ReSharper 2023.3 中实体框架的可视化和查询分析简介。

生成实体关系图、检查没有指定长度限制的字符串、检测无法转换为 SQL 的方法调用等等。

### 现代化 .NET 响应式扩展 | endjin
https://endjin.com/what-we-think/talks/modernizing-reactive-extensions-for-dotnet

关于 Rx.NET 从开始到现在的历史，以及那段时间所做的现代化工作。

### C# 12 和 .NET 8 中拦截器的失败实验
https://andrewlock.net/a-failed-experiment-with-interceptors-in-csharp-12-and-dotnet-8/

我在尝试使用 Interceptor（C# 12 的预览功能）以及枚举和扩展方法时遇到了 Roslyn bug。

### 社区反馈 Building 17.8 和 17.9 预览版 1 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/community-feedback-building-17-8-17-9-preview-1/

了解 Visual Studio 社区的新功能和反馈建议、如何发送反馈等。

### .NET 8 中 Android 资源生成的改进和变化 - .NET 博客
https://devblogs.microsoft.com/dotnet/android-resource-designer-dotnet-8/

.NET 8 中新引入的访问 Android 资源的机制的说明。

新引入的机制具有诸如减少启动时间和由于三聚体友好而减小尺寸等优点。

### 使用 GA 中提供的摘要差异视图创建拉取请求 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/create-a-pull-request/

引入了从 Visual Studio 2022 17.9 Preview 1 中实现的 IDE 创建拉取请求的功能

### 假装它直到你成功...到生产 - .NET 博客
https://devblogs.microsoft.com/dotnet/fake-it-til-you-make-it-to-product/

引入类来实现 .NET 8 中引入的 fakes（FakeLogger、MetricCollector、ITimeProvider）等。

### .NET 之夜派对@品川 - connpass
https://msdevjp.connpass.com/event/303250/

线下活动将于 .NET Conf 2023 Recap Japan 之后举行。

- [.NET Conf 2023 日本回顾](https://mktoevents.com/Microsoft+Event/415522/157-GQE-382)

### 使用 System.Threading.Channels 的生产者/消费者管道
https://blog.maartenballiauw.be/post/2020/08/26/ Producer-consumer-pipelines-with-system-threading-channels.html

快速介绍 System.Threading.Channels 以及如何使用 Open.ChannelExtensions 构建简单的管道。

### .NET 8：身份验证和授权的新增功能
https://auth0.com/blog/whats-new-dotnet8-authentication-authorization/

了解使用 .NET 8 Identity API 进行基于令牌的身份验证。

### 有关 .NET 8 中 Blazor 错误处理的注意事项
https://zenn.dev/microsoft/articles/aspnetcore-blazor-dotnet8-errorhandling

关于ErrorBoundary无法跨不同执行方法处理的问题。

### Path.GetDirectoryName() 根据重载的不同而表现不同 - xin9le.net
https://blog.xin9le.net/entry/2023/11/20/212653

Path.GetDirectoryName 方法可能会也可能不会规范路径分隔符，具体取决于其重载。

### .NET 8 中的本机 AOT 编译
https://medium.com/abp-community/native-aot-compilation-in-net-8-3c9b80a77f06

简要介绍 .NET 8 中与本机 AOT 相关的更改、如何启用它以及结果。

### C# 12 新功能备忘录 - Qiita
https://qiita.com/habakino094/items/57dca2d0c49c9c02395a

快速介绍 C# 12 中的新功能。关于主构造函数、集合表达式、任意类型别名和 lambda 参数的默认值。

### 我不想在 Blazor 中编写 HTML...（.NET 8 上的 Fluent UI Blazor 版本）
https://zenn.dev/microsoft/articles/aspnetcore-blazor-dotnet8- Fluentui

如何合并和使用 Fluent UI Blazor。

## 库、存储库、工具等。

### keithwill/VestPocket
https://github.com/keithwill/VestPocket

AOT 的简单的基于文件的数据存储。

- [VestPocket：AOT .NET 应用程序的基于文件的数据存储](https://khalidabuhakmeh.com/vestpocket-file-based-data-storage-for-aot-dotnet-applications)

### JonPSmith/EfCore.SchemaCompare：用于将 EF Core 数据库模型与数据库架构进行比较的库。
https://github.com/JonPSmith/EfCore.SchemaCompare

基于 Entity Framework Core 模型的架构比较库。

### 调试输出过滤器 - Visual Studio Marketplace
https://marketplace.visualstudio.com/items?itemName=GrantDavies.NiahTextFilter2022

Visual Studio 扩展允许您过滤调试输出并查看历史记录。

https://x.com/mkristensen/status/1726721505193803802?s=12


## 网站、文档等
### 推文

**关于 Win2D 1.27.1 和 Windows App SDK 1.1.1 发布的故事。**

https://x.com/sergiopedri/status/1727279008243482663?s=12

![image-20231201103450297](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231201103450297.png)

---

**服务发现 (Microsoft.Extensions.ServiceDiscovery) 现已在 .NET 8 中提供（不需要 Aspire）。**

https://x.com/david_whitney/status/1726948359523758347?s=12&t=ggvrrZ7oLogHyNoIGNgjbw

![image-20231201103522756](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231201103522756.png)

---

**由于 `ConcurrentDictionary<K,V>.Count` 会加锁，因此在性能方面是不利的，因此如果您只想判断是否为空，则应该使用 IsEmpty。**

https://x.com/steplyakov/status/1727016474211176784?s=12&t=ggvrrZ7oLogHyNoIGNgjbw

![image-20231201103559070](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231201103559070.png)

---

**在会议上，他说他正在创建一个工具来可视化和演示 GC 的运动。**

https://x.com/kookiz/status/1726262030418481643?s=12&t=ggvrrZ7oLogHyNoIGNgjbw

![image-20231201103630242](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231201103630242.png)

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
