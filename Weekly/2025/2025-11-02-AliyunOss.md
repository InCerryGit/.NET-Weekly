## 国内文章
### 《手搓》TaskFactory带你安全的起飞

https://www.cnblogs.com/xiangji/p/19168188

文章讨论了如何使用手动创建的TaskFactory进行程序优化。通过示例，解释了小牛在实现批量获取产品详情时面临性能问题。小牛最初的代码使用了直接await，导致程序效率较低。通过上游的并发限制，小牛的优化尝试失败。最终，作者介绍了ConcurrentTaskFactory，成功降低了请求时间，提升了并发控制能力，并指出HTTP服务的多线程特性。这篇文章不仅传授了优化技巧，还反映了数据库并发访问的挑战。文章结构清晰，条理分明。

### ASP.NET Core WebApi 集成 MCP 协议完全指南

https://www.cnblogs.com/saodiseng2015/p/19172165

本文介绍了模型上下文协议(MCP)在ASP.NET Core WebApi中的集成方法。MCP是一个开放标准，帮助AI客户端如ChatGPT连接API。文章详细说明MCP支持的功能，包括自动发现API、标准化工具描述、多种传输模式及安全认证。作者提供了具体实现步骤，包括NuGet包的安装、MCP服务的配置、以及MCP工具的定义。代码示例展示了如何设置MCP服务器和工具。此外，内容适用于使用.NET相关技术的开发者，具备较高实用性和技术深度。

### 《HelloGitHub》第 115 期

https://www.cnblogs.com/xueweihan/p/19169421

HelloGitHub 分享各种有趣的开源项目，涵盖多个编程语言，如 C、C#、C++ 和 Go。C# 项目包括 DepotDownloader，它是一个 Steam 游戏资源下载工具和 PKHeX，一个宝可梦存档编辑器。此外，SlideSCI 提供 PPT 编辑插件。该平台旨在使用户在短时间内体验开源的乐趣。每月更新，项目涉及实战教程和黑科技，吸引初学者和开发者探索更多可能性。

### Blazor 感觉回到了ASP时代？

https://www.cnblogs.com/shenchuanchao/p/19176211

这篇文章探讨了Blazor与ASP时代的相似之处，如服务端渲染和状态管理机制。作者强调Blazor并非简单复古，而是现代技术的进化，具备组件化和双向数据绑定特性。Blazor Server与经典的Web开发流程相似，使用C#构建逻辑，但比传统ASP更高效、灵活。文章还提出Blazor WebAssembly作为单页应用的解决方案，提升了数据交互的实时性。总之，Blazor为.NET开发者提供了新路径，让其更容易进入现代Web开发领域。文章表达清晰，逻辑严密。 

### .NET开发上手Microsoft Agent Framework(一)从开发一个AI美女聊天群组开始

https://www.cnblogs.com/GreenShade/p/19172851

文章介绍了微软的多个AI开发框架，包括AutoGen、Semantic Kernel和Microsoft Agent Framework，着重阐述了Microsoft Agent Framework的多智能体协作功能及其优势。该框架支持工作流编排，提供Handoff和GroupChat模式，并与Azure AI Foundry深度集成。文章还通过实际代码示例，说明了大模型的基本原理及其作为HTTP API的作用，以及函数调用在LLM操作中的关键机制。具体示例展示了如何定义天气查询函数，强调了该框架的创新应用。

### 给旧版 .NET 也开一扇“私有之门”——ILAccess.Fody 实现原理与设计

https://www.cnblogs.com/huoshan12345/p/19179723

文章讨论了如何在旧版 .NET 中实现 UnsafeAccessor 特性，通过 ILAccess.Fody 来允许访问私有字段、方法和构造函数。ILAccess.Fody 利用 Fody 和 Mono.Cecil 在编译期对 IL 进行修改，提供了几乎与 UnsafeAccessor 一致的体验。作者展示了使用 ILAccess.Fody 的具体实例，并说明了其性能优势。文章深入探讨了核心实现原理，通过编译期注入 IL 来直接访问私有成员，避免了反射和委托的开销，提升了性能。

### C#/.NET/.NET Core技术前沿周刊 | 第 59 期(2025年10.20-10.26)

https://www.cnblogs.com/Can-daydayup/p/19170328

本文章汇集了C#/.NET/.NET Core的最新技术动态和资源，旨在提升开发者的技术水平和视野。它涵盖了对象映射、微服务框架、反编译工具、图表解决方案、RABC权限管理系统、性能优化等实际应用。每篇文章均提供了具体的实现方法和技巧，帮助开发者高效解决实际问题。同时，文章鼓励社区成员进行投稿，以增强内容的丰富性和多样性。

### 一行代码快速开发 AntdUI 风格的 WinForm 通用后台框架

https://www.cnblogs.com/1312mn/p/19011005

这篇文章介绍了一款基于 Ant Design 设计语言的 WinForm UI 框架，旨在提升开发效率。它允许开发者专注于核心业务逻辑，简化了基础设施代码。文章详细列出了项目的功能，包括 AOT 编译、字典管理、用户管理、菜单管理和权限管理等。还说明了如何初始化数据库、启动应用和集成各项功能。通过使用简洁的代码和注入方式，框架提供了强大的扩展性和安全性，便于用户自定义和配置。对于开发企业级桌面应用有重要指导意义。

### Azure MCP Server 1.0 正式发布

https://www.cnblogs.com/shanyou/p/19184023

Microsoft 发布了 Azure MCP Server 1.0.0 的稳定版本。该协议连接 AI Agent 与 Azure 服务，支持 47 种服务的无缝集成。开发人员可利用该框架查询数据、管理存储及自动部署，保持高性能和安全性。这一版本提供 Docker 映像支持，允许在 CI/CD 管道中轻松集成。系统经过结构化设计，提升了开发体验，并实现了灵活的作模式，增强了安全性。其架构旨在实现模块化与可扩展性，代码开源，鼓励开发者反馈和合作以拓展代理工作流框架。

### 一个开源免费、轻量级的 Avalonia UI 控件库

https://www.cnblogs.com/Can-daydayup/p/19175318

本文介绍了Aura.UI，一个基于Avalonia的开源、轻量级UI控件库，适用于.NET跨平台开发。Avalonia框架支持多种平台，开发者可以共享UI代码。文章详细列出了库中的控件，如浮动按钮栏、现代滑块等，并提供了NuGet包的安装说明。通过设置Fluent主题，用户可以自定义应用样式。此外，文章鼓励读者关注C#/.NET领域的最新动态，链接提供了项目源码和推荐的优秀项目。总体来说，内容清晰，实用性强，具备一定的技术深度和原创新意。

### 【RabbitMQ】与ASP.NET Core集成

https://www.cnblogs.com/jixingsuiyuan/p/19167628

本章介绍如何在ASP.NET Core中配置RabbitMQ服务，使用IHostedService实现长时间运行的消费者服务，构建微服务间的异步通信解决方案。理论部分强调依赖注入、生命周期管理和异步消息模式。实操部分则详细描述了创建订单处理微服务的步骤，包括项目结构、API设计和健康检查。内容清晰、实用，适合开发者理解和实现RabbitMQ与ASP.NET Core的集成。

### LVGLSharp：LVGL的C#绑定库介绍

https://www.cnblogs.com/shanyou/p/19185046

LVGL是一个流行的开源图形库，特别适合资源受限的嵌入式系统。LVGLSharp是其C#绑定库，帮助.NET开发者轻松利用LVGL的功能，创建美观有效的图形界面。项目托管在GitHub上，遵循MIT许可证。它支持全面的API互操作，能够在Windows和Linux等多个平台上运行，并且易于集成。文档齐全，提供多种示例，加速开发者上手。LVGLSharp特别适用于智能家居、工业自动化和医疗设备等场景，提供了高效的图形界面开发能力。对.NET开发者来说，LVGLSharp是一个理想的选择，值得尝试。

### 《手搓》线程池优化的追求

https://www.cnblogs.com/xiangji/p/19170910

该文章讨论了一个基于C# .NET的线程池实现。作者回顾了线程池的并发性能，展示了使用ConcurrencyLevel设置为10时的任务执行结果。代码示例中，使用了ConcurrentTaskScheduler来调度任务，展示了如何同时运行多个乘法计算。每个任务的结果和执行时间都有详细记录。这一实现展示了如何高效管理并发任务，提供了可参考的代码和结果。在技术方面，文章具备深度，清晰阐述了实现步骤与结果。

### Serilog 日志库简单实践(一)：文件系统 Sinks(.net8)

https://www.cnblogs.com/hnzhengfy/p/19167604/SerilogSink_FileSystem

本文介绍了 Serilog 及其文件日志组件的用法，重点讲解了如何在 .NET 8 Web API 项目中集成 Serilog。通过对 Serilog.Sinks.File 的详细阐述，说明了该组件的核心功能，包括日志格式、文件滚动策略及多进程共享等。此外，示例中展示了如何进行 NuGet 包安装，并通过 appsettings.json 配置日志记录的级别，提升只关注重要信息的能力。修改 Program.cs 文件部分也进行了说明，提供了整体配置的清晰指导。

### ASP.NET Core Blazor 核心功能一：Blazor依赖注入与状态管理指南

https://www.cnblogs.com/shenchuanchao/p/19173327

本文详细介绍了Blazor框架的依赖注入和状态管理机制。依赖注入部分讨论了服务的三种生命周期(Singleton, Scoped, Transient)及其在组件中的应用。状态管理章节梳理了七种方案，包括组件内状态、父子组件通信、全局状态容器等，并提供了本地存储持久化方案。最后，文章推荐了不同场景下的状态管理解决方案，帮助开发者构建健壮的应用。整体内容清晰且具有实用性，适合开发者学习和应用。

### 【EF Core】“多对多”关系与跳跃导航

https://www.cnblogs.com/tcjiaan/p/19184567

本文讨论了多对多关系在数据库中的实现，介绍了使用辅助表连接学生和课程的方式。通过示例阐述了两个实体类的定义，以及如何通过 EF Core 自动识别多对多关系。解释了跳跃导航的概念，并强调了属性在多对多关系中的作用。整体内容清晰易懂，便于理解多对多关系的构建。这对于数据库设计具有实际指导意义。

### React学习(一)：使用react-router构建导航应用

https://www.cnblogs.com/mingupupu/p/19183327

这篇文章讨论了C#和React的学习体验，强调了AI在学习过程中的辅助作用。作者表示自己在C#的舒适区内，学习新技术时通过官方文档与AI工具结合的方法。React作为构建用户界面的库，以声明式和组件化特征为核心，提供了良好的开发体验。文中还介绍了Vite构建工具及其优势，以及如何使用React Router进行多策略路由。最后，作者提到在AI时代，技术学习需保持自我理解，避免依赖AI结果而失去个人能力的感觉。

### 【VSCode】VS Code 中使用 Cline AI

https://www.cnblogs.com/WilsonPan/p/19171026

本文介绍了如何在 VS Code 中使用 Cline AI，这是一款基于 Claude 模型的智能编程助手。文章详细阐述了安装步骤、API 密钥配置以及核心功能，包括代码生成、审查、调试、文档生成和测试用例编写。用户需在VS Code中搜索并安装 Cline AI 扩展，然后根据需要配置相关参数。文中还提供了使用示例，帮助用户理解如何高效利用 Cline AI 进行编程。总体结构清晰，适合开发者学习。

### 【译】在 Visual Studio 中引入计划功能(公开预览版)

https://www.cnblogs.com/MeteorSeed/p/19168908

该文章介绍了Visual Studio 2022中Copilot的新计划功能。计划功能使Copilot能够在大型项目中制定和执行任务，提供更可预测的工作流程。通过结构化的方式，该功能能有效管理多步骤任务，并实时跟踪进度。测试显示，该功能显著提高了工作完成的可靠性和效果。文章强调正在收集用户反馈，以便进一步改进计划系统，提升其在开发过程中的有效性。这是一项仍在预览阶段的新功能，未来将发展为更智能的协作伙伴。

### 【RabbitMQ】RPC模式(请求/回复)

https://www.cnblogs.com/jixingsuiyuan/p/19181480

本章讨论RabbitMQ的RPC模式，说明其核心组件和工作流程。RPC允许客户端异步调用远程服务，具有请求和回复队列及关联ID。文章介绍了RPC的应用场景，包括微服务通信和计算密集型任务的分布式处理。实操部分展示了如何利用.NET框架创建分布式计算服务，详细描述了项目结构和关键代码。内容详细清晰，适用于对RabbitMQ和微服务架构感兴趣的开发者。

## 主题
### 为 2025 年 .NET 会议做好准备！ - .NET 博客
https://devblogs.microsoft.com/dotnet/get-ready-for-dotnet-conf-2025/

.NET Conf 2025 将于 11 月 11 日开始的公告。

文章介绍了三天内将分发的内容的亮点。 第一天是 .NET 10 发布，第二天是 Azure、云和深入探讨，第三天是社区日。

- [议程 - .NET Conf 2025](https://www.dotnetconf.net/agenda)
- [加入我们的 .NET Conf：深入了解 Visual Studio 2026 开发的未来 - Visual Studio 博客](https://devblogs.microsoft.com/visualstudio/join-us-at-net-conf-dive-into-the-future-of-development-with-visual-studio-2026/)

### Copilot Studio 如何使用 .NET 和 WebAssembly 实现性能和创新 - .NET 博客
https://devblogs.microsoft.com/dotnet/copilot-studio-dotnet-wasm/

了解 Microsoft Copilot Studio 如何利用 .NET 和 WebAssembly。

Copilot Studio 通过在 WebAssembly 中运行 .NET 中实现的 PowerFx(一种低代码语言，如 Excel 的公式语言)来实现浏览器上的作。 这确保了客户端和服务器的行为一致。

本文讨论了混合解释器和 AOT 方法和 。 NET 8 还讨论了提高性能和减小生成大小等方面。

### ReSharper、.NET Tools 和 ReSharper C++ 2025.3 候选版本现已推出 | .NET Tools 博客
https://blog.jetbrains.com/dotnet/2025/11/05/the-resharper-dotnet-tools-2025-3-release-candidate/

适用于 ReSharper、.NET Tools 和 ReSharper C++ 的 2025.3 RC 已经发布。

此版本包括支持 C# 14 的更新、各种性能改进、进程外稳定性改进以及 TeamCity 扩展的重新打包。

### Visual Studio 中的 AI 路线图(11 月) - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/roadmap-for-ai-in-visual-studio-november/

Visual Studio 的 2025 年 11 月 AI 功能路线图。

- 新代理
    - 用户创建的自定义代理
    - 测试剂
    - 调试器代理
    - 并行执行多个代理
- 代理模式/聊天
    - 斜杠命令 - 运行提示并管理聊天
    - 改进的聊天记忆
    - 改进的工具调用
        - 聊天中的动态工具调用
        - 总结线程历史并继续线程
        - 规划
        - 聊天中的只读计划
        - 聊天中规划和内联预览的用户体验改进
- 模型上下文协议 (MCP)
    - MCP 采样窗口用户体验改进
    - 优化 MCP 服务器性能和令牌使用
    - 在 Visual Studio 中启用 MCP 服务器治理
    - MCP 集成用户体验型
    - 聊天中的自动化模型
    - 聊天中的 GPT 5 Codex
    - 已弃用模型的模型用户体验改进
    - 每个模型都有不同的系统提示

### Visual Studio 10 月更新 – 新模型、内存、规划等 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-october-update/

Visual Studio 的 2025 年 10 月更新摘要。

- 新Model
- 指令文件
- 使用 Azure Foundry 自带模型

### 💫 欢迎来到 Aspire：您的堆栈，简化 | Aspire 博客
https://devblogs.microsoft.com/aspire/aspirepolyglot/

.NET Aspire 现在更名为 Aspire，该公告将成为代码优先的多语言开发和部署工具。

- [Aspire——您的堆栈，简化](https://aspire.dev/)

## 发布
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [3.7.1155.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1155.0)， [3.7.1156.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1156.0)， [3.7.1157. 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1157.0) [3.7.1158.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1158.0)、 [3.7.1159.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1159.0)、 [4.0.123.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.123.0)、 [4.0.124.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.124.0)、 [4.0.125.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.125.0)、 [4.0.126.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.126.0)、 [4.0.127.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.127.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.AI.Projects_1.1.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.AI.Projects_1.1.0)， [Azure.ResourceManager.DurableTask_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DurableTask_1.0.0)， [Azure.ResourceManager.MySql_1.2. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.MySql_1.2.0)、[Microsoft.Azure.WebJobs.Extensions.Storage_5.3。 7](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebJobs.Extensions.Storage_5.3.7)， [System.ClientModel_1.8. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/System.ClientModel_1.8.0)
- [社区工具包/Aspire](https://github.com/CommunityToolkit/Aspire)
    - [v9.9.0](https://github.com/CommunityToolkit/Aspire/releases/tag/v9.9.0)
- [CommunityToolkit/毛伊岛](https://github.com/CommunityToolkit/Maui)
    - [12.3.0](https://github.com/CommunityToolkit/Maui/releases/tag/12.3.0)、 [4.0.0-相机](https://github.com/CommunityToolkit/Maui/releases/tag/4.0.0-camera)、 [6.1. 3-媒体元素](https://github.com/CommunityToolkit/Maui/releases/tag/6.1.3-mediaelement)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.30.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.30.0)
- [dotnet/diagnostics](https://github.com/dotnet/diagnostics)
    - [v9.0.652701](https://github.com/dotnet/diagnostics/releases/tag/v9.0.652701)
- [FluentValidation/FluentValidation](https://github.com/FluentValidation/FluentValidation)
    - [12.1.0](https://github.com/FluentValidation/FluentValidation/releases/tag/12.1.0)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.Bigtable.Common.V2-3.3.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Bigtable.Common.V2-3.3.0)， [ Google.Cloud.DevTools.Common-3.3.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.DevTools.Common-3.3.0)， [Google.Cloud.Iam.V1-3.5. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Iam.V1-3.5.0)， [Google.Cloud.Location-2.4. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Location-2.4.0)、[Google.Cloud.Logging.Type-4.3。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Logging.Type-4.3.0)、[Google.Cloud.OsLogin.Common-3.4。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.OsLogin.Common-3.4.0) [Google.Cloud.Workflows.Common.V1-2.5.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Workflows.Common.V1-2.5.0)、[Google.Geo.Type-1.3. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Geo.Type-1.3.0)， [Google.LongRunning-3.5.0]( https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.LongRunning-3.5.0)
- [微软/CsWin32](https://github.com/microsoft/CsWin32)
    - [v0.3.236](https://github.com/microsoft/CsWin32/releases/tag/v0.3.236)， [v0.3.238](https://github.com/microsoft/CsWin32/releases/tag/v0.3.238)， [v0.3. 242](https://github.com/microsoft/CsWin32/releases/tag/v0.3.242)

## 文章、幻灯片等
### 有 6 种类型的 C# 列表。
https://qiita.com/sebayashi-tomoya/items/74b43a66ee36572fcdb6

“<T>List”实现的接口的说明。

### [C#] 在 Blazor.Auth 中简单实现身份验证授权
https://zenn.dev/arika/articles/20251103-use-blazor-auth

了解 Blazor.Auth，这是一个用于在 Blazor 中实现简单身份验证的库，以及如何使用它。

### [C#] 如何在 Blazor 中实现强制重定向
https://zenn.dev/arika/articles/20251104-blazor-force-redirect

如何在 Blazor 中查看页面时强制重定向。

### 驯服十亿美元的错误：Maarten Balliauw 的 C# 可空引用类型指南 | .NET Tools 博客
https://blog.jetbrains.com/dotnet/2025/11/04/maarten-balliauws-guide-to-csharp-nullable-reference-types/

有关迁移现有代码以利用可为 null 的引用类型的会话视频。

### [C#] 从 CI 检查代码指标
https://qiita.com/KM_20005/items/61936376184920f70401

如何使用 CI 构建时检查/警告代码指标。

### 在 .NET 10 中使用 [UnsafeAccessorType] 更轻松地进行反射
https://andrewlock.net/exploring-dotnet-10-preview-features-9-easier-reflection-with-unsafeaccessortype/

一篇关于允许访问 .NET 10 中引入的私有类型的“UnsafeAccessorType”属性的文章。

它还涉及 .NET 8/9 中的“UnsafeAccessor”属性。

### [C#] 如何处理遗留系统中的注册表依赖项 - 迁移、兼容性、权限和实现的完整总结
https://qiita.com/Sakai_path/items/3c379094ca478223c56f

旧系统经常依赖的注册表的摘要，包括如何考虑迁移目标并实施它们。

### [EF Core] 如何注册 DbContext 以及如何使用它
https://qiita.com/yariri/items/95693f040d8a90c817cb

从 DI 容器获取“DbContext”的多种方法的摘要。 本文介绍了“AddDbContext”、“AddDbContextFactory”和“AddPooledDbContextFactory”之间的区别以及如何使用它们。

###  .NET Tools 博客
https://blog.jetbrains.com/dotnet/2025/11/05/dotinsights-november-2025/

JetBrains 2025 年 11 月关于 .NET 的综述信息。

### 总结 .NET 10 中的新增功能 (C# 14)
https://zenn.dev/gkuroki/articles/dotnet10-feature

有关 .NET 10 和 C# 14 中新增功能的综述文章。

### 参考来源/wpf/src.zip 在主要 · 微软/参考源
https://github.com/microsoft/referencesource/blob/main/wpf/src.zip

适用于 .NET Framework 的 WPF 源代码已以 ZIP 格式发布。

## 库、存储库、工具等
### manpukupanda/edinet-xbrl-parser： EDINET XBRL 解析器
https://github.com/manpukupanda/edinet-xbrl-parser

EDINET提供的用于使用XBRL的库。

- [诗意地阅读 EDINET 的 XBRL：对 Manpuku.Edinet.Xbrl 的设计与反思](https://qiita.com/manpukupanda/items/153f0fc1bcbbc90228e2)

## 库、存储库、工具等
### manpukupanda/edinet-xbrl-parser： EDINET XBRL 解析器
https://github.com/manpukupanda/edinet-xbrl-parser

EDINET提供的用于使用XBRL的库。

- [诗意地阅读 EDINET 的 XBRL：对 Manpuku.Edinet.Xbrl 的设计与反思] (https://qiita.com/manpukupanda/items/153f0fc1bcbbc90228e2)

## 今日人物

**艾伦·纽厄尔**(英语：Allen Newell，1927年3月19日—1992年7月19日)是[计算机科学](https://zh.wikipedia.org/wiki/计算机科学)和[认知信息学](https://zh.wikipedia.org/w/index.php?title=认知信息学&action=edit&redlink=1)领域的科学家，曾在[兰德公司](https://zh.wikipedia.org/wiki/兰德公司)，[卡内基梅隆大学](https://zh.wikipedia.org/wiki/卡内基梅隆大学)的计算机学院、[泰珀商学院](https://zh.wikipedia.org/w/index.php?title=泰珀商学院&action=edit&redlink=1)和[心理学](https://zh.wikipedia.org/wiki/心理学)系任职和教研。他是[信息处理语言](https://zh.wikipedia.org/wiki/信息处理语言)(IPL)发明者之一，并写了该语言最早的两个[AI](https://zh.wikipedia.org/wiki/人工智能)程序，合作开发了[逻辑理论家](https://zh.wikipedia.org/wiki/逻辑理论家)(Logic Theorist 1956年)和[一般问题解决器](https://zh.wikipedia.org/wiki/一般问题解决器)General Problem Solver。1975年他和[赫伯特·西蒙](https://zh.wikipedia.org/wiki/赫伯特·西蒙)(司马贺)一起因人工智能方面的基础贡献而被授予[图灵奖](https://zh.wikipedia.org/wiki/图灵奖)。

![艾伦·纽厄尔](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/bZHt5OC3_rVRr8KK_cZXv_1536x1024_20251109_014708_raw.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

* 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
* .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
* 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。