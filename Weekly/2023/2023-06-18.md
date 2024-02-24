## 国内文章

### 揭秘 Task.Wait

https://www.cnblogs.com/eventhorizon/p/17481757.html

Task.Wait 是 Task 的一个实例方法，用于等待 Task 完成，如果 Task 未完成，会阻塞当前线程。**非必要情况下，不建议使用 Task.Wait，而应该使用 await。**本文将基于 .NET 6 的源码来分析 Task.Wait 的实现，其他版本的实现也是类似的。

### 使用 C# 进行AI工程开发

https://www.zhihu.com/column/c_1648375724791808000

一直以来，官方口径都是尽量不要碰 CSharp 里的 unsafe 部分，以至于在大部分其它语言的程序员眼里，甚至 CSharp 程序员的眼里，CSharp 就是一个 Java，做做 CRUD，捣鼓捣鼓局限于 Windows 平台的 Winform 和 WPF 就行了。我觉得这种观念是不对的，东西做出来就是让人用的。准确看待一件事情，需要有一个大局观和整体观，而大局观和整体观，就避免不了去触碰 CSharp 里的 unsafe 部分。必须打开 unsafe，才能完整的理解 dotnet 和 CSharp。这里讲讲我的理解......

### .NET源码解读kestrel服务器及创建HttpContext对象流程 

https://www.cnblogs.com/Z7TS/p/17459777.html

.NET本身就是一个基于中间件（middleware）的框架，它通过一系列的中间件组件来处理HTTP请求和响应。因此，本篇文章主要描述从用户键入请求到服务器响应的大致流程，并深入探讨.NET通过kestrel将HTTP报文转换为HttpContext对象。通过本文，您可以了解以下内容：

- http的数据流转流程
- 源码解读kestrel服务器的运作流程及生成HttpContext对象

### 记一次 .NET 某药材管理系统 卡死分析

https://www.cnblogs.com/huangxincheng/p/17483537.html

前段时间有位朋友找到我，说他们在查询报表的时候发现程序的稳定性会受到影响，但服务器的内存，CPU都是正常的，让我帮忙看下怎么回事，问了下程序的稳定性指的是什么？指的是卡死，那既然是卡死，就抓一个卡死的dump吧。

### .net 项目静态文件自动压缩打包

https://www.cnblogs.com/newton/p/17451112.html

在 ASP.NET MVC 时代，我们常使用 `BundleCollection` 设置需要打包压缩的 js 和 css 文件，运行时框架会自动处理打包压缩过程并将最终结果传入响应。ASP.NET Core 开始，不再提供内置的打包压缩组件，官方推荐 [WebOptimizer](https://github.com/ligershark/WebOptimizer) 替代使用。

### 全面的ASP.NET Core Blazor简介和快速入门

https://www.cnblogs.com/Can-daydayup/p/17157143.html

因为咱们的MongoDB入门到实战教程Web端准备使用Blazor来作为前端展示UI，本篇文章主要是介绍Blazor是一个怎样的Web UI框架，其优势和特点在哪？并带你快速入门上手ASP.NET Core Blazor(当然这个前提是你要有一定的C#编程基础的情况，假如你完全没有接触过C#的话建议你先从基本语法学起)。

### ASP.NET Core 6框架揭秘实例演示[38\]：两种不同的限流策略  

https://www.cnblogs.com/artech/p/inside-asp-net-core-6-38.html

承载ASP.NET应用的服务器资源总是有限的，短时间内涌入过多的请求可能会瞬间耗尽可用资源并导致宕机。为了解决这个问题，我们需要在服务端设置一个阀门将并发处理的请求数量限制在一个可控的范围，即使会导致请求的延迟响应，在极端的情况会还不得不放弃一些请求。ASP.NET应用的流量限制是通过ConcurrencyLimiterMiddleware中间件实现的。（本文提供的示例演示已经同步到《[ASP.NET Core 6框架揭秘-实例演示版](https://www.cnblogs.com/artech/p/inside-asp-net-core-6.html)》）

### 浅聊一下 C#程序的 内存映射文件 玩法

https://www.cnblogs.com/huangxincheng/p/17478410.html

前段时间训练营里有朋友问 `内存映射文件` 是怎么玩的？说实话这东西理论我相信很多朋友都知道，就是将文件映射到进程的虚拟地址，说起来很容易，那如何让大家眼见为实呢？可能会难倒很多人，所以这篇我以自己的认知尝试让大家眼见为实。

### ASP.NET Core 6框架揭秘实例演示[37\]：重定向的N种实现方式

https://www.cnblogs.com/artech/p/17472647.html

在HTTP的语义中，重定向一般指的是服务端通过返回一个状态码为3XX的响应促使客户端像另一个地址再次发起请求，本章将此称为“客户端重定向“。既然有客户端重定向，自然就有服务端重定向，本章所谓的服务端重定向指的是在服务端通过改变请求路径将请求导向另一个终结点。ASP.NET下的重定向是通过RewriteMiddleware中间件实现的。（本文提供的示例演示已经同步到《ASP.NET Core 6框架揭秘-实例演示版》）

### 如何洞察 C# 程序的 GDI 句柄泄露

https://www.cnblogs.com/huangxincheng/p/17474733.html

前段时间有位朋友找到我，说他的程序界面操作起来很慢并且卡顿等一些不正常现象，从任务管理器看了下 `GDI句柄` 已经到 1w 了，一时也找不出什么代码中哪里有问题，让我帮忙看下，其实这种问题看内存dump作用不是很大，主要是写脚本很麻烦，这一篇我们就来简单聊聊如何洞察此类问题。

### 龙芯下如何进行.net core程序开发部署

https://www.cnblogs.com/silent2012/p/17474301.html

2022年4月，基础的运行时架构代码全部通过社区技术评审**.NET国际开源社区正式宣布支持LoongArch（龙架构），目前LoongArch64架构已出现在.NET社区主干分支上。**本文以.NETCore3.1在loongnix-server8.4下部署为例说明开发部署过程。

### 理解ASP.NET Core - 全球化&本地化&多语言(Globalization and Localization)

https://www.cnblogs.com/xiaoxiaotank/p/17466952.html

在众多知名品牌的网站中，比如微软官网、YouTube等，我们经常可以见到“切换页面语言”的功能，我们可以选择最适合的语言浏览页面内容。毫无疑问，为网站提供多种语言，页面内容本地化，大大扩展了受众范围，提升了用户体验。

### .NET的基元类型包括哪些？Unmanaged和Blittable类型又是什么？

https://www.cnblogs.com/artech/p/basic-types.html

在讨论.NET的类型系统的时候，我们经常提到“基元类型（Primitive Type）”的概念，我发现很多人并没有真正理解基元类型就究竟包含哪些（比如很多人觉得字符串是基元类型）。除了明确界定基元类型外，本篇文章还会简单介绍额外两种关于类型的概念——Unmanaged类型和Blittable类型。

## 主题

### 宣布 .NET 8 Preview 5 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-preview-5/

.NET 8 Preview 5 已经发布。

- SDK：改进的指标 API
    - 依赖注入 (DI) 友好的指标 API
    - 创建标记的仪表和仪器
- SDK：源链接现在是 .NET SDK 的一部分
- SDK：新的 .NET 库分析器
- SDK：Linux 上的独立构建
- SDK：非默认自包含
- Alpine ASP.NET Core Docker 复合图像
    - 使用新的 Ready-to-Run 格式编译 ASP.NET Core，将程序集组合成单个二进制文件（复合）以减小大小等，但失去了处理多个版本的能力。
- 运行时主机默认不使用 RID 图来确定特定于 RID 的资产
- 代码生成
    - 默认动态 PGO
    - 优化GC类型的ThreadStatic字段访问
    - Arm64，AVX-512
- C# Dev Kit 扩展并提高了 VSCode 的工作效率

### Visual Studio 2022 17.7 Preview 2 来了！- Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-7-preview-2-is-here/

Visual Studio 2022 17.7 Preview 2 已经发布。

- IDE 生产力和性能
    - 改进的文件比较
    - 创建拉取请求
    - 增强的多分支图支持
    - 并行堆栈过滤
    - 提高 F5 速度
    - 编辑速度优化
- .NET 开发
    - 自动反编译外部 .NET 代码
    - 新的 CPU 利用率自动化洞察
- 现代 C++ 和游戏开发
    - 为 C++ 构建洞察力
    - 虚幻引擎蓝图查找所有参考资料
    - 增强的 Doxygen 过载解析
- C++跨平台及嵌入式开发
    - 远程文件更新
    - WSL自动获取
- JavaScript 和 TypeScript 开发
    - Vite 新项目创建支持 React 和 Vue
- 企业管理
    - 标准用户的 Visual Studio 更新和更新
    - 管理员将私有布局添加到安装程序的“可用”选项卡

### .NET 8 Preview 5 中的 ASP.NET Core 更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/asp-net-core-updates-in-dotnet-8-preview-5/

.NET 8 Preview 5 中对 ASP.NET Core 的更新。

- 改进了 ASP.NET Core 调试体验
    - HttpContext、HttpRequest、HttpRequest、ClaimsPrincipal 上的 DebuggerDisplay 属性
- 服务器和中间件
    -`IHttpSysRequestTimingFeature`
    - `ITlsHandshakeFeature` 中的 SNI 主机名
    - `IExceptionHandler`
    - Blazor
    - 新的 Blazor Web 应用程序项目模板
    - 与 Blazor 路由器端点路由集成
    - 为 Blazor Server 的各个组件启用交互
    - 增强的 Webcil 包
    - Blazor 内容安全策略 (CSP) 兼容性
- API创作
    - 支持通用属性
    - SignalR
    - SignalR 无缝重新连接
    - 原生AOT
    - 支持 AsParameters 和编译时最小 API 的自动元数据生成
- 身份验证和授权
    - 更新了 ASP.NET Core SPA 模板的身份验证
    - 推荐使用 AuthorizationBuilder 的新分析器

### 在 .NET 8 Preview 5 中宣布 .NET MAUI - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-maui-in-dotnet-8-preview-5/

.NET 8 Preview 5 中对 .NET MAUI 的更新。

- iOS键盘滚动
- 增强测试
- 改进的性能
- 错误修复

### 发布 8.0.0-alpha.1 App-vNext/Polly GitHub
https://github.com/App-vNext/Polly/releases/tag/8.0.0-alpha.1

Polly 8.0.0-alpha.1 已经发布。

Polly v8 对 API 进行了重大更改，并以更少的开销构建在新的 API 上。此版本是其第一个预览版本。

- [Polly v8 - 架构更改问题 #1048 App-vNext/Polly](https://github.com/App-vNext/Polly/issues/1048)
- [我们需要您的反馈！介绍 Polly v8](https://www.thepollyproject.org/2023/03/03/we-want-your-feedback-introducing-polly-v8/)### .NET Framework 2023 年 6 月安全和质量汇总 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-framework-june-2023-security-and-quality-rollup/

.NET Framework 的 2023 年 6 月安全修复程序和累积更新已发布。

此版本包含 6 个安全修复和多个错误修复。

- CVE-2023-24897：远程代码执行（PDB 导致 MSDIA SDK 堆溢出）
- CVE-2023-29326：远程代码执行（WPF BAML 权限提升）
- CVE-2023-24895：远程代码执行（WPF XAML 解析器漏洞）
- CVE-2023-24936：权限提升（DataSet 和 DataTable XML 反序列化漏洞）
- CVE-2023-24936：拒绝服务（AIA 客户端证书获取过程漏洞）
- CVE-2023-29330：拒绝服务（X509Certificate2 文件文件处理漏洞）

### .NET 2023 年 6 月更新 – .NET 7.0.7、.NET 6.0.18 - .NET 博客
https://devblogs.microsoft.com/dotnet/june-2023-updates/

.NET 7.0.7、6.0.18 已经发布。

此版本包含各种安全修复和一些错误修复以及质量增强修复。

- CVE-2023-24895：远程代码执行（XAML 框架元素处理漏洞）
- CVE-2023-24897：远程代码执行（PDB 导致 MSDIA SDK 堆溢出）
- CVE-2023-24936：权限提升（DataSet 和 DataTable XML 反序列化漏洞）
- CVE-2023-29330：拒绝服务（X509Certificate2 文件文件处理漏洞）
- CVE-2023-29337：NuGet 客户端远程代码执行（竞争条件符号可利用漏洞）
- CVE-2023-32032：拒绝服务（Tar 文件提取漏洞）
- CVE-2023-33126：拒绝服务（崩溃和堆栈跟踪场景中的漏洞）
- CVE-2023-33128：拒绝服务（P/Invoke Source Generator 生成的代码内存释放漏洞）
- CVE-2023-33135：拒绝服务（.NET SDK 工具恢复权限提升漏洞）

### 介绍 CreatorKit - ServiceStack
https://servicestack.net/posts/creatorkit

CreatorKit 是在 .NET 中实现的 Mailchimp 的自托管替代方案，现已发布。

您可以管理邮寄列表和时事通讯订阅、发送可定制的电子邮件，并获得一套完整的工具，包括管理仪表板。

它是 ServiceStack 的一部分，对个人和开源项目免费。

### 发布 2.6.116 StackExchange/StackExchange.Redis
https://github.com/StackExchange/StackExchange.Redis/releases/tag/2.6.116

StackExchange.Redis 2.6.116 已经发布。

它包括针对本机 AOT 支持的错误修复和更新。

### Blazor Essentials – 新指南教程 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/06/13/blazor-essentials-new-guide-tutorial/

JetBrains 的 Blazor 介绍指南现已推出。

涵盖 Blazor，从实现表单、与 JavaScript 互操作和发布。

### 将 .NET Framework 4.8.1 发布到发布预览频道
https://blogs.windows.com/windows-insider/2023/06/13/releasing-net-framework-4-8-1-to-the-release-preview-channel/

.NET Framework 4.8.1 已发布到 Windows Insiders 的 Release Preview 频道。

已交付至适用于 Windows 11 21H2、Windows 10 21H2、22H2 的 Insider Preview Release Preview 频道。

.NET Framework 4.8.1 包括 Arm64 架构支持、辅助功能改进等。

### Rider 2023.2 EAP 5：改进了对 C# 的支持、更好的性能分析等。| .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/06/16/rider-2023-2-eap-5/

Rider 2023.2 EAP 5 已经发布。

该版本包括对 lambda 默认参数的支持、改进的 Disposable 检查、终端 WinPTY 到 ConPTY 的迁移、按线程分组的 dotTrace 显示等。

### ReSharper 2023.2 EAP 5：改进了对对象处置的控制，支持默认 Lambda 参数和 C++23 标准库模块。| .NET 工具博客

https://blog.jetbrains.com/dotnet/2023/06/16/resharper-2023-2-eap-5/

ReSharper 2023.2 EAP 5 已经发布。

此版本包括对 lambda 默认参数的支持、改进的 Disposable 检查、C++ 中的 C++23 标准库支持、按线程显示分组的 dotTrace 等。

### 在 Discord 上引入 Microsoft Store 频道 - #ifdef Windows
https://devblogs.microsoft.com/ifdef-windows/introducing-the-microsoft-store-channel-on-discord/#microsoft-store 

频道已在 Discord 上开通。

此频道位于 UWP 社区服务器上，可让你讨论与 Microsoft Store 应用和站点、合作伙伴中心、MSIX 程序包和安装程序相关的主题。

您可以在社区中进行讨论并与 Microsoft 团队互动。

### 发布 v1.0 Windows 地图：介绍适用于 Windows CommunityToolkit/Maui 的地图控件
https://github.com/CommunityToolkit/Maui/releases/tag/1.0.0-maps

.NET MAUI Community Toolkit 发布了适用于 Windows 的地图控件。

由于 Windows 没有将地图作为平台功能，并且不支持 .NET MAUI 的地图控件，因此 Bing 提供了一个托管在 WebView2 中的地图控件作为社区实现。

### 公共预览版：.NET 8 的应用服务支持 | Azure 更新 | Microsoft Azure
https://azure.microsoft.com/en-us/updates/public-preview-app-service-support-for-net-8/

宣布在 Azure 应用服务上抢先体验 .NET 8。

Azure 应用服务（Windows 和 Linux）上 .NET 8 的早期访问可用性。

### 使用 Microsoft Endpoint Manager (Intune) 配置 Visual Studio 策略 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/configure-visual-studio-policies-using-microsoft-endpoint-manager-intune/

将 Visual Studio 全局策略添加到 Microsoft Endpoint Manager (Intune) 设置目录。

这允许从 Intune 部署 Visual Studio 配置选项，以前需要手动 ADMX 上传直接从 Intune 进行管理。

## 文章、幻灯片等

### ASP.NET（.NET Framework）各个Session State Provider的大规模更新-Shibayan Miscellaneous
https://blog.shibayan.jp/entry/20230618/1687080471

ASP.NET (.NET Framework) 的会话状态提供程序更新摘要。

有一些使用SQL Server、Cosmos DB和Redis作为ASP.NET的Session State Provider，他们详细解释了今年更新的要点。

### 【VSCode、C#、AWS Lambda】在本地查看C#创建的Lambda Function的运行-Qiita
https://qiita.com/shin4488/items/a01fdf54daf626cb8742

关于如何在本地 Visual Studio Code 中检查在 .NET 中实现的 AWS Lambda 函数的运行情况。

### 在本地运行大型语言模型——你自己的 C# 类 ChatGPT AI
https://dev.to/maartenba/running-large-language-models-locally-your-own-chatgpt-like-ai-in-c-jco

如何使用 LLamaSharp 在您的本地环境中像 ChatGPT 一样与 LLM 实现 AI 聊天。

### 将 F# 编译为 Rust 🦀
https://jkone27-3876.medium.com/compile-f-to-rust-22cf5aa9021

如何将 F# 代码转换为 Rust 并运行它。

它介绍了如何使用 Fable 将 F# 代码转换为 Rust 代码并运行它。

### 在 ASP.NET Core Web API 中实现 Dapr 状态管理
https://dev.to/willvelida/implementing-dapr-state-management-in-aspnet-core-web-apis-42lk

了解如何利用 Dapr 状态管理来实现 ASP.NET Core Web API 应用程序。

### 使用 Sonic 加速您的应用搜索引擎
https://medium.com/@jesielpadilha.ti/speed-up-your-app-search-engine-using-sonic-a4ae788c4d6a

了解如何使用自托管搜索引擎 Sonic 实现搜索、添加等

###  我想用 C# 2 接触 ChatGPT API ~ ReadableStream ~ - Qiita
https://qiita.com/TellMin/items/9059423600a6897cef0c

如何将 ChatGPT API 的响应作为流处理（一种逐字逐渐返回响应的格式）。

### 如何使用 Entity Framework Core 实现软删除策略 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/06/14/how-to-implement-a-soft-delete-strategy-with-entity-framework-core/

如何在 Entity Framework Core 中实现软删除。

文章介绍了拦截器挂钩删除处理，查询自动过滤等方法。

### Reluctant BulkCopy（C#SqlClient实现示例）
https://zenn.dev/panda728/articles/55f45ba18cf29f

简单介绍SqlClient（SQL Server）中的BulkCopy。

### 使用 Project Orleans 在 .NET 平台上构建基于 Actor 的解决方案
https://www.infoq.com/articles/project-orleans-actor-based/

Orleans 的介绍、它的实现和它的好处。

### 使用 ASP.NET Core 在本地准备一个秘密 - Qiita
https://qiita.com/higege-amdeker/items/f403cb10b4c8337a7980

关于 User Secrets，它处理在开发 ASP.NET Core 应用程序时仅在本地保留的秘密。

### 支持旧版浏览器和 SameSite cookie，无需 UserAgent 在 ASP.NET Core 中嗅探。
https://andrewlock.net/supporting-legacy-browsers-and-samesite-cookies-without-useragent-sniffing-in-aspnetcore/

旧版浏览器中 SameSite cookie 的用户代理不可知支持技术。

### ASP.NET Core 8：使用 HTTP.sys 时使用 IHttpSysRequestTimingFeature 公开时间戳数据请求处理

https://anthonygiretti.com/2023/06/16/asp-net-core-8-expose-timestamp-data-request-processing-with-ihttpssysrequesttimingfeature-when-using-http-sys/

如何使用 .NET 8 中 ASP.NET Core 中添加的 IHttpSysRequestTimingFeature 在 HTTP.sys 环境下获取请求时间戳。

### Kubernetes 为 dotnet-monitor 改变 admission webhook？
https://www.poppastring.com/blog/kubernetes-mutating-admission-webhook-for-dotnetmonitor

寻求有关 Kubernetes 准入 Webhook 的 dotnet-monitor 支持的反馈。

### (C#) ValueTuple 大小和布局 - 猫的铃声通行费
https://ikorin2.hatenablog.jp/entry/2023/06/14/184523

关于 ValueTuple 在内存中的大小和布局。

关于 ValueTuple 有一个`StructLayout(LayoutKind.Auto)`，所以它的大小和布局不是恒定的。

### 从内部网站安装 Visual Studio - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/installing-visual-studio-from-an-internal-website/

如何从内部网站安装 Visual Studio。

关于在 Visual Studio 2022 17.6 及更高版本中从 Intranet 站点分发 Visual Studio 布局的能力的评论。

### Qt/.NET — 在 Qt 应用程序中托管 .NET 代码 (1/3)
https://www.qt.io/blog/qt/.net-hosting-.net-code-in-a-qt-application

如何在您的 Qt 应用程序中托管 .NET。

本文介绍了如何使用 Qt/.NET 托管 .NET 代码、如何从 Qt 应用程序调用 .NET 代码以及如何实现包装器。

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

如果提示已经达到200人，可以加我微信，我拉你进群: **lishi-wk**

另外也创建了**QQ群**，群号: 687779078，欢迎大家加入。 

## 抽奖送书活动预热！！！

感谢大家对我公众号的支持与陪伴！为庆祝公众号一周年，抽奖送出一些书籍，请大家关注公众号后续推文！