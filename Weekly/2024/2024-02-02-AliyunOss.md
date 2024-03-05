**祝大家新年快乐，龙年大吉~**

## 国内文章

### C#/.NET/.NET Core优秀项目和框架2024年1月简报

https://www.cnblogs.com/Can-daydayup/p/18000401

本文介绍了公众号“追逐时光者”定期分享的C#/.NET/.NET Core优秀项目和框架，包括项目介绍、功能特点、使用方式和功能截图，并提供了源码地址。文章还特别推荐了三个项目：lin-cms-dotnetcore（仿掘金专栏CMS）、LKY_OfficeTools（Office自动化下载安装激活工具）和DevToys（为开发者设计的工具箱），每个项目都附有详细介绍和源码链接。

### 5个.NET开源且强大的快速开发框架（帮助你提高生产效率）

https://www.cnblogs.com/Can-daydayup/p/18004477

本文介绍了五个基于C# .NET ASP.NET的开源框架，包括中台Admin（基于.NET 8.0）、DncZeus（基于.NET 7和Vue.js）、WalkingTec.Mvvm框架（基于.net core）、OpenAuth.Net（集成多种技术）和Blog.Core（基于.NET Core 6.0和Vue 2.x）。这些框架可用于提高后台开发的效率，支持前后端分离，并集成了权限管理、任务调度等高级功能。同时，文章指出了这些项目和框架已被收录到C#/.NET/.NET Core优秀项目精选中，以及推荐了DotNetGuide技术社区交流群。

### Yarp 与 Nginx性能大比拼不出所料它胜利了！

https://www.cnblogs.com/hejiale010426/p/17998403

本文对比了Yarp和Nginx在Ubuntu 22.04.3 LTS系统上的性能。使用.NET 8 SDK和特定的配置文件，通过Native AOT部署了Yarp环境。同时，安装了Nginx并配置了代理服务。测试代理服务使用.NET 8 SDK创建，返回空字符串的简单接口。最后，使用runnerGo工具进行性能测试。文章提供了详细的环境搭建步骤和配置代码，以及测试工具的使用方法。

### FastGateway 一个可以用于代替Nginx的网关

https://www.cnblogs.com/hejiale010426/p/18004526

FastGateway是一个基于Asp.Net和Yarp的网关代理服务项目，能够实现动态加载HTTPS证书、动态路由管理、身份验证、监控、静态文件服务代理等功能。它采用前后端分离，动态管理均可通过界面操作，支持docker容器部署。FastGateway使用了如JWT和FreeSql等技术，并提供了详细的docker-compose配置指南，允许用户自定义账号密码和HTTPS证书。

### 【OpenVINO™】在 Windows 上使用 OpenVINO™ C# API 部署 Yolov8-obb 实现任意方向的目标检测

https://www.cnblogs.com/guojin-blogs/p/17999039

本文介绍了Ultralytics YOLOv8 OBB模型，这是一种基于深度学习的目标检测模型，能够检测任意方向的对象，提高了检测精度。该模型支持OpenVINO™部署工具，可加速模型推理，适用于多种硬件平台。文章还提供了项目链接，展示了如何结合OpenVINO™ C# API部署YOLOv8 OBB模型。同时，介绍了OpenVINO™ C# API的功能和优势，以及YOLOv8 OBB模型的特点和应用场景。最后，文章详细说明了模型下载、转换和部署的步骤，包括环境安装、模型导出、IR模型转换和项目配置。

### 一个 WPF + MudBlazor 的项目模板(附:多项目模板制作方法)

https://www.cnblogs.com/JiuLing-zhang/p/17999260

本文介绍了一个为.NET 8 + WPF + MudBlazor创建项目的模板，适用于VS2022。通过VS插件市场下载或Github源码编译，可以方便地搭建环境。模板制作包括创建项目、替换关键字和导出模板文件等步骤，通过VS的模板关键字和官方文档，可以制作出复杂的模板。

### Mocha MemoryBufferQueue 设计概述

https://www.cnblogs.com/eventhorizon/p/17997954

本文介绍了Mocha，一个基于.NET的APM系统，它使用MemoryBufferQueue作为内存缓冲区来处理大量数据。MemoryBufferQueue支持多Topic和Consumer Group，并发消费，批量消费，以及重试机制。Buffer模块通过接口抽象，保证了不同数据类型和Topic的BufferQueue相互独立。文章还详细描述了Buffer模块API设计和内部实现，确保了系统的灵活性和可扩展性。

### .NET NativeAOT 指南

https://www.cnblogs.com/hez2010/p/17999838/guidance-for-dotnet-nativeaot

本文介绍了.NET 8发布的NativeAOT应用模型，它在编译时创建依赖图并剪裁未使用代码，但对于反射和动态泛型实例化有限制。NativeAOT通过MSBuild属性启用，但编译器无法处理运行时确定的类型，如反射创建的实例。泛型类型的动态实例化也存在问题，因为编译器无法预测所有可能的实例化。文章还提出了解决这些限制的方法。

### 一次人脸识别ViewFaceCore使用的经验分享，看我把门店淘汰下来的POS机改成了人脸考勤机

https://www.cnblogs.com/datacool/p/18004303/ViewFaceCore2024

本文介绍了POS软件和基于人脸识别的考勤系统。POS是销售终端，能实现电子资金转账，具备消费、预授权等功能。文章提出了使用USB摄像头和改造的人脸识别程序来优化考勤系统，包括无人值守时自动关闭摄像头、记录考勤时间、同步人脸信息和取消传统的消息弹窗交互。还提供了检测键盘和鼠标无操作时间的代码，以判断是否有人使用系统。

### 物联网浏览器(IoTBrowser)-MQTT协议集成和测试

https://www.cnblogs.com/yizhuqing/p/18004476

MQTT是一种基于客户端-服务器架构的消息发布/订阅传输标准协议，特别适合于硬件性能低、网络环境差的远程设备和应用场景。广泛应用于物联网设备之间的通信，如卫星通信传感器、医疗设备和家居自动化。本文详细描述了如何在IoTBrowser平台中集成MQTT协议，并通过创建插件的方式提供了实现MQTT服务器(broker)和客户端的具体代码示例。

### 体验 ABP 的功能和服务

https://www.cnblogs.com/jackyfei/p/18002919

张飞洪在文章中分享了ABP框架的使用心得，强调了它在企业解决方案中的全栈功能。文章详细介绍了如何通过`ICurrentUser`服务获取当前用户信息，包括用户ID、用户名和电子邮件等，并解释了如何在ABP框架中注入和使用这项服务。此外，文章还讨论了与`ASP.NET Core`的集成，以及如何在ABP中定义和使用自定义声明。通过实现`IAbpClaimsPrincipalContributor`接口，可以将自定义声明添加到身份验证票据中，以便在用户请求时使用。

### 【译】命名变得简单：AI 支持的重命名建议

https://www.cnblogs.com/MeteorSeed/p/17995039

本文介绍了Visual Studio最新预览版中的一项新功能：AI支持的重命名建议。这项功能通过分析代码风格和标识符的使用，提供与代码库匹配的命名建议，旨在提升代码的可读性和可维护性。使用时，用户只需选择标识符并执行重命名操作，即可看到个性化的建议列表。该功能需要GitHub Copilot订阅，并在Visual Studio预览版中启用。开发者社区的用户反馈将帮助改进此功能。

### 利用 ASP.NET Core 开发单机应用

https://www.cnblogs.com/coredx/p/17998563

本文讨论了分布式微服务时代下，Web应用的分布式架构和单机应用的架构设计。提出了利用ASP.NET Core的TestServer实现类C/S架构的方法，通过内存流通信，减少网络和进程间通信的开销。同时，介绍了新书《C#与.NET6 开发从入门到实践》，并分享了如何通过复制开源项目代码来增强TestServer的HttpClient功能。最后，作者开发了RedirectHandler来处理需要真实网络交互的情况，它能够处理重定向响应。

### 【译】2023年——社区实验的一年

https://www.cnblogs.com/MeteorSeed/p/18001682

本文回顾了Visual Studio社区实验的成果，这些实验旨在提升用户效率和体验。实验包括多个功能，如区分Visual Studio实例、为括号对添加颜色、文件比较、带适当缩进的复制、获取开发者新闻、环绕选择、滚动文档选项卡和图像悬停预览。部分功能已集成到Visual Studio 2022中，如为括号对添加颜色、文件比较、带适当缩进的复制、环绕选择和滚动文档选项卡。其他功能，如区分实例和获取开发者新闻，尽管受欢迎但未集成，图像悬停预览计划在未来更新中加入。社区反馈和参与对这些实验至关重要。

### 应用--WebApplication

https://www.cnblogs.com/boise/p/18002731

本文介绍了.NET 6.0中的最小托管模型和WebApplication，它简化了Web应用的构建和配置。WebApplication通过封装主机和服务，提供了更简洁的API，如直接配置中间件和路由。构造流程包括获取WebApplicationBuilder，配置服务，构建WebApplication对象，配置中间件，运行主机。WebApplication.CreateBuilder(args)方法支持不同重载，便于根据不同需求创建WebApplicationBuilder对象。

### Json Schema高性能.net实现库 LateApexEarlySpeed.Json.Schema - 直接从code生成json schema validator

https://www.cnblogs.com/dotnet-diagnostic/p/17997545

本文介绍了LateApexEarlySpeed.Json.Schema库，它能从.NET类型生成JSON模式验证器。基本用法是通过JsonSchemaGenerator生成验证器实例。支持多种.NET数据类型和验证属性，如数值、字符串、枚举等。属性用法示例展示了如何通过特定属性限制数据。库默认引用类型可空，但可用NotNullAttribute指定非空。JsonRequiredAttribute和JsonIgnoreAttribute分别用于指定JSON数据中必须包含的属性和忽略的属性。还支持自定义属性名，如JsonPropertyNameAttribute和JsonSchemaNamingPolicy选项，包括驼峰、短横线、下划线等命名策略。

### 【OpenCV】在Linux上使用OpenCvSharp

https://www.cnblogs.com/guojin-blogs/p/17999002

本文介绍了OpenCV和OpenCvSharp的安装与配置。OpenCV是开源的计算机视觉库，支持多种语言和平台。OpenCvSharp是其.Net封装，适用于商业应用。文章详细说明了在Linux上使用C#和Visual Studio Code设置项目环境，创建控制台项目，添加Nuget包，以及安装依赖项目的步骤。通过这些步骤，可以确保项目包含必要的配置文件和依赖项，为使用OpenCV做好准备。

### WPF性能优化：形状(Shape)、几何图形(Geometry)和图画(Drawing)的使用

https://www.cnblogs.com/czwy/p/18000108

本文讲述了WPF中绘图的核心概念，包括形状(Shape)、几何图形(Geometry)和图画(Drawing)。形状是UI元素，可直接绘制且支持事件，但资源占用较多。几何图形定义了图形轮廓，需与Path结合使用，更轻量。图画在几何图形基础上增加了样式细节，也需结合使用。形状如直线、矩形、椭圆、多边形等，通过属性定义样式和尺寸。几何图形的子类如LineGeometry、RectangleGeometry等，与对应形状相似，但使用时需嵌入Path中。GeometryGroup和CombinedGeometry允许组合多个几何图形，StreamGeometry提供了一种性能优化的选择。通过这些工具，WPF能够创建丰富的2D图形和图像。

### XmlDocument 解决 Clone、CloneNode、ImportNode 等节点克隆后的标签自闭合问题

https://www.cnblogs.com/cyq1162/p/18003665

本文讲述了在对Taurus.Mvc进行HTML加载性能优化时遇到的问题。原先使用XmlDocument的LoadXml方法缓存和加载XML，但优化过程中发现使用Clone和CloneNode方法可以提升性能。然而，这些方法会导致空的div标签自闭合，特别是在.NET环境下。解决方案是通过继承XmlDocument并重写CreateElement方法，以确保标签不自闭合。尽管网上缺乏解决方案，但通过研究.NET源码找到了解决方法。

### 物联网浏览器(IoTBrowser)-Modbus协议集成和测试

https://www.cnblogs.com/yizhuqing/p/17997593

本文介绍了Modbus协议在IoTBrowser中的应用，通过串口插件模式与PLC或硬件设备通讯。文章详述了如何开发ModbusRtu和ModbusTcp插件，包括添加NModbus4等引用，并展示了ModbusRtuCom类的初始化过程，实现了与Modbus的通讯控制。

### 通过Demo学WPF—数据绑定（二）

https://www.cnblogs.com/mingupupu/p/18000305

本文介绍了如何在Data Binding中使用Linq创建Demo。首先创建空白解决方案，添加Linq项目，然后通过XAML代码定义窗口资源，包括Tasks对象和DataTemplate。DataTemplate用于设置任务展示模板，Tasks对象存储任务数据。通过键"MyTodoList"引用Tasks对象，实现数据与界面的绑定。最后，通过XAML元素<Window.Resources>定义资源字典，方便在窗口中重用资源。

## 主题

### 使用 SignalR 和其他开源工具构建人工智能驱动的 Microsoft Copilot - .NET 博客
https://devblogs.microsoft.com/dotnet/building-ai-powered-bing-chat-with-signalr-and-other-open-source-tools/

了解使用 SignalR 和其他开源工具构建的 Microsoft Copilot。

- 使用SignalR建立低延迟通信通道
- 使用自适应卡和 Markdown 编写 UI
- 申请流程
- 深入探讨：我们如何使用 SignalR

### Microsoft Office 的 RTC（实时通道）迁移到现代 .NET - .NET 博客
https://devblogs.microsoft.com/dotnet/office-rtc-dotnet-migration/

将 Microsoft Office 的实时通道 (RTC) 迁移到现代 .NET 的案例研究。

本书介绍了一个案例研究，其中用于 Office 应用程序中实时协作的基于 WebSocket (SignalR) 的服务从 .NET Framework 4.7.2 迁移到 .NET。

该公司声称迁移的结果是：“CPU 减少 30%”、“VM 成本减少 30%”、“内存和 GC 时间减少 60%” ”和“主要 API 的延迟减少了 50%”。

迁移涉及到迁移 ASP.NET 的 HTTP 模块和处理程序，确保 ASP.NET SignalR 和 ASP.NET Core SignalR 之间的兼容性，这些问题通过中间件得到了解决，以及迁移后出现的 IIS CPU 使用率问题。 SignalR Core 的 CPU 使用率过高以及如何处理。

其他主题包括使用事件计数器跟踪指标、部署到生产的结果以及未来的前景。

### Uno Platform 5.1：面向 Rider 和 VS Code 用户的实时向导、新控件、性能改进等。
https://platform.uno/blog/uno-platform-5-1/

Uno平台5.1已发布。

此版本为 Rider 和 Visual Studio Code 用户提供了一个向导，用于生成“dotnet new”命令来创建新项目，引入了 TimePicker 控件，提高了性能，减少了 .csproj 占用空间，并引入了 Uno Toolkit。包括更新和删除.NET 7 对 Uno 扩展的支持。

- [发布 5.1.31 · unoplatform/uno](https://github.com/unoplatform/uno/releases/tag/5.1.31)

### 介绍 MSTest Runner - CLI、Visual Studio 等 - .NET 博客
https://devblogs.microsoft.com/dotnet/introducing-ms-test-runner/

发布并推出 MSTest Runner，这是一个用于运行 MSTest 的轻量级工具。

MSTest Runner 的优点是能够独立运行，可以更轻松地在不包含运行时的环境中运行测试，并且占用空间较小。

### NuGetSolver 简介：用于解决 Visual Studio 中 NuGet 依赖关系冲突的强大工具 - NuGet 博客
https://devblogs.microsoft.com/nuget/introducing-nugetsolver-a-powerful-tool-for-resolving-nuget-dependency-conflicts-in-visual-studio/

隆重推出 NuGetSolver，这是一个用于解决 NuGet 版本冲突的工具。

NuGetSolver 是与 Microsoft Research 合作开发的 Visual Studio 扩展，可自动解决 NuGet 依赖项中的版本冲突。

本文还介绍了如何安装它，以及使用它时的注意事项和限制。

### Godot 4.2 中 C# 平台支持的当前状态
https://godotengine.org/article/platform-state-in-csharp-for-godot-4-2/

Godot 4.2 中 C# 平台支持的当前状态。

支持（每个平台的导出）如下。- 从 .NET 7 开始，Mono 支持 Android 导出
- 通过实验性 NativeAOT 导出 iOS .NET 8 支持
- 目前不支持Web导出
- Godot 4.0 支持所有桌面导出（包括适用于 .NET 7 及更高版本的 NativeAOT）

### 版本 1.5 Experimental (1.5.0-experimental2) - Windows App SDK 实验发布通道 - Windows 应用
https://learn.microsoft.com/ja-jp/windows/apps/windows-app-sdk/experimental-channel#version-15-experimental-150-experimental2

Windows App SDK 1.5.0-experimental2 已发布。

此版本修复了多个错误并添加了新的 API，包括与地图相关的 API。

### 发布稳定版 v5.1.5 · dotnet/SqlClient
https://github.com/dotnet/SqlClient/releases/tag/v5.1.5

Microsoft.Data.SqlClient v5.1.5 已发布。

此版本修复了多个错误。

### Rider 2024.1 路线图 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/01/24/rider-2024-1-roadmap/

Rider 2024.1 路线图。

* 用户体验/用户界面

- 调试器改进
    - Blazor WASM 应用程序的稳定调试体验
    - Blazor 上的热重载
    - 步骤执行时间和数据收集的可视化工具
    - 内联断点
    - 改进了运行到光标嵌入选项
- 游戏开发
    - Unity
    - 虚幻引擎
    - Godot
- Web开发
- 改进了 MAUI 支持
- 人工智能助手
- 智能拼写检查器
- 在容器和远程环境中执行单元测试
- 和我一起编码（测试版）

### ReSharper 2024.1 路线图 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/01/24/resharper-2024-1-roadmap/

ReSharper 2024.1 路线图。

- 默认预测调试模式
- 进程外更新
- Web开发
- 在容器和远程环境中执行单元测试
- 人工智能助手
- 其他计划

## 文章、幻灯片等
### 如何将 .NET Aspire 应用程序部署到 Azure 容器应用程序 - .NET 博客
https://devblogs.microsoft.com/dotnet/how-to-deploy-dotnet-aspire-apps-to-azure-container-apps/

创建 .NET Aspire 应用程序并将其部署到 Azure 容器应用程序的简单分步指南。

### 调试器的关注点：一年回顾 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/in-the-debuggers-spotlight-a-year-in-review/

Visual Studio 2022 2023 年提供的新的调试相关功能的总结和介绍。

- 加速内循环生产力
    - 断点组
    - 增强的文本可视化工具
    - 非模态可视化工具
    - 调用堆栈搜索
    - 改进的并行堆栈窗口
    - 永久重新连接到调试器进程
    - CMake调试器
- 使外部源代码更智能、更快速
- 跨平台调试支持
    - 使用 Visual Studio 集成终端调试 Linux 应用程序
    - 部署和调试到远程目标
    - 额外的 Linux 调试功能
- 性能升级

### .NET9 Alpha - LINQ 更新
https://medium.com/codenx/net9-alpha-linq-updates-c2df66d20e1b

介绍将添加到 .NET 9 中的 LINQ 的 CountBy 和 AggregateBy 运算符。

### .NET NativeAOT 指南
https://medium.com/@skyake/guidance-for-net-nativeaot-4b9853c80f8a

处理 NativeAOT 时应注意和应对的指南。

### 了解 C# 8 默认接口方法
https://andrewlock.net/understanding-default-interface-methods/

C# 8 默认接口实现的说明。关于可以做什么以及可能出现什么问题。

### 使用 dotnet-script 执行/调试 C# 脚本 - Qiita
https://qiita.com/toras9000/items/127548c73547f893995c

关于使用 dotnet-script 运行和开发 .csx（C# 脚本）。

### 您应该了解的 JetBrains Rider 中的 12 种调试技术 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/01/29/12-debugging-techniques-in-jetbrains-rider-you-should-know-about/

介绍 JetBrains Rider 的 12 种调试技术。

- 内联监控
- 返回值
- 智能单步调试
- 断点选项
- 拖动执行指针
- 调试外部反编译代码
- 异常断点
- 运行和调试静态方法
- 编辑并继续
- 内存视图
- 线程特定的断点
- 调试器显示属性支持
- 奖励：预测调试器

### 代码审查和时间旅行
https://ayende.com/blog/200577-B/code-review-time-travel

回顾一下RavenDB开发过程中学到的代码审查。

### .NET 8 中 BinaryFormatter 的替代品
https://steven-giesel.com/blogPost/4271d529-5625-4b67-bd59-d121f2d8c8f6

引入序列化器作为过时的 BinaryFormatter 的迁移目标。

### .NET 性能分析：.NET 8 中的 Newtonsoft.Json 与 System.Text.Json
https://trevormccubbin.medium.com/net-performance-analysis-newtonsoft-json-vs-system-text-json-in-net-8-34520c21d054

Newtonsoft.Json 和 System.Text.Json 之间的简单序列化/反序列化性能比较。

### 在 WinUI 3 应用程序中利用 WinForms 功能
https://zenn.dev/shinta0806/articles/winui3-winforms

有关在基于 WinUI 3 的应用程序中使用 Windows 窗体功能的说明。

### 【C#程序】EnityFramework Core枚举一百万条数据库记录消耗多少内存？ | @jsakamoto
https://devadjust.exblog.jp/29836607/

使用 Entity Framework Core 枚举（查找）100 万条记录时大约使用多少内存。

### 我在 rustc_codegen_clr 上的工作经历 - 半年回顾
https://fractalfir.github.io/ generated_html/rustc_codegen_clr_v0_1_0.html

回顾我花在实现 Rust 的 MSIL 后端的六个月时间。比如什么样的项目，有什么样的障碍。

### 使用 ASP.Net+Swagger+TypeScript 自动生成 Enum 显示名称
https://dev.to/garicchi/aspnetswaggertypescriptdeenumnobiao-shi-ming-wozi-dong-sheng- Cheng-suru-1hoh

使用 ASP.NET Core 和 Swagger 从 OpenAPI 架构生成 TypeScript 代码时，如何处理枚举名称混乱的问题。

### 如何开始使用 .NET Aspire 和 Sekiban 创建应用程序
https://zenn.dev/jtechjapan_pub/articles/3da012ed4b49ed

有关通过结合 .NET Aspire 和独特的事件源框架来创建使用 Cosmos DB 作为数据存储的应用程序的说明。

### 使用 GitHub Copilot 的新功能更快更好地编写代码：斜线命令和上下文变量 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/copilot-chat-slash-commands-and-context-variables/

介绍 Visual Studio 中 GitHub Copilot 的新功能。

- 斜线命令
- 上下文变量
- 预览功能
    - 调试器中的异常助手
    - 断点表达式建议
    - 提交消息建议
    - 解决方案参考
    - 性能分析器中的建议
    - 失败测试分析

### 在 C# 中取消数组 (Span) 的移位可以吗？ - Qiita
https://qiita.com/sator_imaging/items/49585b191af978b00ad2

如果您编写的代码在不移动跨度时导致重叠，会发生什么情况，以及 Unity/IL2CPP 会发生什么情况...

### .NET 垃圾收集的工作原理
https://notnullvariable.com/2024/440/

介绍 .NET 垃圾收集的工作原理。

## 库、存储库、工具等。

### NuGet 库 | PlantUmlClassDiagramGenerator.SourceGenerator
https://www.nuget.org/packages/PlantUmlClassDiagramGenerator.SourceGenerator

生成 PlantUML 类图的源生成器。

- [使用 Source Generator 从 C# 源代码生成 PlantUML 类图 - Qiita](https://qiita.com/pierusan2010/items/cdd628f202a9767cf65d)


## 网站、文档等
### 推文

关于 Silverlight Toolkit 示例如何与 OpenSilver 几乎一样工作的故事。

https://x.com/opensilverteam/status/1752735210846781602?s=12

![image-20240210205841934](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240210205841934.png)



## 深入探索

### 史诗：.NET 9 中的 IDistributedCache 更新 · 问题 #53255 · dotnet/aspnetcore
https://github.com/dotnet/aspnetcore/issues/53255

分散高速缓存。NET9中更新的Issue。

### .NET 9 中剩余 AssemblyBuilder.Save 工作的跟踪问题 · 问题 #92975 · dotnet/runtime
https://github.com/dotnet/runtime/issues/92975

面向.NET9的AssemblyBuilder.Save()问题。

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

![image-20230703203249615](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230703203249615.png)