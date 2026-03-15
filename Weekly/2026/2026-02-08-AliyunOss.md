## 国内文章
### asp.net core如何实现Controller热更新

https://www.cnblogs.com/kevin-Y/p/19569791

文章探讨了ASP.NET Core的热更新方法，特别是通过自定义的AssemblyLoadContext类来实现插件的动态加载与卸载。这种方法允许在生产环境中替换DLL文件，而不会导致服务停机。文章介绍了如何使用流加载DLL，以避免文件被锁定，从而实现真正的热更新。这对于希望保持系统持续运行的开发者来说，具有重要的实践意义。

### MWGA让千亿行代码在Web端“复活”！

https://www.cnblogs.com/xdesigner/p/19565029

南京都昌信息研发的MWGA工具，能够将传统Winforms程序无缝迁移至Blazor WASM平台，实现低成本、快速迁移。用户仅需极少的代码修改，便可在多种操作系统上运行，节省大量开发时间与费用。MWGA支持多个平台，并兼容主流浏览器，避免了企业重写业务逻辑的困扰，适合医疗等对信创有需求的行业。通过案例展示，MWGA显著提高迁移效率，技术门槛低，减少了企业的人力、时间和维护成本。此工具改变了企业应用程序迁移的游戏规则，保障了用户体验。 

### 推荐 .NET 8.0 开源项目伪微服务框架

https://www.cnblogs.com/1312mn/p/18376570

本文介绍了一个基于.NET 8.0的小型伪微服务框架，适合快速搭建应用项目。框架简化了微服务特性，专注于业务逻辑，提高了开发效率。集成了EF Core、Redis、RabbitMQ等新技术，以支持高并发。框架提供了完整的接口和文档，便于用户上手。核心功能包括对象映射、查询封装、数据库交互、依赖注入、认证授权、分布式ID生成等。项目已经在GitHub上开源，作者承诺持续改进以增强功能和性能。希望这个框架能帮助开发者解决实际问题。

### .NET 中如何快速实现 List 集合去重？

https://www.cnblogs.com/1312mn/p/18552496

本文介绍了.NET 6 和 .NET 7 的 DistinctBy 方法，用于根据指定键去除集合中的重复元素。方法可以在LINQ查询中使用，保持元素的原始顺序。通过示例，展示了如何使用该方法对用户列表和订单列表进行去重。源码分析揭示了该方法利用HashSet确保高效去重，同时可以扩展至多个属性的去重逻辑，具有良好的实用性和清晰度。

### .NET AI 核心构建块：重塑智能应用开发的架构范式与生态

https://www.cnblogs.com/shanyou/p/19582324

随着.NET 10 发布，微软把人工智能转变为.NET 生态系统的一部分，提供统一的高性能构建块。Microsoft.Extensions.AI 引入 IChatClient 接口，实现与模型供应商解耦，支持灵活切换后端模型。中间件模式增强企业治理，注入安全性和性能监控逻辑。MEAI 简化非结构化数据处理，通过类型安全提高开发效率。同时，向量数据库支持检索增强生成的标准范式，解决生成式 AI 知识截止的问题。这些创新提高了开发者的生产力和应用稳定性。

### 基于 Clean Architecture + DDD 的轻量级工作流系统实践

https://www.cnblogs.com/aishangyipiyema/p/19585669

本文探讨在 .NET 10 和 Vue 3 构建轻量级审批工作流系统的实践，采用 Clean Architecture 和 DDD 模式。Ncp.Admin 系统已有用户管理模块，需新增审批流程。文章比较了现有的 Elsa Workflows 与自建方案，最终选择后者因为自建方案更符合现有架构且维护成本低。文中详细描述了领域模型设计，包括聚合根划分以及强类型 ID 的应用，明确了工作流系统的核心逻辑和功能需求，具有实用性和技术深度。

### .NET Core 双数据库实战：优雅融合 PostgreSQL 与 SQLite 的最佳实践

https://www.cnblogs.com/newbe36524/p/19567317

本文探讨了如何在 .NET Core 项目中同时支持 PostgreSQL 和 SQLite，实现开发与生产环境的最佳适配。通过依赖抽象的设计思想，开发者能在配置层决定数据库选择。同时，文章提供了动态配置的代码实现，以便根据需求配置 DbContext。这样的架构设计确保了开发者的便利性和生产环境的稳定性。HagiCode 平台的实战经验为这一方法提供了实际基础。全篇围绕双数据库适配方案展开，具有实用性和技术深度。

### 浅谈数据访问层

https://www.cnblogs.com/legweifang/p/19575087

文章探讨了数据访问层在现代开发中的淡化，尤其是ORM框架对程序员理解数据库的影响。作者认为，虽然ORM简化了开发，但程序员必须掌握数据库知识，才能有效解决系统问题。他提倡使用传统SQL和DataTable，以增强灵活性和对数据库的理解。文章强调数据准确性和完整性的重要性，指出数据访问层的设计应关注数据库连接和基本操作。作者引发讨论，鼓励程序员对自己的工具和方法负责。虽然多数人已依赖ORM，但老一辈程序员对传统方法的信念依然存在。

### .NET AI 生态系统的重构与演进：Microsoft Agent Framework 对 Semantic Kernel 的继承、超越与战略整合

https://www.cnblogs.com/shanyou/p/19562239

本文探讨了.NET生态系统在生成式人工智能发展中的架构重构，强调AI代理作为软件组件的核心地位。微软提出的Microsoft Agent Framework(MAF)旨在解决开发者面临的工具链碎片化问题，并取代Semantic Kernel，成为统一的企业级平台。MAF与Semantic Kernel深度融合，标志着AI开发进入工业化阶段。微软承诺支持Semantic Kernel v1.x一年，同时推荐新项目使用MAF。这种演进反映了未来AI开发将基于标准化和可互操作的基类库扩展，而不再依赖孤立的SDK。整体上，文章清晰地分析了技术变革与工程实践的密切关联。

### 使用 NanUI 快速创建具有现代用户界面的 WinForm 应用程序

https://www.cnblogs.com/Can-daydayup/p/19571766

本文章介绍了NanUI，一个基于.NET的平台，用于为WinForm应用程序创建现代用户界面。NanUI利用HTML5、CSS3和JavaScript，通过Chromium Embedded Framework(CEF)实现富交互界面。它依赖于Xilium.CefGlue来转换CEF的C++ API为C#接口。文章详细描述了环境要求、项目源代码以及快速使用的方法，包括创建WinForm应用程序和安装所需的NuGet包。该框架适合开发现代化WinForm应用程序，具有良好的实践性和技术深度。

### 字符编码知多少(二)

https://www.cnblogs.com/lmy5215006/p/19567495

BOM头是Unicode编码标准中的字节顺序标记，用于标识字节顺序和编码格式。UTF-8引入BOM主要是为兼容ANSI编码。不同编码格式有各自的BOM字节序列。UTF-8无须BOM，因为其编码特性已解决大小端问题。UTF-16/32需要BOM来标识字节顺序，避免解析错误。UTF-8采用可变长编码，用1-4个字节表示Unicode字符，并通过指定的起始和续字节格式有效传输数据。

### MWGA 双线编译技术方案：一份代码，双端生成

https://www.cnblogs.com/xdesigner/p/19579270

MWGA技术解决了企业在桌面与网页端开发中的双重需求，采用模块化架构和跨平台编译引擎，实现了一份C#核心代码双向生成EXE与WebAssembly应用，确保逻辑统一和低维护成本。通过100%复用核心逻辑，显著提升研发效率，降低维护与迭代成本，同时规避业务风险。MWGA支持灵活部署，满足客户多样化需求，延长产品生命周期并提高竞争力，且无需重构核心代码即可快速实现Web化，适用于多个行业，包括工业、医疗和政务等。整体上，该技术提升了软件开发的便捷性与经济性。

### MAF快速入门(14)快速集成A2A Agent

https://www.cnblogs.com/edisontalk/p/-/quick-start-on-maf-chatper14

这篇文章介绍了如何在MAF中集成A2A协议，实现智能代理间的交流。A2A协议提供了标准的沟通方式，促进了不同平台间的无障碍协作。作者解释了将A2A Agent封装为Tool的方法，使得MAF中的代理能够像调用本地函数一样调用远程Agent。文章中包含了示例代码，展示了通过AgentFunctionHelper类创建功能工具的具体实现。这为读者提供了实用的技术深度和应用示例，促进了对多智能体协作的理解。

### 基于Ai Coding,20天完成一个基于大模型的医学分析系统：Ai体征分析助手

https://www.cnblogs.com/lsjwq/p/19577341

本文介绍了一名C#开发者利用AI Copilot在20天内独立开发医学分析系统的经历。作者强调AI工具在提高开发效率方面的优势，尤其是在需求变更和代码生成的过程中。AI Copilot帮助其快速生成前后端代码并减少开发周期。尽管AI提高了工作效率，但作者也警示普通工程师面临失业风险，因技术门槛被重新定义。对创新设计的需求增加，依然需要开发者具备扎实的编程基础和逻辑思维能力。本文总结了AI对软件开发带来的深远影响。

### 揭开 C#中的异步/等待：隐藏状态机

https://www.cnblogs.com/powertoolsteam/p/19563347

本文深入解析了C#中async和await关键字的底层机制，重点是编译器如何将异步方法转换为状态机结构。传统的同步I/O操作会导致线程阻塞，而async/await通过非阻塞操作解决了这一问题。C#编译器将标记为async的方法重写为实现IAsyncStateMachine接口的结构体，保持方法的线性结构。文中示例展示了编译器如何将DownloadDataAsync方法转化为状态机，生成存根方法以处理异步调用，实现任务的非阻塞执行和状态管理。相关技术细节清晰易懂，对C#开发者理解异步编程大有裨益。

### HagiCode 启动页设计：React 19 应用中填补 Hydration 空白期的极致体验

https://www.cnblogs.com/newbe36524/p/19572516

本文探讨了 HagiCode 项目中的启动体验设计，包含 12 种风格。HagiCode 基于 ASP.NET Core 10 和 React 19，强调前后端分离架构。为了解决用户在加载过程中的空白界面，提出了在 index.html 中内联代码的技术方案。通过设计高优先级的启动样式，降低了全局样式对启动页的影响，同时利用 CSS 的性能优势提升用户体验。文章还介绍了基于配置的渲染逻辑，使得不同风格的切换变得简单。这一解决方案体现了对性能与视觉的双重关注。

### AI 白嫖代码：中小型开发组织的开源困境与破局之道 —— Blazor WASM 与 MWGA 如何帮助中小团队在 AI 时代破局

https://www.cnblogs.com/xdesigner/p/19589317

在AI编程时代，大模型的无授权复用对中小型开发组织构成挑战，尤其是开源动力减退和技术选型变革。中小团队需划分闭源与开源区域并选择更严格的协议以保护自身利益。技术栈重构如Blazor WASM优先解决安全与开发效率问题，通过编译为Wasm，提升系统安全性。MWGA工具简化迁移，不需重写代码，支持双端生成，降低开发成本。C#的强类型特性有助于避免AI生成的错误代码。中小组织需与开源生态理性互动，推动高质量开源发展，实现AI时代的良性循环。

### C# 设置 Word 文档背景颜色/背景图

https://www.cnblogs.com/jazz-z/p/19565731

在.NET开发中，自动化处理Word文档的背景设置常见。Free Spire.Doc for .NET是无需依赖Microsoft Office的工具，实现文档创建和格式调整。文章首先介绍通过NuGet快速安装组件的方法。接着，讲解如何设置文档背景颜色，使用Document.Background属性指定颜色类型和具体颜色。完整代码示例演示了如何加载现有文档并保存修改。最后，介绍背景图片的设置方法，代码示例同样展示了如何加载图片并保存为新文档。此文具有实用性和技术深度。

### 基于 Starlight 文档站点接入 Microsoft Clarity 的完整实践指南

https://www.cnblogs.com/newbe36524/p/19577415

本文介绍了如何在 HagiCode 文档站点中接入 Microsoft Clarity，以洞察用户行为并确保隐私合规。作者分析了使用 Clarity 的必要性，尤其是其相较于 Google Analytics 的优点。文章详细讲解了代码如何动态加载 Clarity 脚本，同时考虑到不同环境的需求。通过这一整合，团队希望更好地理解用户的阅读习惯，提高文档的有效性。HagiCode 项目展现出通过数据统计提升用户体验的努力。

## 话题
### C# 与 Anders Hejlsberg 的 TypeScript 历史 | GitHub
https://www.youtube.com/watch?v=uMqx8NNT4xY

### 宣布winapp，Windows应用开发CLI
https://blogs.windows.com/windowsdeveloper/2026/01/22/announcing-winapp-the-windows-app-development-cli/

- [microsoft/winappCli：winapp，Windows 应用开发 CLI，是一个用于管理 Windows SDK、打包、生成应用身份、清单、证书的单一命令行界面， 以及使用任何应用框架的构建工具。](https://github.com/microsoft/WinAppCli)

### ReSharper 和 Rider 2025.3.2 更新现已发布！| .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/01/29/resharper-and-rider-2025-3-2/

### Visual Studio 一月更新 — 增强版编辑器体验 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-january-update-enhanced-editor-experience/

### .NET AI 基础——核心构建模块解析——.NET博客
https://devblogs.microsoft.com/dotnet/dotnet-ai-essentials-the-core-building-blocks-explained/

### Rider 2026.1抢先体验计划现已开放！ | .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/01/22/rider-2026-1-early-access-program-start/

### ReSharper 2026.1 抢先体验计划已启动 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/01/22/resharper-2026-1-early-access-program/

## 发布
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [3.7.1207.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1207.0)，[3.7.1208.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1208.0)，[3.7.1209。 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1209.0)， [3.7.1210.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1210.0)， [3.7.1211. 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1211.0)， [3.7.1212.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1212.0)， [3.7.1213. 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1213.0)， [4.0.175.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.175.0)， [4.0.176.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.176.0)， [4.0.177.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.177.0)， [4.0.178.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.178.0)， [4.0.179.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.179.0)， [4.0.180.0]( https://github.com/aws/aws-sdk-net/releases/tag/4.0.180.0)， [4.0.181.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.181.0)
- [Azure/azure-cosmos-dotnet-v3](https://github.com/Azure/azure-cosmos-dotnet-v3)
    - [3.57.0](https://github.com/Azure/azure-cosmos-dotnet-v3/releases/tag/3.57.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.Communication.CallAutomation_1.5.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Communication.CallAutomation_1.5.1)，[Azure.Core_1.51。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Core_1.51.0)， [Azure.Data.AppConfiguration_1.8.0]( https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Data.AppConfiguration_1.8.0)，[Azure.Monitor.OpenTelemetry.Exporter_1.6. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Monitor.OpenTelemetry.Exporter_1.6.0)，[Azure.ResourceManager.NetworkCloud_1.3。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.NetworkCloud_1.3.0)，[Azure.ResourceManager.PostgreSql_1.4。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.PostgreSql_1.4.0)， [System.ClientModel_1.9. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/System.ClientModel_1.9.0)
- [CommunityToolkit/Maui](https://github.com/CommunityToolkit/Maui)
    - [14.0.0](https://github.com/CommunityToolkit/Maui/releases/tag/14.0.0)、[6.0.0-camera](https://github.com/CommunityToolkit/Maui/releases/tag/6.0.0-camera)、[8.0. 0-mediaelement](https://github.com/CommunityToolkit/Maui/releases/tag/8.0.0-mediaelement)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.36.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.36.0)
- [domaindrivendev/Swashbuckle.AspNetCore](https://github.com/domaindrivendev/Swashbuckle.AspNetCore)
    - [v10.1.1](https://github.com/domaindrivendev/Swashbuckle.AspNetCore/releases/tag/v10.1.1)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.BackupDR.V1-2.8.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.BackupDR.V1-2.8.0)，[Google.Cloud.Container.V1-3.37。 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Container.V1-3.37.0)， [Google.Cloud.DevTools.ContainerAnalysis-3.13. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.DevTools.ContainerAnalysis-3.13.0) [Google.Cloud.Kms.V1-3.21.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Kms.V1-3.21.0)，[Google.Cloud.NetworkConnectivity.V1-2.14. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.NetworkConnectivity.V1-2.14.0)， [Google.Cloud.NetworkManagement.V1-2.18. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.NetworkManagement.V1-2.18.0)， [Google.Cloud.PubSub.V1-3.32. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.PubSub.V1-3.32.0)， [Google.Cloud.Storage.V1-4.14. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Storage.V1-4.14.0)
- [newrelic/newrelic-dotnet-agent](https://github.com/newrelic/newrelic-dotnet-agent)
    - [v10.48.1](https://github.com/newrelic/newrelic-dotnet-agent/releases/tag/v10.48.1)
- [开放遥测/开放遥测点网贡献](https://github.com/open-telemetry/opentelemetry-dotnet-contrib)
    - [Exporter.Geneva-1.15.0](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/Exporter.Geneva-1.15.0)，[Instrumentation.AspNet-1.15。 1](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/Instrumentation.AspNet-1.15.1)， [Instrumentation.SqlClient-1.15. 0](https://github.com/open-telemetry/opentelemetry-dotnet-contrib/releases/tag/Instrumentation.SqlClient-1.15.0)

## 文章、幻灯片及更多内容

### microsoft/dcp：开发者控制平面API服务器和CLI。
https://github.com/microsoft/dcp

- [开发者控制面板 - 源代码/许可澄清 · dotnet/aspire · 讨论#1913](https://github.com/dotnet/aspire/discussions/1913)

### .NET 10 和 C# 14 新增内容：多租户速率限制
https://blog.elmah.io/new-in-net-10-and-c-14-multi-tenant-rate-limiting/

### 确保CI/CD的网页无障碍 - axe DevTools × Playwright C# 实践指南
https://zenn.dev/tomokusaba/articles/035e696351e16d

### 在 ASP.NET Core 中使用 OpenID Connect、OAuth DPoP 和 OAuth 的客户端断言 PAR
https://damienbod.com/2026/02/02/use-client-assertions-in-asp-net-core-using-openid-connect-oauth-dpop-and-oauth-par/

### 用C#er、现代C#/来思考。 2026年初的.NET及LLM时代的挑战
https://zenn.dev/nossa/articles/12591dab29df30

### 如何同时对本地和NuGet的包处理进行基准测试
https://zenn.dev/prozolic/articles/4ecb9bd1d931d7

### 由MassTransit支持的事件驱动架构
https://zenn.dev/pksha/articles/18e25967d45855

### 绕过dotnet-trace的100堆帧限制
https://dfamonteiro.com/posts/dotnet-trace-100-limit/

### 利用 FusionCache 的背板同步多个实例之间的 HybridCache 实例
https://timdeschryver.dev/blog/hybridcache-sync-with-fusioncache-backplane

### 2025年游戏开发：游戏开发现状报告节选 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/01/29/game-dev-in-2025-excerpts-from-the-state-of-game-development-report/

### LLM 行为：HTTP 数据包确认
https://zenn.dev/yy7613/articles/b9c1de0c2f2616

### Will光标的新调试模式，是遗留代码的救星？ 我尝试用C# WinForms验证
https://zenn.dev/nexta_/articles/38f5e7fb61f4ab

### MCP in C#(新闻API集成)入门 - 移植《MCP入门》一书中的Python代码(5)
https://zenn.dev/zead/articles/mcp-learning-5

### 试试在Aspire 13中进行docker compose生成
https://zenn.dev/arika/articles/20260124-aspire-docker-compose-integration

### 源生成器技巧 (#1)：使用 IndentStringBuilder 进行代码整形
https://zenn.dev/arika/articles/20260201-source-generator-use-indentbuilder

### 使用 dotnet-trace 和 Perfetto 诊断 .NET 应用的性能问题
https://dfamonteiro.com/posts/using-dotnet-trace-with-perfetto/

### 加入Microsoft 2026 NDC London - 让我们共同打造.NET的未来 - .NET博客
https://devblogs.microsoft.com/dotnet/join-us-at-ndc-london-2026/

### 使用 System.Diagnostics.Metrics API 创建和使用指标：System.Diagnostics.Metrics API - 部分 1
https://andrewlock.net/creating-and-consuming-metrics-with-system-diagnostics-metrics-apis/

### EF Core 懒惰加载性能 抓到了
https://markheath.net/post/2026/1/8/efcore-lazy-loader-gotcha

### 用C#编写.NET垃圾回收器 - 第6部分：标记和清理
https://minidump.net/writing-a-net-gc-in-c-part-6/

### 修复了.NET 10 + VS Code(Copilot)中dotnet工作负载修复失败 - kkamegawa的博客
https://kkamegawa.hatenablog.jp/entry/2026/01/24/215747

## 今日人物

**理查德·曼宁·卡普**（英语：Richard Manning Karp，1935年1月3日—）是一名[美国](https://zh.wikipedia.org/wiki/美國)[计算机科学家](https://zh.wikipedia.org/wiki/計算機科學家)和[计算理论家](https://zh.wikipedia.org/wiki/計算理論)。他因在[计算理论](https://zh.wikipedia.org/wiki/計算理論)方面的研究而知名，并于1985年获得[图灵奖](https://zh.wikipedia.org/wiki/图灵奖)，2004年获得[本杰明·富兰克林计算机和认知科学奖](https://zh.wikipedia.org/wiki/富兰克林研究所奖项#本杰明·富兰克林奖章)，2008年获得[京都奖](https://zh.wikipedia.org/wiki/京都獎)[[2\]](https://zh.wikipedia.org/wiki/理查德·卡普#cite_note-2)。

由于在NP完备性的理论和应用、构建高效组合算法以及在计算机科学中应用概率方法方面的重大贡献，卡普于1992年获选为[美国国家工程院](https://zh.wikipedia.org/wiki/美国国家工程院)院士。

![理查德·曼宁·卡普](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/msSvOyOBepjS1a5yzaTKH_1536x1024_20260305_121027_raw.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

* 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
* .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
* 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。