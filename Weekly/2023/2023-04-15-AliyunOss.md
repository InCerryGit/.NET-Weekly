## 国内文章

### Semantic Kernel 入门系列：📅 Planner 规划器

https://www.cnblogs.com/xbotter/p/semantic_kernel_introduction_planner.html

本文介绍了Semantic Kernel的一个核心能力，即实现目标导向的AI应用。文中以一个示例展示了如何使用Planner规划器，将一个目标分解为任务列表，并执行相应的技能，最终完成一个中文新闻稿的写作和发送。文中还介绍了Semantic Kernel的一些基本概念和使用方法，以及相关的参考资料。

### 介绍ServiceSelf项目

https://www.cnblogs.com/kewei/p/17321517.html

本文介绍了ServiceSelf项目，它是一个为.NET泛型主机的应用程序提供自安装为服务进程的能力的开源项目，支持windows和linux平台。本文还展示了如何使用nuget包和代码示例集成ServiceSelf，以及如何在不同平台下控制服务的安装和卸载。

https://www.cnblogs.com/xbotter/p/semantic_kernel_introduction_connector.html

本文是一篇关于Semantic Kernel的入门教程，介绍了Connector的概念和作用，以及如何在Native Function中使用Connector进行外部数据源和服务的对接。本文还给出了几个官方示例，展示了Connector的使用方法和场景。

### .NET Core反射获取带有自定义特性的类，通过依赖注入根据Attribute元数据信息调用对应的方法

https://www.cnblogs.com/Can-daydayup/p/17320282.html

本文介绍了.NET Core中如何通过反射和依赖注入根据自定义特性调用对应的方法，实现更灵活的编程方式。文章给出了自定义特性、服务类和反射调用的示例代码，并展示了输出结果。

### Semantic Kernel 入门系列：🥑Memory内存

https://www.cnblogs.com/xbotter/p/semantic_kernel_introduction_memory_part_2.html

本文介绍了Semantic Kernel的Memory功能，包括内存配置、信息存储、语义搜索、语义问答、引用存储和内存的持久化，以及相关的代码示例和参考资料。

### .NET 8新预览版本使用 Blazor 组件进行服务器端呈现

https://www.cnblogs.com/hejiale010426/p/17309490.html

本文是关于.NET 8预览版中使用Blazor组件进行服务器端呈现的介绍，作者分享了如何创建一个空的ASP.NET Core web app，并在其中添加一个简单的Razor组件，然后在Program.cs中设置Razor组件服务和映射组件的终结点，最后运行应用程序并查看组件渲染的效果。作者还尝试了给组件添加一个点击事件，但发现无法触发，欢迎大佬一起讨论新的技术。

### 【C#表达式树】最完善的表达式树Expression.Dynamic的玩法

https://www.cnblogs.com/1996-Chinese-Chen/p/17307019.html

本文介绍了C#表达式树的概念和用法，表达式树是定义代码的数据结构，基于编译器的解析和输出结构[1](https://learn.microsoft.com/zh-cn/dotnet/csharp/advanced-topics/expression-trees/expression-trees-explained)。作者展示了如何使用Expression.Dynamic方法和不同的绑定器来动态执行各种操作，如创建实例，调用方法，进行二元和一元运算，设置和获取属性和索引，判断属性是否是事件，调用委托，转换类型等。

### 由ASP.NET Core读取Response.Body引发的思考

https://www.cnblogs.com/wucy/p/17295708.html

本文主要讲解了如何读取ASP.NET Core中的Response.Body，分析了它的源码实现和原理，以及如何使用中间件和MemoryStream来解决默认情况下无法读取的问题。本文还对比了Http日志记录中间件的处理方式，以及为什么要把替换后的结果还原到原始的Response.Body上。本文是作者对ASP.NET Core源码探究的一部分，旨在分享自己的体验和思考，帮助读者更好地理解和使用这个框架。

## 主题

### 【英文】宣布 .NET 8 Preview 3 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-preview-3/

.NET 8 Preview 3 已经发布。

本文介绍了以下功能和改进：

* SDK
  - 简化的目的地路径
  - dotnet 工作负载清理命令

- 运行
    - 验证选项结果生成器
    - 配置绑定源生成器
    - 改进的本机代码生成
- 容器
    - 为多个平台构建图像
    - 非根用户 UID 值的环境变量

### 【英文】.NET 8 Preview 3 中的 ASP.NET Core 更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/asp-net-core-updates-in-dotnet-8-preview-3/

在 .NET 8 Preview 3 中引入 ASP.NET Core 更新。

此版本引入了各种新功能，例如 ASP.NET Core Native AOT 支持、支持范围/兼容性、模板等。

- ASP.NET Core 支持原生 AOT
- Blazor 中的服务器端呈现
- 在 ASP.NET Core 之外呈现 Razor 组件
- 支持 Blazor 中的部分
- 监控 Blazor 服务器线路活动
- 在 Blazor WebAssembly 应用程序中默认启用 SIMD
- 请求超时
- 短路路线

### 【英文】在 .NET 8 Preview 3 中宣布 .NET MAUI - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-maui-in-dotnet-8-preview-3/

在 .NET 8 Preview 3 中引入 .NET MAUI 更新。

此版本包括质量改进和改进的内存管理。

### 【英文】查看新的 C# 12 预览功能！- .NET 博客
https://devblogs.microsoft.com/dotnet/check-out-csharp-12-preview/

引入 C# 12 预览功能。

- 非记录类和结构中的主构造函数
- 任何类型的别名
- lambda 表达式中参数的默认值

### 【英文】.NET 2023 年 4 月更新 – .NET 7.0.5、.NET 6.0.16 - .NET 博客
https://devblogs.microsoft.com/dotnet/april-2023-updates/

.NET 7.0.5 和 6.0.16 发布。

此版本不包含任何安全修复，仅包含错误修复和小改进。

### 【英文】Windows 应用程序 SDK v1.3.0 的稳定通道发行说明 - Windows 应用程序
https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/stable-channel#version-13

Windows App SDK v1.3.0 发布。

此版本引入了几个新功能，例如 XAML Backdrop API（例如将 Mica 应用于窗口背景）和用于访问应用程序窗口的 Window.AppWindow API。

- [发布 v1.3.0 microsoft/WindowsAppSDK](https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.3.0)

### 【英文】mysql-net/MySqlConnector 发布 2.3.0 Beta 2
https://github.com/mysql-net/MySqlConnector/releases/tag/2.3.0-beta.2

Async MySQL Connector 2.3.0 Beat 2 已经发布。

此版本包括一些改进，例如在 MariaDB 上跳过元数据和 MySqlDataReader 回收提高性能。

### 【英文】NuGet.org 服务条款关于意外行为和仇恨言论的更新 - NuGet 博客
https://devblogs.microsoft.com/nuget/nuget-org-terms-of-service-update-on-unexpected-behavior-and-hate-speech/

更新 NuGet.org 服务条款。

服务条款已更新，增加了两条关于作弊的规则。一个是关于包描述或 README 中没有提到的意外行为（恶意后门等）的规则，另一个是关于仇恨言论的规则。

## 文章、幻灯片等
### 【英文】在 C# 应用程序中调试本机内存问题
https://ayende.com/blog/199265-A/debugging-native-memory-issues-in-a-c-application

一个关于调查 C# 应用程序中访问冲突的崩溃问题的故事。

Avx2读取内存时读取无效内存导致的问题。

### 【英文】使用 ASP.NET Core 的 Fluent Validation 进行数据验证
https://medium.com/c-sharp-progarmming/data-validation-with-fluent-validation-for-asp-net-core-6613c71211f8

如何在 ASP.NET Core 中使用 Fluent Validation 实现输入验证。

### 【日文】.NET + AvaloniaUI制作日记①
https://zenn.dev/jun_murakami/articles/87c79a3c622b6f

关于使用 Avalonia UI v11 预览所做更改的一些注意事项。

### 【英文】使用新的检测工具提高 Visual Studio 性能 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/improving-visual-studio-performance-with-the-new-instrumentation-tool/

一篇关于提高 Visual Studio 性能的文章，介绍了 Visual Studio 的新检测工具。

### 【英文】📈 通过 .NET 中的快照测试增强 REST API 的集成测试
https://dev.to/kamilbaczek/boost-your-integration-testing-for-rest-apis-with-snapshot-testing-g2b

了解如何使用 Verify 进行单元测试以比较和验证数据。

### 【日文】[C#11] 在通用数学中实现无溢出的加法
https://zenn.dev/shimat/articles/c4b5b05dcd85c7

在 Generic Math 中定义自己的 Vector 结构并实现它，使其在执行加法时不会溢出。

### 【英文】.NET 8 中的新功能🧐？发现所有 .NET 8 功能⚡🚀
https://medium.com/abp-community/whats-new-in-net-8-discover-all-net-8-features-bf98bc9cf68c

它引入了 .NET 8 的新功能和 Random.GetItems 等 API。

### 【英文】查看 C# 12 提案及其他提案
https://michaelscodingspot.com/csharp-12-proposals/

它介绍了 C# 12 提案和其他 C# 功能。

- 主要构造函数
- 半自动属性
- 扩展到 IEnumerable 以进行列表模式匹配
- Pure Unions 和 Discriminating Unions

### 【英文】使用 C# 规范化和比较 URL
https://blog.elmah.io/normalize-and-compare-urls-with-csharp/

如何粉碎、规范化和比较 URL 中包含的 ID。

### 【英文】ExternalFinalizer：向 3rd 方对象添加终结器
https://ravendb.net/articles/externalfinalizer-adding-a-finalizer-to-3rd-party-objects

一种在外部使用终结器来销毁没有终结器的对象的技术。

### 【英文】带有 SIMD 的 LINQ
https://steven-giesel.com/blogPost/faf06188-bae9-484d-804d-a42d58d18cad

尝试使用 SIMD 加速 LINQ 并实现一个库。

- [linkdotnet/LinqSIMDExtensions：C# 的类似 LINQ 的扩展，使用 SIMD 扩展来并行化操作](https://github.com/linkdotnet/LinqSIMDExtensions)

### 【英文】多租户访问的旅程继续存在一些问题
https://danielwertheim.se/the-journey-with-multi-tenancy-accesses-continues-with-some-issues/

多租户接入时的实现和注意事项。


### 【英文】使用嵌套任务
https://itnext.io/working-with-nested-tasks-9acd700c0e86

关于嵌套任务行为及其控制。

### 【日文】GitHub免费发布软件BOM创建功能——轻松管理漏洞
https://japan.zdnet.com/article/35202341/

介绍 GitHub 对导出 SBOM 的支持。

### 【英文】WASM、WASI、WTF?WebAssembly 101 – 面向 .NET 开发人员
https://speakerdeck.com/christianweyer/wasm-wasi-wtf-webassembly-101-for-net-developers

有关 .NET 开发人员的 WebAssembly、WASI 和 Blazor 的当前状态和未来的幻灯片。

### 【日文】C#客户端/服务器开发语言统一带来的高效开发系统~Pric-connection！大师级开发范例~
https://speakerdeck.com/cygames/sabanokai-fa-yan-yu-tong-gamotarasugao-xiao-lu-nakai-fa-ti-zhi-purikone-gurandomasutazukai-fa-shi-li

基于C#的客户端/服务器开发语言统一带来的高效开发体制~预联系！大型大师开发案例~

### 【日文】.NET 实验室学习会议 2023 年 4 月 - connpass
https://dotnetlab.connpass.com/event/279139/

- Azure OpenAI 服务概述和示例应用程序介绍
- 让我们使用 Microsoft PowerToys
- 适用于所有员工的 Windows 365 Frontline Cloud PC！
- 尝试在 Azure OpenAI 服务上使用带有 C# 的 ChatGPT
- 使用 CICD 部署 monorepo 库的故事

## 库、存储库、工具等。

### HoloLabInc/IwasmUnity：iwasm 的 Unity C# 包装器
https://github.com/HoloLabInc/IwasmUnity

### 用于 Unity 的 WebAssembly Micro Runtime 的 iwasm 绑定。

https://twitter.com/ikorin24/status/1646773888767119361?s=12


## 站点、文档等
### 推文
**谈论 AVX-512 支持**

https://twitter.com/egorbo/status/1645390605818773505?s=12

![image-20230419093559070](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230419093559070.png)

![image-20230419093626376](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230419093626376.png)

---

**谈谈对齐和不对齐在内存访问性能上的区别。**

https://twitter.com/egorbo/status/1646922981744992261?s=12

![image-20230419093512691](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230419093512691.png)

---

**谈论在 486 MS-DOS 上运行C#本机构建的代码 (SeeSharpSnake)。最后，它在真正的 PC 上运行。**

https://twitter.com/lukaaash/status/1644761881721044994?s=12

![image-20230419093444405](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230419093444405.png)



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