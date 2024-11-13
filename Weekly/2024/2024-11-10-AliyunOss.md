## 国内文章
### .NET 全能高效的 CMS 内容管理系统

https://www.cnblogs.com/1312mn/p/18511224

SSCMS 是一个完全开源的企业级内容管理系统，基于 .NET Core 开发，适合跨平台部署。其特点包括支持多终端发布和功能插件，具有完善的权限控制和安全机制，可通过标签和 API 接口进行二次开发。SSCMS 能管理多个网站和微信公众号，实现自动回复和用户管理等功能，提供多种内容模型和安全防护，并支持 Docker 部署。项目还提供详细开发文档及源码，用户可通过 GitHub 和 Gitee 获取项目更新。

### .NET 全功能流媒体管理控制接口平台

https://www.cnblogs.com/1312mn/p/18502466

AKStream是基于C#开发的全功能流媒体管理平台，支持GB28181、RTSP、RTMP等设备的控制。其具备低延时、标准Restful WebAPI接口和稳定的Sip信令网关。AKStream能在Linux、macOS、Windows系统运行，支持多种数据库。使用ZLMediaKit作为流媒体服务器，支持H265、H264等编码格式及流转换。其Web管理端AKStreamWebUI基于React和Vue框架，简化流媒体管理。用户可通过自动添加设备至数据库，实现设备管理和视频预览。平台提供流媒体服务的启动控制和配置热加载。项目代码可在GitHub和Gitee上获取。

### 一个.NET开源、轻量级的运行耗时统计库 - MethodTimer

https://www.cnblogs.com/Can-daydayup/p/18528659

.NET开发中，MethodTimer是一个开源库，能在编译时自动注入计时代码，简化手动计时。开发者可创建控制台应用并安装Fody和MethodTimer.Fody包，通过Time属性在方法上添加计时代码，避免重复编写。MethodTimer在编译时生成的代码使用Stopwatch进行时间统计，可通过ILSpy查看。MethodTimeLogger类提供两种耗时记录方式，分别以毫秒或TimeSpan形式输出。项目开源地址在GitHub和Gitee，并被收录于优秀项目和框架精选集中，供开发者借鉴和提交建议。

### .NET开发者福音：JetBrains官方宣布 Rider 非商用免费开放！

https://www.cnblogs.com/Can-daydayup/p/18524088

JetBrains宣布WebStorm和Rider IDE免费供非商业用途，支持学习、开源和业余开发。Rider是跨平台IDE，适用于整个.NET技术堆栈和游戏开发，支持C#、ASP.NET、Unity等。Rider提供智能代码补全、强大调试和单元测试功能，简化NuGet管理，支持多种版本控制系统，提升开发效率。

### 为 .NET Conf 2024 做好准备之本地社区活动 .NET Conf China 2024 启动

https://www.cnblogs.com/shanyou/p/18534346

.NET Conf 2024将于11月12日至14日举行。作为一个面向.NET生态系统的虚拟活动，旨在通过主旨演讲和展示为开发者提供关于.NET 9新功能的深入探讨，包括AI、Web和移动开发等领域的新技术。所有活动将被录制并上传至YouTube，便于后续观看。此次会议为开发者提供与专家互动和沟通的机会，是探索.NET前沿技术的绝佳平台。.NET Conf China 2024也即将举办，将展示云原生改进和智能应用开发的最新进展，为开发者提升生产力和简化部署流程提供支持。

### 我的博客网站为什么又回归Blazor了

https://www.cnblogs.com/Dotnet9-com/p/18533958

这篇文章描述了博客网站开发的历程，开发者使用了多种技术如MVC、Razor Pages、Vue、Go、Blazor等，网站经历了近10次迭代。目前网站使用Blazor和静态SSR技术，结合了Ant Design风格，提升了访问速度。文章感激了Known等开源项目的支持，介绍了网站的开源代码结构及其基于Blazor的开发框架KnownCMS的特点。提到了静态SSR技术的优点，如降低托管成本和提高可扩展性，并解释了静态SSR与Blazor Server和Blazor Client的区别及其SEO优越性。

### .NET Core  泛型底层原理浅谈

https://www.cnblogs.com/lmy5215006/p/18529501

文章介绍了泛型的优势如代码重用、类型安全和性能提升，重点在于减少装箱/拆箱带来的性能问题。泛型通过开放和封闭类型实现代码复用，但开放类型需在JIT编译阶段生成多种本机代码，影响性能。CLR通过共享方法体优化，引用类型实例能共享，而值类型则不行。示例代码验证了引用类型使用同一方法集的观点。

### .NET 8 高性能跨平台图像处理库 ImageSharp

https://www.cnblogs.com/1312mn/p/18528685

ImageSharp 是一个专为 .NET 设计的开源高性能图像处理库，特别适用于.NET8。它能够跨平台使用，提供丰富的图像处理功能和优异的性能。ImageSharp 支持 JPEG、PNG、GIF 等多种格式，以及多种像素格式和元数据编辑。它的主要功能包括图像裁剪、旋转、调整亮度对比度、应用滤镜等，并且操作简单。该库的安装也十分便利，通过 NuGet 包管理器即可轻松集成到项目中，适合桌面、Web 和云服务应用。

### .NET 高性能异步套接字库，支持多协议、跨平台、高并发

https://www.cnblogs.com/1312mn/p/18521691

.NET 生态中，NetCoreServer 是一个开源、高性能的异步通信框架，支持多种协议，如TCP、SSL、UDP和WebSocket等。它适用于高并发、低延迟的需求，跨平台支持Linux、macOS和Windows。开发环境包括.NET 6.0等，提供示例和详细文档，助力快速上手。它实现了多种服务器和客户端，如聊天服务器和HTTP服务器。性能测试涵盖回显和Web服务器测试等。该框架减少内存分配与CPU占用，优化网络I/O，以提升通信性能。

### 解决DDD最大难题-如何划分领域

https://www.cnblogs.com/xiaoweiyu/p/18531028

文章探讨了如何划分领域的原则，强调基于“创建xxx”需求来识别聚合根，进而划分领域。作者认为xxx需求代表了不可分割的整体，是系统的“原子单元”。当领域之间的复杂度可控时，可以考虑合并，否则应保持边界明确，避免耦合。文中强调通过需求分析和领域识别来控制系统复杂度。作者提到保持边界明确是设计中的核心价值观，符合域驱动设计（DDD）的理念。

### C# 单例模式的多种实现

https://www.cnblogs.com/Can-daydayup/p/18531236

单例模式是一种创建型设计模式，确保一个类只有一个实例并提供全局访问点。在C#中，单例模式可以通过饿汉式、懒汉式和懒加载实现，每种方式都有优缺点。设计模式的作用包括提高代码可重用性、增强可读性和提高系统可维护性。饿汉式在类加载时创建实例，实现简单，但可能浪费资源。懒汉式在首次访问时创建实例，通过锁机制保证线程安全。懒加载利用.NET的Lazy类实现线程安全的单例。

### AOT使用经验总结

https://www.cnblogs.com/Dotnet9-com/p/18529239

.NET AOT技术提前编译.NET代码为本机代码，提升启动速度和安全性，降低资源占用，支持老旧系统，方便部署，但挑战重重，需要细心测试。站长总结AOT项目经验，指出测试策略的重要性，需及时进行AOT测试，避免问题累积。同时需注意rd.xml配置，Prism和DryIOC容器支持，App.config管理，HttpClient和Dapper使用等问题。

### 一款.NET开源的屏幕实时翻译工具

https://www.cnblogs.com/Can-daydayup/p/18534867

Translumo是一款.NET开源屏幕翻译工具，支持实时翻译字幕等文本。它结合多个OCR引擎，通过机器学习选择最佳识别结果，界面简单，无需手动调整。翻译支持多种语言，适用于Windows 10/11，需Nvidia GPU与DirectX11。源码开放，收录于C#/.NET优秀项目中。

### 基于XAML框架和跨平台项目架构设计的深入技术分析

https://www.cnblogs.com/vickyqu115/p/18534549

本文探讨了基于XAML平台的多平台开发策略，详细介绍了WPF、Silverlight、Xamarin.Forms等主要框架，并讨论了在不同平台上选择.NET版本的重要性。建议选择.NET Core或最新的.NET版本来确保最大兼容性和性能。文章还分析了MVVM模式中View和ViewModel的连接策略。传统DataContext分配简便但耦合性强，而在XAML中实例化ViewModel虽提高预览能力但缺乏灵活性。最终建议使用.NET Standard 2.0编写通用库，并选择.NET 6及以上版本以获得最新特性。

### ASP.Net Core使用Jenkins配合pm2自动化部署项目

https://www.cnblogs.com/w821759016/p/18525620

文章介绍了如何配置一个软件项目，包括选择服务器，设置环境变量，管理源码，和构建步骤。详细步骤涉及到如何使用SSH命令传输文件、执行命令，以及如何配置Jenkins服务器以自动化这些流程。特别强调了如何使用参数化构建，实现根据不同环境和配置部署项目。最后指出了如何使用pm2和Powershell命令发布.NET Core程序到服务器并启动。

### 如何避免 HttpClient 丢失请求头：通过 HttpRequestMessage 解决并优化

https://www.cnblogs.com/morec/p/18529308

在使用HttpClient发起HTTP请求时，可能会遇到请求头丢失的问题，尤其是像Accept-Language这样的请求头。HttpClient设计为可复用以提高性能，但共享机制可能导致请求头在多线程请求中意外传递或丢失。本文探讨了这类问题的根源，并提供了解决方案。通过使用HttpRequestMessage可以更好地控制每个请求的请求头，避免丢失。示例代码展示了在多线程环境下，如何设置和发送请求，确保每个请求独立地设置请求头以获得正确的响应。

### 开源 - Ideal库 - 常用时间转换扩展方法（一）

https://www.cnblogs.com/hugogoos/p/18531206

作者分享了一系列方便软件开发的帮助类代码，这些代码将以《开源-Ideal库》系列文章和Nuget包形式发布。文章重点介绍了时间转换的封装，包括日期时间与时间戳之间的相互转换，涉及本地和UTC时间的转换方法。

### 基于surging 的木舟平台如何通过HTTP网络组件接入设备

https://www.cnblogs.com/fanliang11/p/18527947

木舟（Kayak）是基于.NET6.0的微服务引擎，支持异步和响应式编程。平台提供物模型、设备、产品和网络组件的管理，支持多种协议的适配与配置。木舟能够通过设备告警、消息通知、数据可视化等功能快速建立微服务物联网平台系统。本文介绍了创建与管理HTTP协议的网络组件，包括自定义协议模块的编码解码、协议说明文档、身份鉴权及数据上报例子。

### 使用Roslyn的源生成器生成DTO

https://www.cnblogs.com/vipwan/p/18535459

文章介绍了源生成器的优点，特别是在提高性能和实现AOT编译方面的作用。通过示例展示如何使用源生成器自动生成DTO及Mapper扩展方法。首先定义User类和UserDto，再通过AutoDto特性标注，让源生成器自动生成DTO代码。实现代码部分讲解如何在编译过程中利用源生成器生成所需代码。整体内容集中于改善C#程序开发中的对象映射问题，有效提升效率。

### dotnet core微服务框架Jimu ~ 会员注册微服务

https://www.cnblogs.com/flamesky/p/18533144

本文介绍如何使用.Net Core 6.0框架创建会员注册服务，用户需注册成为会员才能使用服务。系统提供两个API：CheckName用于检测用户名是否可用，Register则用于注册新会员。文章详细说明了接口的声明与实现，并运用Jimu框架来支持服务。项目包含接口类库Register.IServices和实现类库Register.Services，通过Jimu微服务框架接入。宿主服务器Register.Server通过控制台应用实现，并使用DotNetty进行通讯和Consul服务发现。整体过程展示了使用C# .NET技术创建微服务的步骤与关键点。

### MudBlazor：基于Material Design风格开源且强大的Blazor组件库

https://www.cnblogs.com/Can-daydayup/p/18536079

MudBlazor是一个开源的Blazor组件框架，使用Material Design风格，便于.NET开发者快速构建Web应用。它完全采用C#编写，允许自由调整和扩展，文档提供丰富示例。Blazor使用.NET框架和C#语言，通过Razor语法构建Web应用，能够替代JavaScript操控HTML DOM，适合创建单页应用和Web服务。MudBlazor框架强调使用C#编程，提升开发效率，降低学习成本。项目包括ASP.NET Core Blazor的快速入门指南和组件库的引入方法。

### 精选2款C#/.NET开源且功能强大的网络通信框架

https://www.cnblogs.com/Can-daydayup/p/18538257

本文介绍了两个C#/.NET丰富的网络通信框架：NetCoreServer和TouchSocket。NetCoreServer是一款高性能、跨平台、多协议支持的异步套接字库，适合创建可扩展网络应用。TouchSocket提供了一键解决TCP黏包问题和多种数据报文解析功能，支持多种通信模块。这些项目已被收录在C#/.NET优秀项目精选中，推动开发者们交流分享最佳实践。DotNetGuide技术社区则为.NET开发者提供资料学习、技术交流和项目推荐的平台。

### 在 Github Action 管道内集成 Code Coverage Report

https://www.cnblogs.com/kklldog/p/18538651

文章介绍如何在GitHub Actions上运行CICD pipeline，尤其是使用.NET工具进行代码构建、测试和覆盖率分析。作者成功解决了此前在集成测试中的问题，实现了测试和代码覆盖率的自动化。通过集成CodeCoverageSummary，Github Actions不仅可生成覆盖率报告，还支持多种配置。作者提供了详细的操作步骤和相关命令，帮助读者在Actions中查看代码覆盖率，提高项目的健康度。

### 基于surging 的木舟平台如何通过Tcp或者UDP网络组件接入设备

https://www.cnblogs.com/fanliang11/p/18538177

文章介绍了基于.NET6.0的surging微服务引擎开发的木舟平台，支持异步响应编程和多协议适配。它提供物模型、设备、产品和网络组件的统一管理。文章详细描述了如何使用Tcp和Udp网络组件接入设备以及创建自定义协议模块，包括协议说明、身份鉴权和消息编解码处理。此外，示例代码展示了如何通过特定解析脚本进行协议编码解码处理，提升了对不同设备和协议的适配能力。该平台通过设备告警、消息通知和数据可视化等功能，快速构建微服务物联网平台。

### 开源 - Ideal库 - 常用时间转换扩展方法（二）

https://www.cnblogs.com/hugogoos/p/18535467

文章介绍了用于时间和日期转换的多个扩展方法：将TimeOnly转换为DateTime，使用当前系统日期；将DateOnly与系统当前时间或指定DateTime中的时间合并；从DateTime提取日期或时间。虽然大多数方法是简单的原生方法调用，但使用扩展方法提高了编码效率。文章还讨论了代码结构的重要性，建议通过分类组织代码，提高可读性、可维护性和扩展性，例如按入参类型或功能分组。最后强调了单元测试的重要性，以确保代码的正确性。

## 主题
### ReSharper 和 .NET Tools 2024.3 候选版本现已推出 | .NET Tools 博客
https://blog.jetbrains.com/dotnet/2024/11/07/rsrp-net-tools-2024-3-rc/

### Rider 2024.3 候选版本现已推出 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/11/07/the-rider-2024-3-rc/

### 发布诊断版本 - v9.0.553101 · dotnet/diagnostics
https://github.com/dotnet/diagnostics/releases/tag/v9.0.553101

### 为 .NET Conf 2024 做好准备 - .NET 博客
https://devblogs.microsoft.com/dotnet/get-ready-for-dotnet-conf-2024/

### .NET 和 NuGet 生态系统的 OpenSSF 记分卡 - NuGet 博客
https://devblogs.microsoft.com/nuget/openssf-scorecard-for-net-nuget/


## 文章、幻灯片等
### smart F 开发的当前问题和未来计划 ~ 从 WinForms 到 Blazor ~
https://zenn.dev/nexta_/articles/789121c6186b51

### .NET 8 和 9 上 DataTable 数据提取方法的性能比较
https://zenn.dev/microsoft/articles/performance-of-datatable-on-dotnet9

### 使用 Next.js 和 .NET API 后端构建全栈应用程序
https://argosco.io/building-a-full-stack-application-with-next-js-and-net-api-backend/net/

### UUID v7 与 UUID v8：为可扩展分布式系统选择理想的标识符
https://medium.com/@anderson.buenogod/uuid-v7-vs-uuid-v8-choosing-the-ideal-identifier-for-scalable-distributed-system-fa8efc0550f7

### 将 Azure Functions（进程中）转换为 .NET8 时，函数主机不会启动
https://zenn.dev/tessecraft_r/articles/6b19ec48805fdb

### 引入一种新的、更具对话性的方式与 GitHub Copilot 聊天 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/conversational-way-to-chat-with-github-copilot/

### EF Core 与 VS2022 和 SQL Server 的官方培训
https://zenn.dev/zead/articles/6084fc2001212f

### 了解如何在新的 AI 季节中在 45 分钟内创建客户端-服务器应用程序 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/learn-how-to-create-a-client-server-application-in-under-45-mines-in-the-new-season-of-ai/

### NetEscapades.EnumGenerators 的最新更新：拦截器！
https://andrewlock.net/recent-updates-for-netescapades-enumgenerators-interceptors/

### dotInsights | 2024 年 11 月 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/11/04/dotinsights-november-2024/

### [C#] 我想在任务栏上运行PowerShell！
https://zenn.dev/onakamanpuku/articles/726ec3d99f3287

### 新的锁对象和历史记录
https://mareks-082.medium.com/new-lock-object-and-history-d69877f46521

### .NET 9 中的新增功能：System.Text.Json 改进
https://blog.elmah.io/whats-new-in-net-9-system-text-json-improvements/

### 如何使用 xUnit 如何准备测试用例并传递数据 - Qiita
https://qiita.com/te-k/items/c97425ab12ef2a73c34f

### 有关使用 .NET 应用程序连接到数据库的更多信息 - Qiita
https://qiita.com/tinymouse/items/a01087fc132b43e8dbb2

### 使用 Excel-DNA 创建异步处理函数 - Qiita
https://qiita.com/msms/items/0978934282c0067e6450

### 介绍 .NET 的现代 Web 应用程序 (MWA) 模式
https://techcommunity.microsoft.com/blog/appsonazureblog/introducing-the-modern-web-app-pattern-for-net/4278895

### .NET 9 中 System.Text.Json 的新增功能
https://okyrylchuk.dev/blog/whats-new-in-system-text-json-in-dotnet-9/

## 活动、分发等

### Visual Studio 用户社区日本学习会#7 (2024/11/30 13:30~)
https://vsuc.connpass.com/event/335130/

## 库、存储库、工具等。

### LittleLittleCloud/StepWise：使用 typescript 和 C# 构建的代码优先工作流引擎
https://github.com/LittleLittleCloud/StepWise

- [StepWise：用于任务执行的强大 C# 工作流引擎](https://dev.to/littlelittlecloud/stepwise-a-powerful-c-workflow-engine-for-parallel-task-execution-2nc4)

### velopack/velopack：跨平台桌面应用程序的安装程序和自动更新框架
https://github.com/velopack/velopack

- [(valopack)C#自动更新实现&WPF应用程序自动发布](https://zenn.dev/johmaru/articles/535c12baee666d)


## 网站、文档等
### 推文
https://x.com/dotnetfdn/status/1854534018768736410?s=12

![image-20241112221813739](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20241112221813739.png)

---

https://x.com/sergiopedri/status/1853853796063129979?s=12

![image-20241112221953020](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20241112221953020.png)

---

https://x.com/mkristensen/status/1852473805748498660?s=12

![image-20241112222530145](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20241112222530145.png)

---

https://x.com/mkristensen/status/1852033780338327705?s=12

![image-20241112222605109](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20241112222605109.png)

