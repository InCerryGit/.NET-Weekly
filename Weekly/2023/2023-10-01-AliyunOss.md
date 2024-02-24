## 国内文章

### .NET应用如何防止被反编译

https://www.cnblogs.com/Can-daydayup/p/17736700.html

本文主要讲述了如何防止.NET应用被反编译。虽然无法完全防止反编译，但可以通过混淆代码、加密敏感数据、动态生成代码、使用代码混合技术和代码签名等方法增加反编译的难度。文章还介绍了ConfuserEx，这是一款.NET代码混淆工具，支持多种混淆技术，包括控制流混淆、字符串加密、资源加密等。使用ConfuserEx工具可以对.NET Fx的.dll文件和.exe文件进行混淆，增加反编译的难度，提高代码的安全性。

### .NET开发工作效率提升利器 - CodeGeeX AI编程助手

https://www.cnblogs.com/Can-daydayup/p/17724111.html

本文介绍了CodeGeeX，一款基于大模型的全能的智能编程助手。CodeGeeX可以实现代码的生成与补全、自动添加注释、代码翻译以及智能问答等功能，帮助开发者显著提高工作效率。CodeGeeX2是其第二代模型，性能更优，支持多种主流编程语言和IDE。CodeGeeX的优势包括无需特殊网络即可使用，对个人用户完全免费，对中文支持友好，有详细的中文官方文档。此外，CodeGeeX还有VS Code插件，免费且易于安装。

### 模拟.NET应用场景，综合应用反编译、第三方库调试、拦截、一库多版本兼容方案

https://www.cnblogs.com/Dotnet9-com/p/17731551.html

本文首发于Dotnet9，作者是沙漠尽头的狼。文章设计了一个案例，教读者如何应用前两篇文章中的技能，并介绍了一种支持多个版本的库的兼容性解决方案。文章中，作者回答了读者关于Lib.Harmony库的疑问，并设计了一个小动画游戏，发布到NuGet上，引导读者一步步解决游戏中的问题。文章的目的是通过实际操作，让读者理解这个工具的正经用途。

### C#/.NET/.NET Core优秀项目和框架2023年9月简报

https://www.cnblogs.com/Can-daydayup/p/17739048.html

本文介绍了公众号“追逐时光者”定期推广和分享的C#/.NET/.NET Core优秀项目和框架。其中包括DncZeus，一个基于.NET 7 + Vue.js的通用后台管理系统框架；JIEJIE.NET和Obfuscar，两个.NET程序集混淆工具，用于保护.NET应用程序的版权和知识产权；ConfuserEx，一个功能强大的.NET代码混淆工具；以及Common.Utility，一个收集和整理了许多常用的C#帮助类和工具类库的项目。这些项目和框架都是开源的，源码地址在文章中有提供。

### 记一次 .NET某新能源MES系统 非托管泄露

https://www.cnblogs.com/huangxincheng/p/17727400.html

本文主要讲述了作者帮助朋友分析程序内存泄露问题的过程。首先，作者使用WinDbg工具对用户态内存段进行分组处理，发现可能存在托管内存泄露。然后，通过观察托管堆内存，发现托管堆的内存使用量并不大，推测可能存在非托管内存泄露。最后，作者提出可以通过监控VirtualAlloc，HeapAlloc分配来找出问题，但由于只有一个dump，所以作者建议可以查看clr的私有堆，也就是loader堆，以期找到新的线索。

### 使用 OpenTelemetry 构建 .NET 应用可观测性（3）：.NET SDK 概览

https://www.cnblogs.com/eventhorizon/p/17729014.html

本文主要介绍了OpenTelemetry .NET SDK的设计和使用，包括其核心组件如Logging, Metrics, Tracing等，以及如何在ASP.NET Core应用程序中使用。文章还提到了三个与OpenTelemetry相关的GitHub仓库：opentelemetry-dotnet（OTel SDK的核心库），opentelemetry-dotnet-contrib（第三方贡献的Instrumentation和Exporter），和opentelemetry-dotnet-instrumentation（无侵入的Instrumentation）。此外，文章还详细介绍了如何使用OTel SDK，包括安装依赖，使用Resource标识应用程序的元数据，以及通过ActivitySource实现的Tracing模块。

### 《HelloGitHub》第 90 期

https://www.cnblogs.com/xueweihan/p/17733161.html

"HelloGitHub"是一个分享GitHub上有趣、入门级的开源项目的平台。它提供了实战项目、入门教程、黑科技、开源书籍、大厂开源项目等，涵盖多种编程语言如Python、Java、Go、C/C++、Swift等。这里有适用于macOS的虚拟音频驱动BlackHole，用4个函数实现的C语言编译器c4，超好用的Windows优化器optimizer，免费开源的屏幕实时翻译工具Translumo，类似SQLite的分析型数据库duckdb，神似Vim的代码编辑器kakoune，简单好用的Web应用防火墙SafeLine，自己动手制作的触感智能旋钮smartknob等多个项目。

### EarthChat SignalR原理讲解

https://www.cnblogs.com/hejiale010426/p/17729734.html

SignalR是Microsoft开发的库，用于ASP.NET开发人员实现实时web功能，如实时聊天、通知、实时数据更新等。SignalR提供了抽象层的连接、连接管理、组播、扩展性和跨平台等特点。SignalR核心为.NET Core重新设计和实现的SignalR版本，提供了更好的性能和跨平台支持。MessagePack是一种快速而紧凑的二进制序列化格式，SignalR为MessagePack格式提供内置支持。横向扩展是一种增加系统容量的方法，通过在现有的硬件集群中添加更多的机器或节点来实现。SignalR通过一种称为“后端”或“后台”存储的机制实现横向扩展。

### 记一次 .NET 某拍摄监控软件 卡死分析

https://www.cnblogs.com/huangxincheng/p/17729749.html

本文主要讲述了如何使用WinDbg分析监控软件卡死的问题。首先，通过查看主线程的调用栈，发现程序在等待临界区锁。然后，通过提取RtlEnterCriticalSection方法中的参数，找到了持有锁的线程。最后，通过查看持有线程的线程栈，分析出它在等待某个对象。这种分析方法可以帮助我们找出导致软件卡死的原因，从而解决问题。

### Abp vNext 依赖注入

https://www.cnblogs.com/WangJunZzz/p/17729743.html

本文介绍了ABP的依赖注入系统，基于Microsoft的依赖注入扩展库开发，支持dotnet自带的注入方式。每个模块都定义自己的服务并在自己的模块类中通过依赖注入进行注册。同时，介绍了Autofac，一种常用的依赖注入框架，提供了动态代理和属性注入等高级特性。还介绍了如何集成Autofac，以及如何使用依赖注入，包括构造函数注入、属性注入和IServiceProvider。此外，还提到了一些特定类型会默认注册到依赖注入，以及在需要使用自定义工厂方法或singleton实例时，如何向IServiceCollection手动注册服务。

### WPF中以MVVM方式，实现RTSP视频播放

https://www.cnblogs.com/maoleigepu/p/17727894.html

本文主要讨论了在上位机开发中如何使用视频播放。作者首先提到了两种常见的解决方案：使用厂家提供的sdk和前端控件，或者开启相机onvif协议，通过rtsp视频流进行播放。然后，作者详细介绍了如何使用开源项目Flyleaf进行视频播放。Flyleaf是一个基于FFmpeg/DirectX的媒体播放器.NET库，适用于WinUI 3/ WPF/WinForms。作者详细介绍了如何在App.xaml和App.xaml.cs中配置ffmpeg的dll文件地址，并提供了相关代码示例。最后，作者提到了使用CommunityToolKit.MVVM作为MVVM框架。

### 开源.NetCore通用工具库Xmtool使用连载 - 扩展动态对象篇

https://www.cnblogs.com/bcbr/p/17731652.html

本文介绍了Xmtool工具库中的扩展动态对象类库，这是工具库中最重要的设计之一。扩展动态对象允许开发人员像使用Javascript一样，无需预定义就可以直接赋值使用数据对象，大大简化了定义过程。此外，扩展动态对象还提供了丰富的方法，如TrySetValue、TryGetValue、GetValue、GetValueByPath等，用于对动态对象进行更多的判断和控制，满足各种应用场景的需求。

### Abp vNext 模块加载机制

https://www.cnblogs.com/WangJunZzz/p/17728392.html

本文主要介绍了应用程序的生命周期和加载流程。生命周期包括添加依赖注入或其他配置前、中、后，初始化所有模块前、中、后，以及应用关闭执行等阶段。加载流程包括进入Startup，查看AddApplication源码，进入AbpApplicationWithExternalServiceProvider，查看AbpApplicationBase构造函数，以及查看加载模块逻辑等步骤。在加载模块逻辑中，会扫描模块并按照模块的依赖性重新排序。在ConfigureServicesAsync方法中，会依次执行每个模块的PreConfigureServices，ConfigureServices，PostConfigureServices。

### C#开源且免费的Windows桌面快速预览神器 - QuickLook

https://www.cnblogs.com/Can-daydayup/p/17732473.html

本文推荐了一款由C#开源且免费的Windows桌面快速预览工具：QuickLook。QuickLook提供了一种快速预览文件内容的方式，用户可以在不打开文件的情况下，直接在文件资源管理器中快速查看文件的内容。只需选中文件，在文件资源管理器中按下空格键即可快速预览文件。它支持多种文件格式，包括文本文档、图片、音频、视频等。此外，QuickLook还有许多亮点特性，如支持大量文件类型、Fluent设计、触摸屏友好、HiDPI支持、在打开和保存文件对话框中预览、与第三方文件管理器兼容、易于通过插件扩展、严格的GPL许可证等。

### 【23种设计模式】外观模式（十）

https://www.cnblogs.com/wml-it/p/17730188.html

"外观模式"是一种软件设计模式，它通过提供一个统一的接口来隐藏系统的复杂性，使得子系统更易于使用。在软件系统中，完成一个功能可能需要调用多个接口，这增加了开发难度和维护复杂度。外观模式通过封装这些接口，提供一个简单的外观，使得使用者只需调用一个接口就能完成任务。外观模式包括外观角色和子系统角色。外观角色将所有请求委派给相应的子系统处理，而子系统角色处理由外观角色传来的请求。外观模式的优点是简化了接口，实现了子系统与客户之间的松耦合关系。缺点是如果增加新的子系统可能需要修改外观类或客户端的源代码，违背了"开闭原则"。

### [WPF]浅析依赖属性（DependencyProperty）

https://www.cnblogs.com/czwy/p/17734460.html

本文主要介绍了WPF中的依赖属性，它可以节省内存开销，支持多属性值，并具有属性变化通知、限制、验证等功能。依赖属性的使用需要继承自DependecyObject，声明一个静态只读的DependencyProperty类型变量，并使用依赖属性的实例化包装属性读写依赖属性。依赖属性的存取值机制涉及到三个关键类型：DependencyProperty、DependencyObject、EffectiveValueEntry。其中，DependencyProperty是单例，存储了依赖属性的默认值和回调；DependencyObject是依赖属性的宿主对象，用于存储修改过值的依赖属性；EffectiveValueEntry存储依赖属性真实数值的对象，可以实现多属性值。

### Blazor前后端框架Known-V1.2.16

https://www.cnblogs.com/known/p/17734850.html

"Known"是一个基于C#和Blazor开发的前后端分离快速开发框架，具有跨平台、开箱即用的特点，一处代码可以在多处运行。它包含模块、字典、组织、角色、用户、日志、消息、工作流、定时任务等功能，代码简洁易扩展，使开发更简单、更快捷。在2023年9月28日的更新中，Known增加了系统管理模块列表查看链接、用户管理更换部门功能，修复了多个问题，并优化了运维人员字段配置。此外，还添加了获取用户信息接口，支持Server端呈现模式部署，并对多个组件进行了增强和优化。

### CAP项目集成带身份和证书验证的MongoDB

https://www.cnblogs.com/edisonchou/p/cap_with_authenticated_mongodb_practice.html

本文由Edison分享了如何在ASP.NET 6中使用带身份验证和SSL根证书验证的MongoDB的CAP事件总线。CAP是一个开源的事件总线项目，提供了多种存储方式，包括MongoDB。文章详细介绍了如何安装和集成CAP.MongoDB组件，并提供了相关代码示例。同时，文章还提到了CAP的Options选项，以及如何准确构造Mongo连接字符串。最后，文章假设了一个针对MongoDB的配置项格式，并提供了相关代码示例。

### Biwen.QuickApi代码生成器功能上线

https://www.cnblogs.com/vipwan/p/biwen-quickapi-gen.html

本文介绍了Biwen.QuickApi，这是一个使用REPR风格编写的minimalApi。最近，作者实现了一个代码生成器版本的Biwen.QuickApi，以解决代码中反射和动态带来的性能问题。Biwen.QuickApi的原理是反射查找所有标记[QuickApi]特征的Api，然后批量注册服务和批量映射路由。如果使用代码生成器，那么原来可能性能堪忧的代码就都变成了强类型引用，从而提高了性能。最后，作者提供了代码生成器的实现代码，并欢迎大家交流。

## 主题

### .NET 8 中的调试增强功能 - .NET 博客
https://devblogs.microsoft.com/dotnet/debugging-enhancements-in-dotnet-8/

### Polly v8 正式发布
https://www.thepollyproject.org/2023/09/28/polly-v8-officially-released/

- [发布 8.0.0 · App-vNext/Polly](https://github.com/App-vNext/Polly/releases/tag/8.0.0)

### CoreWCF v1.4 和 v1.5 预览版 1 发布 · 问题 #15 · CoreWCF/公告
https://github.com/CoreWCF/announcements/issues/15

- [CoreWCF 1.4.0 发布：添加 RabbitMQ 和 Apache Kafka 支持](https://www.infoq.com/news/2023/09/corewcf-140-released/)

### 发布诊断版本 - v7.0.447801 · dotnet/diagnostics
https://github.com/dotnet/diagnostics/releases/tag/v7.0.447801

### .NET Framework 2023 年 9 月累积更新预览 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-framework-september-2023-cumulative-update-preview/

### 先睹为快：Visual Studio“茶与技术”迷你系列 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-tea-technology-miniseries/

## 文章、幻灯片等
### CI/CD 释放：使用 Jenkins 和 Docker 优化 .NET Web 应用程序交付
https://medium.com/@shubnimkar/ci-cd-unleashed-optimizing-net-web-application-delivery-with-jenkins-and-docker-ed67ca06aeba

### 关于EF和SQLDB的加密 - Qiita
https://qiita.com/gsrh/items/cd77acbc2af350b3ee03

### 导入GitLab CI/CD自动进行C#/WPFapurike的Tesuto和insutorara的构建部署
https://zenn.dev/hacarus_blog/articles/3-gitlab-ci-for-c-application

### 处理 .NET 序列化中的未知枚举以进行 API 集成
https://gaevoy.com/2023/09/26/dotnet-serialization-unknown-enums-handling-api.html

### 服务器使用 .NET 7 发送事件
https://blog.devgenius.io/server-sent-events-with-net-7-4f06499a7762

### [C#]控制DI容器的范围 - Qiita
https://qiita.com/jun1s/items/a4ebf7e897dc3cb1fea9

### ASP.NET Core SignalR× 用Redis冗余Hub - Qiita
https://qiita.com/takasan/items/c9f245d0be24111e0cc1

### 防止 .NET 类库中的重大更改
https://medium.com/workleap/preventing-writing-changes-in-net-class-libraries-e61ae93b1b46

### .NET 的便利 - .NET 博客
https://devblogs.microsoft.com/dotnet/the-convenience-of-dotnet/

### 分析单元使分配消失 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/a-unit-of-profiling-makes-the-allocations-go-away/

### Rider 启动 2023.3 版本的抢先体验计划！ | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/09/25/rider-2023-3-eap1/

### 【Windows/C#】更改akusesutokun的特权 - Qiita
https://qiita.com/mitsu_at3/items/8e5fa9cdbd61a315cb32

### ReSharper 2023.3 抢先体验计划开始！ | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/09/25/rsrp-2023-3-eap1/

### 如何修改 ASP.NET Core 中间件中的响应标头
https://blog.elmah.io/how-to-modify-response-headers-in-asp-net-core-middleware/

### 在 C# 中访问私有成员而不进行反射 - Gérald Barré

https://www.meziantou.net/accessing-private-members-without-reflection-in-csharp.htm

### .NET 迁移战壕的故事 - 我们的第一个控制器
https://www.jimmybogard.com/tales-from-the-net-migration-trenches-our-first-controller/

### 功能标志 101：.NET 开发人员指南
https://www.code4it.dev/blog/feature-flags-dotnet/

### 通过 Nuke Build 上的代码构建 .NET 解决方案
https://medium.com/@alex.ozr/building-net-solutions-through-code-on-nuke-build-de40be06b091

### 在 .NET 中使用 Coverlet 进行测试覆盖率分析
https://victormagalhaes-dev.medium.com/test-coverage-analysis-with-coverlet-in-net-2e38df3c6ed7

### .NET 迁移战壕的故事 - 迁移初始业务逻辑
https://www.jimmybogard.com/tales-from-the-net-migration-trenches-migration-business-logic/

## 网站、文档等
### 推文

https://x.com/mhmd_azeez/status/1706713404415549906?s=12

![image-20231008212622262](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231008212622262.png)

---

https://x.com/egorbo/status/1706316706316996947?s=12

![image-20231008212702686](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20231008212702686.png)

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