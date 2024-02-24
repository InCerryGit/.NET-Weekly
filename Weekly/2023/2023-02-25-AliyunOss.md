## 国内文章

### .NET微服务系统迁移至.NET6.0的故事

https://www.cnblogs.com/InCerry/p/microservice-migration-net-6.html

本次迁移涉及的是公司内部一个业务子系统，该系统是一个多样化的应用，支撑着公司的多个业务方向。目前，该系统由40多个基于.NET的微服务应用构成，使用数千个CPU核心和数TB内存，在数百个Linux容器中运行。每天，该系统需要处理数十亿次请求。

### 我做的百度飞桨PaddleOCR .NET调用库
https://www.cnblogs.com/sdflysha/p/paddle-sharp-ocr.html

.NET Conf 2021中国我做了一次《.NET玩转计算机视觉OpenCV》的分享，其中提到了一个效果特别好的OCR识别引擎——百度飞桨PaddleOCR，可离线部署，后来我逐步把它封装了一下，代码全部开源（可点击查看原文跳转到Github）：https://github.com/sdcb/paddlesharp，可以直接安装NuGet包使用，支持.NET Framework/.NET Core、支持Linux、支持GPU调用，支持14种语言模型的自动下载。

### 快学会这个技能-.NET API拦截技法

https://www.cnblogs.com/Dotnet9-com/p/17139986.html

您是否曾经遇到过不属于您但想要更改其行为的类库方法？通常，该方法是非公开的，并且没有很好的方法来覆盖其行为。你可以看到它是如何工作的（因为你很棒，并且使用像Resharper、dnSpy之类反编译工具，对吧？），你只是无法改变它。你真的需要改变它，因为XXX原因。

### 研究C#异步操作async await状态机的总结

https://www.cnblogs.com/wucy/p/17137128.html

前一段时间得闲的时候优化了一下我之前的轮子[[DotNetCoreRpc\]](https://github.com/softlgl/DotNetCoreRpc)小框架，其中主要的优化点主要是关于RPC异步契约调用的相关逻辑。在此过程中进一步了解了关于`async和await`异步操作相关的知识点，加深了异步操作的理解，因此总结一下。关于`async和await`每个人都有自己的理解，甚至关于`异步和同步`亦或者关于`异步和多线程`每个人也都有自己的理解。因此，如果本文涉及到个人观点与您的观点不一致的时候请勿喷。结论固然重要，但是在这个过程中的引发的思考也很重要。

### 记一次 .NET 某医保平台 CPU 爆高分析

https://www.cnblogs.com/huangxincheng/p/17139891.html

一直在追这个系列的朋友应该能感受到，我给这个行业中无数的陌生人分析过各种dump，终于在上周有位老同学找到我，还是个大妹子，必须有求必应 😁😁😁。妹子公司的系统最近在某次升级之后，在高峰期会遇到 CPU 爆高的现象，有些单位你懂的，很强势，所以就苦逼了程序媛，不管怎么说，既然找上我，得想各种办法给解决掉，用远程的方式告诉了老同学怎么用 procdump 去抓 dump，在一个小时之后 dump 成功拿到，接下来就来分析了。

### 【译】.NET 7 中的性能改进(一到六)

一：https://mp.weixin.qq.com/s/w6nR6zOSazEi7fmHkxi3kQ

二：https://mp.weixin.qq.com/s/pduJO4E_qpL1Pqk_B4zpXQ

三：https://mp.weixin.qq.com/s/1hC7vJ3Rvl2aFolE44YV7g

四：https://mp.weixin.qq.com/s/jqQ4Wih-d9Gm-kopoLsIAQ

五：https://mp.weixin.qq.com/s/u-p4db392O07fhUV7oIFZg

六：https://mp.weixin.qq.com/s/C58z5OucltOI4WCeF2RqKw

一年前，我发布了.NET 6 中的性能改进，紧接着是.NET 5、.NET Core 3.0、.NET Core 2.1和.NET Core 2.0的类似帖子。我喜欢写这些帖子，也喜欢阅读开发人员对它们的回复。去年的一条评论特别引起了我的共鸣。评论者引用了虎胆龙威的电影名言，“'当亚历山大看到他的领域的广度时，他为没有更多的世界可以征服而哭泣'”，并质疑 .NET 的性能改进是否相似。水井干涸了吗？是否没有更多的“[性能]世界可以征服”？我有点头晕地说，即使 .NET 6 有多快，.NET 7 明确地强调了可以做的和已经做的更多。

### 使用一个文件集中管理你的 NuGet 依赖版本号

https://mp.weixin.qq.com/s/J1rmtcCLxODQdiQa0bsrqQ

在 .NET 7 以前，项目对于 NuGet依赖项的版本依赖散落与解决方案的各个角落。这导致升级维护和查看的时候都比较麻烦。在 .NET 7 中，你可以使用一个文件来集中管理你的 NuGet 依赖版本号。本篇文章将介绍如何使用这个功能。

### C# 如何部分加载“超大”解决方案中的部分项目

https://mp.weixin.qq.com/s/ut7KjJ_RqNU1BkCi8iGTmg

在有的特有的项目环境下，团队会将所有的项目使用同一个解决方案进行管理。这种方式方面了管理，但是却会导致解决方案变得非常庞大，导致加载时间过长。那么，如何部分加载解决方案中的部分项目呢？就让我们来借用微软退出的 slngen 工具来体验一下部分加载解决方案中的部分项目吧。

### 三星为其基于 RISC-V的 Tizen平台移植.NET

https://mp.weixin.qq.com/s/UccJv2cYje4bTM1qDTbyBQ

最近.NET团队在这篇文章中介绍了对.NET移植的一般政策：https://devblogs.microsoft.com/dotnet/why-dotnet/#binary-distributions。自从.NET 2014年开源以来，社区还扩展了 .NET 以在其他平台上运行。三星为其基于ARM的Tizen平台移植了.NET。Red Hat 和 IBM 将 .NET 移植到 LinuxONE/s390x。龙芯中科将.NET移植到LoongArch。 现在三星为其基于RISC-V的Tizen平台移植.NET。

### 用 Visual Studio 升级 .NET 项目

https://mp.weixin.qq.com/s/jEiXcCCwAxIk9Qe1RncULw

现在，你已可以使用 Visual Studio 将所有 .NET 应用程序升级到最新版本的 .NET！这一功能可以从 Visual Studio 扩展包中获取，它会升级你的 .NET Framework 或 .NET Core 网页和桌面应用程序。一些项目类型仍正在开发中并将在不久的未来推出，请参阅以下的详细信息。

### 初尝 .NET 8 Preview 1

https://mp.weixin.qq.com/s/8r4xejLlJGEotS5VjyU3tA

.NET 8 的第一个 preview 版本发布了，.NET 8 是新的 LTS 版本，有三年的长期支持，体验一下 .NET 8 preview 1 看看引入进来的变化.

### .NET 8 Preview 1 中新增的 Random 方法

https://mp.weixin.qq.com/s/AjLrwsMiBPUdUj2nTqto3Q

在 .NET 8 Preview 1 中引入了两个非常实用的 Random 方法，`GetItems` 和 `Shuffle`，下面我们简单的看个简单的示例吧。

### .NET 8 Preview 1 中 SDK 的更新

https://mp.weixin.qq.com/s/fC21hXMtjTxwRQY__LuC4A

在 .NET 8 中 dotnet publish 和 dotnet pack 的默认行为会发生一些变化，之前 publish 和 pack 默认是 Debug，从 .NET 8 开始默认的配置就变成了 Release。



**由于Mayuki大佬上周没有时间，所以国际板块没有简介，只有标题和链接。**

## 主题

### 【英文】Visual Studio 2022 - 17.5 发布 - Visual Studio Blog
https://devblogs.microsoft.com/visualstudio/visual-studio-2022-17-5-released/

### 【英文】.NET 8 Preview 1 发布 - .NET Blog
https://devblogs.microsoft.com/dotnet/announcing-dotnet-8-preview-1/

### 【英文】EF Core 8 Preview 1 发布: 原始SQL查询, 延迟加载和日期类型  - .NET Blog
https://devblogs.microsoft.com/dotnet/announcing-ef8-preview-1/

### 【英文】ASP.NET Core 在 .NET 8 Preview 1 中的更新 - .NET Blog
https://devblogs.microsoft.com/dotnet/asp-net-core-updates-in-dotnet-8-preview-1/

### 【英文】Visual Studio for Mac 17.5 现在发布 - Visual Studio Blog
https://devblogs.microsoft.com/visualstudio/visual-studio-for-mac-17-5-is-now-available/

### 【英文】.NET 2023年2月更新 - .NET 7.0.3 和 .NET 6.0.14 - .NET Blog
https://devblogs.microsoft.com/dotnet/february-2023-updates/

### 【英文】Windows 11 22H2版本中对.NET Framework更新的改进 - .NET Blog
https://devblogs.microsoft.com/dotnet/improvements-to-net-framework-updates-for-windows-11-22h2/

### 【英文】.NET Framework 2023年2月安全和质量滚动更新 - .NET Blog
https://devblogs.microsoft.com/dotnet/dotnet-framework-february-2023-security-and-quality-rollup-updates/

### 【英文】用Visual Studio升级你的.NET项目 - .NET Blog
https://devblogs.microsoft.com/dotnet/upgrade-assistant-now-in-visual-studio/

### 【英文】更新了WinForm的InitializeComponent的代码生成 - .NET Blog
https://devblogs.microsoft.com/dotnet/winforms-codegen-update/

### 【英文】Rider 2023.1 EAP 6: 新的用户界面改进和更好的调试体验 | The .NET Tools Blog
https://blog.jetbrains.com/dotnet/2023/02/24/rider-2023-1-eap-6/

### 【英文】microsoft/WindowsAppSDK 发布 v1.2.4 版本
https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.2.4

### 【英文】jbogard/MediatR 发布 v12.0.0 版本
https://github.com/jbogard/MediatR/releases/tag/v12.0.0

## 文章、幻灯片等
### 【英文】通过API使用实例最大化IntelliCode的价值，指尖上的真实世界代码实例 - Visual Studio博客

https://devblogs.microsoft.com/visualstudio/intellicode-api-usage-examples/

### 【英文】在macOS和Linux上开始使用dotTrace | The .NET Tools Blog

https://blog.jetbrains.com/dotnet/2023/02/22/getting-started-with-dottrace-on-macos-and-linux/

### 【英文】构建最终的RequestDelegate 最小API的幕后 - 第七部分

https://andrewlock.net/behind-the-scenes-of-minimal-apis-7-building-the-final-requestdelegate/

### 【英文】List 和 Span 模式匹配 - 在Rider和ReSharper中使用C# 11 | The .NET Tools Blog

https://blog.jetbrains.com/dotnet/2023/02/20/list-and-span-pattern-matching-using-csharp-11-in-rider-and-resharper/

### 【英文】Blazor的npm使用 - Qiita
https://qiita.com/villhell/items/9993a132767b284ba2f6

### 【英文】从.Net Framework MVC迁移到Blazor WebAssembly
https://codingberry.com/migration-from-net-framework-mvc-to-blazor-webassembly-faf5937acd2a

### 【英文】Blazor United - 解决Blazor的最大挑战？
https://jonhilton.net/blazor-united/

### 【英文】C# vs Rust vs Go. 在Kubernetes中进行性能基准测试
https://medium.com/@shyamsundarb/c-vs-rust-vs-go-a-performance-benchmarking-in-kubernetes-c303b67b84b5

### 【日文】在C#.NET中过滤和检索CloudWatch日志事件

https://zenn.dev/sbstani/articles/3c18a3a58e03b4

### 【英文】Visual Studio 2022现在可以在关闭时始终更新!

https://devblogs.microsoft.com/visualstudio/visual-studio-2022-can-now-always-update-on-close/

### 【英文】在Visual Studio中参考GitHub问题和拉动请求 - Visual Studio博客

https://devblogs.microsoft.com/visualstudio/reference-github-issues-and-pull-requests-in-visual-studio/

### 【英文】在MAUI中使用.NET Google API客户端库

https://medium.com/@CORDEA/using-net-google-api-client-library-wit-maui-11ae98e34a35

### 【日文】在.NET中考虑全角/半角，大/小写的字符串比较 - Qiita

https://qiita.com/miswil/items/9e139202337ce881ca5f

### 【英文】ASP.NET Core Web API中的异常处理与问题细节服务

https://medium.com/@a.skuratovich/exception-handling-in-asp-net-core-web-api-with-problem-details-service-1f29de4116d4

### 【日文】Blazor WebAssembly + OpenCVSharp: 一个在浏览器中工作的客户条码阅读器（实现） - Qiita

https://qiita.com/EmEpsilon/items/1e8c38ba2c5ebb906607

### 【日文】仍在工作! 查看Windows Forms应用程序的新功能（1） - rksoftware

https://rksoftware.hatenablog.com/entry/2023/02/18/160000

### 【英文】在几分钟内重构巨大的C#代码库

https://laurentkempe.com/2023/02/20/refactoring-huge-csharp-code-base-in-minutes/

### 【英文】任务事件处理程序 - 你不知道的小秘密 - Dev Leader

https://www.devleader.ca/2023/02/18/task-eventhandlers-the-little-secret-you-didnt-know/

### 【英文】.NET上的快速控制台IO

https://medium.com/@epeshk/fast-console-io-on-net-6cb56a6db529

### 【日文】Console.ReadLine()中断

https://zenn.dev/nuits_jp/articles/2023-02-18-cancelling-console-readline

### 【英文】使用.NET和C#开始使用MongoDB Atlas和Azure Functions | MongoDB

https://www.mongodb.com/developer/languages/csharp/getting-started-with-mongodb-atlas-and-azure-functions-using-net/

### 【日文】围绕着C#继承的一些小事

https://www.slideshare.net/mishizaki1/c-256109925

### 【日文】Orleans概览及基础配置部署 | ドクセル
https://www.docswell.com/s/hiro128_777/K6YMNL-2023-02-19-170020#p20

### 【日文】让我们使用 OpenTelemetry 进行测量，而无需重建 ASP.NET（.NET Framework）制作的应用程序 | ドクセル
https://www.docswell.com/s/tanaka_733/KLLXRQ-2023-02-24-csharptokto-opentelemetry-dotnet-autoinstrumentation-aspnetdfx

## 开源库、存储库、工具
### 在 Newtonsoft.Json 中使用 System.Text.Json 注释对象
https://medium.com/cloudnimble/using-system-text-json-annotated-objects-in-newtonsoft-json-ca51d23605c1

### 各个语言编译HelloWorld程序大小比较（越小越好）

https://github.com/MichalStrehovsky/sizegame

![image-20230227215158401](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230227215158401.png)

## 网站、文档等
### 推特
https://twitter.com/jamesnk/status/1627309572087218177?s=12

![image-20230227195014998](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230227195014998.png)

## 深入探索
### [跟踪] 在Webcil文件中发布.NET程序集 · Issue #80807 · dotnet/runtime
https://github.com/dotnet/runtime/issues/80807

### .NET 8预览版1中的新内容 [WIP］ · Issue #8133 · dotnet/core
https://github.com/dotnet/core/issues/8133

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