## 国内文章

### NativeBuferring，一种零分配的数据类型（上篇）

https://www.cnblogs.com/artech/p/17586781.html

之前一个项目涉及到针对海量（千万级）实时变化数据的计算，由于对性能要求非常高，我们不得不将参与计算的数据存放到内存中，并通过检测数据存储的变化实时更新内存的数据。存量的数据几乎耗用了上百G的内存，再加上它们在每个时刻都在不断地变化，所以每时每刻都无数的对象被创建出来（添加+修改），同时无数现有的对象被“废弃”（删除+修改）。这种情况针对GC的压力可想而知，所以每当进行一次2代GC的时候，计算的耗时总会出现“抖动”。为了解决这类问题，几天前尝试着创建了一个名为[NativeBuffering](https://github.com/jiangjinnan/NativeBuffering)的框架。目前这个框架远未成熟，而且是一种“时间换空间”的解决方案，虽然彻底解决了内存分配的问题，但是以牺牲数据读取性能为代价的。这篇文章只是简单介绍一下NativeBuffering的设计原理和用法，并顺便收集一下大家的建议。[本文演示源代码从[这里](https://files.cnblogs.com/files/artech/native-bufffering-1.7z?t=1690759387&download=true)下载]

### NativeBuferring，一种零分配的数据类型（下篇）

https://www.cnblogs.com/artech/p/17587660.html

这篇文章是关于NativeBuffering，一种零分配的数据类型，它可以用来高效地处理缓冲字节序列。文章介绍了NativeBuffering支持的两种基本数据类型：Unmanaged和IReadOnlyBufferedObject，以及它们的集合和字典类型。文章还介绍了如何利用Source Generator生成BufferedMessage类型，以及如何通过无限嵌套的形式定义一个具有任意结构的数据类型。文章的目的是让读者了解NativeBuffering的设计原理和使用方法。

### 揭秘 .NET 中的 TimerQueue（下）

https://www.cnblogs.com/eventhorizon/p/17609210.html

关于.NET中的TimerQueue的文章，它是一个用于管理定时任务的类。文章主要介绍了以下内容：

- TimerQueue是如何与操作系统的定时器进行交互的，包括注册、取消、设置和回调等细节。
- TimerQueue是如何在删除数据时维持B树的平衡性的，包括从叶子节点和非叶子节点删除数据，以及提前扩充只有t-1个Item的节点的三种方法：从左兄弟节点借用Item，从右兄弟节点借用Item，与左兄弟节点或右兄弟节点合并。
- TimerQueue是如何实现最值的删除的，包括最小值和最大值的查找和删除。
- 作者还提供了完整的代码实现和性能测试，与优先队列PriorityQueue进行了比较。

### 重返照片的原始世界：我为.NET打造的RAW照片解析利器

https://www.cnblogs.com/sdflysha/p/20230801-sdcb-libraw-intro.html

这篇文章介绍了作者如何为.NET打造了一个RAW照片解析的库，基于libraw这个开源项目。文章主要包括以下几个方面：

- 作者介绍了RAW照片的概念和优势，以及libraw的功能和特点。
- 作者展示了如何使用他的库Sdcb.LibRaw来将RAW照片转换为Bitmap或者其他格式的图像，以及如何获取支持的相机列表。
- 作者解释了他的库的架构和设计思路，以及如何使用PInvoke来封装libraw的C API。
- 作者提供了一些示例代码和截图，以及一些相关的下载链接和参考资料。

文章的目的是帮助.NET开发者更好地理解和使用RAW照片，以及展示作者的开源项目。

### 你真的知道吗？catch、finally和return哪个先执行

https://www.cnblogs.com/rupeng/p/17599580.html

我的一位朋友前阵子遇到一个问题，问题的核心就是try……catch……finally中catch和finally代码块到底哪个先执。这个问题看起来很简单，当然是“catch先执行、finally后执行”了？真的是这样吗？

### 堆 Heap & 栈 Stack（.Net）【概念解析系列_3】【C# 基础】

https://www.cnblogs.com/hnzhengfy/p/GNJXXL_HeapStack.html

本文主要围绕 .Net 框架中的托管堆（Heap，简称堆）和堆栈（Stack，简称栈）展开。

.Net 程序在 CLR（Common Language Runtime 公共语言运行时）上运行时，内存被从逻辑上划分为两个主要部分：堆和栈。除了栈和堆之外，CLR 还维护了其他一些内存区域，例如静态存储区域（Static Storage Area）、常量存储区域（Constant Storage Area）等。这些内存区域都有各自的特点和用途，可以帮助我们更好地管理程序内存和资源的使用。

因此，熟知堆和栈的运行机制，对提升系统性能和稳定性至关重要。

### 记一次 .NET某培训学校系统 内存碎片化分析

https://www.cnblogs.com/huangxincheng/p/17602611.html

前些天有位朋友微信上找到我，说他们学校的Web系统内存一直下不去，让我看下到底是怎么回事，老规矩让朋友生成一个dump文件丢给我，看一下便知。

### 记一次 .NET 某物流API系统 CPU爆高分析

https://www.cnblogs.com/huangxincheng/p/17593608.html

前段时间有位朋友找到我，说他程序CPU直接被打满了，让我帮忙看下怎么回事，截图如下：

![img](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/214741-20230731153115090-546047217.png)

看了下是两个相同的程序，既然被打满了那就抓一个 dump 看看到底咋回事。

### .NET Core WebAPI中使用Swagger（完整教程）

https://www.cnblogs.com/kimiliucn/p/17602073.html

这篇文章介绍了如何使用Swagger来生成和测试Web API的文档，以及如何自定义Swagger UI的界面和功能。文章主要包括以下几个部分：

- Swagger的概念和优势，以及它与Open API和Restful API的关系。
- 如何在.NET Core项目中安装和配置Swashbuckle.AspNetCore包，以及如何生成JSON格式的Swagger文档。
- 如何在项目中启用Swagger UI，并修改默认的启动URL。
- 如何在代码中添加XML注释，以便在Swagger UI中显示更多的信息和说明。
- 如何自定义Swagger UI的样式和主题，以及如何添加授权功能。

文章还提供了一些示例代码和截图，以及一些相关的下载链接和参考资料。文章的目的是帮助开发者更好地理解和使用Swagger来构建和测试Web API。

### 【.NET6 + Vue3 + CentOS7.9 + Docker + Docker-Compose + SSL】个人博客前后端运维部署

https://www.cnblogs.com/lujiesheng/p/17599850.html

这篇文章介绍了如何使用Docker和Docker Compose来部署个人博客的前后端和运维服务。文章主要包括以下几个步骤：

- 在腾讯云轻量应用服务器上安装和配置CentOS 7.6，设置防火墙和域名解析，申请SSL证书，创建容器镜像服务。
- 在服务器上安装和启动Docker和Docker Compose，准备部署目录和配置文件，创建nginx、ui、api、portainer等服务。
- 在本地使用VS2022打包.NET6 API镜像，推送到腾讯云容器仓库，然后在服务器上拉取并启动。
- 使用docker-compose命令来管理服务的启动、停止、重启等操作，查看服务的状态和网络。

文章还提供了一些示例代码和截图，以及一些相关的下载链接和参考资料。

### C#.NET 国密SM2 加密解密 与JAVA互通 ver:20230805

https://www.cnblogs.com/runliuv/p/17607568.html

如标题所示，本文介绍了国密SM2 .NET 如何与 JAVA互通。

.NET 环境：.NET6 控制台程序(.net core)。

JAVA 环境：JAVA8，带maven 的JAVA控制台程序。

## 主题

### 【英文】发布 ILSpy 8.1 icsharpcode/ILSpy
https://github.com/icsharpcode/ILSpy/releases/tag/v8.1

ILSpy 8.1 已发布。

此版本包括对一些 C# 11 符号的支持和各种修复。

### 【英文】宣布推出 Visual Studio Code 的 Unity 扩展 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/announcing-the-unity-extension-for-visual-studio-code/

Visual Studio Code 的 Unity 扩展现已推出预览版。

该扩展基于 C# 开发套件构建，支持代码编辑的 AI 辅助、Roslyn 分析器和 Unity 中的游戏调试等功能。文章还介绍了如何在Unity中使用。

该扩展还以与 C# 开发工具包相同的许可模式提供，并且需要 Visual Studio Community 许可证或订阅。

### 【英文】Rider 2023.2：更好的 C# 支持、UX/UI 增强、AI 驱动的功能等等 | JetBrains 博客
https://blog.jetbrains.com/dotnet/2023/08/02/rider-2023-2-release/

Rider 2023.2 已发布。

- C# 更新
- 改进的用户界面/用户体验
    - 改进的构建工具窗口
    - 默认外观是新的用户界面
    - 定制和简化
        - 固定项目标题、主工具栏自定义、运行配置
- 人工智能辅助（访问受限）
- 版本控制
    - GitLab 集成
    - 后台提交检查
    - 行提交选项
- 性能改进
    - 减少缓存数据（减少 I/O）
- 游戏开发
    
    * Unity AI 协助、ShaderLab 支持、Unity DOTS 支持
    
    - 虚幻引擎
        - 改进的蓝图索引、热重载和实时编码、更好的 Perforce 支持 .NET SDK
    - 重新启动源生成器模板和源生成器
    - Docker快速模式
    - .NET MAUI 热重载

### 【英文】ReSharper 2023.2：更多 C#、C++ 20 和 C++ 23 功能、创建和导航单元测试的能力、预测调试器模式等等 | JetBrains 博客
https://blog.jetbrains.com/dotnet/2023/08/02/resharper-2023-2-release/

ReSharper 2023.2 已发布。

- C# 更新
- C++ 更新
- 性能改进
    - 减少解决方案加载时间
- 单元测试创​​建和导航
- 人工智能辅助（访问受限）
- 预测调试器（测试版）
- 反编译器中的程序集差异

### 【英文】.NET Conf 2023 - 庆祝 .NET 8 的发布！ - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-conf-2023-celebating-the-release-of-dotnet-8-save-the-date/

关于 .NET Conf 2023 的公告。

.NET Conf 2023 将于 11 月 14 日至 16 日举行，为期三天，包括各种会议，包括 .NET 8 的发布。

### 【英文】Microsoft 作者签名证书将于 2023 年 8 月 14 日更新 - NuGet 博客
https://devblogs.microsoft.com/nuget/microsoft-author-signing-certificate-update-2023/

用于签署微软发布的NuGet包的证书将在8月14日之后更新。

现有软件包不会通过此支持进行更新，未来的软件包将使用新证书进行签名。

如果您拥有并验证 NuGet 客户端策略中的受托人允许列表，则会受到影响。


### 【英文】dotCover、dotMemory、dotPeek 和 dotTrace 2023.2 发布！| JetBrains 博客
https://blog.jetbrains.com/dotnet/2023/08/02/2023-2-dottools-release/

dotCover、dotMemory、dotPeek、dotTrace、dotMemory 2023.2 

-  Rider 中的快照分析

- dotTrace
      * 采样、跟踪、按线程分组的逐行快照
          *  Linux 和 macOS 上的源代码查看工具窗口

- dotPeek
    - 组件比较
- dotCover
    - 错误修复和稳定性改进

## 文章、幻灯片等
### 【英文】C# 12 拦截器！
https://dev.to/bugandfix/c-12-interceptors-an-insane-feature--517l

一篇关于在 C# 12 中运行拦截器的文章。

### 【英文】哪个 RDBMS 具有最快的 .NET Bulk Insert 实现？
https://servicestack.net/posts/bulk-insert-performance

不同 RDBMS 和架构/操作系统之间批量插入的性能比较。

### 【英文】C# 中的类与结构：做出明智的选择 - NDepend
https://blog.ndepend.com/class-vs-struct-in-c-making-informed-choices/

总结类和结构的优缺点并决定使用哪一种。

### 【日文】C# 将数据库提供程序合并到通用主机 DI - Qiita
https://qiita.com/mxProject/items/232ee4d0feb30a41a2f3

如何在 Generic Host 的服务中嵌入和使用数据库提供程序 (ADO.NET)。

### 【英文】ASP.NET Core 中的插件架构 – 如何掌握它
https://dev.to/devleader/plugin-architecture-in-aspnet-core-how-to-master-it-1824

如何在 ASP.NET Core 应用程序中实现插件架构。

### 【英文】.NET8 依赖注入中的键控服务
https://dev.to/xelit3/keyed-services-in-net8s-dependency-injection-2gni

关于 .NET 8 中的 M.E.DependencyInjection 以及 ASP.NET Core 中支持的键控服务。

### 【英文】在 EFCore 中利用自定义 PostgreSQL 函数：映射和使用指南
https://gor-grigoryan.medium.com/leveraging-custom-postgresql-functions-in-efcore-a-guide-to-mapping-and-usage-53941b10fe89

如何在 Entity Framework Core 中映射和使用 PostgreSQL 自定义函数。

### 【英文】通过单元测试创​​建和导航加速您的测试工作流程 | JetBrains 博客
https://blog.jetbrains.com/dotnet/2023/08/01/acceleating-your-testing-workflow-with-unit-test-creation-and-navigation/

介绍 ReSharper 中的单元测试创​​建和导航功能。它介绍了可用于在代码之间导航和创建新单元测试的函数。

### 【日文】使用VisualStudio.Extensibility-Qiita进行扩展开发介绍
https://qiita.com/mngreen/items/d712930b5894aa6ea17f

引入使用 Visual Studio.Extensibility（Visual Studio 的新扩展模型）的扩展实现。

### 【英文】基于命令行的 .NET 应用程序
https://dev.to/asimmon/instrumenting-systemcommandline-based-net-applications-1p88

如何使用 System.CommandLine 将自定义工具合并到您的应用程序中。

### 【日文】DateTime.MaxValue 翻译错误 - Qiita
https://qiita.com/hiro_t/items/0a8e5ce1c1552366a8f4

关于DateTime.MaxValue日文文档解释中的错误。

### 【英文】C# 中的 `ImmutableArray<T>` 迭代性能
https://antao-almada.medium.com/immutablearray-t-iteration-performance-in-c-99e490d4d352

`ImmutableArray<T>` 上枚举操作的性能。与列表、数组等的比较

### 【英文】学习 Resharper PostFix 和源模板
https://dev.to/karenpayneoregon/learn-resharper-postfix-and-source-templates-32lo

如何使用和创建 ReSharper 和 Rider 中提供的 postfix 部署模板。

### 【英文】为所有 ASP.NET Core 生成站点地图
https://khalidabuhakmeh.com/generate-sitemaps-for-all-of-aspnet-core

如何使用 DotnetSitemapGenerator 在 ASP.NET Core Web 应用程序中生成站点地图 (XML)### 将异常转化为问题详细信息响应
https://timdeschryver.dev/blog/translated-exceptions-into-problem-details-responses

ASP.NET Core 如何将异常转换为问题详细信息响应并返回它。

### 【英文】.NET 8 时间提供程序和单元测试
https://khalidabuhakmeh.com/dotnet-8-timeprovider-and-unit-tests

了解 .NET 8 中引入的 TimeProvider API 以及如何使用它编写单元测试。

### 【英文】释放 .NET 源代码生成器的力量
https://medium.com/@bnayae/unleashing-the-power-of-net-source-code-generators-3115156df775

使用源生成器的库简介。本文介绍了 Refit、System.Text.Json、Dunet、Mapperly 和 Generator.Equals。

### 【英文】我在 ASP.NET Core 应用程序中尝试了 Application Insights 的代码优化功能
https://blog.shibayan.jp/entry/20230805/1691227089

如何将 Application Insights 代码优化应用于 ASP.NET Core 应用程序。

代码优化包括基于人工智能的应用程序性能问题检测/建议。

### 【日文】.NET中基于长度的switch分支调度
https://ufcpp.net/blog/2023/8/lengthbasedswitch/

自 Roslyn 4.6 以来，关于字符串分支的 switch 分支以新的方式进行。

### 【日文】.NET 中的 WebSocket 和处理断开连接 -castaneai 的博客
https://castaneai.hatenablog.com/entry/closing-websocket-connection-in-dotnet

关于 .NET WebSocket 中的断开连接处理。关于CloseAsync、CloseOutputAsync和Dispose等方法之间的区别。

### 【日文】[C#] [备忘录] 设置为在 build-Qiita 期间不输出不必要的语言文件夹
https://qiita.com/minoura_a/items/092b141bc6ecde5bbb24

如何避免在构建时包含不必要的语言本地化资源。

### 【日文】在 Azure Functions (.NET 6) 项目中升级 NuGet 包引用时出错 | @jsakamoto
https://devadjust.exblog.jp/29654451/

关于更新Azure Functions (.NET 6)项目的NuGet包时发生的错误。

在进程内模式下运行时，Azure Functions 运行时使用 Microsoft.Extensions.* 6.0，因此在应用程序依赖的包中更新到 7.0 会导致版本不一致。

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

如果提示已经达到200人，可以加我微信，我拉你进群: **lishi-wk**

另外也创建了**QQ群**，群号: 687779078，欢迎大家加入。 

## 抽奖送书活动预热！！！

感谢大家对我公众号的支持与陪伴！为庆祝公众号一周年，抽奖送出一些书籍，请大家关注公众号后续推文！

![image-20230703203249615](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230703203249615.png)