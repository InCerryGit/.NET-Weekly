**C# .NET 周刊｜2026年6月2期 2026-06-14 dotnet_week_26_6_2**

## 国内文章
### C#实现控制台多区域输出

https://www.cnblogs.com/wucy/p/20292775/csharp-multi-region

文章介绍如何用原生 C# Console 实现多区域动态终端界面。作者指出 Console.SetCursorPosition 是核心，视控制台为字符画布。示例将窗口分为系统时间、任务进度和滚动日志三部分，并给出绘制边框和布局代码。文中实现实时刷新、滚动日志、多线程安全输出和优雅退出。实现不依赖第三方组件，适合构建简单 Agent CLI 可视化。文章实用且示例明确，但缺少引用与更深入的性能或异常处理讨论。

### 由罗技 K380 键盘 FN 键模式切换引发的血案

https://www.cnblogs.com/liuxw/p/20419710

作者介绍用 .NET 控制台程序向罗技 K380 蓝牙键盘发送 HID 指令以切换 Fn 模式，并记录了实际踩坑过程。文章列出官方 Feature Report 的字节序列，尝试过 HidSharp 2.6.4(缺少 SetReport)、WinRT HID API(需复杂配置且兼容性问题)和直接 P/Invoke HidD_SetFeature(蓝牙 HID 不受支持)等方案并失败。作者目标是实现轻量化的一行命令切换工具。文章实践性强，技术细节清晰，但未给出最终可行方案并缺少外部引用和完整代码示例。

### C#从零开始：自己实现一个截屏工具

https://www.cnblogs.com/luojin765/p/20385046

文章介绍基于 .NET 10、Avalonia 12、Skia 与 Win32 PInvoke 的截屏工具架构。作者选 Avalonia 因支持 Native AOT、跨平台与现代绑定，可生成单文件可执行并保证低冷启动。抓屏采用 Win32 GDI BitBlt 以最大兼容性，放弃 DXGI 与 WGC 的复杂依赖。工程分四层：Core(抓取接口与平台实现、注释数据模型)、UI(Avalonia 控件与服务)、LumScreenShot(最小启动 exe)、Test(Headless 单元测试)。Core 避免反射与 System.Drawing，XAML 启用编译生成以优化体积与启动。文章论证清晰，示例代码截断但技术选择合理且实用。

### CSharp 后端服务器如何做到：一边发请求一边看代码覆盖率

https://www.cnblogs.com/ahfuzhang/p/20474477

作者介绍了一种按请求实时采集 .NET 应用代码覆盖率的方法。作者构建了包含多版本 .NET SDK、dotnet-coverage 和 reportgenerator 的 all-in-one 调试镜像并提供镜像链接。流程用 dotnet-coverage collect 启动并生成 session id，使用 dotnet-coverage snapshot 导出覆盖数据，使用 merge 转为 Cobertura XML，再用 reportgenerator 生成 HTML 报告。文中给出 CodeCoverageCallbackAsync 示例，展示如何通过请求中的 session-id 触发快照并生成报告文件。该方案无需改动业务代码，便于在测试或调试时覆盖多分支。

### [MAF预定义ChatClient中间件-07]PerServiceCallChatHistoryPersistingChatClient——基于ReAct循环的一步一存档

https://www.cnblogs.com/artech/p/20436414/chat-client-pipeline-07

文章指出默认情形下ChatHistoryProvider在一次调用结束后才存档消息，导致ReAct多轮循环中若最终存盘失败会丢失所有中间消息。作者建议通过注册PerServiceCallChatHistoryPersistingChatClient中间件，实现每次迭代即时持久化。文章分析了ChatClientAgent管道中FunctionInvokingChatClient与ChatHistoryProvider的上下游关系，说明该结构如何决定加载与保存时机。文中给出ChatHistoryProviderWrapper示例，重写InvokingCoreAsync和InvokedCoreAsync并打印日志，用以验证每次加载和保存的消息列表。

### [MAF预定义ChatClient中间件-04]ReducingChatClient——精减对话历史又不丢失基本语义

https://www.cnblogs.com/artech/p/20365576/chat-client-pipeline-04

文章指出对话历史常占用LLM上下文窗口，过多上下文会干扰推理。ReducingChatClient为中间件，靠对话摘要精简历史以保留语义并腾出窗口空间。示例用C#基于OpenAIClient构建IChatClient，使用ChatClientBuilder注册ReducingChatClient，并传入SummarizingChatReducer作为摘要器。摘要器用另一个基于相同模型的chatClient生成摘要，并通过targetCount和threshold控制保留消息数与触发阈值。示例还展示了中间件打印请求消息数的用法。总体聚焦于提高Agent决策可靠性与上下文管理。

### 使用 dotnet-counters 观测升讯威客服系统内存占用情况和数据吞吐性能

https://www.cnblogs.com/sheng_chao/p/20407746

文章介绍了使用 dotnet-counters 在不停机情况下对已部署的 .NET 应用进行实时性能采集与离线导出。作者展示了通过 dotnet-counters ps 和 monitor 命令挂载进程或按名监控，并说明了可选 providers(如 System.Runtime 与 Microsoft.AspNetCore.Hosting)以获取 CPU、GC、线程池和每秒请求等指标。文中用真实的升讯威客服系统数据示例，结合 AI 解读，指出 Working Set 明显大于托管堆且 Gen2 占比高，提示长期驻留对象或非托管内存占用。文章实用且表述清晰，但原创性与参考引文不足。它适合现场快速健康检查与生产诊断。

### 精选 5 款基于 .NET 开源免费、功能强大的 Windows 系统优化工具

https://www.cnblogs.com/Can-daydayup/p/20408715

本文介绍五款基于 .NET 的开源 Windows 优化工具：Optimizer 提供服务管理、垃圾清理、硬件检测与网络工具；SophiApp 提供130+项微调选项以平衡性能与稳定性；WinMemoryCleaner 调用系统接口回收泄露内存；ZyperWin++ 覆盖性能、服务、隐私、更新及 Office 激活等优化；Winhance 以图形化整合应用管理、定制安装与配置导入导出。文章列出各项目 GitHub 地址并纳入 C#/.NET 优秀项目精选，鼓励提交 PR 推荐项目。该汇总便于 .NET 开发者快速获取实用开源工具和参考。

### EF Core 8 + SQL Server：Contains() 突然报 "关键字 WITH 附近有语法错误"？一篇避坑指南

https://www.cnblogs.com/shenchuanchao/p/20368616/ef-core-8-sql-server-contains-with-syntax-error-guide

作者说明在升级到 .NET 8 / EF Core 8 后，常见的 ids.Contains 导致 SQL 报错“WITH 附近有语法错误”。根因是 EF Core 8 将常量列表改为通过 OPENJSON/CTE 传参，生成以 WITH 开头的查询但未补分号引发 SQL Server 错误。文章列举高风险触发场景并给出五种修复方案，推荐优先用参数化 Raw SQL 绕过翻译。作者并引用了微软 EF Core 8 的 Breaking Changes 文档，提供实用可行的解决路径。

### [MAF预定义ChatClient中间件-05]动态修改ChatOptions和请求消息

https://www.cnblogs.com/artech/p/20388547/chat-client-pipeline-05

文章介绍如何用 ConfigureOptionsChatClient 在每次调用中动态设置 ChatOptions，从而在 IChatClient 调用间切换模型。它解释了 ChatClientAgentOptions 的绑定作用，并提到 AIContextProviderChatClient 可以为每次调用生成 AIContext 以提供请求消息和系统指令。示例用 C# 展示了基于 OpenAIClient 的中间件配置，并交替使用 gpt-5.2-chat 与 DeepSeek-V4-Pro 生成响应。代码清晰且实用。文章缺少并发、安全、错误处理和引用等深入讨论。

### C# 实现优雅的热重载：基于 PicoServer 的 Live Reload 方案

https://www.cnblogs.com/juziyu/p/20394417

.NET 10 支持开源跨平台开发。本文用不到50行代码基于 PicoServer 实现零配置热重载服务器。服务器用 FileSystemWatcher 监控 wwwroot，使用200毫秒的 Timer 防抖以合并多重文件事件。检测到变更后通过 WebSocket 广播 reload 消息。返回 HTML 时自动注入客户端脚本，脚本连接 /ws-reload 并在收到消息后刷新页面。文章提供依赖和示例代码，实用且实现简洁，但缺少安全、错误处理与性能评估。

### Zenith.NET 开发札记：把 .NET 图形 API 推向现代 RHI

https://www.cnblogs.com/xymfblogs/p/20508874

Zenith.NET 进行了大规模 RHI 重构，将封装层改为贴近 DirectX12/Vulkan/Metal 的低层模型。新版引入 bindless、显式屏障、布局转换、多队列和 shader-visible descriptor heap。作者启用 Slang 跨后端编译至 DXIL、metallib 和 SPIR-V。核心新增 TextureLayout、BarrierStages、ResourceHandle 等概念。目标是支持 ray tracing、mesh shading、GPU-driven rendering 及引擎集成。文章对比了旧版按表绑定的写法，强调现代 API 让应用显式控制资源可见性、转换和同步，从而提高上限和性能潜力。

### [MAF预定义ChatClient中间件-06]利用ImageGeneratingChatClient开发专业图片生成Agent

https://www.cnblogs.com/artech/p/20410861/chat-client-pipeline-06

文章介绍将LLM与图片生成模型结合的中间件ImageGeneratingChatClient。用户通过与Agent对话描述图片，LLM生成专业提示词。注册的ImageGenerator接收提示词，调用图片生成API并返回结果。示例展示了C#实现的ImageGenerator类，构造函数接收endpoint、apiKey和model。GenerateAsync使用HttpClient发送包含prompt和model的JSON请求，解析响应并转换为Data URI。出现异常时返回ErrorContent。文章强调实现流程和异常处理，便于快速实现图片生成Agent。

### .NET Core自定义 ALC 中启动WebHost的HostingStartup解析异常

https://www.cnblogs.com/CreateMyself/p/20520236

文章描述在 .NET Core 插件系统中，插件程序集通过自定义 AssemblyLoadContext 加载。插件自托管 Web 服务时，Host.CreateDefaultBuilder 触发 ASP.NET Core 的 HostingStartup 机制。GenericWebHostBuilder.ExecuteHostingStartups 使用 Assembly.Load 按名称加载带有 HostingStartup 特性的程序集。Assembly.Load 仅在 Default ALC 查找，忽略自定义 ALC，因而出现致命级别的加载异常但应用仍能运行。文章解释了 HostingStartup 的用途、程序集发现与加载流程，并定位了冲突根因。文章技术深度与实用性较高，但缺少解决方案和参考引用。

### OpenVINO™ C# API 3.3 全新发布！正式接入 OpenVINO GenAI，C# 本地大模型开发全面启航！

https://www.cnblogs.com/guojin-blogs/p/20437610

本文介绍 OpenVINO C# API 3.3 的核心升级。3.3 正式接入 OpenVINO GenAI，新增 OpenVinoSharp.GenAI 命名空间，支持本地调用 LLM、Whisper 和 VLM。GenAI runtime 提供 NuGet 包，简化 native DLL 的部署。传统推理接口保持兼容，旧项目无需强制迁移。文章提供适用读者分类、升级理由、示例入口和后续教程安排。内容实用且时效性强，但缺乏引用与深度实现细节。

### [MAF预定义ChatClient中间件-08]OpenTelemetryChatClient-实现链路跟踪和性能监控

https://www.cnblogs.com/artech/p/20464876/chat-client-pipeline-08

文章介绍使用OpenTelemetry为LLM调用增加可观测性。OpenTelemetryChatClient通过重写GetResponseAsync和GetResponseStreamAsync记录链路与性能指标。文中演示在本地用Docker部署Jaeger、Prometheus和Grafana，并给出docker命令与prometheus.yml示例。示例还展示了一个Console应用，引用OpenTelemetry相关NuGet包，分别创建TracerProvider和MeterProvider，设置服务名与版本，并通过OTLP将Trace发送到Jaeger，通过PrometheusHttpListener暴露Metrics供Prometheus抓取。文档便于复现，但部分内容截断且存在小错别字。

### 基于AScript的SQL脚本语言发布啦！

https://www.cnblogs.com/rockey627/p/20385305

AScript 是开源的 C# 动态脚本引擎，2026-06-08 发布了 SQL 脚本语言 AScript.Lang.Sql。它支持 SqlServer/MySql 基础语法与常用数据类型，支持 SELECT(含 FROM/WHERE/多种 JOIN/GROUP BY/ORDER BY/LIMIT)、INSERT、UPDATE、DELETE、创建存储过程与表、定义变量，并能调用外部方法与变量。当前不支持存储过程 OUT 参数、SELECT 使用 * 和聚合函数。通过 NuGet 安装并在 Script 上注册语言后，可以在 C# 环境对内存集合执行 SQL 风格查询。示例展示了返回匿名类型和单字段查询的用法。

### 用 39 元跑出 1.3B token 的代码知识库：OpenDeepWiki 最新 wiki 质量抽检

https://www.cnblogs.com/token-ai/p/20392986

本文抽检 OpenDeepWiki 与 AIDotNet/Means 的生成结果。样本配置为目录用 gpt-5.5，正文用 Mimo-2.5，累计消费约1.3B token，成本约39元。OpenDeepWiki 可把项目拆成约22个主题页，覆盖数据面、存储层、管理面、SDK、部署和测试，并在页面保留已读源码列表，适合作为新项目的第一版知识库。它支持从 Git/ZIP/本地导入，产出结构化 wiki、多语言内容和聊天/嵌入 API。后端基于 ASP.NET Core/.NET 10，前端 Next.js 16 + React 19，使用 Microsoft.Agents.AI 与 LibGit2Sharp。生成链路把目录模型与内容模型分离，使用 GitTool、DocTool 和 TokenUsage 跟踪来源与成本。样本显示生成存在快照滞后或过度信任计划文档的风险，需自动校验或人工抽检。

### 从零开始：如何将 Reasonix CLI 集成到 HagiCode 系统中

https://www.cnblogs.com/newbe36524/p/20393164

文章介绍将 Reasonix CLI 作为一等 Agent Provider 集成到 HagiCode 的完整实践。采用三层架构。HagiCode.Libs 提供 ICliProvider<ReasonixOptions> 与 ReasonixProvider，处理 ACP 流式与会话及 effort、budget、yolo 等参数。hagicode-core 注册 AIProviderType.ReasonixCli，提供 ReasonixCliProvider 适配器并实现 ReasonixGrain 管理会话与执行流，集成 Hero 做参数映射。web 层更新 OpenAPI、视觉类型、CLI 参数表单与多语言支持。关键决策包括使用专用 Grain、优雅降级与 thin adapter 模式。方案可复用且实用。缺少引用与示例代码降低可验证性。

### 将 Pi Agent 接入 HagiCode 的实践之路

https://www.cnblogs.com/newbe36524/p/20384918

本文介绍在 HagiCode 项目中将 Pi agent 作为一等 Agent CLI 的接入实践。作者采用 thin adapter 模式，复用 HagiCode.Libs 中已实现的 PiProvider，避免在 core 层重复实现进程协议。文章展示了新增 AIProviderType 枚举并在 AIProviderFactory 注册 PiCli 分支，以及 PiCliProvider 的关键实现思路。方案强调避免重复实现、保持与现有 CLI 接入方式一致并实现关注点分离，从而简化维护并加速新提供商集成。

### Jasmine.Format - 一个高性能、线程安全的 .NET HTML 生成库

https://www.cnblogs.com/dingshuanglei/p/20512856

文章介绍了面向高性能场景的 .NET HTML 生成库 Jasmine.Format。库提供自动 HTML 编码以防 XSS，链式 API，基于不可变对象的线程安全设计，以及对象池、线程本地 StringBuilder 缓存和容量预估等性能优化。示例展示了包安装和基本用法，支持 .NET Standard 2.0 及 .NET 6–10。文章实用性和可读性强，技术细节适中，但缺少引用和对比评估，原创性一般。总体适合寻找轻量、安全、高性能 HTML 构建方案的 .NET 开发者。

### 【EF Core】继承策略——TPC

https://www.cnblogs.com/tcjiaan/p/20499508

文中说明在 EF Core Code First 小项目中，同时支持 SQLite 和 SQL Server 时为实体配置 CHECK 约束的方法。示例定义 Person 实体和 TestContext，上下文 OnModelCreating 中用 Database.IsSqlite() 和 IsSqlServer() 判断数据库类型，分别设置标识符边界(SQLite 用双引号，SQL Server 用方括号)，拼接列名并通过 HasCheckConstraint 添加约束。上下文通过构造函数接收 DbContextOptions，并可用 UseSqlServer/UseSqlite 切换数据库。该方法可行但属于硬编码，实现简单但缺乏更通用的 EF Core 适配方案。


---

## 国际周报

## 话题

### .NET 11 预览版5现已上线！ - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-11-preview-5/

### .NET 和 .NET Framework 2026 年 6 月服务发布更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-and-dotnet-framework-june-2026-servicing-updates/

### .NET 在 Microsoft Build 2026：必看的会议 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-at-microsoft-build-2026/

- [Azure 更新 (2026-06-03) Microsoft 2026 Build Day 1 | Buchizakki](https://blog.azure.moe/2026/06/03/azure-updates-2026-06-03-microsoft-build-2026-day-1/)
- [Microsoft Build 2026 第一天主题演讲](https://blog.azure.moe/2026/06/03/microsoft-build-2026-day-1-keynote/)
- [Build 2026：进一步提升Windows作为可信开发平台的地位](https://blogs.windows.com/windowsdeveloper/2026/06/02/build-2026-furthering-windows-as-the-trusted-platform-for-development/)

### 加入我们的.NET日，关注代理现代化直播——.NET博客
https://devblogs.microsoft.com/dotnet/join-us-for-dotnet-day-on-agentic-modernization-livestream/

### WPF 热重载来了：编辑你的 XAML，观看 Rider 中实时更新 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/06/03/wpf-hot-reload-in-jetbrains-rider/

### Rider 2026.2 EAP 5：为你的AI代理进行代码质量检查及更多内容。 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/06/08/rider-2026-2-code-quality-check-hooks-for-ai-agents/

### RESP3 和 StackExchange.Redis
https://stackexchange.github.io/StackExchange.Redis/Resp3

- [3.0.47 版本预览版 · StackExchange/StackExchange.Redis](https://github.com/StackExchange/StackExchange.Redis/releases/tag/3.0.47-preview)

### 弃用点记忆单元 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/05/28/deprecating-dotmemory-unit/

### microsoft/microsoft-ui-reactor：Reactor 是一套 WinUI 的实验性扩展
https://github.com/microsoft/microsoft-ui-reactor

## 发布
- [App-vNext/Polly](https://github.com/App-vNext/Polly)
    - [8.7.0](https://github.com/App-vNext/Polly/releases/tag/8.7.0)
- [AvaloniaUI/Avalonia](https://github.com/AvaloniaUI/Avalonia)
    - [2017年3月11日](https://github.com/AvaloniaUI/Avalonia/releases/tag/11.3.17)、[12.0.4](https://github.com/AvaloniaUI/Avalonia/releases/tag/12.0.4)
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [4.0.256.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.256.0)， [4.0.257.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.257.0)， [4.0.258. 0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.258.0)， [4.0.259.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.259.0)， [4.0.260.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.260.0)， [4.0.262.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.262.0)， [4.0.263.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.263.0)， [4.0.264.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.264.0)， [4.0.265.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.265.0)， [4.0.266.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.266.0)， [4.0.267.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.267.0)
- [Azure/azure-cosmos-dotnet-v3](https://github.com/Azure/azure-cosmos-dotnet-v3)
    - [3.61.0](https://github.com/Azure/azure-cosmos-dotnet-v3/releases/tag/3.61.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.AI.Translation.Text_2.0.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.AI.Translation.Text_2.0.0)，[Azure.Core_1.58。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Core_1.58.0)， [Azure.Core_1.59.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Core_1.59.0)，[Azure.ResourceManager.ApplicationInsights_1.1. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ApplicationInsights_1.1.0)， [Azure.ResourceManager.AppService_1.5. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.AppService_1.5.0)， [Azure.ResourceManager.ArtifactSigning_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ArtifactSigning_1.0.1)， [Azure.ResourceManager.Avs_1.6. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Avs_1.6.1)， [Azure.ResourceManager.Batch_1.7. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Batch_1.7.0)， [Azure.ResourceManager.CertificateRegistration_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.CertificateRegistration_1.0.0)， [Azure.ResourceManager.Compute.Recommender_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Compute.Recommender_1.0.0) [Azure.ResourceManager.ContainerInstance_1.3.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ContainerInstance_1.3.1)，[Azure.ResourceManager.DataBoxEdge_1.1. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataBoxEdge_1.1.2)，[Azure.ResourceManager.Dell.Storage_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Dell.Storage_1.0.1)，[Azure.ResourceManager.ManagedNetworkFabric_1.2。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ManagedNetworkFabric_1.2.0)， [Azure.Security.KeyVault.Certificates_4.9. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Security.KeyVault.Certificates_4.9.0)， [Azure.Storage.Blobs_12.29。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Blobs_12.29.0)，[Azure.Storage.Blobs.Batch_12.26。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Blobs.Batch_12.26.0)，[Azure.Storage.Common_12.28。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Common_12.28.0)，[Azure.Storage.Files.DataLake_12.27。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Files.DataLake_12.27.0)，[Azure.Storage.Files.Shares_12.27。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Files.Shares_12.27.0)， [Azure.Storage.Queues_12.27。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Queues_12.27.0)， [Microsoft.Azure.WebJobs.Extensions.WebPubSub_1.10. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebJobs.Extensions.WebPubSub_1.10.2)，[System.ClientModel_1.14。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/System.ClientModel_1.14.0)
- [CommunityToolkit/Aspire](https://github.com/CommunityToolkit/Aspire)
    - [v13.4.0](https://github.com/CommunityToolkit/Aspire/releases/tag/v13.4.0)
- [CommunityToolkit/Maui](https://github.com/CommunityToolkit/Maui)
    - [10.0.0-mediaelement](https://github.com/CommunityToolkit/Maui/releases/tag/10.0.0-mediaelement)， [14.2.0](https://github.com/CommunityToolkit/Maui/releases/tag/14.2.0)， [6.1.0-camera](https://github.com/CommunityToolkit/Maui/releases/tag/6.1.0-camera)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.45.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.45.0)
- [domaindrivendev/Swashbuckle.AspNetCore](https://github.com/domaindrivendev/Swashbuckle.AspNetCore)
    - [v10.2.0](https://github.com/domaindrivendev/Swashbuckle.AspNetCore/releases/tag/v10.2.0)， [v10.2.1](https://github.com/domaindrivendev/Swashbuckle.AspNetCore/releases/tag/v10.2.1)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.Bigtable.V2-3.28.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Bigtable.V2-3.28.0)，[Google.Cloud.Container.V1-3.39。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Container.V1-3.39.0)， [Google.Cloud.Dataproc.V1-5.26. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Dataproc.V1-5.26.0)， [Google.Cloud.Dlp.V2-4.26. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Dlp.V2-4.26.0)， [Google.Cloud.PubSub.V1-3.35. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.PubSub.V1-3.35.0)， [Google.Cloud.Recommender.V1-3.9. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Recommender.V1-3.9.0)， [Google.Cloud.Security.PrivateCA.V1-3.12. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Security.PrivateCA.V1-3.12.0)， [Google.Cloud.Storage.Control.V2-1.8. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Storage.Control.V2-1.8.0)， [Google.Cloud.Storage.V1-4.15. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Storage.V1-4.15.0)， [Google.Cloud.Workstations.V1-1.5. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Workstations.V1-1.5.0)
- [MessagePack-CSharp/MessagePack-CSharp](https://github.com/MessagePack-CSharp/MessagePack-CSharp)
    - [v2.5.198](https://github.com/MessagePack-CSharp/MessagePack-CSharp/releases/tag/v2.5.198)， [v3.1.7](https://github.com/MessagePack-CSharp/MessagePack-CSharp/releases/tag/v3.1.7)
- [微软/Aspire](https://github.com/microsoft/aspire)
    - [v13.4.0](https://github.com/microsoft/aspire/releases/tag/v13.4.0)、[v13.4.2](https://github.com/microsoft/aspire/releases/tag/v13.4.2)、[v13.4. 3](https://github.com/microsoft/aspire/releases/tag/v13.4.3)
- [microsoft/WindowsAppSDK](https://github.com/microsoft/WindowsAppSDK)
    - [v2.2.2-exp9](https://github.com/microsoft/WindowsAppSDK/releases/tag/v2.2.2-exp9)
- [mysql-net/MySqlConnector](https://github.com/mysql-net/MySqlConnector)
    - [2.6.0](https://github.com/mysql-net/MySqlConnector/releases/tag/2.6.0)
- [newrelic/newrelic-dotnet-agent](https://github.com/newrelic/newrelic-dotnet-agent)    - [v10.51.1](https://github.com/newrelic/newrelic-dotnet-agent/releases/tag/v10.51.1)
- [NPGSQL/NPGSQL](https://github.com/npgsql/npgsql)
    - [v10.0.3](https://github.com/npgsql/npgsql/releases/tag/v10.0.3)
- [开放遥测/开放遥测点网](https://github.com/open-telemetry/opentelemetry-dotnet)
    - [core-1.16.0](https://github.com/open-telemetry/opentelemetry-dotnet/releases/tag/core-1.16.0)
- [spectreconsole/spectre.console](https://github.com/spectreconsole/spectre.console)
    - [0.56.0](https://github.com/spectreconsole/spectre.console/releases/tag/0.56.0)
- [StackExchange/StackExchange.Redis](https://github.com/StackExchange/StackExchange.Redis)
    - [2.3.17](https://github.com/StackExchange/StackExchange.Redis/releases/tag/2.3.17)， [3.0.47-preview](https://github.com/StackExchange/StackExchange.Redis/releases/tag/3.0.47-preview)

## 文物、幻灯片等
### 如何从S&Box开启calc.exe
https://slugcat.systems/post/26-05-21-how-to-open-calc-exe-from-sbox/

### ASP.NET NCronJob 和 SignalR 的核心后台任务
https://damienbod.com/2026/06/08/asp-net-core-background-tasks-with-ncronjob-and-signalr/

### 在 C# 中创建 Windows 服务 [1] 服务注册与日志输出，配置最小 - Qiita
https://qiita.com/Tom-Panasonic/items/fa464c139560c5274002

### 用 OR-Tools 解决 C# 二维打包 CP-SAT——比最优解更快
https://zenn.dev/sitio1/articles/9de31f703af95e

### 关于我不断优化，直到能用自制的二维物理引擎生成一万个物体的故事
https://zenn.dev/rubioa/articles/1eeae24d28ddb6

### [代理黑客松] 创建了一个防变代理，将DNS变更任务转化为带有AI代理的试验
https://zenn.dev/kaiedakensuke/articles/changeproof-agent-hackathon

### [Codex 真实故事] 用 WPF 重建 WinUI 3 中的 Markdown 查看器，结合 Codex
https://zenn.dev/como/articles/article-ko-md-viewer-wpf

### 用OpenTelemetry观察SqlBulkCopy。
https://zenn.dev/xin9le/articles/ef378773820649

### [C#] 构建您自己的面向数据(ECS)游戏引擎基础
https://zenn.dev/rubioa/articles/e69f680f65dcff

### 因为iPhone浏览器的条码扫描器不够准确而开发专用应用的故事(2)——Qiita。
https://qiita.com/onigiripudding/items/0858be71d7e2ba23b87f

### 在AWS Bedrock - Qiita上使用 C# 的 GPT-5.5
https://qiita.com/karuakun/items/a73bd8bcd46d5300d318

### [M5Stack] 尝试用nanoFramework创建Stack Chan(仅面部)#スタックチャン - Qiita
https://qiita.com/ymd65536/items/660eee036dca7ed0a7e9

### 试用基于MCP的Microsoft代理框架(C# v1.8.0)
https://zenn.dev/yy7613/articles/179b546688fd48

### 用C#的异步/等待倒带过程
https://zenn.dev/aakei/articles/async-playback

### 将 ASP.NET 核心认证页面转化为PDF的故事
https://zenn.dev/harness/articles/phycock-playwright-pdf-export

### 从 .NET Framework 迁移到 .NET 的步骤 - Qiita
https://qiita.com/masayasu_t/items/61dea79ba9665aa0a689

### 一键打开持久任务计划仪表盘
https://zenn.dev/microsoft/articles/durable-task-scheduler-aspire-dashboard

### [.NET 11预览] API行为变化(例外类型变更)仍然有显著影响(MemoryStream)
https://zenn.dev/prozolic/articles/c68acd8f201272

### [C#] 二进制搜索工作原理笔记
https://zenn.dev/someone7140/articles/9d60d6a2257b91

### [C#] 什么是ReadOnlySpanT？ 组织了无需复制即可读取内存的机制——Qiita。
https://qiita.com/nakamuuu_ow/items/f56b1e5f3f4fc43f080e

### [C#/Go/PHP] 在指定数组初始大小时，实际测量速度 - Qiita
https://qiita.com/simoyama2323/items/7fe670abb8ccf6b9812a

### 使用 Microsoft Agent Framework A2A 预览测试多代理
https://zenn.dev/yy7613/articles/c118c14f1ce9f6

### . 如果你在NET中分开图层，可能有哪些方法？
https://zenn.dev/toripeeeeee/articles/77a45b092d9d7c

### Cloudflare 页面上的 Blazor WebAssembly - Qiita
https://qiita.com/minerva_jupiter/items/1f2ea3310c8a6e78833a

### 我构建了一个原生的C# Grep引擎，它在ripgrep(零 分配)
https://dev.to/iancowley/i-built-a-native-c-grep-engine-that's-holding-its-own-with-ripgrep-with-zero-allocations-2nf7

### iOS设备启动时.NET MAUI + AdMob崩溃：原因是iOS部署目标号低于15
https://zenn.dev/auctor/articles/zenn-admob-ios-crash

### 如何在 C#/WPF 中创建从屏幕边缘出现的侧边栏
https://zenn.dev/maedan/articles/433ade2bffa748

### WSL 2 的 Windows 文件系统访问速度正在加快
https://www.boxofcables.dev/wsl2-per-device-swiotlb-pools-for-virtiofs-and-virtioproxy/

### 为什么要用Docker ASP.NET 构建多阶段的核心应用？
https://zenn.dev/j_sakamoto/articles/0dc4f4abdd8380

### 尝试用 ASP.NET 核心构建一个简单的MCP服务器
https://zenn.dev/yy7613/articles/0f1ecba8352ad6

### C# 网络深度探访 io_uring 第六部分 - 数字
https://dev.to/mda2av/c-networking-deep-dive-with-iouring-part-6-numbers-49fe

### 【C#】。 .NET 10 “基于文件执行”后仅运行 Dotnet - Qiita 后，AOT 错误导致崩溃的原因与解决方案
https://qiita.com/KM_20005/items/be5229a2944df6fa3e97

### [C#] 用集合表达式初始化让事情更干净 - Qiita
https://qiita.com/nakamuuu_ow/items/5c3e08b6f0272249802c

### [超级dotnet新人] 做了我的第一场演讲，题为“从个人视角看dotnet运行时趋势”
https://zenn.dev/prozolic/articles/d7f518c69c182e

<div class=“docswell-link”><a href=“https://www.docswell.com/s/prozolic/KR8672-2026-05-30-214517”> Dotnet 运行时趋势的个人视角 by @prozolic</a></div>
### 在 Super dotnet 发布，主题为“Aspire 与 GitHub Copilot 的集成”
https://zenn.dev/microsoft/articles/super-dotnet-new-aspire-copilot

### 月亮点转C#

https://www.docswell.com/s/akeit0/ZQ29WV-2026-06-02-165448

<div class=“docswell-link”><a href=“https://www.docswell.com/s/akeit0/ZQ29WV-2026-06-02-165448”>MoonBit 转成 C# by @akeit0</a></div>
### 用C#创建WebAssembly运行时
https://www.docswell.com/s/nuskey/59NR6X-super-dotnet-new

<div class=“docswell-link”><a href=“https://www.docswell.com/s/nuskey/59NR6X-super-dotnet-new”> @nuskey 在 C# 中创建 WebAssembly 运行时</a></div>
### Avalonia桌面开发——也许你还能做得更多
https://speakerdeck.com/mogamit/avaloniadedesukutotupukai-fa-motutoyatutemoiinziyanai

### .NET for Android 原生 AOT 并用光标构建
https://speakerdeck.com/neuecc/dot-net-for-android-with-native-aot-built-with-cursor

### 试试和罗丝琳的流程分析
https://speakerdeck.com/ruccho/flow-analysis-with-roslyn

### 利用GitHub Copilot CLI提升网页无障碍的故事
https://speakerdeck.com/tomokusaba/github-copilot-clidewebakusesibiriteiwogai-shan-sitahua

### 利用AI和 ASP.NET 核心创建杂项网页应用的故事
https://speakerdeck.com/mayuki/build-your-own-apps-with-ai-20260529-dotnetnew

### C# 和 C# 之间的互操作性(或不互操作性)
https://docs.google.com/presentation/d/1wkFJCkgCRpwEHld6MnL5zgZ8go3UkfMZbeaQGBWU-98/mobilepresent?slide=id.p

---

## 今日人物

**奥利-约翰·达尔**(英语：Ole-Johan Dahl，1931年10月12日—2002年6月29日)与**克利斯登·奈加特**(英语：Kristen Nygaard，1926年8月27日—2002年8月10日)，是挪威计算机科学家、Simula 语言共同创造者和面向对象程序设计的先驱。他们确立了对象、类、继承和虚过程等核心概念，对现代软件开发产生了深远影响。

2001年，达尔与奈加特因“通过设计 Simula I 和 Simula 67，为面向对象程序设计的诞生奠定基础”共同获得图灵奖。

![奥利-约翰·达尔与克利斯登·奈加特](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/dahl-nygaard.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

- 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
- .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
- 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。
