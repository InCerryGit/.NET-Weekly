## 国内文章

### 用最清爽的方式开发dotNet

https://www.cnblogs.com/ncellit/p/17881779.html

本文介绍了如何以清爽的方式开发dotNet应用，特别是简单的API。作者推荐使用.Net6的miniapi，提供了官方文档链接，并分享了基于国内实际情况的个人方法。这包括创建一个企业官网API，涉及数据库操作、授权鉴权、Swagger文档和文件上传。作者建议引入必要的组件，如Swashbuckle.AspNetCore和SqlSugarCore，并强调根据需求添加组件以避免冗余。还提到了将控制台项目转换为Web项目的步骤，并展示了如何在`Program.cs`中设置项目，包括上传大小限制、授权鉴权和Swagger配置。

### C#/.NET/.NET Core优秀项目和框架2023年11月简报

https://www.cnblogs.com/Can-daydayup/p/17873700.html

本文介绍了公众号“追逐时光者”定期分享的C#/.NET/.NET Core优秀项目和框架，包括项目介绍、功能特点和源码地址。CAP是一个轻量级的.NET库，用于处理分布式事务和EventBus功能，有助于构建可扩展的微服务系统。ZEQP.WMS是一个支持多操作系统的仓储管理系统，基于.Net Core 3.1和Colder.Admin.AntdVue框架开发。HandyControl是一套WPF控件库，提供80多款自定义控件，易于创建美观的WPF应用程序。这些资源有助于开发者提高开发效率和项目质量。

### .NET使用分布式网络爬虫框架DotnetSpider快速开发爬虫功能

https://www.cnblogs.com/Can-daydayup/p/17884311.html

本文介绍了DotnetSpider，一个.NET平台下的轻量级、高性能网络爬虫框架。它支持异步操作，通过内存型消息队列实现组件解耦，可配置为分布式爬虫。文章还指导如何使用DotnetSpider爬取博客园文章信息，并保存至文本文件。

### TIOBE 12月榜单: C# 即将成为2023 年度编程语言

https://www.cnblogs.com/shanyou/p/17892164.html

TIOBE在2023年12月公布了编程语言排行榜，C#有望成为年度编程语言，因为它在一年内增长了2.38%，而竞争对手Fortran和F#的增长远低于此。C#与Java的差距也在缩小，12月份仅相差0.69%。C#的优势在于能高效对接C和C++代码，尤其是在.NET 8的NativeAOT支持下。北京将举办.NET Conf Local Event，主题为“智能 开源 安全”，探讨.NET在开源领域的发展。会议还将讨论.NET云原生开发，特别是Aspire和Dapr的关系及其在云原生开发中的应用。

### 博客园又崩了，这个锅要不要阿里云背？

https://www.cnblogs.com/bossma/p/17889457.html

本文分析了博客园频繁崩溃的原因。博客园近期多次遭遇数据库CPU使用率100%的故障，官方怀疑是参数嗅探问题导致SQL Server缓存了低效的执行计划。博客园使用SQL Server和存储过程，这在.NET技术体系中较为常见。尽管SQL Server作为商业数据库性能可靠，但在特定参数下可能导致查询效率低下。博客园未能定位具体问题SQL，导致问题持续存在。有观点认为SQL Server性能优于MySQL，但博客园的问题可能与SQL Server本身或阿里云服务有关。

### .NET8极致性能优化AOT

https://www.cnblogs.com/tangyanzhi1111/p/17876898.html

本文讲述了.NET8中对AOT（Ahead-of-Time）编译的性能优化。AOT允许.NET源码通过ILC编译器直接编译成原生二进制代码，无需JIT（Just-In-Time）编译。优化的重点是减少AOT生成的可执行文件大小，例如在.NET8中，一个ASP.NET应用程序的AOT文件大小从.NET7的13MB减少到1.5MB。进一步优化可以通过配置csproj文件，如设置优化偏好为体积、启用不变全球化和关闭堆栈跟踪支持，使文件大小进一步减小到1.2MB。除了体积优化，.NET8还改进了AOT编译器内部和单个库的性能，如HttpClient，并支持BenchmarkDotNet进行性能测试，显示出AOT的性能提升。

### 聊一聊 .NET高级调试 中的一些内存术语

https://www.cnblogs.com/huangxincheng/p/17874509.html

本文解释了Windows内存管理的几个关键术语。Virtual Size是预定和提交地址的总和，可以通过测试代码和工具对比验证。Working Set指物理内存条上的内存，包括独占和共享两部分。Private Bytes是WS Private和换页内存的总和，对分析内存泄露有帮助。通过实验代码，作者展示了换页内存的计算和pagefile.sys的使用情况。WS Shared是实际被共享的内存页集合，与WS Shareable（可共享的内存页集合）不同。

### 自己写个网盘系列：① 来学习开启这个项目吧

https://www.cnblogs.com/Start201505/p/17892327.html

本文介绍了作者使用.NET 8开发的Simple Framework快速开发框架，以及如何利用该框架创建一个个人网盘项目。框架特点是简化开发流程，支持多数据库，包含基础库和多个扩展库。作者计划通过实战项目教授项目对接、编码、完善和部署。网盘项目旨在实现基本的文件管理功能，支持在线预览编辑，多用户隔离，以及在家部署使用。项目模拟了多个角色的合作，包括项目经理、前端开发、后端开发和运维，并使用了现成的前端页面进行对接。

### ML.NET 3.0 增强了深度学习和数据处理能力

https://www.cnblogs.com/shanyou/p/17878059.html

.NET团队于2023年11月28日发布ML.NET 3.0，强调深度学习和数据处理的重要性，使开发者能在.NET生态中创建AI应用。ML.NET 3.0通过CLI和模型生成器等工具，支持开发者使用C#和F#构建和集成自定义ML模型。深度学习方面，新增了对象检测、命名实体识别和问答功能，特别提出了TorchSharp支持的对象检测API。数据处理方面，DataFrame和IDataView功能得到增强，改进了数据加载、转换和可视化步骤。未来，开发团队计划发布.NET 9和ML.NET 4.0，继续扩展深度学习场景和DataFrame集成。更多信息可查看发行说明。

### 七天.NET 8操作SQLite入门到实战 - 第六天后端班级管理相关接口完善和Swagger自定义配置

https://www.cnblogs.com/Can-daydayup/p/17880839.html

本文讲述了如何在.NET后端框架中使用SQLite-net ORM，并设计班级管理的数据库表。作者首先封装了SQLiteHelper，然后介绍了班级表和班级学生表的字段设计，包括班级ID、名称、创建时间以及学生ID、姓名、年龄、性别等。接着，展示了对应的班级管理模型SchoolClass和Student，并提供了项目源码地址。最后，文章强调了完善后端班级管理接口和自定义Swagger配置的重要性。

### 基于DotNetty实现自动发布 - 通信实现

https://www.cnblogs.com/broadm/p/17875559.html

本文介绍了基于DotNetty的通信实现，DotNetty是微软Azure团队开发的.NET网络库。项目OpenDeploy.Communication类库包含编码解码模块和定义通信约定。自定义消息格式NettyMessage包括消息头NettyHeader和消息体Body，消息头包含唯一标识、是否同步、终结点等信息，可序列化为JSON。编码器和解码器分别负责将NettyMessage转换为字节流和从字节流中恢复NettyMessage。

### 构建一个语音转文字的WebApi服务

https://www.cnblogs.com/hejiale010426/p/17881978.html

本文讲述了如何构建一个将语音转换为文字的WebApi服务。首先，使用Vscode创建WebApi项目，添加必要的Whisper.net依赖包。然后，下载模型和语音示例文件，将其复制到项目目录。接着，创建WhisperService.cs处理音频文件并返回识别结果。最后，修改Program.cs注册服务并构建API。服务完成后，通过控制台命令运行并体验，不同显卡的耗时有所差异。

### C#中的并行处理、并行查询的方法你用对了吗？

https://www.cnblogs.com/hanbing81868164/p/17876423.html

本文介绍了Parallel.ForEach和AsParallel两种并行编程工具。Parallel.ForEach能够在多核处理器上并行执行集合的迭代操作，简化并行编程，适用于简单循环。AsParallel是LINQ的方法，能将查询操作并行化，适合复杂的LINQ查询。两者的性能取决于任务类型和数据规模，Parallel.ForEach适合直接的集合迭代，而AsParallel适合需要筛选和映射的复杂查询。在实际应用中，应根据任务需求选择合适的并行工具。

### AgileConfig 1.8.0 已适配 .NET8

https://www.cnblogs.com/kklldog/p/agileconfig-up-to-net8.html

本文讲述了作者将AgileConfig项目升级到.NET8的经验。首先，作者更新了项目的目标框架和所有nuget包，解决了一个弃用包的问题。然后，修改了dockerfile以适应.NET8。在本地和docker desktop环境中运行正常，但服务器上出现了兼容性错误，通过添加特定参数解决。作者总结.NET接口稳定，升级过程简单，但新的runtime镜像可能与旧版docker engine不兼容。文末提供了项目的GitHub和Gitee地址，并邀请关注公众号。

### .NET企业应用安全开发动向-概览

https://www.cnblogs.com/xiyuanMore/p/17893362.html

本文探讨了安全的重要性和安全开发的概念，提出了从全局视角识别和防范安全问题的必要性。通过分析近期互联网大厂的安全事故，强调了从教训中学习的重要性，并概述了内容、数据、设备和行为四个安全维度。文章还介绍了.NET的安全基础设施和威胁建模分析方法，强调了随着技术发展，新的安全挑战也随之而来。作者通过分享个人思考和经验，鼓励开发者建立体系化的安全思考框架，并在.NET Conf China上进一步探讨这些问题。

### .net 温故知新【15】：Asp.Net Core WebAPI  配置

https://www.cnblogs.com/SunSpring/p/17879703.html

本文讲述了Asp.Net Core中配置的概念和实践。主机配置是项目启动时的配置，应用程序配置是运行时的配置。默认主机配置优先级为命令行、DOTNET_环境变量、ASPNETCORE_环境变量，且部分变量在启动时锁定。launchSettings.json文件用于本地开发环境配置。默认应用程序配置优先级为命令行、环境变量、用户机密配置、appsettings.{Environment}.json、appsettings.json和主机配置。配置提供程序负责读取这些配置。机密管理器工具用于存储开发环境中的敏感配置，不在项目目录下。

### CoreFlex框架发布 `0.1.1`

https://www.cnblogs.com/hejiale010426/p/17893528.html

本文介绍了CoreFlex框架，支持.NET 6、.NET 7和.NET 8，集成MasaFramework，提供企业级应用开发和Blazor的JS工具库。框架目标包括JS操作、Serilog日志、限流、审计日志、虚拟文件、系统设置、后台任务和ChatGpt客户端案例等模块。Core Flex模块是框架基础，支持模块化和自动依赖注入。使用时，通过NuGet安装包，创建模块需继承CoreFlexModule类，实现生命周期方法，并可添加依赖其他模块的特性。CoreFlex.Razor.JsInterop是JS工具库，提供Cookie和LocalStorage/SessionStorage操作API。

### Net 高级调试之十二：垃圾回收机制以及终结器队列、对象固定

https://www.cnblogs.com/PatrickLiu/p/17874330.html

本文是《Net 高级调试》系列的第十二篇，深入介绍了GC垃圾回收算法、根对象概念及其存在区域、带析构函数对象的回收机制、终结器队列与线程的作用，以及大对象堆的回收策略。文章强调了对.Net框架底层的理解对调试的重要性，并提供了调试环境的详细说明。通过实际代码的调试过程，验证了理论知识，帮助读者更深入地理解对象的生命周期和GC的工作原理。

### c# 高并发必备技巧（三）

https://www.cnblogs.com/pzscit/p/17880912.html

本文讨论了高并发场景下的技术策略。介绍了异步编程以避免阻塞，多线程和线程池以提高效率并控制资源使用。并行编程可同时执行多任务，数据流编程则适合大数据处理。强调了内存管理的重要性，提倡使用并发集合和优化数据库访问，如使用缓存和连接池。最后，建议根据实际需求选择合适的优化策略。

## 主题

### Rider 2023.3：支持 .NET 8 SDK、C# 12 的最新版本、性能增强、预测性调试以及更多 AI 驱动的功能。 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/12/07/rider-2023-3-release/

### ReSharper 2023.3：支持 C# 12、性能增强和更多 AI 驱动的功能 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/12/07/resharper-2023-3-release/

### dotCover、dotMemory、dotPeek 和 dotTrace 2023.3 发布 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/12/07/dotcover-dotmemory-dotpeek-and-dottrace-2023-3-release/

### BenchmarkDotNet v0.13.11 · dotnet/BenchmarkDotNet · 讨论 #2479
https://github.com/dotnet/BenchmarkDotNet/discussions/2479

### 2.7.10 版 · StackExchange/StackExchange.Redis
https://github.com/StackExchange/StackExchange.Redis/releases/tag/2.7.10

### 发布 v8.0.1 · npgsql/npgsql
https://github.com/npgsql/npgsql/releases/tag/v8.0.1

### 版本 11.0.6 · AvaloniaUI/Avalonia
https://github.com/AvaloniaUI/Avalonia/releases/tag/11.0.6

### 发布 v1.5-experimental1 · microsoft/WindowsAppSDK
https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.5-exp1

- [在 WinAppSDK 1.5-experimental1·microsoft/microsoft-ui-xaml 中发布 WinUI 3](https://github.com/microsoft/microsoft-ui-xaml/releases/tag/winui3/release/1.5-experimental1)
- [Windows App SDK 实验性发布通道 - Windows 应用](https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/experimental-channel#version-15-experimental-150 -实验1)

### .NET 8 网络改进 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-8-networking-improvements/

### 使用 .NET 将 WebAssembly 扩展到云 - .NET 博客
https://devblogs.microsoft.com/dotnet/extending-web- assembly-to-the-cloud/

### .NET Conf 2023 回顾 - 庆祝社区、创新和 .NET 8 的发布 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-conf-2023-recap-videos-slides-demos-and-more/

### .NET 8 的 Qdana 即将准备就绪！尝试 EAP，让我们知道您的想法 |科达纳博客
https://blog.jetbrains.com/qodana/2023/12/qodana-for-net-8-is-almost-ready-try-the-eap-and-let-us-know-what-you-think/


## C# 2023 年降临节日历

### [.NET8]在真正的BlazorWebApp上加上巧克力制作PWA-Qiita
https://qiita.com/nr_ck/items/f22c24c0583309577a5e

### C#12.0.NET8.0中Utf8字符串的制作方法和性能研究
https://gitan.dev/?p=320

### 在MVVM中，简洁地使用INotifyPropertyChanged。带代码sunipto。-Qiita
https://qiita.com/hiro_t/items/556868bc6d1f5fd53a6f

#### 用C#写的让自制键盘方便一点的工具
https://blog.alglab.net/archives/csharp-prkkeymap/

### 在NET SDK8.0中尝试PublishTrimmed时可能会失败的话-Qiita
https://qiita.com/skitoy4321/items/c6ae2b58245b6874ec35

### 试着制作了简单HTTP Server（C#编）-Qiita
https://qiita.com/t0r/items/ef2fa3ae15af592e8674

### 迷宫般的if文秒变漂亮的魔法[C#，元组，模式匹配ngu]-Qiita
https://qiita.com/hysui/items/ea0b00788f98cbb15980

### [C#] 让我们编写不安全的代码 - Annulus Games
https://annulusgames.com/blog/unsafe/

### 记录 StackTrace 时，追溯添加异常 - Qiita
https://qiita.com/up-hash/items/47feaf9dbd94763431d7

### 与整个团队一起努力编写最新的 C# - Qiita
https://qiita.com/wipiano/items/7fbf5d61d68f29fdbd36

### 使用 C# 的内联汇编器 - Qiita
https://qiita.com/up-hash/items/8e9e18c55d23686b2eb1

### 将前缀添加到使用 Microsoft.Extensions.Configuration.Json 读取的配置值
https://zenn.dev/guil/articles/dfdcba6a7f4636

### 无法重新分配的 const 变量风味（小故事）- Qiita
https://qiita.com/up-hash/items/8eb07cdace041896e3e8

### 【C#】我思考抽象类和接口一起使用的原因 - Qiita
https://qiita.com/seiya2130/items/6c639efadbfcb279e4ed

### 在 ExcelDNA 中使用 async/await - Qiita
https://qiita.com/hiro_t/items/f37256a59946c6c0faa7

### [C#] 像 StringBuilder 一样使用 DefaultInterpolatedStringHandler - TekuMemo
https://aneuf.hatenablog.com/entry/2023/12/12/000000

### C# Boost、DotNext 库 - Qiita
https://qiita.com/up-hash/items/059975d06347b81087de

### 让我们尝试使用 Roslyn API！概述 - Qiita
https://qiita.com/lx-sasabo/items/d3791b305d85bb686ae4

### 关于使用 C# TimeProvider (.NET8) - Qiita
https://qiita.com/sh1ch/items/936945705d0c7a4ab655

### 让我们使用 ISpanFormattable - Qiita
https://qiita.com/Shaula/items/563ef337ae578ceebede


## 文章、幻灯片等
### 在 Azure Blob 存储中创建 Zip 文件
https://markheath.net/post/create-zip-files-in-blob-storage

### [Blazor]使用 BECanvas 进行绘图处理 - Qiita
https://qiita.com/onsen_koichi/items/a0d9a88254eec34c1afc

### 即使与 .NET Framework 一起使用 C# 的最新功能 - Qiita
https://qiita.com/diontools/items/2d5625419bb4f43da1a5

### 使用 VSCode 构建 .NET MAUI 开发环境 - Qiita
https://qiita.com/aqua_ix/items/ba9533d60633abe4c850

### [C#] 根据合成语音软件的时序信息文件（.lab）创建字幕文件（.srt）
https://zenn.dev/inuinu/articles/07ea814ca573c1

### 使用 SkiaSharp 绘制地图 - Qiita
https://qiita.com/ingen084/items/8c4492bfb3cc50129507

### .NET Conf Japan 2023“.NET + AI”补充文章
https://zenn.dev/chomado/articles/231219-dot-net-conf

### .NET Native AOT 解释 - NDepend 博客
https://blog.ndepend.com/net-native-aot-explained/

### 语义内核（RC-3 版本）用日语运行 Hello World
https://zenn.dev/chomado/articles/231207-semantic-kernel-rc3

### Snyk 能检测出这么多漏洞吗？（C#/.NET 版）- Qiita
https://qiita.com/akid3020/items/df2fed5ecfd1ec9e4d33

### 通过新的初学者视频学习 .NET 8 - .NET 博客
https://devblogs.microsoft.com/dotnet/learn-dotnet8-beginner-videos/

### 在非 UWP 环境中使用 Windows.Data.Pdf
https://zenn.dev/nuits_jp/articles/2023-12-06-use-windows-data-pdf-out-of-uwp

### 使用 .NET 对 PDF⇒JPEG 转换进行基准测试
https://zenn.dev/nuits_jp/articles/2023-12-06-pdf-to-jpeg-benchmarks

### 介绍使用 Source Generator 和 Rider 创建工具的流程 - Qiita
https://qiita.com/Tanakancolle/items/b12c48e0cf0fe78af2ad

### 通过项目解耦优化.NET解决方案架构以加快编译速度
https://dev.to/asimmon/optimizing-net-solution-architecture-for-faster-compilation-through-project-decoupling-5eg6

### [.NET 8] 使用 MVVM 创建的 Blazor Web 应用程序 - Qiita

https://qiita.com/nr_ck/items/6faa86c5e381fb96c67a

### 使用 [TagProvider] 和 ILogEnricher 丰富日志
https://andrewlock.net/customising-the-new-telemetry-logging-source-generator/

### .NET Aspire
https://henriquesd.medium.com/net-aspire-296e24b952c0

### 滚动以展开文档选项卡 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/scroll-to-expand-document-tabs/

### 使用 Rider 的预测调试器再次展望未来 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/12/04/another-look-into-the-future-with-riders-predictive-debugger/

### ASP.NET Core 8 中的全局错误处理
https://dev.to/milanjovanovictech/global-error-handling-in-aspnet-core-8-2mki

### 如何使用 .NET8 Application Insights 在时间线上显示跟踪/信息日志 - Qiita
https://qiita.com/Hydrangeas/items/bca8ecc5d5cb0f14a37c

### 使用键控服务的依赖注入终于出现在 ASP.NET 中
https://blog.elmah.io/dependency-injection-using-keyed-services-is-finally-in-asp-net/

### .NET 8.0 如何将 JSON Schema 性能提高 20% | endjin
https://www.endjin.com/blog/2023/12/how-dotnet-8-boosted-json-schema-performance-by-20-percent-for-free

### 将环境变量添加到 .NET Aspire 服务
https://timheuer.com/blog/add-environment-variables-to-aspire-services/

### 如何使库与本机 AOT 兼容 - .NET 博客
https://devblogs.microsoft.com/dotnet/creating-aot-兼容-libraries/

### \e（转义字符转义序列）
https://ufcpp.net/blog/2023/12/escape-escape/

### 使用 Testcontainers 和 .NET 测试 Typesense 搜索
https://khalidabuhakmeh.com/testing-typesense-search-with-testcontainers-and-dotnet

### 使用 C# 为 Raspberry Pi 构建裸机可启动游戏
https://migeel.sk/blog/2023/12/08/building-bare-metal-bootable-game-for-raspberry-pi-in-csharp/

### 使用 Husky.NET 进行预提交挂钩 - 在 Git 提交之前构建、格式化和测试您的 .NET 应用程序
https://dev.to/bellonedavide/pre-commit-hooks-with-huskynet-build-format-and-test-your-net-application-before-a-git-commit-3cbd

### 使用 Microsoft.Extensions.Compliance.Redaction 编辑日志中的敏感数据
https://andrewlock.net/redacting-sensitive-data-with-microsoft-extensions-compliance/

### 将硬件内在函数与 .NET Native AOT 结合使用
https://zenn.dev/naminodarie/articles/dotnet_native_aot_i

### .NET 带注释的月刊 | 2023 年 12 月 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/12/11/net-annotated-monthly-december-2023/

## 库、存储库、工具等。

### GitHub Actions - Visual Studio Marketplace
https://marketplace.visualstudio.com/items?itemName=TimHeuer.GitHubActionsVS

https://x.com/timheuer/status/1731011137389695140?s=12

![image-20231213224233925](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231213224233925.png)


## 网站、文档等
### 推文

https://x.com/aaronontheweb/status/1731500517816201611?s=12

![image-20231213224321452](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231213224321452.png)

## 版权声明

* 国内板块由 InCerry 进行整理 : https://github.com/InCerryGit/WeekRef.NET
* 其余内容来自 Myuki WeekRef，由InCerry翻译（已获得授权） : https://github.com/mayuki/WeekRef.NET

**由于笔者没有那么多时间对国内的一些文章进行整理，欢迎大家为《.NET周刊-国内文章》板块进行贡献，需要推广自己的文章或者框架、开源项目可以下方的项目地址提交Issue或者在我的微信公众号私信。**

格式如下：

* 10~50字左右的标题
* 对应文章或项目网址访问链接
* 200字以内的简介，如果太长会影响阅读体验

https://github.com/InCerryGit/.NET-Weekly