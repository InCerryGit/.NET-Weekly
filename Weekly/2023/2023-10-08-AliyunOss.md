## 国内文章

### 起风了，NCC 云原生项目孵化计划

https://www.cnblogs.com/liuhaoyang/p/ncc-the-wind-rises.html

2016年，我和几位朋友发起了.NET Core中文学习组和ASP.NET Core文档翻译项目，随后创建了.NET Core Community开源社区，吸引了近30个优秀的开源项目加入。然而，随着时间的推移，社区的活跃度逐渐降低。现在，我们计划发起名为"wind rises"的项目孵化，以弥补.NET平台上缺少云原生基础设施项目的遗憾。我们规划了使用.NET开发的"可观测性平台"和"分布式应用框架"两个项目。其中，"可观测性平台"已经完成项目原型的开发，计划在年底发布第一个版本。"分布式应用框架"还在原型讨论阶段，初步的想法是提供一个可插拔的应用框架。

### .NET 数据库大数据操作方案（插入、更新、删除、查询 、插入或更新）

https://www.cnblogs.com/sunkaixuan/p/17747938.html

本文介绍了SqlSugar的各种功能。SqlSugar是一种ORM工具，它优化了实体转换的性能，并使用数据库的最佳API。它提供了BulkCopy、BulkUpdate、BulkMerge、BulkQuery、BulkDelete和Select INTO等功能。BulkCopy用于高效批量插入大量数据到数据库，BulkUpdate用于高效批量更新数据，BulkMerge用于大规模数据的插入或更新，BulkQuery用于高效查询，BulkDelete用于高效批量删除数据，Select INTO用于表和表之间的数据导入。此外，SqlSugar还结合了.NET中的SqlBulkCopy类，提供了更高的性能。通过调整参数、合理使用事务、关闭索引和约束等方式，可以最大限度地提高大数据插入和更新的性能。

### .NET Core使用SkiaSharp快速生成二维码（ 真正跨平台方案）

https://www.cnblogs.com/Can-daydayup/p/17745369.html

在.NET 6之前，我们使用QRCoder生成二维码，但从.NET 6开始，非Windows操作系统编译引用代码时会发出警告。原因是System.Drawing.Common设计为Windows技术的简化包装器，跨平台实现不佳。在非Windows环境中，官方建议使用SkiaSharp和ImageSharp等库进行跨平台的图像处理操作。SkiaSharp是Mono团队维护的开源项目，基于Google的Skia图形库的.NET跨平台绑定，提供强大的2D图形绘制和处理功能，适用于多个平台。使用SkiaSharp可以快速生成二维码，无需使用System.Drawing。

### C# 12 中的新增功能

https://www.cnblogs.com/baibaomen-org/p/17748318.html

本文介绍了C# 12的新功能，包括主构造函数、集合表达式、默认Lambda参数等。主构造函数可以在任何class和struct中创建，不再局限于record类型，可以初始化属性或字段，也可以用于依赖注入和初始化基类。集合表达式引入了新的语法来创建常见的集合值，可以使用展开运算符将其他集合内联到这些值中。默认Lambda参数允许为Lambda表达式的参数定义默认值，语法和规则与将参数的默认值添加到任何方法或本地函数相同。这些新功能使得代码更灵活、更强大、更可控。

### 一种对数据库友好的GUID的变种使用方法

https://www.cnblogs.com/ensleep/p/17745166.html

本文讨论了如何改造GUID以实现有序性，以提高数据库索引效率。GUID和雪花算法是常见的唯一ID生成方案，但GUID是无序的，对数据库索引不友好。作者提出了一种新的方法，将时间值和GUID结合，生成一个byte[]，前8位放时间值，后面放GUID。在比较大小时，前端的位置优先级更高，所以，后面的GUID的无序特性会被覆盖。然后，将其进行类似Base64的转换，得到一个长度大概32位长度的字符串。这个字符串的字节数至少是32，但是，其具体更好的可读性。

### 关于Async、Await的一些知识点

https://www.cnblogs.com/tianqing/p/17742818.html

在ASP.NET Core中，HTTP请求到达服务器后，会被分配给线程池中的一个线程处理。如果处理方法是异步的并使用了await关键字，那么在await的代码执行完之前，该线程会被释放回线程池处理其他请求。当await的代码执行完毕后，会再次从线程池获取一个线程继续执行剩余代码。ASP.NET Core使用中间件管道模型处理请求，不需要使用SynchronizationContext来在异步操作完成后将执行上下文切换回原始请求上下文。这种模型提高了性能和可扩展性。SynchronizationContext和线程上下文是两个不同的概念，前者在多线程环境中控制和协调代码的执行，后者是与特定线程相关的一组数据或状态信息。

### 【ASP.NET Core】在 Mini-API 中注入服务

https://www.cnblogs.com/tcjiaan/p/17742167.html

本文介绍了Mini API的依赖注入功能。首先，定义一个服务类MyService，然后在容器中注册这个服务。然后，通过参数传入服务类的实例，调用服务类的公共方法。使用httprepl工具进行Web API测试，可以直接在命令终端输入httprepl，然后使用connect命令建立连接。发起请求时，可以用get、post、put等命令，对应HTTP的请求方式。最后，添加一个参数x，调用API时，可以直接将URL作为命令行参数传给httprepl工具。

### .NET周刊【9月第4期 2023-09-24】

https://www.cnblogs.com/InCerry/p/dotnet_week_23_9_4.html

本文介绍了多篇关于.NET和C#的技术文章。包括介绍了“可扩展近似计数”算法，使用C#+Win32Api实现进程注入到wechat的方法，.Net 6中使用SkiaSharp生成验证码的过程，深度比较了几种.NET Excel导出库的性能差异，四个常用的序列化和反序列化库的性能测试，.NET8中新增的特性UnsafeAccessor，C#开源的Windows系统优化工具 - Optimizer，.NET 8 的 green thread 异步模型被搁置的情况，以及两次.NET程序内存暴涨的分析过程。这些文章涵盖了.NET和C#的多个重要领域，包括算法、进程注入、验证码生成、Excel导出库性能比较、序列化和反序列化库性能测试、访问私有成员、系统优化工具、异步模型以及内存分析等。

### Asp-Net-Core开发笔记：快速在已有项目中引入EFCore

https://www.cnblogs.com/deali/p/17749676.html

本文以StarBlog项目为例，介绍了如何在项目中引入EFCore。首先，安装EFCore的cli工具，然后在StarBlog.Data项目中添加EFCore的依赖。接着，创建一个DbContext，这是EFCore与数据库交互的入口。然后，使用Fluent Config方式配置数据表和字段。文章还讨论了主键类型的选择，包括自增、GUID、自增+GUID和Hi/Lo等几种方式。最后，创建DesignTime配置，让EFCore知道如何执行迁移，并使用migrations和database命令进行数据库迁移。最后，将数据库连接字符串写入配置文件，完成在AspNetCore项目中集成EFCore的过程。

### 执行SQL语句&amp;存储过程的真正【神器】，不用ORM的全选它，比dapper好

https://www.cnblogs.com/digital-college/p/17747634.html

本文介绍了一个支持.Net Core(2.0及以上)与.Net Framework(4.0及以上)的工具，已被.Net圈内多家大厂采用。该工具在IDataAccess接口中提供，主要提供了执行Sql语句、执行Sp存储过程、创建参数(输入/输出/返回)和事务等四大功能。它可以通过设定DatabaseType属性，支持所有种类数据库，包括MySql、Oracle、PostgreSQL、SqlServer、Sqlite、Access、ODBC等。同时，它还提供了查询多数据、选出单数据、参数等使用示例。

### 【算法】国庆加班，火锅与Linq.AddRange的奇妙螺旋

https://www.cnblogs.com/lan80/p/17744494.html

在国庆假期，小悦在家享受火锅时接到公司电话，需要处理一个关于小视频螺旋排序算法的紧急项目。尽管感到棘手，小悦还是决定挑战。她通过研究和实践，逐渐掌握了螺旋排序算法的核心思想，并开始编写代码实现这个算法。虽然劳累，但解决问题的过程让她感到乐趣和喜悦。最终，她成功运行出结果，心中充满了成就感。这个国庆假期，虽然没有休息和放松，但她在工作中取得了宝贵的进步。回到家中，她继续享受火锅，收获了成长和充实。

### C#使用iKvm黑科技无缝接入JVM生态

https://www.cnblogs.com/deali/p/17744798.html

本文介绍了如何在C#中使用Java的NLP工具。作者首先介绍了iKvm，这是一个Java在Microsoft .NET平台的实现，可以在C#中直接调用Java的jar包或将其转译为.Net平台的dll。然后，作者详细介绍了如何在项目中添加iKvm和Maven的依赖，并使用iKvm将Java的jar包转译为.Net的dll。最后，作者以HanLP为例，展示了如何在C#中使用Java的NLP工具进行命名实体识别。

### 一套基于 .NET Core 开发的支付SDK集 - paylink

https://www.cnblogs.com/Can-daydayup/p/17745110.html

本文介绍了基于.NET Core开发的支付SDK集：paylink，它可以简化API调用和通知处理流程，提高工作效率。paylink支持.NET Core 3.1、.NET 6.0、.NET 7.0等运行环境，并且支持支付宝支付和微信支付等渠道。文章还提供了微信公众号支付的示例代码，详细代码可以在示例项目中查阅。

### 本计划在 .NET 8 中推出的 WASI 推迟到 .NET 9

https://www.cnblogs.com/shanyou/p/17739970.html

.NET 8计划中的WASI已被推迟到.NET 9。从.NET 8 Preview 4开始，支持生成与WASI兼容的.wasm文件，可以使用WebAssembly运行时Wasmtime CLI运行。WASI的支持最早在Steve Sanderson的个人仓库开始引入，后来正式引入到dotnet/dotnet-wasi-sdk，现在已经引入到dotnet/runtime的WASI跟踪问题。.NET 8添加了一个新的“wasi-experimental”工作负载，取代了早期的Wasi.Sdk，这是为服务器端WebAssembly方案提供.NET本机内置支持的一个步骤。由于WASI预览版2和3可能会引入重大变化，这对于.NET对WASI的支持非常有意义。

### 解决因对EFCore执行SQL方法不熟练而引起的问题

https://www.cnblogs.com/azrng/p/17750328.html

本文主要讨论了在使用EFCore执行SQL文件时遇到的问题和解决方案。作者在尝试使用ExecuteSqlAsync方法执行SQL语句时遇到了错误，原因是方法接收的参数是FormattableString，而作者在构建这个参数时使用了错误的方式。通过查看源码和进行测试，作者发现问题出在ExecuteSqlAsync方法的入参上，解决方案是先定义一个FormattableString类型直接传入，或者在SQL语句中直接插入变量。但是，作者提醒读者注意，ExecuteSqlAsync方法中的SQL在EFCore中并没有被放入一个事务中，如果有需要，就需要自己创建事务。最后，作者提出了一个未完成的问题，即如何执行SQL文件，提出了使用ADO.NET进行操作的可能解决方案。

### 文章《Semantic Kernel -- LangChain 的替代品？》的错误和疑问 探讨

https://www.cnblogs.com/shanyou/p/17742002.html

本文主要讨论了Semantic Kernel（SK），这是微软推出的一种结合大语言模型（LLM）与传统编程技术的开源编程框架。SK采用C#开发，因为微软的许多产品都是用C#开发的，而且许多商业系统也是用C#或Java这样的强类型语言构建的。SK不仅支持OpenAI，Azure OpenAI，HuggingFace上的模型，还可以支持任何LLM。SK鼓励对大模型的支持作为单独插件独立维护，以增强SK的模块化和可维护性。SK还有一个基于YAML的DSL定义和执行复杂工作流的流业务流程协调程序扩展，提供灵活性，支持通用技能，包括语义函数、原生函数和需要聊天交互的技能。SK使构建企业AI编排器变得容易，是Copilot Stack的中心。

### 记一次 .NET某账本软件 非托管泄露分析

https://www.cnblogs.com/huangxincheng/p/17746280.html

本文主要讲述了一个.NET程序集泄露导致的CLR私有堆泄露的案例。作者在中秋国庆长假结束后，分享了这个奇奇怪怪的.NET生产事故。通过使用WinDbg分析，作者发现当前的提交内存占用了2.19G，进程堆占用1G，差不多占了一半，但不能说明就是非托管内存泄露。接下来，作者继续观察下托管堆，发现当前的托管堆占用仅195M，这就更好的验证当前确实存在非托管内存泄露。最后，作者通过观察CLR私有堆，发现总的大小是1.19G，基本就搞清楚了，然来是程序集泄露。

### .Net7自定义GC垃圾回收器

https://www.cnblogs.com/tangyanzhi1111/p/17748346.html

本文介绍了如何在.Net7中自定义垃圾回收器（GC）。在.Net7中，CLR和GC已经分离，使得自定义GC变得更容易。首先，下载并将Custom.dll复制到.Net目录。然后，在C#代码中，设置环境变量DOTNET_GCName的值为Custom.dll。运行代码后，可以看到自定义GC的效果。CLR在初始化时，会检查是否存在DOTNET_GCName环境变量，如果存在，则使用该环境变量指定的GC替换默认的GC。自定义GC需要新建一个C++ DLL库项目，引入两个头文件，实现三个接口，并导出两个函数。

### ASP.NET 6启动时自动创建MongoDB索引

https://www.cnblogs.com/edisonchou/p/auto-create-mongoindex-in-aspnet6.html

本文由Edison撰写，介绍了如何在ASP.NET 6应用启动时通过代码自动创建MongoDB的索引。索引是一种提高查询速度和防止脏数据插入的数据结构，支持普通字段、内嵌文档中的键和数组元素进行索引。MongoDB支持多种类型的索引，如唯一索引、稀疏索引、复合索引、TTL索引、全文索引、二维平面索引和地理空间索引。通过Mongo Shell可以进行索引的创建、查询和删除。文章还提供了一个Entity的定义示例，并介绍了如何使用MongoDbConnection，一个包裹MongoClient的单例对象，来操作MongoDB。

## 主题

### C# 开发工具包 - 现已全面上市 - .NET 博客
https://devblogs.microsoft.com/dotnet/csharp-dev-kit-now-generally-available/

C# 开发工具包现已全面上市。

C# Dev Kit 是 Visual Studio Code 中 C# 开发的扩展。通过将 Visual Studio 中包含的解决方案资源管理器和测试资源管理器等功能引入 Visual Studio Code，它提供了超越现有 C# 开发扩展的功能。它不仅支持在 Windows 上使用，还支持在 Linux 和 macOS 上使用。

使用此扩展需要 Visual Studio 订阅（包括社区）许可证。

### .NET 8 中的 Arm64 性能改进 - .NET 博客
https://devblogs.microsoft.com/dotnet/this-arm64-performance-in-dotnet-8/

.NET 8 中 Arm64 性能改进的说明。

- 条件选择
- 条件比较
- 条件递增、否定、反转
- VectorTableLookup 和 VectorTableLookupExtension
- 连续寄存器分配
- 窥视孔优化
    - 将连续的“ldr”和“str”替换为“ldp”和“stp”
    - 将 `ldp`/`stp` 与 SIMD 寄存器结合使用
    - 将“str wzr”对替换为“str xzr”
    - 将负载替换为“mov”
    - mul + neg -> mneg 转换
- 提高代码质量
    - 更快的 Vector128/Vector64 比较
    - 改进的向量 == Vector128<>.Zero
    - 展开记忆移动
- 提高吞吐量


### System.Text.Json 的便利 - .NET 博客
https://devblogs.microsoft.com/dotnet/the-convenience-of-system-text-json/

System.Text.Json 的便利性说明。

本文介绍了使用常用 API（序列化器、读取器/写入器）作为模型（包括 JSON.NET）的性能和用法。

### 宣布新版本！ | Evergine 9 月 23 日 - Evergine
https://evergine.com/evergine-release-september-2023/

Evergine 2023 年 9 月版已发布。

此版本包括对 iOS、Metal 和 .NET MAUI 的支持，以及用于变形动画系统和 XRV 框架的新模块以及性能改进。

- [Evergine 通过 Metal API 扩展到 iOS - Evergine](https://evergine.com/ios-metal-api/)


## 文章、幻灯片等
### 显示少量小数 - Qiita
https://qiita.com/hiro_t/items/b83af07c232ce677cae3

格式化 Decimal 字符串时小数部分规范的比较。

### 内存映射文件和覆盖结构
https://blog.stephencleary.com/2023/09/memory-mapped-files-overlaid-structs.html

如何将内存映射文件上的数据作为结构引用。

### Microsoft 如何为残障开发人员提供支持：庆祝 NDEAM - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/celebating-ndeam-vs-code-visual-studio/

为了庆祝 NDEAM（全国残疾人就业意识月），了解 Microsoft 对残疾开发人员的支持。

### 如何将Godot的C#项目分成多个项目来管理？
https://zenn.dev/numani/articles/godot-split-project

在 Godot 中创建 C# 项目且无法在类库项目中附加类的问题。

### 如何使用 gdb 调试 .NET 项目 - Qiita
https://qiita.com/daredeshow/items/aa2b80e4463266ac3cb0

当 .NET 应用程序在 Linux 上因 SEGV 崩溃时，如何使用 gdb 调试 .NET 应用程序。

### 可以将 .NET 8 Identity API 端点与 IdentityServer 一起使用吗？
https://andrewlock.net/can-you-use-the-dotnet-8-identity-api-endpoints-with-identityserver/

关于 .NET 8 Identity API 和 IdentityServer 之间的关系和机制，以及关于用 .NET 8 Identity API 端点替换 IdentityServer 模板。

### Resharper 2023.2 带来预测调试器
https://www.infoq.com/news/2023/10/resharper-predictive-debugger/

ReSharper 2023.2 中引入预测调试器

### .NET Conf 学生专区回来了！-.NET 博客
https://devblogs.microsoft.com/dotnet/the-dotnet-conf-student-zone-is-back/

关于2023年.NET Conf学生专区的举办。

.NET Conf 学生专区是针对初学者/学习者的会议活动。该活动将于11月13日举行。

### JetBrains .NET Day Online '23 的录音现已推出 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/10/02/recordings-jetbrains-dotnet-day-online-23/

JetBrains .NET Day Online 的录制现已推出。提供了 10 个与 .NET 相关的会议的录音。

### GitHub Actions Runner 深入探究：注册和设置
https://dev.to/cwprogram/github-actions-runner-deep-dive-registration-and-setup-1ojb

一篇解释 GitHub Actions Runner 源代码的文章。本文介绍了如何注册为跑步者并开始使用。

### 了解 IAsyncEnumerable - Qiita
https://qiita.com/TsuyoshiUshio@github/items/c4b9929d88d1cd8cabb1

简要说明如何使用 IAsyncEnumerable 和用例。

### 前滚到 .NET 的主要版本
https://weblog.west-wind.com/posts/2023/Oct/02/Rolling-Forward-to-Major-Versions-in-NET

如何前滚运行应用程序的运行时版本（例如在 .NET 8 上运行使用 .NET 7 构建的应用程序）。

### 将 http/2 与 ASP.NET Core 结合使用 - Traefik/Kubernetes/container 示例
https://josef.codes/using-http2-with-asp-net-core-traefik-kubernetes-container-example/

关于在 Kubernetes 上配置 ASP.NET Core 应用程序以侦听具有 TLS 的 HTTP/2。

### .NET 迁移的故事 - 我们的第一视角
https://www.jimmybogard.com/tales-from-the-net-migration-trenches-our-first-views/

.NET Framework 到 .NET 迁移差距系列。迁移视图等时的捆绑处理

### SQL-Server (C#) 的多个结果集，包括 Dapper
https://dev.to/karenpayneoregon/multiple-result-sets-for-sql-server-c-include-dapper-1fpa

如何使用 Dapper 等从 SQL Server 接收多个结果集

### C# 提示：通过初始化集合大小来改进内存分配
https://www.code4it.dev/csharptips/initialize-collection-size/

关于List和HashSet通过设置初始大小来分配内存的区别。

### 糟糕：应用程序随机崩溃！
https://chnasarre.medium.com/crap-the-application-is-randomly-crashing-b105a6a5a7e8

根据 Datadog 分析器中的示例，了解如何使用 WinDbg 调查应用程序崩溃。

## 网站、文档等
### .NET 多平台应用程序 UI (.NET MAUI) 文档：2023 年 9 月的新增功能 - .NET MAUI
https://learn.microsoft.com/en-us/dotnet/maui/whats-new/dotnet-docs-maui-mod0

.NET MAUI 2023 年 9 月最新信息文档。包含来自 Xamarin.Forms 的迁移文档。

- [新的 .NET MAUI 文档详细介绍了如何从 Xamarin.Forms 迁移 -- Visual Studio 杂志](https://visualstudiomagazine.com/articles/2023/10/06/net-maui-docs.aspx)

### 推文

**引入一个总结与 Stride（游戏引擎）相关信息的存储库。**

https://x.com/strdedotnet/status/1708525831864139906?s=12

![image-20231014104653195](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231014104653195.png)

---

**使用 .NET MAUI 和 Evergine 合并 3D 图形的示例应用程序。**

https://x.com/jsuarezruiz/status/1708875963260346409?s=12

![image-20231014104738538](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231014104738538.png)



## 深入探索

### JonDouglas 为 NuGet 添加赞助商链接功能 · Pull Request #12922 · NuGet/Home
https://github.com/NuGet/Home/pull/12922

建议 PR 在 NuGet 包信息中包含赞助商链接。

https://x.com/nuget/status/1709955756823314756?s=12

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