.NET周刊【10月第2期 2024-10-13】dotnet_week_24_10_2
## 国内文章
### C#/.NET/.NET Core优秀项目和框架2024年9月简报

https://www.cnblogs.com/Can-daydayup/p/18457705

文章介绍了多个与C#.NET和ASP.NET相关的优秀开源项目和框架，包括Avalonia UI、WaterCloud、CodeMaid、NetCoreServer等。这些项目各具特色，涵盖UI设计、快速开发、代码简化、网络服务器等领域。Avalonia UI支持跨平台应用，WaterCloud适合ASP.NET快速开发，CodeMaid提升开发效率，NetCoreServer适用于高并发网络应用。同时，Entity Framework Plus和Elasticsearch.NET等项目增强数据库操作和搜索功能。每个项目均附源码链接，方便开发者获取详细信息。

### YoloDotNet v2.1：实时物体检测的利器

https://www.cnblogs.com/shanyou/p/18457208

YoloDotNet v2.1 是一个基于 C# 和 .NET 8 的实时物体检测框架，整合了最新的 Yolov8 至 Yolov11 模型，支持 GPU 加速和多种视觉任务。它应用于智能监控、自动驾驶、工业检测、医疗影像分析和体育分析。该项目突出高性能、多功能、跨平台并开源免费。开发者可以通过简洁的 API 和丰富的示例代码轻松上手。YoloDotNet 适应复杂视觉任务，为不同用户提供高效可靠的解决方案。可以在 GitHub 获取这款工具并进行自由使用与分发。

### 一张图带你了解.NET终结(Finalize)流程

https://www.cnblogs.com/lmy5215006/p/18456380

文章介绍了终结机制，分为确定性和非确定性终结。确定性终结通过try-finally和using提供显式清理方法，非确定性终结则通过IDisposable和析构函数注册操作。终结机制并不等同于垃圾回收，而是用于处理对象持有的非托管资源。例子中展示了HttpClient在没有终结机制时可能导致资源未释放的问题，并通过代码示例说明了终结器的实用性和实现方式。

### .NET云原生应用实践（一）：从搭建项目框架结构开始

https://www.cnblogs.com/daxnet/p/18172088

本文主要介绍如何在.NET环境下构建云原生应用。作者计划通过“贴纸墙”案例，讲解使用ASP.NET Core Web API和Blazor WebAssembly实现微服务架构和容器化的分布式应用开发过程。文章探讨了云原生概念，强调容器化、微服务和动态管理等特性。计划使用nginx、Keycloak等搭建项目框架。本文旨在覆盖.NET云原生应用的各个方面，不从头介绍技术细节。读者需具备C#编程基础及设计模式等知识。工具推荐包括.NET 8 SDK、Visual Studio 2022和Docker等。

### .NET 8.0 酒店管理系统设计与实现

https://www.cnblogs.com/1312mn/p/18430990

本文介绍了基于.NET 8.0开发的酒店管理系统，适用于中小型酒店。系统使用多种开源工具，如Fody、SQLSugar、SunnyUI等，并详细列出了开发环境和功能模块。此应用无需安装即可使用，默认连接远程数据库。文章还提供了项目的GitHub和Gitee下载链接。希望文章能帮助开发者更好地设计酒店管理软件。

### C#|.net core 基础 - 删除字符串最后一个字符的七大类N种实现方式

https://www.cnblogs.com/hugogoos/p/18453906

文章介绍了删除字符串最后一个字符的多种实现方法。第一类方法使用字符串自带方法，如Substring、范围运算符、Remove和Create。测试显示Remove性能最佳。第二类使用StringBuilder，特别是Length方法表现优越。第三类方法涉及字符串与数组之间的转换，如For方法、Array.Resize和CopyTo方法。每种方法针对100、1000、10000长度字符串进行性能测试，StringBuilder的Length方法性能优于Append方法。

### PC软件开发新体验！用 Blazor Hybrid 打造简洁高效的视频处理工具

https://www.cnblogs.com/deali/p/18455870

作者在国庆假期期间更新了一款名为Clipify的小工具，这是对之前开发的QuickCutSharp进行的功能拓展。鉴于WinForms界面开发繁琐，作者决定使用Blazor Hybrid重新开发，并将其用于WinForms宿主容器。项目主要用到Blazor WebView、MediatR、xFFmpeg.NET等技术，以简化视频功能的实现。作者选择Blazor主要是因为不需要学习JavaScript框架即可实现交互，同时Blazor Hybrid允许直接调用系统功能，实现良好的开发体验。项目代码已开源，并提供了功能界面截图。

### .NET 白板书写延迟-触摸屏报点率

https://www.cnblogs.com/kybs0/p/18453947

触摸书写延迟是触摸屏的重要参数，影响应用如白板书写和游戏。关键因素包括触摸框报点率和软件延迟。报点率指每秒报告触控数据的次数。本文通过WPF应用程序探讨触摸数据间隔，举例Dell触摸屏报告约16-17ms间隔。触摸线程的合并操作减慢了WPF的响应速度。开启StylusPlugin可减少延迟，接近硬件帧率。市场上其他触摸框产品也表现出类似限制，由于WPF内可能阻碍更高帧率，从而降低书写延迟。

### .NET 8 实现无实体库表 API 部署服务

https://www.cnblogs.com/1312mn/p/18454788

该技术文章介绍了无需实体数据库即可进行增删改查操作的项目，支持多种查询条件、分页、列表等功能。项目提供详细的接口文档和多项高级功能，如Auth授权、接口限流、获取客户端真实IP及动态API等。特别适用于非技术人员，支持各平台的应用程序版本，易于部署和使用。项目依赖的技术包括Panda.DynamicWebApi、SqlSugar、Swashbuckle.AspNetCore等，并支持.NET 8 SDK开发环境。详细的前后端启动步骤指导用户轻松运行系统。文末提供了项目地址和社区交流信息，期望为.NET开发者提供帮助。

### 6款支持C#语言的AI辅助编程工具，开发效率提升利器！

https://www.cnblogs.com/Can-daydayup/p/18455117

文章介绍了6款AI辅助编程工具，均支持C#语言，并集成于DotNetGuide中。这些工具旨在提高编程效率，改善代码质量，支持多种语言和开发工具，包括Visual Studio、JetBrains等。每款工具提供不同的功能，如代码生成、代码注释、代码审核等。DotNetGuide技术社区为.NET开发者提供资源和交流平台，促进学习与成长。

### .NET云原生应用实践（二）：Sticker微服务RESTful API的实现

https://www.cnblogs.com/daxnet/p/18456878

文章探讨Sticker微服务的数据访问层设计，不引入复杂的领域驱动设计或ORM框架，而是选择ADO.NET，实现简单的数据存取。设计一个简单数据访问器（SDAC）来增删改查业务实体。通过接口定义和PostgreSQL集成，为未来潜在的ORM引入做好设计准备。在API实现中，使用SDAC管理数据。StickersController依赖SDAC接口，由ASP.NET Core注入。在后续部分，计划使用内存列表暂时实现SDAC，具体数据库实现将留待后续章节。

### .NET 代码混淆工具-JIEJIE.NET

https://www.cnblogs.com/1312mn/p/18435527

JIEJIE.NET是一款开源.NET程序集混淆工具，使用深度加密技术保护代码安全，防止未经授权的访问。由C#开发，解决其它工具无法满足的特定需求，完全免费且开源。主要功能包括名称混淆、控制流混淆、字符串和资源加密等。通过重命名类型和成员、随机化控制流、隐藏调用栈和加密字符串值等方法提高破解难度，有效保护软件版权。

### C#/.NET/.NET Core技术前沿周刊 | 第 8 期（2024年10.01-10.06）

https://www.cnblogs.com/Can-daydayup/p/18450775

本周刊专注于C#/.NET/.NET Core领域的最新技术动态。内容涵盖官方OpenAI库的发布、C#和.NET开发教程、LiteDB使用指南、EF Core查询可视化、Eto.Forms跨平台框架、ScottPlot绘图库、以及文件转换器应用等。此外，分享了EF Core扩展库和使用ValueConverters实现枚举显示的方法。一系列文章为开发者提供了丰富的资源，帮助提升开发效率和技术能力。DotNetGuide技术社区则是一个分享、学习和交流的平台，为.NET开发者提供全方位支持。

### ASP.NET Core OData 9的发布，放弃 .NET Framework

https://www.cnblogs.com/shanyou/p/18453400

微软于2024年8月30日推出ASP.NET Core OData 9包，此包与.NET 8 OData库一致。关键更改包括支持.NET 8及更高版本，不再支持旧版.NET Framework。OData 8库使用新的System.Text.Utf8JsonWriter进行JSON负载序列化，比旧的JsonWriter更快且节省内存。新的JSON写入器输出大写Unicode字符，而非ASCII字符不再编码为数字，从而提高效率。ASP.NET Core OData 9还在依赖注入中使用IServiceProvider。此新库移除了旧标准如JSONP格式，并作为NuGet包分发。源代码在GitHub上提供，并有多个未解决的问题。

### QToss：基于.NET架构的跨境电商的工具，助力企业实现智能数据营销

https://www.cnblogs.com/shanyou/p/18463099

2024年10月13日下午在深圳，一场跨境电商会议上，推出了由.NET技术支持的AI产品Qtoss。Qtoss是一款SaaS产品，结合.NET、多智能体系统、人工智能与数据智能，为企业提供高效智能的解决方案。其采用.NET机器学习框架BotSharp构建，具备稳定性、安全性以及扩展性，能处理海量数据和高并发。Qtoss利用多智能体系统实现业务协同，用AI技术进行精准营销和数据智能分析以洞察市场动态，为企业提供决策支持。Qtoss提升了跨境电商运营效率，同时展示了.NET在云原生和AI时代的强大功能。

### Blazor Hybrid 实战体验：那些你可能没预料到的坑没预料到的坑

https://www.cnblogs.com/deali/p/18458357

文章讨论了使用Blazor Hybrid技术时遇到的拖放事件限制、代码冗余、不易实现拖放功能和窗口调整不流畅等问题。Blazor Hybrid在拖放事件中仅获得文件流，缺乏对浏览器行为的控制，导致桌面应用体验差异。作者指出，这些问题影响了用户体验和开发者预期，尽管Blazor Hybrid具有跨平台开发的潜力。文章还探索了可能的解决方案和其他平台的比较。

### .NET 9 RC 2正式发布

https://www.cnblogs.com/shanyou/p/18455510

.NET 9 的第二个候选版本已发布，重点在性能和稳定性优化，未添加新功能。开发者被鼓励试用并反馈。新版本支持 Xcode 16 和新的 iOS、iPadOS SDKs，ASP.NET Core 模板更新至最新的 Bootstrap 和 jQuery 版本。可从 .NET 网站下载，推荐与 Visual Studio 2022 预览版一起使用。

### .NET 工控网关 轻量级组态软件

https://www.cnblogs.com/1312mn/p/18436159

SharpSCADA 是一个开源项目，提供轻量级工控网关和组态软件，支持多种工业协议如 Profinet、EtherNet/IP、Modbus，并通过 OPC 接口实现数据通信。其主要功能包括数据采集、归档、预警及人机界面设计，支持拖放、连线及变量绑定。项目使用 Visual Studio 作为开发工具，支持 SQL 数据库备份及还原。未来计划支持 .NET Core、增加更多通讯接口及图元组件并加强安全性。项目源代码可在 GitHub 上获取。

### .NET 实现的交互式 OA 系统

https://www.cnblogs.com/1312mn/p/18435039

文章介绍了一款基于 C# 和 ASP.NET 开发的办公自动化系统 MicroOA。此系统无需用户具备开发知识，提供直观界面可动态搭建表单和审批流程。系统适合于大量表单管理，支持文本框、列表框等元素的生成。使用 Visual Studio 2019 开发，运行环境需 Windows Server 2012 及 IIS。项目提供详细的部署和使用文档，便于快速上手。欢迎用户通过演示地址体验系统功能，并加入社区交流。

### C#轻松实现Modbus通信

https://www.cnblogs.com/xiketangedu/p/18461727

文章介绍如何在C#中使用开源库NModbus4实现Modbus通信，包括ModbusRTU和ModbusTCP协议。使用NModbus4，开发者无需关注协议细节，只需在库基础上进行简单封装即可实现串口或以太网通信。文章提供了具体的代码示例，展示了如何打开和关闭串口或TCP连接，以及读取保持寄存器和输出线圈的方法。文章强调NModbus4的开源特点和MIT许可证的灵活性。

### 分享几个实用且高效的EF Core扩展类库，提高开发效率！

https://www.cnblogs.com/Can-daydayup/p/18462503

文章介绍了三款开源的EF Core扩展库，旨在提升数据库开发的效率和灵活性。EF Core是一种跨平台的.NET对象数据库映射器。文中推荐的库包括Entity Framework Plus，用于提升性能和增加功能；Core Generic Repository，简化仓储层开发；以及ShardingCore，针对分表分库的高性能解决方案。这些工具已被列入优秀的C#/.NET项目和框架精选中，帮助开发者提高工作效率和质量。

### 如何自己动手实现一个图片解答小助手

https://www.cnblogs.com/mingupupu/p/18453894

这篇文章介绍如何使用C#调用Python实现图片文字识别。作者采用Python中的PaddleOCR进行OCR处理，并通过System.Diagnostics.Process在C#中运行Python脚本。文章详细描述了ProcessStartInfo各属性的用法，包括启动程序的路径、传递参数的方式以及输出处理等。作者还演示了如何通过命令行传递参数，使OCR处理更灵活。整体内容结合了.NET与Python技术，为开发者提供了实用的解决方案。

### WPF中的ListBox怎么添加删除按钮并删除所在行

https://www.cnblogs.com/lvpp13/p/18454644

本文讲解如何在C#中使用数据绑定和命令删除列表项。首先创建一个测试类BeautifulGirl并设置Name属性。接着在ViewModel中用ObservableCollection定义数据源，绑定到ListBox进行界面显示。然后，通过在每个ListBox项后面添加一个删除按钮，实现对列表项的删除。删除功能通过创建CommandBase类实现，使用ICommand接口处理Execute和CanExecute方法。最后在ViewModel中实例化DelCommand并绑定到UI，实现与用户交互并更新显示。

### Serilog文档翻译系列（七） - 应用设置、调试和诊断、开发接收器

https://www.cnblogs.com/hugogoos/p/18451412

Serilog支持在App.config和Web.config中通过简单的配置语法设置日志级别、添加属性和控制输出。主要通过代码配置，配置文件用于补充。可以从NuGet安装支持包并使用ReadFrom.AppSettings()方法读取配置。日志级别通过serilog:minimum-level设置。接收器通过serilog:write-to键添加，需确保唯一性。可指定接收器程序集和参数，支持环境变量展开。额外属性和命名空间最小级别覆盖也可通过配置实现。日志问题可通过SelfLog进行诊断。

### 数据结构 - 链表

https://www.cnblogs.com/hugogoos/p/18459678

文章详细介绍了链表的数据结构，包括链表的定义、分类和实现方法。链表是非顺序性和非连续性的存储结构，每个节点包含数据域和指针域。分类上，链表分为单向、双向和循环链表。实现部分通过自己管理内存，以自定义类和结构实现一个链表。具体实现步骤包括内存分配、初始化、长度获取和节点插入等操作。同时提供了相关代码示例。

### （系列六）.net8 全局异常捕获机制

https://www.cnblogs.com/cyzf/p/18460420

文章介绍OverallAuth2.0系统，为权限和流程管理提供解决方案。详细说明全局异常捕获机制的重要性，帮助优化日志记录，减少错误处理时间。通过创建接口返回模型和异常帮助类，简化错误响应和处理。此方法有助于提高系统的健壮性和用户体验。

### 如何创建免费版本的ABP分离模块？

https://www.cnblogs.com/hejiale010426/p/18449699

ABP最近更新后，通过Cli创建模板无法选择层次结构类型。为创建Trered模板，需卸载现有的Volo.Abp.Studio.Cli，并安装旧版本0.7.0的Cli。然后用于创建项目Raccoon，执行相应命令即可。这版本是最后的免费版本，其后版本均收费。创建项目后可看到熟悉的目录结构。

### WebAssembly 基础以及结合其他编程语言

https://www.cnblogs.com/SRIGT/p/18462925

WebAssembly（WASM）是一种新型编码方式，能够在现代浏览器中运行，通过将多种编程语言（如C/C++、C#、Go、Python等）编写的代码编译为WA格式，实现接近原生的性能。WASM具有高灵活度、紧凑的二进制格式，并可以与JavaScript共存。关键概念包括模块、内存、表格和实例。WASM代码通常编译成.wasm文件，并通过JavaScript API进行加载和运行。应用包括Figma等。不同语言（如C、C#、Go、Python）的代码可以通过编译工具转译为WASM文件，在浏览器环境中执行，这展示了WebAssembly的多语言兼容性和实用性。

## 主题

### .NET 9 候选版本 2 现已推出 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-9-rc-2/

.NET 9 候选版本 2 已发布。

此版本包括以错误修复为中心的质量改进，为正式版本做准备。

### .NET 和 .NET Framework 2024 年 10 月服务版本更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-and-dotnet-framework-october-2024-servicing-updates/

2024 年 10 月 .NET 和 .NET Framework 更新。 .NET 6.0.35、.8.0.10、.NET Framework 已发布。

此版本包括多项错误修复、改进和安全修复。

- [CVE-2024-38229](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2024-38229)：远程代码执行漏洞 (.NET 8、9)
    - [Microsoft 安全通报 CVE-2024-38229 | .NET 远程代码执行漏洞 · 问题 #326 · dotnet/announcements](https://github.com/dotnet/announcements/issues/326)
    - ASP.NET HTTP/3 处理中的 Use-After-Free
- [CVE-2024-43483](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2024-43483)：拒绝服务漏洞（.NET 6、8、9、.NET Framework）
    - [Microsoft 安全通报 CVE-2024-43483 | .NET 拒绝服务漏洞 · 问题 #327 · dotnet/announcements](https://github.com/dotnet/announcements/issues/327)
    - System.Security.Cryptography.Cose、System.IO.Packaging、System.Runtime.Caching 中的哈希洪泛
- [CVE-2024-43484](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2024-43484)：拒绝服务漏洞（.NET 6、8、9、.NET Framework）
    - [Microsoft 安全通报 CVE-2024-43484 | .NET 拒绝服务漏洞 · 问题 #328 · dotnet/announcements](https://github.com/dotnet/announcements/issues/328)
    - 由于 System.IO.Packaging 的输入不受信任而导致复杂操作中的拒绝服务
- [CVE-2024-43485](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2024-43485)：拒绝服务漏洞 (.NET 6、8、9)
    - [Microsoft 安全通报 CVE-2024-43485 | .NET 拒绝服务漏洞 · 问题 #329 · dotnet/announcements](https://github.com/dotnet/announcements/issues/329)
    - 由于对 System.Text.Json 中的“[ExtensionData]”属性中不受信任的输入进行反序列化而导致拒绝服务

### Microsoft.Extensions.AI 预览版简介 - .NET 的统一 AI 构建块 - .NET 博客
https://devblogs.microsoft.com/dotnet/introducing-microsoft-extensions-ai-preview/

Microsoft.Extensions.AI 已发布预览版。

Microsoft.Extensions.AI据说是SLM/LLM和Embedding等AI服务的抽象层。预览版包括 OpenAI、Azure AI Inference 和 Ollama 的参考实现。本文还介绍了如何安装和使用该库。

### 在 .NET 中设计可扩展矢量扩展 - .NET 博客
https://devblogs.microsoft.com/dotnet/engineering-sve-in-dotnet/#4.-beyond-code- Generation

关于 Arm64 上对 SVE（可扩展矢量扩展）的支持，该支持是在 .NET 9 中实验性添加的。

本文介绍了 API 的介绍、实际代码生成、API 实现过程中的测试、Native AOT 中的支持状态、限制等。

### 发布 Windows App SDK 1.5.7 (1.5.241001000) · microsoft/WindowsAppSDK
https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.5.7

Windows App SDK 1.5.7 已发布。

此版本包含多个错误修复。

## 文章、幻灯片等
### 使用新资源 (.resx) 管理器更轻松地本地化 - Visual Studio 博客

https://devblogs.microsoft.com/visualstudio/easier-localization-with-the-new-resource-resx-manager/

在 Visual Studio 中引入新的资源浏览器。

这篇文章涵盖了加载多个文件、搜索和过滤、评论翻译、检查文本中的占位符、可访问性和设置等内容。

### Draco 博客 - Draco 编译器两周岁生日快乐！
https://draco-lang.org/blog/birthday02

回顾 Draco 编译器开发两周年，Draco 是一种 .NET 专有编程语言。

### 取消，第 6 部分：链接
https://blog.stephencleary.com/2024/10/cancellation-6-linking.html

说明如何使用 CreateLinkedTokenSource 创建链接多个 CancellationToken 的 CancellationTokenSource、如何使用它以及陷阱。

### SIMD并行化库SmartVectorDotNet开发成果总结（四）C#和.Net的优化
https://zenn.dev/aka_nse/articles/e8a72ba241ac5b

用于实现 SmartVectorDotNet 库的优化技术的描述。

本文解释了泛型的运行时优化。

### C#/.NET - 如何在未连接到 nuget.org 的环境中进行构建
https://zenn.dev/j_sakamoto/articles/97f183b180ebed

如何在无法访问 nuget.org 的环境中（例如没有 Internet 连接时）安装 NuGet 包。

本文介绍了如何从缓存安装并使用本地包源。

### [C#] 使用反射尽可能快地获取类成员 - Qiita
https://qiita.com/radian-jp/items/97a1eaf3cec02d722fd4

比较使用反射读取属性和字段值的速度。

在本文中，使用 .NET Framework 4.8.1 和 .NET 8 进行了测量。

### 如何在 C# 中使用 DPAPI 安全地加密敏感数据
https://zenn.dev/nuits_jp/articles/2024-10-05-encrypt-sensitive-data-csharp-dpapi

了解如何在 Windows 中使用 DPAPI 加密数据。

### 使用 Octokit.NET 并使用设备流身份验证将文件直接添加到任何存储库
https://zenn.dev/nuits_jp/articles/2024-10-05-octokit-device-flow-auth

使用 Octokit 通过设备流进行身份验证并将文件添加到存储库的步骤。

### 支持 SLNX 解决方案文件 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/10/04/support-for-slnx-solution-files/

Rider 2024.3 EAP 现在支持新的解决方案格式 .slnx（预览版）。

本文介绍了如何保存为 .slnx 及其限制。

### .NET 中可用于语义内核的新函数调用 
https://devblogs.microsoft.com/semantic-kernel/new-function-calling-model-available-in-net-for-semantic-kernel/

引入 Semantic Kernel v1.20 支持的新函数调用。

### .NET 上的身份验证：OpenID Connect、BFF、SPA - DZone
https://dzone.com/articles/modern-authentication-on-dotnet

关于使用 BFF 模式通过 OpenID Connect 在单页面应用程序中实现身份验证。

### 使用 .NET 8 GraphQL 和 React 构建实时股票价格跟踪器：市场脉搏
https://www.codeproject.com/Articles/5387952/Building-a-Real-Time-Stock-Price-Tracker-with-NET

说明使用 GraphQL 连接 ASP.NET Core 服务器和 React 前端以实时显示股票价格的应用程序的示例实现。

### 【C#】Record（类）、Record struct、readonly 我们来反编译一下用 SharpLab 来看看 record struct 的实现 - Hanachiru 的我的笔记
https://www.hanachiru-blog.com/entry/2024/09/30/120000

我们正在使用SharpLab检查反编译结果，看看记录类型、值记录类型和只读值记录类型是如何实现的。

### SponsorLink v2：新希望
https://www.cazzulino.com/sponsorlink2.html

## 库、存储库、工具等。
### altmann/FluentResults：.NET/C# 的通用 Result 对象实现
https://github.com/altmann/FluentResults

用于实现使用类型表示成功/失败的结果模式的库。

- [C#“FluentResult”自述文件摘录的结果模式库 - Qiita](https://qiita.com/sy_delphoxy/items/29d56623f198b0f0aafc)## 网站、文档等
### 推文

我说的是从 Visual Studio 代码编辑器复制到 GitHub 或 Azure DevOps 代码的链接 (URL) 的功能。

https://x.com/mkristensen/status/1844419458787619211?s=12

![image-20241016204712564](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20241016204712564.png)

---

讨论如何将 IntelliSense 与 IEnumerable 可视化工具结合使用。

https://x.com/mkristensen/status/1844068358846808264?s=12

![image-20241016204739485](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20241016204739485.png)


## 版权声明

* 国内板块由 InCerry 进行整理 : https://github.com/InCerryGit/.NET-Weekly
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