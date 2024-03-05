## 国内文章

### 在.NET 8 RC1 版本中 MAUI、ASP.NET Core 和 EF8 的新特性

https://www.cnblogs.com/shanyou/p/17698428.html

从年初2 月份发布第一个预览版，经历7个预览版后，Microsoft 西雅图时间9月13日发布了 .NET 8 RC 1： https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-rc1， 这是该框架在 11 月初正式发布之前的两个版本中的第一个。 .NET 8 RC1 是在生产中受支持，随着开发团队修复和完善内容，该框架基本上已经准备好了新的和令人兴奋的功能，以便在 11 月 14 日开始的 [.NET Conf 2023](https://www.dotnetconf.net/) 期间正式发布RTM。

- [.NET 8 预览版 1：NativeAOT 升级和新的Blazor United](https://www.cnblogs.com/shanyou/p/17143105.html)
- [NET 8 预览版 2 亮点是Blazor](https://www.cnblogs.com/shanyou/p/17220483.html)
- [ASP.NET Core 8 预览版 4的重大更新](https://www.cnblogs.com/shanyou/p/17437899.html)
- [.NET 8 Preview 5发布，了解一下Webcil 是啥](https://www.cnblogs.com/shanyou/p/17479138.html)
- [.NET 8 Preview 6发布，支持新的了Blazor呈现方案 和 VS Code .NET MAUI 扩展](https://www.cnblogs.com/shanyou/p/17546509.html)
- [.NET 8 发布的最后一个预览版Preview 7， 下个月发布RC](https://www.cnblogs.com/shanyou/p/17615851.html)

### .NET 8 Release Candidate 1 (RC1)现已发布，包括许多针对ASP.NET Core的重要改进！

https://www.cnblogs.com/hejiale010426/p/17698366.html

这是我们计划在今年晚些时候发布的最终.NET 8版本之前的两个候选版本中的第一个。大部分计划中的功能和变更都包含在这个候选版本中，可以供您尝试使用。您可以在文档中找到完整的[ASP.NET Core在.NET 8中的新功能列表](https://learn.microsoft.com/aspnet/core/release-notes/aspnetcore-8.0)。一些领域（尤其是Blazor）仍然有一些重大的变更待完成，我们预计将在下一个.NET 8候选版本中完成这些变更。

### .NET中测量多线程基准性能

https://www.cnblogs.com/baibaomen-org/p/17695662.html

多线程基准性能是用来衡量计算机系统或应用程序在多线程环境下的执行能力和性能的度量指标。它通常用来评估系统在并行处理任务时的效率和性能。测量中通常创建多个线程并在这些线程上执行并发任务，以模拟实际应用程序的并行处理需求。

### 升讯威在线客服系统的并发高性能数据处理技术：PLINQ并行查询技术

https://www.cnblogs.com/sheng_chao/p/17701792.html

我在业余时间开发维护了一款免费开源的升讯威在线客服系统，也收获了许多用户。对我来说，只要能获得用户的认可，就是我最大的动力。

> 最近客服系统成功经受住了客户现场组织的**压力测试**，获得了客户的认可。
> 客户组织多名客服上线后，所有员工**同一时间**打开访客页面**疯狂不停**的给在线客服发消息，系统稳定**无异常无掉线**，客服回复消息正常。消息**实时到达**无任何延迟。

> https://kf.shengxunwei.com/

我会通过一系列的文章详细分析升讯威在线客服系统的并发高性能技术是如何实现的，使用了哪些方案以及具体的做法。

本篇介绍 PLINQ 并行查询技术。

并行 LINQ (PLINQ) 是语言集成查询 (LINQ) 模式的并行实现。 PLINQ 将整套 LINQ 标准查询运算符实现为 System.Linq 命名空间的扩展方法，并提供适用于并行操作的其他运算符。 PLINQ 将 LINQ 语法的简洁和可靠性与并行编程的强大功能结合在一起。

### .NET Core 实现Excel的导入导出

https://www.cnblogs.com/lucasDC/p/17707810.html

我们在日常开发中对Excel的操作可能会比较频繁，好多功能都会涉及到Excel的操作。在.Net Core中大家可能使用Npoi比较多，这款软件功能也十分强大，而且接近原始编程。但是直接使用Npoi大部分时候我们可能都会自己封装一下，毕竟根据二八原则，我们百分之八十的场景可能都是进行简单的导入导出操作，这里就引出我们的主角Npoi。

### Avalonia开发（一）环境搭建

https://www.cnblogs.com/sesametech-dotnet/p/17705388.html

如题，介绍了如何使用跨平台的UI框架Avalonia开发.NET应用程序。

1. 开源 GitHub：https://github.com/AvaloniaUI/Avalonia/
2. 多平台支持，包括`Windows`、`mac OS`、`Linux`、`iOS`、`Android`、`Samsung Tizen`（很快支持）、`WebAssembly`
3. IDE支持，`Visual Studio`扩展支持，`JetBrains Rider` & `Resharper`支持
4. 依托`.NET`平台
5. 社区支持
6. `MIT` 协议

### C#反射实现插件式开发

https://www.cnblogs.com/wml-it/p/17706182.html

插件式架构,一种全新的、开放性的、高扩展性的架构体系。插件式架构设计好处很多，把扩展功能从框架中剥离出来，降低了框架的复杂度，让框架更容易实现。扩展功能与框架以一种很松的方式耦合，两者在保持接口不变的情况下，可以独立变化和发布。基于插件设计并不神秘，相反它比起一团泥的设计更简单，更容易理解。

### WPF动画入门教程

https://www.cnblogs.com/baibaomen-org/p/17696049.html

Windows Presentation Foundation (WPF)是一种用于创建Windows客户端应用程序的UI框架。它让我们能够创建丰富的图形界面，包括各种各样的动画效果。接下来，我们将介绍如何在WPF中创建简单的动画。文章最后将给出源码，源码包括文章中的动画和一个水印按钮，一个简单的时钟动画，一个复杂的时钟动画。

### 【算法】湖心岛上的数学梦-用C#实现一元多次方程的展开式 

https://www.cnblogs.com/lan80/p/17691306.html

如题所示，本文介绍了如何使用C#实现一元多次方程的展开式。

### Unity 游戏开发、03 基础篇 | C#初级编程

https://www.cnblogs.com/linxiaoxu/p/17703722.html

如题，使用C#进行Unity游戏开发的教程。

### 树莓派4b装系统到运行 Blazor Linux 本地程序全记录

https://www.cnblogs.com/densen2014/p/17706168.html

如题，树莓派4b装系统到运行 Blazor Linux 本地程序全记录。

### .NET使用quartz+topshelf实现定时执行任务调度服务

https://www.cnblogs.com/jack-yan/p/17700312.html

如题，使用quartz+topshelf实现.NET定时执行任务调度服务。

## 主题

### 【英文】发布 .NET 8 RC1 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-rc1/

.NET 8 RC1 已发布。

此版本包括对 System.Text.Json 的改进、Android 和 WASM 上的后 AOT IL 剥离、对配置绑定生成器的重大更改、切换到容器的非预览标签以及对非 Windows 上具有 Win32 资源的 Windows 应用程序的支持.它包括诸如建筑之类的支持。

### 【英文】EF Core 8 RC1：作为值对象的复杂类型 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-ef8-rc1/

Entity Framework Core 8 RC1 已发布。

本文介绍了 Entity Framework Core 8 中的一系列新功能以及对复杂类型的支持。

### 【英文】.NET 8 候选版本 1 中的 ASP.NET Core 更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/asp-net-core-updates-in-dotnet-8-rc-1/

关于更新 .NET 8 RC1 中的 ASP.NET Core。

- 服务器和中间件
    - HTTP/3 默认禁用
- API 编写
    - 支持 Minimal API、MVC、SignalR 中的密钥服务
- Blazor
  - Blazor Web 应用程序模板更新
  - 从静态服务器渲染中的附加程序集中发现组件
  - 路由改进
  - 触发页面刷新
  - 将任意属性传递给 QuickGrid
  - 判断表单域是否有效
  - 配置.NET WebAssembly运行时
  -  (AOT) 后修剪 .NET IL
- 身份
    - 删除用户名属性
- 单页应用程序（SPA）
  - 标准.NET 模板选项
- 性能指标

### 【英文】在 .NET 8 候选版本 1 中宣布 .NET MAUI：质量更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/announcing-dotnet-maui-in-dotnet-8-rc-1/

关于更新 .NET 8 RC1 中的 .NET MAUI。

此版本包括各种质量改进和对 Xcode 15 的支持。

### 【英文】.NET 8 中的性能改进 - .NET 博客
https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-8/

详细了解 .NET 8 中的性能改进。

它提供了广泛领域的改进的详细说明，包括 JIT、VM 和 GC，以及基元、字符串、集合、文件 I/O 和网络以及基准。

### 【英文】Visual Studio 2022 17.8 预览版 2 已发布！- Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-8-preview-2-has-arrived/

Visual Studio 2022 17.8 预览版 2 已发布。

此版本包括与 Git 和 GitHub 相关的改进、与 C++ 相关的改进、与 F# 相关的改进、跨平台编辑和继续/热重载支持、将 Linux 附加到应用服务以及 .NET 包括对带有 Meters API 的计数器的支持、测试分析、企业管理等等。

### 【英文】.NET 2023 年 9 月更新 – .NET 7.0.11、.NET 6.0.22 - .NET 博客
https://devblogs.microsoft.com/dotnet/september-2023-updates/

.NET 7.0.11 和 6.0.22 发布。

此版本包括五个安全修复，以及多项改进和错误修复。

### 【英文】.NET Framework 2023 年 9 月安全和质量汇总更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-framework-september-2023-security-and-quality-rollup-updates/

.NET Framework 2023 年 9 月安全和质量累积更新已发布。

此版本包括五个安全修复和多个错误修复。

## 文章、幻灯片等
### 【英文】LOH 与 POH：了解 .NET 堆的两个特殊堆

https://medium.com/@ramin.h/loh-vs-poh-understanding-the-two-special-segments-of-the-net-heap-60badb4842f0

关于.NET 5中引入的LOH（大型对象堆）和POH（固定对象堆）之间的区别。

### 【日文】ref 只读参数 - 通过引用传递
https://ufcpp.net/study/csharp/sp_ref.html#ref-readonly-param

C# 12 中“ref readonly”参数的解释。

### 【英文】构建最小的 ASP.NET Core 克隆
https://steven-giesel.com/blogPost/e84dec43-51f1-4c70-8b3b-dcdb1c3164ce

尝试通过实现控制器、DI、中间件和路由来重新创建最小的 ASP.NET Core。

### 【日文】[发行].NET 8 RC1！ C# 东京活动 - connpass
https://csharp-tokyo.connpass.com/event/296696/

9月19日（周二）将在C#东京举办分发活动。

### 【英文】在 .NET Core 中创建自定义运行状况检查
https://dev.to/me_janki/creating-custom-health-checks-in-net-core-e5n

了解如何实施自定义健康检查。文章实现了一个检查数据库连接的例子。

### 【英文】构建 Ambie 4.0
https://kidjenius.medium.com/architecting-ambie-4-0-c0a69da915db

关于在 UWP 中实现的名为 Ambie 的环境声音播放器的架构。

### 【英文】设计 Ambie 4.0
https://kidjenius.medium.com/designing-ambie-4-0-9615fdc7a752

关于在UWP中实现的名为Ambie的环境声音播放器的UI设计。

### 【英文】使用 JetBrains Annotations 对 ASP.NET Core 进行一流升级 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/09/14/first-class-upgrades-for-aspnet-core-with-jetbrains-annotations/

了解如何使用 JetBrains.Annotations 来改善 Rider 和 ReSharper 的 ASP.NET Core 应用程序开发体验。

### 【英文】Teams Toolkit for Visual Studio 2022 中有哪些新增功能？ - .NET 博客
https://devblogs.microsoft.com/dotnet/teams-toolkit-vs177-update/

引入 Teams Toolkit for Visual Studio 2022 中的新功能。

了解应用程序生命周期自动化、使用隧道进行调试等。

### 【日文】使用 Power Automate Desktop .NET 脚本操作数据表
https://zenn.dev/pfirsich/articles/3db3f81dc6436d

关于 Power Automate Desktop 中脚本操作支持的 .NET 脚本。

但是，可以使用的C#版本是5。

### 【英文】对本机编译的 .NET 应用程序进行逆向工程
https://migeel.sk/blog/2023/09/15/reverse-engineering-natively-compiled-dotnet-apps/

如何对 NativeAOT 反编译的 .NET 应用程序进行逆向工程。

### 【英文】不要在 Akka.NET 之上构建您自己的定制公司框架
https://petabridge.com/blog/akkadotnet-application-management-best-practices/

一篇文章推荐使用面向模式的方法，而不是在 Akka.NET 之上构建公司特定的框架。

### 【英文】平衡用户更新与安全最佳实践 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/standard-user-update/

介绍标准用户现在​​可以更新和安全功能。

### 【英文】使用自定义 YamlDotNet 类型转换器将复杂的 YAML 转换为 .NET 类型
https://dev.to/asimmon/convert-complex-yaml-to-net-types-with-custom-yamldotnet-type-converters-4l9

如何实现类型转换器以将复杂的 YAML 转换为 YamlDotNet 中的 .NET 类型。

### 【英文】.NET 迁移的故事 - 共享库
https://www.jimmybogard.com/tales-from-the-net-migration-trenches-shared-library/

介绍 .NET Framework 到 .NET 迁移方法中的共享库。

### 【日文】.NET 8 的 Azure Functions 更新已发布 - Shibayan Miscellaneous
https://blog.shibayan.jp/entry/20230912/1694509574

关于 Azure Functions 中的 .NET 8 更新。

除了Isolated和In-Process之间的对应关系之外，还涉及到ASP.NET Core集成方面对冷启动的一些改进。

### 【英文】使用 nx Standalone Angular 和 ASP.NET Core 服务器实现安全的 Web 应用程序
https://damienbod.com/2023/09/11/implement-a-secure-web-application-using-nx-standalone-angular-and-an-asp-net-core-server/

了解如何使用 Angular 和 ASP.NET Core 实现安全应用程序。

### 【日文】使用 Windows App SDK 创建具有现代标题栏的应用程序 - Shibayan Miscellaneous
https://blog.shibayan.jp/entry/20230911/1694400481

了解如何使用 Windows App SDK 的标题栏自定义为计算器和商店等现代 Windows 应用程序创建标题栏。

## 库、存储库、工具等。
### jonathanpeppers/dotnes：用于 NES 游戏控制台的 .NET
https://github.com/jonathanpeppers/dotnes

使用 .NET 为 NES (Famicom) 生成可执行二进制文件的工具。

它是通过将 MSIL 转译为 6502 程序集生成的。

### leonardochaia/dotnet-affected：.NET 工具，用于确定哪些项目受到一组更改的影响。对于大型项目或单一存储库很有用。
https://github.com/leonardochaia/dotnet-affected

用于找出哪些项目受变更集影响的工具。

### 异常可视化工具 - Visual Studio Marketplace
https://marketplace.visualstudio.com/items?itemName=elmahio.exceptioninspector

Visual Studio 的异常可视化工具扩展。

- [为 Visual Studio 2022 创建自定义调试可视化工具](https://blog.elmah.io/creating-custom-debug-visualizers-for-visual-studio-2022/)

https://x.com/thomasardal/status/1701220984320049643?s=12

## 网站、文档等
### 推文

在一个示例中，空集合的 GetEnumerator 全部返回相同的枚举器。
(如果你跟着代码走，似乎返回的是同一个具有单例的实例）。
如果应用这个方法和 PGO 的 guarded devirtualisation，foreach (var x in list ? []）类型循环可能会消失。

https://x.com/ufcpp/status/1703065887627231314?s=12

![image-20230923155107334](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230923155107334.png)

---

为了参加 #MicrosoftHackathon，我在 #VisualStudio 中为 C# 字符串添加了 SQL 语法高亮。

https://x.com/bricelambs/status/1702777696932266417?s=12

![image-20230923155222700](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230923155222700.png)

---

在阅读 Stephen Toub 关于 .NET 8 性能的文章时，我注意到 .NET 8 中引入了一个非常有趣的功能，但我从未听说过： [UnsafeAccessor]。
它允许您在忽略可见性检查的情况下获取目标类型的私有字段或方法的引用。因为它返回的是对字段的引用，所以你可以用它来读取和写入一个值。

例如，这对 Datadog 跟踪器非常有用，因为我们经常需要访问第三方库中的私有字段，以对其进行检测。为此，我们需要在运行时发射 IL，这对启动时间有很大影响。这项新功能为我们提供了零开销的替代方案。https://github.com/dotnet/runtime/issues/81741

https://x.com/kookiz/status/1702050892587954242?s=12

![image-20230923155345411](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230923155345411.png)

![image-20230923155357329](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230923155357329.png)

---

今天，我们回顾了 .NET 8 中的 C# 12 功能。集合字面量是我最喜欢的功能之一。代码生成也得到了大程度的优化，并将在未来的版本中变得更好！

https://x.com/davidfowl/status/1701449085784592888?s=12

![image-20230923155530514](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230923155530514.png)

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

