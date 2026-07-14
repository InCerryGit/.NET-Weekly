**C# .NET 周刊｜2026年5月2期 2026-05-10 dotnet_week_26_5_2**

## 国内文章
### OpenHarmony.Avalonia 归档事件对中国自主软件生态的影响--信任的坍塌与生态的异化

https://www.cnblogs.com/shanyou/p/19998663

2026年5月8日，开发者“布布”宣布 OpenHarmony-NET/OpenHarmony.Avalonia 停更并归档，引发技术圈强烈讨论。布布称他以业余身份推进 Avalonia 在鸿蒙的底层适配，并与 Avalonia 官方接触，期待官方或华为合作并获聘。布布为保护商业利益曾放缓公开发布并移至闭源仓库。后来他发现华为在与 Avalonia 洽谈同时在招标平台发布技术标书，外包公司如软通动力中标并在招聘中寻觅 Avalonia 工程师。布布据此怀疑存在利用官方交流信息进行招标的行为。此事触发对企业诚信、开源治理和国产操作系统生态建设路径的广泛争议。

### .NET 8 Web开发入门(二)：C# 现代语法速成——为 Web API 量身定制

https://www.cnblogs.com/shenchuanchao/p/19990124/dotnet-8-web-development-part2-modern-csharp-for-webapi

文章讲述在现代.NET 8中将 DTO 从 class 迁移到 record，展示 record 的构造、不变性、值相等性与 with 用法。文章强调异步编程(async/await)对提升 Web 并发的关键性，并用餐厅类比解释同步阻塞的问题。示例直观且实用。文章技术深度中等，原创性一般，缺少引用，个别章节未完整展开。

### 记一次 .NET 某智慧工厂视觉程序 崩溃分析

https://www.cnblogs.com/huangxincheng/p/19980635

文章记录作者用 WinDbg 分析 .NET 程序崩溃的过程。作者提供 dump 输出，显示 CLR 异常 e0434352 和 System.Reflection.TargetInvocationException。作者用 !t 查看线程与托管异常，用 !pe -nested 展开异常链。示例真实，步骤可复现，适合有调试基础的读者。文章实践性强但细节与解决步骤不足，引用缺乏。

### 【EF Core】值转换器

https://www.cnblogs.com/tcjiaan/p/19966652

作者开篇提及近况和裁员观察，认为多数裁员与 AI 无关。正文介绍 EF Core 值转换器的概念与用途。文章区分两种值：Provider(数据库映射到 .NET 的类型)与 Model(实体属性类型)。当二者不一致时需要值转换器。文中举例说明枚举与数据库字符串互转，以及将自定义 Point 结构序列化为“100,85”字符串保存并还原的场景。文章还提供了建表脚本和部分 C# 实体代码示例。技术性为入门到中级，注重实用示例，未见引用说明来源。

### .NET 10 使用 Microsoft.AspNetCore.OpenApi 实现 API 版本管理

https://www.cnblogs.com/denglei1024/p/19975811

文章说明 API 版本管理的重要性，目标是在不破坏现有用户的前提下持续迭代。列举了 URL 路径、查询参数、请求头和媒体类型四种常见策略。指出在 C# 生态中长期用 Swashbuckle 配合 Asp.Versioning，而 .NET 10 推出 Microsoft.AspNetCore.OpenApi，且 Asp.Versioning v10 已支持该库，实现版本管理与文档生成的无缝结合。给出需安装的 NuGet 包列表并示例 Program.cs 配置流程：AddApiVersioning、AddApiExplorer、为每个版本 AddOpenApi、MapOpenApi 和 MapScalarApiReference。示例展示为每个版本生成独立 OpenAPI 文档，并在路由中通过 apiVersion 指定版本，但控制器示例未完整展开。

### C# 也能像 Python 一样写脚本 |  .NET 10 构建基于文件的应用

https://www.cnblogs.com/denglei1024/p/19979190

文章介绍 .NET 10 的基于文件的应用功能。开发者可在单个 .cs 文件中编写、运行和构建应用，适合快速原型、脚本和小型工具。需要安装 .NET 10 SDK。文中给出两个示例：一个显示当前日期，另一个用 CsvHelper 处理销售数据并生成 CSV。说明了 #:package、#:property、#:sdk、#:reference、#:project 等指令用法及版本写法，并展示 dotnet run <file.cs> 等 CLI 命令。文章实用清晰，但缺少引用和更深入的性能或限制分析。

### OpenClaw.NET .NET 原生插件开发完全指南：以 Mempalace 插件为范例

https://www.cnblogs.com/shanyou/p/19974437

文章介绍 OpenClaw.NET，一个用 C#13 从零构建的独立 AI Agent 网关与运行时。项目以 NativeAOT 为核心设计以实现毫秒级冷启动和低内存占用。默认以本地 AOT 模式在回环地址 18789 运行，插件以内进程方式加载以换取性能。框架支持多种插件加载模式并允许标记为仅 JIT 的插件以兼顾扩展性。为兼容 OpenClaw 生态，采用语义兼容的插件契约和配置，并利用 Microsoft.Extensions.AI 与依赖注入实现与 LLM 提供商的集成。插件承担模型接入、消息通道、工具、记忆和后台服务等核心职责，记忆采用独占插槽策略。

### .NET 8 Web开发入门(一)：启程——.NET生态全景与开发环境构建

https://www.cnblogs.com/shenchuanchao/p/19972855/dotnet-8-web-development-part1-ecosystem-setup

.NET 8 是LTS版本，具备跨平台、高性能与统一生态。作者纠正了“.NET很老”的误解，指出其可在Linux和macOS上稳定运行并在基准测试中表现优异。文章分解技术栈：CLR 负责将IL即时编译并管理垃圾回收，BCL 提供丰富基础库，SDK 包含运行时、编译器与CLI。文中区分了Runtime与SDK的安装用途并提示常见部署错误。作者回顾了从.NET Framework到.NET Core再到.NET 5+的演进。最后给出安装.NET 8 SDK并用 dotnet --info 验证的实操步骤。

### .NET+AI | Harness | MAF 1.4 发布，Harness Engineering 如约而至，智能体工程化更进一步

https://www.cnblogs.com/sheng-jie/p/19995466

文章将 Harness Engineering 定义为模型外的可执行脚手架，强调四要素：有输入、有步骤、有验收、有兜底。文章指出 Harness 解决任务接入、任务拆解、状态管理、环境安全、长上下文收敛与失败恢复等工程问题。作者认为 MAF 1.4 把 Harness 提升为运行时控制面，推动智能体开发从能力拼装走向工程化。文章区分 Skills(能力包)与 Harness(执行治理)，并拟用简单的 .NET 示例说明 Harness 的实际价值。

### 基于AScript的python3脚本语言发布啦！

https://www.cnblogs.com/rockey627/p/19971851

AScript是开源C#动态脚本引擎，2026-05-04发布AScript.Lang.Python3 0.0.1。它支持Python3基础语法、主要数据类型、函数、列表/集合/字典操作，以及字符串插值和切片。文中提供NuGet安装命令和丰富的C#示例，示范注册语言、上下文指定、@lang嵌入与集合行为。技术深度中等，覆盖基础特性但缺少高级互操作与安全细节。实用性高，示例可直接运行。表达清晰，可读性好。原创性一般，时效性佳，但缺乏引用与性能评估。总体评价良好。

### C# SwaggerLoginAuthPlugin  一款给Swagger文档加登录页面的小插件

https://www.cnblogs.com/zhangboyan/p/20001532

文章介绍一款用于局域网限制Swagger查看权限的小插件。作者提供NuGet包和示例代码，说明在非最小API的Web API项目中通过 builder.Services.AddSwaggerAuth 配置默认用户名密码，并在 UseSwagger 前调用 app.UseSwaggerAuth 实现拦截。作者提醒插件仅适合内网使用并给出开源仓库地址。插件由作者借助 deepseek 和 AI 在约2小时内开发，功能简单实用但技术细节和安全说明有限，适合项目组快速加固Swagger访问控制。

### .NET生态系统中的A2A(Agent-to-Agent)协议支持与跨平台多智能体协同

https://www.cnblogs.com/shanyou/p/19974558/dotnet-a2a

文章论述从单一大语言模型向分布式多智能体的架构演进。提出A2A v1.0作为跨智能体互操作性标准，基于HTTP+JSON与JSON-RPC 2.0，并通过SSE支持流式传输。引入Agent Card实现发现优先机制，声明身份、能力、数据模式与认证。将交互建模为有状态的Task，消息由多种Parts(TextPart、FilePart、DataPart)构成，输出为可被下游消费的Artifact。重点评估.NET生态对A2A的采用与实现路径，列举Microsoft Agent Framework、BotSharp(PR 1345)与OpenClaw.NET(PR 90)的具体集成与安全、NativeAOT等优化。文章技术深度高且面向企业实用场景。

### 一款基于 C# 开发的 Windows 10/11 系统增强工具，精简、优化、定制一站完成！

https://www.cnblogs.com/Can-daydayup/p/20007914

Winhance 是一款基于 C# 的开源 Windows 10/11 系统增强工具。它以图形界面整合应用管理、系统优化、隐私设置、界面定制、常用软件安装、配置导入导出和自定义 ISO 制作等功能。适合新机初始化、系统重装后快速恢复和日常优化维护。核心模块包括软件管理(移除/安装应用、WinGet 支持)、系统优化(隐私、性能、更新、通知等)、界面定制和高级工具(生成 autounattend.xml)。项目托管在 GitHub，并已收录于 C#/.NET 项目精选，便于开发者参考和贡献。

### Memgraph 与 Neo4j 图数据库对比及 .NET 生态适配分析

https://www.cnblogs.com/shanyou/p/19976092/neo4jvsmemgraph

文章比较 Memgraph 与 Neo4j 在设计哲学、实现语言、存储模型、事务一致性、索引策略、查询兼容性和 .NET 生态适配上的差异。Neo4j 基于 Java、磁盘优先、采用 Index-Free Adjacency、保持 ACID 强一致并拥有成熟的 .NET 工具链。Memgraph 基于 C++、内存优先、提供亚毫秒延迟和高吞吐、兼容 openCypher 与 Bolt、采用 BSL 许可并提供可选的分析模式以换取吞吐。文章引用实测数据比较内存占用、延迟和持久化差异，并指出对于万级节点的读分析场景优先选 Neo4j，对于实时增量更新和高吞吐写入优先选 Memgraph。

### AScript中一个很有意思的语法

https://www.cnblogs.com/rockey627/p/19998021

文章介绍AScript开源C#动态脚本引擎的static语法。解析执行模式下，static语句与普通语句等效；编译执行模式下，static语句在编译期执行并返回结果，static内定义的变量在脚本执行前已计算。通过示例展示static在eval函数中用于预拼接表达式，以及在编译委托中用于初始化配置。最后给出StaticTokenHandler实现片段以说明实现原理。

### OpenClaw.NET 外部 CLI 连接器 (External CLI Connectors) 详细技术总结

https://www.cnblogs.com/shanyou/p/20009085

本文介绍 OpenClaw.NET 的 External CLI Connectors，封装官方平台 CLI 为 AI Agent 可控工具。设计默认禁用，不接受自由命令，只允许预配置具名命令。安全采用多层防护：命名命令白名单、风险评分、dry-run 预览、审批流程、脱敏、超时限制和审计日志。Agent 通过指定连接器名、命令名和命名参数调用，运行时将参数展开为 ProcessStartInfo.ArgumentList，不经 Shell。文档列出顶层配置和连接器示例，关键默认值包括 Enabled=false、AllowFreeformCommands=false、RequireApprovalForMutatingCommands=true、RiskLevel=high、ReadOnly=false。

### 【EF Core】使用自定义的值比较器

https://www.cnblogs.com/tcjiaan/p/20008424

文章讨论 EF Core 的值比较器问题。默认比较器按值比较，但有时不同格式表示同一含义。以 Company.Phone 为例，固话可写成 (010)88988989 或 010-88988989，默认比较器会误判为不同。作者介绍通过继承 ValueComparer<string> 自定义比较器。需要提供三种委托：相等判断、哈希计算与快照创建。示例通过正则解析区号与号码，重写相等与哈希逻辑，快照可用内置实现，从而实现语义相等比较并避免错误的状态变更检测。

### 我的开源项目分享-基于SharpBrowser二次开发的定制浏览器，过程中填坑无数

https://www.cnblogs.com/rrooyy/p/19995607

为满足仅允许固定电脑登录的安全需求，作者定制浏览器。每个请求头加入设备ID，由服务器校验。项目基于C#开源SharpBrowser。作者发现多个缺陷。包括不支持alert/prompt/confirm、window.open无返回、下载页面日期与排序错误及CEF不支持H.264。作者修正安装脚本路径、内置存储位置、下载日期显示及window.open返回值。作者新增中文界面、打开文件夹功能、公司打印管理器自定义协议、设备ID与设备密钥设置。对不支持H.264的视频，选择上传时自动转换为webm。构建需自行放置ffmpeg.exe于src\\bin\\net8.0-windows，安装包用Inno Setup并加中文语言包。

### 【译】Azure MCP 工具现已内置集成至 Visual Studio 2022，无需额外安装扩展

https://www.cnblogs.com/MeteorSeed/p/19979206

文章说明Azure MCP工具已内置于Visual Studio 2022的Azure开发工作负载(自17.14.30起)，无需单独安装扩展。作者指出内置后可避免扩展兼容性问题并随VS统一更新，但Visual Studio 2026独有功能不包含在2022中。Azure MCP通过GitHub Copilot Chat提供覆盖45项Azure服务的230余种工具。示例包括列出订阅中的存储账户、将ASP.NET Core应用通过azd部署到Azure、使用AppLens诊断应用服务和在Log Analytics中运行KQL查询。工具默认禁用，需在IDE中手动启用即可在所有会话中持续使用。

### CsGrafeq: 比 Desmos 更“能折腾”的几何函数画板(.NET + Avalonia)

https://www.cnblogs.com/StuLittleLi/p/20005397

CsGrafeq 是一款由高中生开发的跨平台几何草图與隐函数作图工具。它支持点、线、圆等几何构造与拖拽交互，能高质量绘制隐函数 f(x,y)=0 的图像。项目基于 .NET 与 Avalonia，强调即时交互与易用性，适合学习、验证与探索数学问题。作者说明了开发动机、功能场景與跨平台优势，并开源在 GitHub，欢迎 Issue 与 PR。文章实用性与可玩性强，但技术实现细节与引用较少。

### 【译】TypeScript 7 测试版已在 Visual Studio 2026 18.6 Insiders 3 中默认启用

https://www.cnblogs.com/MeteorSeed/p/19996925

Visual Studio 2026 18.6 预览版3 将内置 TypeScript SDK 升级为 TypeScript 7 Beta 原生预览版。该更新影响使用内置 SDK 的所有项目，包括 TypeScript 项目和使用 npm 的 ASP.NET Core 项目。TypeScript 7 带来原生执行和共享内存并行处理，编译速度最高提升约 10 倍，内存占用显著下降，项目加载和语言服务响应约提升 8 倍。编辑体验的智能感知、查找引用、转到定义和错误诊断均明显加速。若需使用其他版本，可在项目中安装 typescript@^6.0.0 或 @typescript/native-preview@beta，Visual Studio 优先使用本地 node_modules。可在 Tools > Options > Preview Features 中禁用原生预览。文末列出若干正在修复的已知问题。


---

## 国际周报

## 话题

### .NET 10.0.7 带外安全更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-10-0-7-oob-security-update/
### Aspire 13.3 最新动态 | Aspire 博客
https://devblogs.microsoft.com/aspire/whats-new-aspire-13-3/

### Windows 应用 SDK 2.0 发布说明 - Windows 应用
https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/release-notes/windows-app-sdk-2-0?pivots=stable

- [发布 Windows 应用 SDK 2.0 (2.0.1) 🎉 · microsoft/WindowsAppSDK](https://github.com/microsoft/WindowsAppSDK/releases/tag/v2.0.1)

### VSTest 正在移除其 Newtonsoft.Json 依赖 - .NET 博客
https://devblogs.microsoft.com/dotnet/vs-test-is-removing-its-newtonsoft-json-dependency/

### Visual Studio 四月更新 – 云代理集成 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-april-update-cloud-agent-integration/

### Copilot Studio 在 WebAssembly 上运行 .NET 10 加速 - .NET 博客
https://devblogs.microsoft.com/dotnet/copilot-studio-dotnet-10-migration/

### 欢迎来到SkiaSharp 4.0预览1 - .NET博客
https://devblogs.microsoft.com/dotnet/welcome-to-skia-sharp-40-preview1/

### Ubuntu 26.04 中 .NET 的新内容 - .NET 博客
https://devblogs.microsoft.com/dotnet/whats-new-for-dotnet-in-ubuntu-2604/

### 宣布WinApp VS Code扩展——在VS Code中运行、调试和打包Windows应用 - #ifdef 窗户
https://devblogs.microsoft.com/ifdef-windows/announcing-the-winapp-vs-code-extension-run-debug-and-package-windows-apps-in-vs-code/

### 宣布WinUI 3图库2.9 - #ifdef Windows
https://devblogs.microsoft.com/ifdef-windows/announcing-winui-3-gallery-2-9/

### TypeScript 7 测试版现已默认启用，已在Visual Studio 2026 18.6 Insiders 3 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/typescript-7-beta-now-enabled-by-default-in-visual-studio-2026-18-6-insiders-3/

### 通过代理治理工具包在.NET中管理MCP工具调用 - .NET博客
https://devblogs.microsoft.com/dotnet/governing-mcp-tool-calls-in-dotnet-with-the-agent-governance-toolkit/

### SDK 风格的扩展项目支持 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/sdk-style-support-for-extension-projects/

## 发布
- [AvaloniaUI/Avalonia](https://github.com/AvaloniaUI/Avalonia)
    - [12.0.2](https://github.com/AvaloniaUI/Avalonia/releases/tag/12.0.2)
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [4.0.235.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.235.0)，[4.0.236.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.236.0)，[4.0.237。 0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.237.0)， [4.0.238.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.238.0)， [4.0.239.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.239.0)， [4.0.240.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.240.0)， [4.0.241.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.241.0)， [4.0.242.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.242.0)， [4.0.243.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.243.0)， [4.0.244.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.244.0)， [4.0.245.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.245.0)， [4.0.246.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.246.0)
- [Azure/azure-cosmos-dotnet-v3](https://github.com/Azure/azure-cosmos-dotnet-v3)
    - [3.59.0](https://github.com/Azure/azure-cosmos-dotnet-v3/releases/tag/3.59.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.AI.Projects_2.0.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.AI.Projects_2.0.1)， [Azure.Core_1.54.0]( https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Core_1.54.0)， [Azure.Core_1.55.0]( https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Core_1.55.0)，[Azure.Extensions.AspNetCore.DataProtection.Blobs_1.5. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Extensions.AspNetCore.DataProtection.Blobs_1.5.2)、[Azure.Extensions.AspNetCore.DataProtection.Keys_ 1.6.2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Extensions.AspNetCore.DataProtection.Keys_1.6.2)， [Azure.Monitor.OpenTelemetry.AspNetCore_1.5. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Monitor.OpenTelemetry.AspNetCore_1.5.0)，[Azure.Monitor.OpenTelemetry.Exporter_1.8。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Monitor.OpenTelemetry.Exporter_1.8.0)，[Azure.ResourceManager.Automanage_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Automanage_1.1.2)，[Azure.ResourceManager.Automation_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Automation_1.1.2) [Azure.ResourceManager.Billing_1.2.2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Billing_1.2.2 年)，[Azure.ResourceManager.CarbonOptimization_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.CarbonOptimization_1.0.1)，[Azure.ResourceManager.ChangeAnalysis_1.1. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ChangeAnalysis_1.1.2 年)，[Azure.ResourceManager.Chaos_1.1。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Chaos_1.1.1)， [Azure.ResourceManager.ComputeLimit_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ComputeLimit_1.0.0)，[Azure.ResourceManager.ConnectedVMwarevSphere_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ConnectedVMwarevSphere_1.1.2)， [Azure.ResourceManager.CostManagement_1.0. 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.CostManagement_1.0.3)， [Azure.ResourceManager.CustomerInsights_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.CustomerInsights_1.0.0)，[Azure.ResourceManager.DataBox_1.1。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataBox_1.1.1)，[Azure.ResourceManager.DataLakeAnalytics_1.1. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataLakeAnalytics_1.1.2)，[Azure.ResourceManager.DataLakeStore_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataLakeStore_1.1.2)，[Azure.ResourceManager.DataShare_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataShare_1.1.2)， [Azure.ResourceManager.DeviceUpdate_1.0. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DeviceUpdate_1.0.2)， [Azure.ResourceManager.DevOpsInfrastructure_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DevOpsInfrastructure_1.0.0)， [Azure.ResourceManager.DevSpaces_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DevSpaces_1.0.0)，[Azure.ResourceManager.DigitalTwins_1.3。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DigitalTwins_1.3.2)，[Azure.ResourceManager.EdgeOrder_1.1. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.EdgeOrder_1.1.2)，[Azure.ResourceManager.ExtendedLocations_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ExtendedLocations_1.1.2 年)，[Azure.ResourceManager.FluidRelay_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.FluidRelay_1.1.2)，[Azure.ResourceManager.GraphServices_1.1。 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.GraphServices_1.1.3)，[Azure.ResourceManager.GuestConfiguration_1.2。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.GuestConfiguration_1.2.2)， [Azure.ResourceManager.HardwareSecurityModules_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.HardwareSecurityModules_1.0.1)， [Azure.ResourceManager.HealthcareApis_1.3. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.HealthcareApis_1.3.2)，[Azure.ResourceManager.HealthDataAIServices_1.0。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.HealthDataAIServices_1.0.1)，[Azure.ResourceManager.HybridConnectivity_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.HybridConnectivity_1.1.1)，[Azure.ResourceManager.HybridContainerService_1.0. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.HybridContainerService_1.0.2)，[Azure.ResourceManager.InformaticaDataManagement_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.InformaticaDataManagement_1.0.0)，[Azure.ResourceManager.KubernetesConfiguration_1.2。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.KubernetesConfiguration_1.2.1)， [ Azure.ResourceManager.KubernetesConfiguration.Extensions_1.0.0]( https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.KubernetesConfiguration.Extensions_1.0.0)，[Azure.ResourceManager.LabServices_1.1。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.LabServices_1.1.2)，[Azure.ResourceManager.LambdaTestHyperExecute_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.LambdaTestHyperExecute_1.0.1)，[Azure.ResourceManager.Logic_1.2。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Logic_1.2.0)， [Azure.ResourceManager.ManagedNetworkFabric_1.1. 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ManagedNetworkFabric_1.1.3)，[Azure.ResourceManager.ManagedServiceIdentities_1.4。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ManagedServiceIdentities_1.4.1) [Azure.ResourceManager.Marketplace_1.1.3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Marketplace_1.1.3)，[Azure.ResourceManager.MarketplaceOrdering_1.1. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.MarketplaceOrdering_1.1.2)， [Azure.ResourceManager.MongoDBAtlas_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.MongoDBAtlas_1.0.1 年)，[Azure.ResourceManager.NetApp_1.16。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.NetApp_1.16.0)， [Azure.ResourceManager.NetworkFunction_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.NetworkFunction_1.0.0)， [Azure.ResourceManager.Orbital_1.1. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Orbital_1.1.2)，[Azure.ResourceManager.Peering_1.2。 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Peering_1.2.3)， [Azure.ResourceManager.PlanetaryComputer_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.PlanetaryComputer_1.0.0)，[Azure.ResourceManager.PostgreSql_1.4。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.PostgreSql_1.4.2)， [Azure.ResourceManager.PowerBIDedicated_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.PowerBIDedicated_1.0.0)，[Azure.ResourceManager.PrivateDns_1.2。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.PrivateDns_1.2.2)， [Azure.ResourceManager.PureStorageBlock_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.PureStorageBlock_1.0.1)，[Azure.ResourceManager.RecoveryServicesSiteRecovery_1.3. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.RecoveryServicesSiteRecovery_1.3.1)， [Azure.ResourceManager.ScVmm_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ScVmm_1.0.0)， [Azure.ResourceManager.Sphere_1.0. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Sphere_1.0.2)， [Azure.ResourceManager.StorageActions_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.StorageActions_1.0.1)，[Azure.ResourceManager.StorageMover_1.4。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.StorageMover_1.4.0)， [Azure.ResourceManager.Subscription_1.1. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Subscription_1.1.2)，[Azure.ResourceManager.Synapse_1.2。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Synapse_1.2.2)，[Azure.Search.Documents_12.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Search.Documents_12.0.0)，[Azure.Security.KeyVault.Administration_4.8。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Security.KeyVault.Administration_4.8.0)，[Azure.Security.KeyVault.Keys_4.10。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Security.KeyVault.Keys_4.10.0)，[Azure.Security.KeyVault.Secrets_4.11。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Security.KeyVault.Secrets_4.11.0)， [Microsoft.Extensions.Azure_1.14. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Extensions.Azure_1.14.0)， [System.ClientModel_1.11.0]( https://github.com/Azure/azure-sdk-for-net/releases/tag/System.ClientModel_1.11.0)
- [CommunityToolkit/Maui](https://github.com/CommunityToolkit/Maui)
    - [14.1.1](https://github.com/CommunityToolkit/Maui/releases/tag/14.1.1)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.43.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.43.0)
- [dotnet/诊断](https://github.com/dotnet/diagnostics)
    - [v10.0.721401](https://github.com/dotnet/diagnostics/releases/tag/v10.0.721401)
- [dotnet/SqlClient](https://github.com/dotnet/SqlClient)
    - [v6.1.5](https://github.com/dotnet/SqlClient/releases/tag/v6.1.5)， [v7.0.1](https://github.com/dotnet/SqlClient/releases/tag/v7.0.1)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.Redis.Cluster.V1-1.7.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Redis.Cluster.V1-1.7.0)， [ Google.Shopping.Merchant.Products.V1-1.6.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Shopping.Merchant.Products.V1-1.6.0)， [ Google.Shopping.Merchant.Reports.V1-1.2.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Shopping.Merchant.Reports.V1-1.2.0)
- [grpc/grpc-dotnet](https://github.com/grpc/grpc-dotnet)
    - [v2.80.0](https://github.com/grpc/grpc-dotnet/releases/tag/v2.80.0)
- [icsharpcode/ILSpy](https://github.com/icsharpcode/ILSpy)
    - [v10.0.1](https://github.com/icsharpcode/ILSpy/releases/tag/v10.0.1)
- [微软/Aspire](https://github.com/microsoft/aspire)
    - [v13.2.3](https://github.com/microsoft/aspire/releases/tag/v13.2.3) [v13.2.4](https://github.com/microsoft/aspire/releases/tag/v13.2.4)， [v13.3.0](https://github.com/microsoft/aspire/releases/tag/v13.3.0)
- [microsoft/WindowsAppSDK](https://github.com/microsoft/WindowsAppSDK)
    - [v1.8.7](https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.8.7)， [v2.0.1](https://github.com/microsoft/WindowsAppSDK/releases/tag/v2.0.1)
- [newrelic/newrelic-dotnet-agent](https://github.com/newrelic/newrelic-dotnet-agent)
    - [v10.51.0](https://github.com/newrelic/newrelic-dotnet-agent/releases/tag/v10.51.0)
- [开放遥测/开放遥测点网](https://github.com/open-telemetry/opentelemetry-dotnet)
    - [core-1.15.3](https://github.com/open-telemetry/opentelemetry-dotnet/releases/tag/core-1.15.3)
- [开放遥测/开放遥测点网贡献](https://github.com/open-telemetry/opentelemetry-dotnet-contrib)
    - [Exporter.Instana-1.1.0](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/Exporter.Instana-1.1.0)， [PersistentStorage-1.0。 3](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/PersistentStorage-1.0.3)， [PersistentStorage-1.1. 0](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/PersistentStorage-1.1.0)
- [unoplatform/uno](https://github.com/unoplatform/uno)
    - [6.5.229](https://github.com/unoplatform/uno/releases/tag/6.5.229)

## 文章、幻灯片及更多内容
### Doco 用到 C# 吗？ 2026
https://zenn.dev/inuinu/articles/where-is-csharp-used-2026

### 理解 Microsoft 代理框架的 Harness 机制及 LM Studio 和本地大型语言模型的执行流程
https://zenn.dev/yy7613/articles/74265daaf7929a

### AI 子代理“即将登陆”Visual Studio Copilot——Visual Studio 杂志
https://visualstudiomagazine.com/articles/2026/05/06/ai-subagents-coming-to-visual-studio-ides-copilot.aspx

### Microsoft代理框架中的持久工作流 - .NET 博客
https://devblogs.microsoft.com/dotnet/durable-workflows-in-microsoft-agent-framework/

### 试试带本地LLM的Microsoft代理框架第13部分(中间件)
https://zenn.dev/yy7613/articles/bb5fa8cdb6bf64

### Microsoft代理框架 - AI构建模块 第三部分 - .NET博客
https://devblogs.microsoft.com/dotnet/microsoft-agent-framework-building-blocks-for-ai-part-3/

### 绑定列举
https://zenn.dev/shinta0806/articles/enum-binding

### 用 Blazor WebAssembly 制作的工程师诊断应用 - 本地化、通用协议和 cookie 同意
https://zenn.dev/nekojoker/articles/c9f17b69690031

### [C#] CSharpier 推荐
https://zenn.dev/nuskey/articles/csharpier-is-good

### ASP.NET 生产中核心 Cookie 大小限制：原因与修复
https://duendesoftware.com/blog/20260429-aspnet-core-cookie-size-limits

### 渴望WPF界面，最终回归.NET MAUI Blazor Hybrid - Qiita的故事
https://qiita.com/maki_s/items/527469f0ff9fa94cefb2

### . 如何在 .NET - Qiita 中使用 OpenAI API
https://qiita.com/qOpenDev/items/fc3ca29355956c1d0381

### . 如何通过API将.NET包上传到NuGet
https://zenn.dev/loach/articles/upload-nuget

### 解释SQL和LINQ中的范畴论 - Qiita
https://qiita.com/yaju/items/38a283f4b1fba434f620

### [Blazor + Syncfusion] 我在实现以SfGrid为中心的商业应用列表界面后——Qiita的感受
https://qiita.com/af-dev-hub/items/79eb00a4306a01a2a12f

### [树莓派5] 从Antigravity远程SSH连接开发C#
https://zenn.dev/minenote/articles/2c93232bab8b61

### 现金策略深度比较 ~专注于懒惰现金~ - Qiita
https://qiita.com/Mitsuki0003/items/260d0f64cdc580de181c

### 用.NET代码生成模板尝试的多个代理开发循环
https://zenn.dev/tomokusaba/articles/14f2373c51e1f2

### 在.NET中评估CRON和RRule表达式 - Gérald Barré
https://www.meziantou.net/evaluating-cron-and-rrule-expressions-in-dotnet.htm

### 在C#中用Facet .NET：.NET的TypeScript工具类型
https://tim-maes.com/blog/2026/04/17/pick-and-omit-in-csharp-with-facet/

### .NET 11 预览版3 基于文件的应用文件拆分
https://zenn.dev/prozolic/articles/a861cc1da6b0e1

### 让我们读ZString (4) 缓冲区 - Qiita
https://qiita.com/kuto110/items/75c0336a25c6d0afd1af

### System.CommandLine 稳定版发布 - Qiita
https://qiita.com/KM_20005/items/94d1db2f49c7436d598b

### C#：自动将只调用一次的动作集中
https://zenn.dev/ruccho/articles/csharp-pooled-actions

### 构建一个由 . NET的可组合AI协议栈——.NET博客
https://devblogs.microsoft.com/dotnet/building-ai-conference-app-dotnet-composable-stack/

### 试试带本地LLM的Microsoft代理框架第12部分(结构化输出)
https://zenn.dev/yy7613/articles/27d7ed3c97ff1a

### 联盟类型性能比较：非拳击定制联盟 [C#15预览]
https://zenn.dev/inuinu/articles/csharp-union-performance

### 尝试带本地LLM的Microsoft代理框架第11部分(带AIContextProvider的简化RAG)
https://zenn.dev/yy7613/articles/d5b22b11d40fca

### Azure 上 .NET 和 Postgres 的高性能分布式缓存 - .NET 博客
https://devblogs.microsoft.com/dotnet/high-performance-distributed-caching-dotnet-postgres-azure/

### 尝试用 Windows Forms 做 MVVM，结果却陷入自满，且 。 NET 10 可以写出这样的故事——Qiita
https://qiita.com/inuta-one/items/4cb48340bdfe32b15592

### 在.NET 10应用中结合API版本管理与OpenAPI - .NET博客
https://devblogs.microsoft.com/dotnet/api-versioning-in-dotnet-10-applications/
### 你目前使用的GitHub Copilot CLI + .NET的自定义代理和技能
https://zenn.dev/microsoft/articles/github-copilot-dotnet-project

### Entra 验证ID发行实现：含.NET样本的数字ID API
https://zenn.dev/kumaik/articles/entra-verified-id-dotnet-issuance

### Windows 应用开发 CLI v0.3：新增运行命令和界面命令，以及对打包应用的 dotnet run 支持 - #ifdef 窗户
https://devblogs.microsoft.com/ifdef-windows/windows-app-development-cli-v0-3-new-run-and-ui-commands-plus-dotnet-run-support-for-packaged-apps/

### 首次使用Claude Design重新设计了Blazor应用的默认界面 - Qita
https://qiita.com/non-k/items/bcc3cf14e072b74ae730

### [C#] 深入思考例外与日志：第一部分 例外类的完整解剖——Qiita。
https://qiita.com/KM_20005/items/eab8ab1db5ab28d9164e

### [C#] 关于C#开发工具包生成的.lscache文件
https://zenn.dev/nuskey/articles/csharp-lscache

### 使用 GitHub Copilot CLI 和 VS Code 代理模式供 C# 开发者使用
https://zenn.dev/tomokusaba/articles/838cdac8d71e52

### 使用 ReadOnlySpanT 移除 .NET Framework 中的字节[] 分配
https://andrewlock.net/removingbyte-array-allocations-in-dotnet-framework-using-readonlyspan-t/

### 如何在不继承 Microsoft 365 Agents SDK 的 AgentApplication 类的情况下编写
https://zenn.dev/karamem0/articles/2026_04_21_090000

### mruby 在 C# 上：从虚拟机实现到游戏脚本(RubyKaigi 2026)
https://speakerdeck.com/hadashia/mruby-on-c-number-from-vm-implementation-to-game-scripting

## 库、仓库、工具等
### r-dev95/OpRec
https://github.com/r-dev95/OpRec

- [开发了Windows屏幕录制应用OpRec](https://zenn.dev/r_dev95/articles/0004-introduce-oprec)

### ulex/windows_defender_performance_tool：实时Windows Defender扫描性能监控器
https://github.com/ulex/windows_defender_performance_tool

### akeit0/Enaga：用于直接渲染html/css(及浏览器)或ReactNative的实验性C#项目。
https://github.com/akeit0/Enaga

- [我用C#创建了自己的JavaScriptEngine + 浏览器](https://zenn.dev/aakei/articles/my-scratch-browser)

## 今日人物

阿米尔·伯努利（英语：Amir Pnueli，1941年4月22日—2009年11月2日），以色列计算机科学家。伯努利出生于英国巴勒斯坦（以色列）的那哈啦，并获得了海法以色列理工学院的数学学士学位和博士学位。来自魏茨曼科学研究所的应用数学。他的论文主题是“海洋潮汐的计算”。在斯坦福大学担任博士后研究员期间，他转到计算机科学专业。他的计算机科学着作侧重于时态逻辑和模型检查，特别是关于并发系统的公平性。

1996年因“开创性地将时序逻辑引入计算机科学和对程序和系统验证领域的杰出贡献”而获得图灵奖。电脑协会（ACM）会士。

![image-20260610225327920](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20260610225327920.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

- 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
- .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
- 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。