## 国内文章
### 史诗级警报：ASP.NET Core 被曝 CVSS 9.9 分漏洞，几乎所有.NET 版本无一幸免！

https://www.cnblogs.com/netry/p/19147223/CVE-2025-55315

2025年10月的微软补丁星期二更新中，ASP.NET Core 漏洞 CVE-2025-55315 引起关注，其 CVSS 评分为9.9，预示重大风险。这个漏洞涉及HTTP请求走私，允许攻击者绕过安全检查。受影响的.NET版本包括.NET 10、9、8及老版本.NET Core 2.x。微软明确指出，没有缓解措施，唯一修复方案是升级到最新SDK版本或更新NuGet包引用。漏洞危害严重，开发者需高度重视。此文章提供了详细的漏洞解析和修复指引。官方链接也提供了更多信息。

### .NET 10 Release Candidate 2(RC2)发布

https://www.cnblogs.com/shanyou/p/19142462

.NET 团队发布了 .NET 10 RC2，此版本为长期支持版本，提供三年支持。RC2 是正式版前的最终候选，已具备生产环境可用性。其主要更新包括JIT编译器优化、支持AVX10.2硬件加速、JSON序列化增强和安全性改进。ASP.NET Core与Blazor也有重大提升，如组件状态持久化和API开发的强化。跨平台支持方面，MAUI和WPF增加了新功能。开发工具链标准化，支持容器化，提升了效率。此版本适合生产环境部署，建议关注官方动态以获取最新信息。

### 从零开始：如何用 C# 开发一款媲美 “AnyTxt” 的文件内容搜索工具

https://www.cnblogs.com/luojin765/p/19145746

本文章介绍了一个基于C#开发的开源全文搜索工具TDSContent，旨在弥补现有工具AnyTxt的不足。TDSContent具备快速检索及对多种文档类型的支持，采用Lucene.Net作为索引架构，并实现了多种格式的解析器，包括PDF、docx、pptx等。文章详细分析了与AnyTxt的对比，突出TDSContent的技术优势。同时，讨论了索引的实时性和文件内容的敏感性问题，强调软件安全性。整个项目已完全开源，力求提升文档管理的效率与安全。

### 使用 Visual Studio 快速创建 NuGet 程序包并发布到 NuGet 官网

https://www.cnblogs.com/Can-daydayup/p/19142268

本文讲解如何将 .NET EF Core 通用仓储类库打包为 NuGet 包并发布到 NuGet 官网。教程中使用 Visual Studio 2022 和 .NET CLI 工具指导用户从注册账号到生成和发布 NuGet 包的每个步骤。内容包括创建 API 密钥、配置包属性、生成 NuGet 包的方法，并提供了在项目中引入和使用 NuGet 包的示例代码。文章链接到相关资源，便于读者进一步学习。

### 【EF Core】FromExpression 方法有什么用？

https://www.cnblogs.com/tcjiaan/p/19136951

本文主要探讨了 DbContext 类中的 FromExpression 方法及其用法。首先，介绍了该方法的签名及返回类型，强调其可用于 LINQ 查询。通过分析方法参数，说明了如何利用此方法在一开始就返回经过筛选的查询，从而避免多次执行 SQL 语句，提升效率。此外，适用场景还包括从表值函数返回数据的情况。最后，给出了一个示例，包含了一个实体类的定义及 DbContext 的继承，深度介绍了其实际应用。

### 为 .NET 10 GC(DATAS)做准备

https://www.cnblogs.com/InCerry/p/19146679

本文讨论了.NET 9和.NET 10中的DATAS功能，重点在于性能特性及内存管理的变化。DATAS旨在动态适应应用程序大小，但不是所有场景适用。文章建议开发者在升级后检查应用性能指标，并决定是否关闭DATAS。作者提供了在特定场景下调优DATAS的实例，并解释了如何选择和实现GC性能功能。DATAS适合在内存限制环境和小型负载下使用，作者提醒开发者考虑如何有效利用内存。

### ASP.NET Core Blazor简介和快速入门一(基础篇)

https://www.cnblogs.com/shenchuanchao/p/19142586

Blazor是Microsoft开发的开源Web UI框架，基于.NET，可以使用C#和HTML创建单页应用程序。Blazor有两种托管模型：Blazor Server和Blazor WebAssembly。Blazor Server在服务器端运行，依赖SignalR进行实时交互，具有较小的下载量和快速加载速度，但不支持离线工作。Blazor WebAssembly在客户端直接运行，能够充分利用客户端资源，支持独立部署并能在无服务器环境中运行。Blazor适合各种现代浏览器，提供开发人员以高效开发工具和强大功能。

### 使用Scalar.AspNetCore来管理你的OpenApi

https://www.cnblogs.com/wangbin5542/p/19148516

本文介绍了Scalar组件在ASP.NET Core中的集成使用，提供了官方文档链接和GitHub地址。作者分享了简单使用、基本配置和高级配置的步骤，包括创建API项目、添加所需包、配置路由和自定义文档。注意到新版2.9.0后增加了编辑配置的功能，用户可自由保存调试后的配置，强调了主题自定义等功能。整体结构清晰明了，适合开发者学习。

### 多智能体微服务实战(1/4)：康威定律在 AI 时代的应用

https://www.cnblogs.com/madtom/p/19140138

本文探讨了多智能体协作在现代项目管理中的必要性。传统项目管理面临信息孤岛、沟通成本高和响应速度慢等问题。单一AI助手无法满足企业的专业需求，因为缺乏行业特定的理解和灵活性。多智能体微服务的理念能够确保各专业团队集中各自的知识与技能，有效应对项目挑战。利用康威定律，企业组织结构与智能体系统结构的映射能够实现更高效的协同工作。文章强调了通过专业分工来提升项目管理的效果。

### 从零开始:C# 解析docx提取文本-无需安装office软件且完美支持aot

https://www.cnblogs.com/luojin765/p/19147754

本文介绍了docx格式的概念和使用Open XML SDK来解析该格式文件的方法。docx文件基于XML，使用zip压缩，便于存储和传输。Open XML SDK简化了开发人员对Office Open XML文件的操作，无需安装Office软件即可进行文本提取。文章详细描述了如何使用WordprocessingDocument类提取文档内容，包括段落、表格及批注的处理。文章还附带了示例代码，适合开发者参考和实践。

### .NET 10中GC(垃圾收集器)默认启用DATAS

https://www.cnblogs.com/shanyou/p/19144782

.NET GC的大总管Maoni发布的文章介绍了.NET 10的GC特性。新版本重点在于代码优化、配置预留和环境兼容。DATAS功能默认启用，旨在根据应用程序实际大小动态调整堆，以提高内存效率并减少GC压力。虽然在内存紧张的环境中效果显著，但在吞吐量要求高的场景下可能不适用。用户需要根据应用需求调整配置，并评估是否启用DATAS，以优化性能。文章提供了调优建议和监控分析工具的使用。

### C#/.NET/.NET Core技术前沿周刊 | 第 57 期(2025年10.1-10.12)

https://www.cnblogs.com/Can-daydayup/p/19142317

本文介绍了C#/.NET/.NET Core领域内的技术动态和资源，包括AutoMapper的替代品Mapster，以及MAUI UI组件库、任务调度框架.NET Aspire等。各项技术与工具不仅提升了开发效率，还增强了项目的功能和视觉体验。此外，文章涵盖了开发者如何在.NET环境中审查AI生成的代码，为开发者提供了新的视角和挑战。

### WPF应用绑定系统快捷键

https://www.cnblogs.com/mingupupu/p/19145116

全局快捷键功能提升用户体验，允许用户通过特定键盘组合快速触发应用功能。本文介绍WPF应用中的全局键盘钩子实现，利用Windows API监听系统级键盘事件。首先，导入必要API函数，包括设置和卸载钩子，以及获取模块句柄。这些函数的详细用途和参数说明清晰呈现，并强调了在代码中的具体应用，确保资源的正确管理。通过对函数的逐一解析，读者能够理解如何有效实现全局快捷键的绑定与处理。

### .NET运行时核心仓库的治理架构解析：责任分配与协作机制

https://www.cnblogs.com/shanyou/p/19150635

这份文档是dotnet/runtime仓库的核心治理文件，详细定义区域划分和责任分配。它阐述了Pull Request和Issue的标签策略，强调扁平化协作。文档涉及多个技术领域，包括编译器、运行时组件和诊断工具，标明了各个领域的责任人。特别指出，编辑文档不会自动更新配置，保障可读性与安全性。文中还提到了一些归档组件，变更会受到限制。此外，列出操作系统支持和处理器架构的负责人。

### Roslyn 技术解析：如何利用它做代码规范检查与运行时代码生成？

https://www.cnblogs.com/yuxl01/p/19142945

本文介绍了Roslyn，C# .NET的编译平台。Roslyn利用C#编写，能够将C#和VB.NET源码编译为IL代码。文章简述了C#的编译流程，包括源代码、编译器、IL生成和运行时编译。文中还回答了常见问题，强调Roslyn的限于仅编译C#和VB.NET。作者提到Roslyn的多种应用，如开发Visual Studio插件、静态分析工具和代码生成工具等，并探讨其语法树的解析与分析。整体上，文章尝试让读者了解Roslyn的强大功能及其在开发中的实际应用。

### WPF/C#：使用Microsoft Agent Framework框架创建一个带有审批功能的终端Agent

https://www.cnblogs.com/mingupupu/p/19149202

本文介绍了微软的Agent Framework框架，重点展示如何利用该框架创建一个可以执行终端命令并具备人工审批的WPF应用。讨论了框架的基本功能，包括AI代理和工作流构建，强调了在执行敏感操作时，人工审批的重要性。实例演示了如何通过人工审批来获取时间和新建文件的过程。还包含了GitHub的链接，以及如何安装NuGet包和编写执行命令的函数，为读者提供了实际操作指导。整体上，文章能够结合实例，系统地阐述该框架的应用与实现细节。

### 我来说说读写分离，就是数据库读写分离在ORM中是如何实现的，附上源码

https://www.cnblogs.com/pastespider/p/19143981

文章深入探讨了读写分离的实际问题，指出主从数据库的延迟可能导致读取旧数据。作者强调，不应简单地将所有读取请求指向从库，以避免新用户注册后无法立即登录的情形。通过具体示例，作者展示了如果不妥善处理读写分离，可能引发的连锁问题。此外，文章提供了代码示例，说明如何在用户注册和立即登录时处理数据库操作。整体上，文章旨在引起对读写分离设计的关注和思考。

### 幂等的双倍快乐，你值得拥有

https://www.cnblogs.com/JulianHuang/p/19150319

本文解释了幂等性在软件开发中的重要性，尤其是对于网络不可靠和分布式系统的场景。通过具体示例，讨论了如何避免重复请求的问题，并分享了解决方案，如前端响应机制。文中提到的双将军理论和重试机制深入探讨了工程上的解决思路。具体代码示例展示了如何设计幂等的开户请求。文章内容具有实用性和可读性，适合开发者参考和学习。

### WPF 调用 ChangeWindowMessageFilterEx 修改指定窗口 (UIPI) 消息筛选器的用户界面特权隔离

https://www.cnblogs.com/wuty/p/19142059

这篇文章讨论了WPF进程间通信的问题，特别是在发送普通权限窗口消息时，管理员权限窗口无法接收的问题。文章详细介绍了Windows的受保护模式，强调了自Windows NT6.0引入的UIPI机制。为解决此问题，微软提供了ChangeWindowMessageFilterEx函数，允许开发者控制窗口消息筛选器。文中清晰阐述了函数的语法、参数及其返回值，并提供了使用示例，帮助开发者理解如何实现消息传递。整体而言，文章提供了实用的技术细节，有助于开发者解决特定问题。

### ManySpeech.AliParaformerAsr 使用指南

https://www.cnblogs.com/manyeyes/p/19144047

ManySpeech.AliParaformerAsr是一个语音识别组件，支持多种模型和多个开发环境，包括Windows、macOS和Linux。其底层使用Microsoft.ML.OnnxRuntime进行解码，提供了跨平台和AOT编译特性。安装推荐通过NuGet包管理器，支持Package Manager Console和.NET CLI方式。配置文件asr.yaml的特定参数可调整，以优化识别效果，例如实现逆文本正则化。提供了详细的代码调用方法，适合开发者快速集成。

### 从零开始实现简易版Netty(九) MyNetty 实现池化内存的线程本地缓存

https://www.cnblogs.com/xiaoxiongcanguan/p/19148861

本文介绍MyNetty实现池化内存的线程本地缓存，以提高内存分配效率。前文已经实现Normal和Small规格池化内存，当前阶段将引入线程本地缓存，减少线程间同步竞争。线程本地缓存允许当前线程先尝试使用自己的缓存而非公共PoolArena，显著提升内存分配吞吐量。虽然增加了内存开销，但能改善访问性能。具体实现细节将在后续源码分析中揭示。读者需熟悉系列博文内容，以便更好理解。

### Sql Server安装报错“服务没有及时响应启动或控制请求”

https://www.cnblogs.com/bkyqtr/p/19141193

文章描述了在重装电脑系统后安装SQL Server时遇到的问题，特别是防火墙导致MSSQLSERVER服务无法启动。作者经过多次尝试，发现关闭Windows Defender防火墙后问题得到解决，服务正常启动。最终，安装成功，作者提供了相关解决方案的参考网址，并提醒转载时注明出处。文章内容直观、具体，适合需要解决类似问题的读者。

## 主题

### .NET 和 .NET Framework 2025 年 10 月服务版本更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-and-dotnet-framework-october-2025-servicing-updates/

### 宣布推出 .NET 10 候选版本 2 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-10-rc-2/

### 宣布 Uno 平台和 Microsoft .NET 团队协作
https://platform.uno/blog/announcing-unoplatform-microsoft-dotnet-collaboration/

### 宣布成立 .NET 安全组 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-security-group/

### Visual Studio 中的规划简介(公共预览版) - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/introducing-planning-in-visual-studio-public-preview/

### 宣布在 NuGet.org 上获得赞助 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-sponsorship-on-nugetdotorg-for-maintainer-appreciation/

### 宣布发布 SQL Server Management Studio 22 预览版 3 | Microsoft 社区中心
https://techcommunity.microsoft.com/blog/sqlserver/announcing-the-release-of-sql-server-management-studio-22-preview-3/4461548

## 发布
- [阿瓦洛尼亚UI/阿瓦洛尼亚](https://github.com/AvaloniaUI/Avalonia)
    - [11.3.8](https://github.com/AvaloniaUI/Avalonia/releases/tag/11.3.8)
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [3.7.1144.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1144.0)， [3.7.1145.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1145.0)， [3.7.1146. 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1146.0)、 [3.7.1147.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1147.0)、 [3.7.1148. 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1148.0)、 [3.7.1149.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1149.0)、 [3.7.1150. 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1150.0)， [4.0.112.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.112.0)， [4.0.113.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.113.0)、 [4.0.114.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.114.0)、 [4.0.115.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.115.0)、 [4.0.116.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.116.0)， [4.0.117.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.117.0)、 [4.0.118.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.118.0)
- [Azure/azure-cosmos-dotnet-v3](https://github.com/Azure/azure-cosmos-dotnet-v3)
    - [3.53.2](https://github.com/Azure/azure-cosmos-dotnet-v3/releases/tag/3.53.2)， [3.54.0](https://github.com/Azure/azure-cosmos-dotnet-v3/releases/tag/3.54.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.Monitor.Query.Logs_1.0.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Monitor.Query.Logs_1.0.0)， [Azure.Monitor.Query.Metrics_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Monitor.Query.Metrics_1.0.0)， [Azure.ResourceManager.FrontDoor_1.4. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.FrontDoor_1.4.1) [Azure.ResourceManager.HealthBot_1.2.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.HealthBot_1.2.0)、[Azure.ResourceManager.MongoCluster_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.MongoCluster_1.0.0)， [Azure.ResourceManager.Network_1.13. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Network_1.13.0)， [Azure.ResourceManager.PolicyInsights_1.3. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.PolicyInsights_1.3.0)， [Azure.ResourceManager.ProviderHub_1.2. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ProviderHub_1.2.0)， [Azure.ResourceManager.Qumulo_1.2. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Qumulo_1.2.0)， [Azure.ResourceManager.ResourceGraph_1.1. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ResourceGraph_1.1.0)， [Azure.ResourceManager.Storage_1.6. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Storage_1.6.0)， [Azure.ResourceManager.StorageDiscovery_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.StorageDiscovery_1.0.0)， [Azure.ResourceManager.StorageMover_1.3. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.StorageMover_1.3.0)， [Azure.Storage.DataMovement_12.3. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.DataMovement_12.3.0)， [Azure.Storage.DataMovement.Blobs_12.3. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.DataMovement.Blobs_12.3.0)， [Azure.Storage.DataMovement.Files.Shares_12.3. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.DataMovement.Files.Shares_12.3.0)、[Microsoft.Azure.WebJobs.Extensions.EventHubs_6.5。 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebJobs.Extensions.EventHubs_6.5.3)、[Microsoft.Azure.WebPubSub.Common_1.5。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebPubSub.Common_1.5.0)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.29.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.29.0)
- [dotnet/aspire](https://github.com/dotnet/aspire)
    - [v9.5.2](https://github.com/dotnet/aspire/releases/tag/v9.5.2)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.AIPlatform.V1-3.49.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.AIPlatform.V1-3.49.0)， [ Google.Cloud.AIPlatform.V1-3.50.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.AIPlatform.V1-3.50.0)， [Google.Cloud.AIPlatform.V1-3.51. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.AIPlatform.V1-3.51.0)， [Google.Cloud.AIPlatform.V1-3.52. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.AIPlatform.V1-3.52.0) [谷歌云计算.V1-3.18.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Compute.V1-3.18.0)、[Google.Cloud.Container.V1-3.36。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Container.V1-3.36.0)、[Google.Cloud.DiscoveryEngine.V1-1.11。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.DiscoveryEngine.V1-1.11.0)、[Google.Cloud.Dlp.V2-4.21。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Dlp.V2-4.21.0)、[Google.Cloud.Firestore-3.11。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Firestore-3.11.0)， [Google.Cloud.OracleDatabase.V1-1.4. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.OracleDatabase.V1-1.4.0)、[Google.Cloud.PubSub.V1-3.29。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.PubSub.V1-3.29.0)、[Google.Cloud.Spanner-5.4。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Spanner-5.4.0)、[Google.Cloud.Storage.Control.V2-1.5。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Storage.Control.V2-1.5.0)、[Google.Cloud.TextToSpeech.V1-3.16。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.TextToSpeech.V1-3.16.0)、[Google.Cloud.WebRisk.V1-2.8。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.WebRisk.V1-2.8.0)、[Google.Maps.RouteOptimization.V1-1.3。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Maps.RouteOptimization.V1-1.3.0)
- [grpc/grpc](https://github.com/grpc/grpc)
    - [v1.76.0](https://github.com/grpc/grpc/releases/tag/v1.76.0)
- [微软/CsWin32](https://github.com/microsoft/CsWin32)
    - [v0.3.217](https://github.com/microsoft/CsWin32/releases/tag/v0.3.217)， [v0.3.228](https://github.com/microsoft/CsWin32/releases/tag/v0.3.228)
- [microsoft/WindowsAppSDK](https://github.com/microsoft/WindowsAppSDK)
    - [v1.7.5](https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.7.5)， [v1.8.2](https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.8.2)
- [open-telemetry/opentelemetry-dotnet-contrib](https://github.com/open-telemetry/opentelemetry-dotnet-contrib)
    - [Exporter.Instana-1.0.4](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/Exporter.Instana-1.0.4)， [Instrumentation.Runtime-1.13. 0](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/Instrumentation.Runtime-1.13.0)
- [testcontainers/testcontainers-dotnet](https://github.com/testcontainers/testcontainers-dotnet)
    - [4.8.0](https://github.com/testcontainers/testcontainers-dotnet/releases/tag/4.8.0)

## 文章、幻灯片等
### Blazor Server SignalR：扩展到 10,000 个用户
https://amarozka.dev/blazor-server-signalr-scale-10000-users/

### 读取 ZString
https://qiita.com/kuto110/items/17b9c550e88c53678403

- [让我们读一下 ZString (1)](https://qiita.com/kuto110/items/189cf89d26350fad800f)
- [让我们阅读 ZString (2) 初始提交](https://qiita.com/kuto110/items/541846a10b9a72890744)
### 即将登陆 Rider 2025.3：监控工具窗口中的 ASP.NET 和数据库问题检测 | .NET Tools 博客
https://blog.jetbrains.com/dotnet/2025/10/20/rider-2025-3-asp-dotnet-and-database-issue-monitoring/

### Microsoft Entra ID 的应用角色方法可以轻松控制 ASP.NET Core 中的页面访问
https://zenn.dev/zead/articles/entraid-approle

### 本周项目：.NET 运行时
https://dev.to/pullflow/project-of-the-week-net-runtime-26n4

### 《独光 ASP.NET Core》回顾
https://qiita.com/Fujiwo/items/e00b8fb16c4b85b24ee4

### 了解 Microsoft 代理框架 (C#) 第 11 部分 了解代理
https://zenn.dev/microsoft/articles/agent-framework-011

### 将元数据添加到 ASP.NET Core 中的回退端点
https://andrewlock.net/adding-metadata-to-fallback-endpoints-in-aspnetcore/

### 分解和理解 C# 中的 async/await - 我尝试创建自己的事件循环和 SynchronizationContext 机制
https://zenn.dev/luxiar/articles/fa5206b1968037

### 使用 aspnet-client-validation 实现核心 MVC ASP.NET 的客户端验证
https://zenn.dev/zead/articles/aspnet-client-validation

### 在 .NET 中使用 Silhouette 中的分析器函数钩子
https://minidump.net/using-function-hooks-with-silhouette/

### 从 EFCore 更改为 Dapper 考虑
https://qiita.com/Mitsuki0003/items/ddef5c928dce498927c1

### [C#/.NET] AI 代理开发教程，使用 Microsoft 代理框架
https://qiita.com/Fujiwo/items/d31902e622fc1e915135

### BoldSign 如何利用 JetBrains dotUltimate 实现大规模开发现代化 | .NET Tools 博客
https://blog.jetbrains.com/dotnet/2025/10/23/how-boldsign-modernized-development-at-scale-with-jetbrains-dotultimate/

### 在 .NET AI 聊天应用中升级到 Microsoft Agent Framework - .NET 博客
https://devblogs.microsoft.com/dotnet/upgrading-to-microsoft-agent-framework-in-your-dotnet-ai-chat-app/

### 实现 Visual Studio 扩展兼容性现代化：扩展开发人员和用户轻松迁移 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/modernizing-visual-studio-extension-compatibility-effortless-migration-for-extension-developers-and-users/

### . 我创建了一个程序，将 NET8 和 Azure AI Foundry 的 Sora 2 生成的视频自动上传到 YouTube。
https://zenn.dev/ymd65536/articles/sora_youtube_upload

### 第 3 部分：使用 VSCode 修复和调试 C# 容器环境中的 Blazor Web 应用 - Qiita
https://qiita.com/eyesworks/items/0f5af5a369468dedbed3

### 我尝试了 .NET Aspire 9.5
https://zenn.dev/mck9595/articles/ce4474aba727f7

### 让我们来看看 Microsoft 代理框架 (C#) 第 10 部分：具有持久函数的工作流
https://zenn.dev/microsoft/articles/agent-framework-010

### 第 4 部分：在容器环境中反映自动构建和修复以及部署前验证到 AWS Fargate - Qiita
https://qiita.com/eyesworks/items/0553e6bb3dcf5a219358

### [C#] 在 Blazor 中使用 tailwindcss [轻松]
https://zenn.dev/arika/articles/20251016-tailwind-in-blazor

### 在 Azure 静态 Web 应用中实现 iOS 应用的通用链接
https://zenn.dev/poipoionigiri/articles/d2b6b69ceed16d

### ReSharper 现已进入开放 VSX 注册表 | .NET Tools 博客
https://blog.jetbrains.com/dotnet/2025/10/14/resharper-open-vsx/

## 库、存储库、工具等
### nuskey8/AsyncConsoleReader：提供 Console.Read / ReadKey / ReadLine 的可取消、非阻塞替代方案

https://github.com/nuskey8/AsyncConsoleReader

-[ [C#] AsyncConsoleReader - CancellationToken 的标准输入读取](https://zenn.dev/nuskey/articles/library-asyncconsolereader)



## 今日人物

**约翰·麦卡锡**(英语：John McCarthy，1927年9月4日—2011年10月24日[[2\]](https://zh.wikipedia.org/wiki/约翰·麦卡锡#cite_note-2)[[3\]](https://zh.wikipedia.org/wiki/约翰·麦卡锡#cite_note-3))，生于[美国](https://zh.wikipedia.org/wiki/美国)[马萨诸塞州](https://zh.wikipedia.org/wiki/马萨诸塞州)[波士顿](https://zh.wikipedia.org/wiki/波士顿)，[计算机科学家](https://zh.wikipedia.org/wiki/计算机科学家)。他因在[人工智能](https://zh.wikipedia.org/wiki/人工智能)领域的贡献而在1971年获得[图灵奖](https://zh.wikipedia.org/wiki/图灵奖)。实际上，正是他在1956年的[达特矛斯会议](https://zh.wikipedia.org/wiki/达特矛斯会议)上提出了“人工智能”这个概念。

1927年9月4日，约翰·麦卡锡出生于美国[马萨诸塞州](https://zh.wikipedia.org/wiki/麻薩諸塞州)[波士顿](https://zh.wikipedia.org/wiki/波士頓)。他的父亲John Patrick是[爱尔兰裔美国人](https://zh.wikipedia.org/wiki/愛爾蘭裔美國人)，母亲Ida Glatt McCarthy是[立陶宛](https://zh.wikipedia.org/wiki/立陶宛)的[犹太人](https://zh.wikipedia.org/wiki/猶太人)。

他于1948年获得[加州理工学院](https://zh.wikipedia.org/wiki/加州理工学院)数学学士学位，1951年获得[普林斯顿大学](https://zh.wikipedia.org/wiki/普林斯顿大学)数学博士学位。分别短暂地为普林斯顿大学、斯坦福大学、[达特茅斯学院](https://zh.wikipedia.org/wiki/达特茅斯学院)和[麻省理工学院](https://zh.wikipedia.org/wiki/麻省理工学院)供职后，麦卡锡于1962年-2000年底在斯坦福担任教授，退休后成为名誉教授。

麦卡锡发明了[LISP](https://zh.wikipedia.org/wiki/LISP)并于1960年将其设计发表在《[ACM通讯](https://zh.wikipedia.org/wiki/ACM通讯)》上。他帮助推动了[麻省理工学院](https://zh.wikipedia.org/wiki/麻省理工学院)的[MAC项目](https://zh.wikipedia.org/wiki/MIT計算機科學與人工智慧實驗室)。然而，他在1962年了离开麻省理工学院，前往[斯坦福大学](https://zh.wikipedia.org/wiki/斯坦福大学)并在那里协助建立了[斯坦福人工智能实验室](https://zh.wikipedia.org/w/index.php?title=斯坦福人工智能实验室&action=edit&redlink=1)，成为MAC项目多年来的一个友好的竞争对手。[[5\]](https://zh.wikipedia.org/wiki/约翰·麦卡锡#cite_note-科學人-5)

![约翰·麦卡锡](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/HdbJ3-_5_nJvomYUeyMpm_1536x1024_20251030_130939_raw.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET性能优化经验的群组，主题包括但不限于：

* 如何找到.NET性能瓶颈，如使用APM、dotnet tools等工具
* .NET框架底层原理的实现，如垃圾回收器、JIT等等
* 如何编写高性能的.NET代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我vx，我拉你进群: **ls1075** 另外也创建了**QQ Group**: 687779078，欢迎大家加入。