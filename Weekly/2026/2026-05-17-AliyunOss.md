**C# .NET 周刊｜2026年5月3期 2026-05-17 dotnet_week_26_5_3**

## 国内文章

### 在 Avalonia 中编写高性能动画

https://www.cnblogs.com/BettaFish/p/20012355

文章介绍 Avalonia 中的合成动画。作者先示例常见的 XAML 动画，指出其运行在 UI 线程上，会被 Measure/Arrange 等操作卡顿影响。文中说明 Avalonia 11 引入合成渲染器与 Composition Animation。每个控件在 UI 线程上有 CompositionVisual，渲染线程上对应 ServerCompositionVisual。修改属性先作用于 CompositionVisual，再序列化到 ServerCompositionVisual，渲染器根据 ServerCompositionVisual 生成渲染指令并发送到后端(如 Skia、Vulkan)。作者指出官方资料稀少，需阅读源码才能深入理解。

### OpenHarmony.NET 停更事件复盘和思考

https://www.cnblogs.com/juziyu/p/20022301

文章复盘了布布的OpenHarmony .NET项目归档事件。作者梳理事实，指出布布将自己与Avalonia绑定并误解口头承诺，忽视法人招标与供应链合规。文章分析Avalonia作为商业样品的角色，华为/基金会因自主可控和合规要求启动招标并引入外包，这是合理的风险管控。作者警示开源开发者要重视书面合同、法人资质、合规审查与商业谈判，不要把中间方的口头承诺当成直接聘用保证。

### .NET 11 Preview 4 震撼发布：MAUI 抛弃 Mono，全量迁移 CoreCLR，性能与 NativeAOT 双炸场！

https://www.cnblogs.com/shenchuanchao/p/20043743/dotnet-11-preview-4-maui-coreclr-nativeaot

2026 年 .NET 11 Preview 4 将 CoreCLR 设为 Android、iOS、Mac Catalyst 和 tvOS 上 .NET MAUI 的默认运行时，结束了 Mono 在移动端长达 25 年的主导地位。文章回顾了 Mono 从 2001 年到 Xamarin 被微软收购的演进，强调 Mono 在 Unity、Avalonia、Uno、MonoGame 和 Godot 中的广泛影响。CoreCLR 统一运行时带来一致的 JIT、GC 与工具链。Blazor WebAssembly 仍使用 Mono。若遇问题，.NET 11 可回退到 Mono。NativeAOT 与运行时无关，提供极致的启动与体积优化。文章强调此举为 .NET 统一的重要里程碑。

### 高性能百度OCR ONNX Runtime C#实现

https://www.cnblogs.com/luoht/p/20026520

RapidOCRSharpOnnx 是基于 OpenCV 与 ONNX Runtime 的 C# 推理库。它重写并优化 RapidOCR，实现对多种 ONNX Runtime 执行提供程序的部署。支持直接导入 PP-OCR 模型，PP-OCRv5 可识别 106 种语言并离线运行。支持 CPU、CUDA/TensorRT、OpenVINO、CoreML、DirectML，支持批量与异步性能优化。使用 OpenCvSharp4 做图像处理，SkiaSharp 绘制结果，兼容 PP-OCRv4/v5。文档包含模型导出、NuGet 包安装与各执行提供程序的初始化示例。内容实用且实现细节较多，但示例末尾不完整，缺少性能基准和外部链接。

### 2026 年 .NET 客户端常用 MVVM 框架推荐

https://www.cnblogs.com/Can-daydayup/p/20012540

文章回顾2026年常见的.NET客户端MVVM框架，阐明MVVM将视图、视图模型和模型分离的作用。介绍CommunityToolkit.Mvvm的跨平台、模块化、按需取用特性并提供GitHub链接。说明Prism支持多平台、内置依赖注入与事件聚合，区分社区版与商业授权要求并给出许可证链接。文章开始介绍ReactiveUI，强调其响应式和函数式编程思想。整体实用且时新，适合选型参考，但缺少深度对比、性能或案例验证，部分段落未完结。

### 曝华为&quot;白嫖&quot;开源团队技术方案事件——网友评论总结

https://www.cnblogs.com/shanyou/p/20028083

2026年5月8日，独立开发者“布布”宣布其主导的 OpenHarmony.Avalonia 项目永久归档。该项目将 .NET 的跨平台 UI 框架 Avalonia 适配到鸿蒙系统，曾在 HDC 2025 展示成果。布布称项目在与 Avalonia 和华为沟通后转为闭源并暂停公开更新，随后发现中标方案与其开源 Demo 高度一致。多家媒体报道疑似外包公司中标相关适配项目。华为尚未就此事做出公开回应。事件引发社区对开源贡献、知识产权和采购流程的广泛讨论。

### .NET 11 Preview 4 正式发布：Runtime-Async 全面启用、Process API 大幅扩展

https://www.cnblogs.com/shanyou/p/20027731

本文梳理了 .NET 11 Preview 4 的核心改进。运行时全面启用 Runtime-Async，JIT 增加常量折叠优化并支持 1024+ CPU。类库引入一组高阶 Process API(如 Process.Run/RunAsync、RunAndCaptureText 等)，显著简化子进程启动与输出捕获。新增基于 Span 的 Deflate/ZLib/GZip 压缩 API，减少中间分配。新增浮点数十六进制格式化与解析。System.Text.Json 持续优化。SDK 在 dotnet watch、Fish Shell 和 OpenTelemetry 上改进。C# 改善 Shebang 诊断并提供可选编译缓存。ASP.NET Core 在 OpenAPI、Blazor 电路管理和模板方面增强。EF Core 增加向量搜索与 JSON 映射集成。

### AI 开发狂飙！.NET 11 Preview 4 原生集成向量搜索 + MCP 模板，EF Core 直接对标 RAG 应用

https://www.cnblogs.com/shenchuanchao/p/20060331/dotnet-11-preview-4-vector-search-mcp-template-ef-core-rag

.NET 11 Preview 4 在 ASP.NET Core AI 集成和 EF Core 向量搜索上带来关键改进。EF Core 原生支持 SqlVector<float> 与相似度查询，配合 SQL Server 存储嵌入，直接赋能 RAG 场景。MCP Server 模板为模型调用提供标准化方案。文章解释向量检索原理、EF Core 演进和示例代码，并指出用 IEmbeddingGenerator 生成嵌入。内容实用且具时效性，对构建 AI 原生 .NET 应用提供明确技术路径。

### C# ESP32/STM32 轻量 Web 能力库：PicoServer.Nano

https://www.cnblogs.com/juziyu/p/20059639

文章介绍 .NET nanoFramework 及作者的 PicoServer.Nano 项目。它在 MCU 上运行精简的 .NET，允许在 ESP32/STM32 用 C# 提供轻量 Web 服务。PicoServer.Nano 不用反射，减少内存和 CPU 占用，支持路由、中间件、Token 认证、静态文件托管、SSE 与文件上传下载等功能。文中给出 ESP32 快速上手命令和示例代码，并在 ESP32-S3 上做并发性能测试：并发6时无 PSRAM QPS≈8、有 PSRAM QPS≈26，平均延迟≈210–220ms，成功率100%。作者比较了 ESP32 与 STM32 的场景并强调一致的 C# 开发体验。文章末尾注意事项部分被截断。

### C#/.NET/.NET Core技术前沿周刊 | 第 70 期(2026年5.01-5.10)

https://www.cnblogs.com/Can-daydayup/p/20026493

C#/.NET周刊汇总近期生态动态与实用文章。内容涵盖2026年常用MVVM框架选型、基于C#的Windows优化工具Winhance、Copilot Studio在.NET 10上提升的WASM性能、Microsoft Agent Framework的持久化工作流与AI Agent构建块等。每条均附原文链接并鼓励投稿与交流。

### .NET 8 Web开发入门(四)：注入燃料——Entity Framework Core 与 Code First 实战

https://www.cnblogs.com/shenchuanchao/p/20035907/dotnet-8-web-development-part4-entity-framework-core-code-first

文章介绍如何用 EF Core 将内存数据持久化到数据库。先解释 ORM 概念，再给出安装 Microsoft.EntityFrameworkCore.SqlServer 与 Design 包的命令。定义了 TodoItem 实体，说明 Id、Title、IsDone、CreatedAt 等属性及为何用 class。展示了 AppDbContext 的实现、DbSet 用法和 OnModelCreating 的可选配置。内容实用且示例清晰，适合入门。文章未展开迁移、连接字符串和依赖注入的完整配置，缺少更多生产环境注意事项与引用。

### .NET 与鸿蒙的“技术巧遇”

https://www.cnblogs.com/juziyu/p/20046749

文章指出 .NET 与鸿蒙在 linux-musl 上实现技术交汇。微软在 RID 中支持 linux-musl，并通过 NativeAOT 预编译生成符合 C ABI 的 musl 格式 .so，便于在轻量 Linux 环境运行。鸿蒙采用并定制 musl，提供动态库延迟加载和命名空间隔离以兼容并优化 musl 动态库。两者依赖 Linux 与 musl 开源社区的长期贡献。开发者可直接用 .NET 编译出可被鸿蒙通过 dlopen 调用的 .so。文中列出 PublishAotCross、华为云验证等参考资料，并比较了其他跨平台框架的适配进展。

### OpenClaw.NET 外部 CLI 预设系统：从零编写第三方 CLI 集成指南

https://www.cnblogs.com/shanyou/p/20047683

文章基于 OpenClaw.NET(clawdotnet/openclaw.net，commit 113151c7)，系统讲解 External CLI Preset 的架构与扩展方法，并以 Terraform CLI 演示完整自定义预设开发流程。文章从手动配置过渡到预设即代码，分析手写 appsettings.json 中 Connectors 与逐条 ArgsTemplate 的繁琐与错误风险。作者展示了 GitHub CLI 的配置示例，说明预设系统如何在保证安全基线下压缩复杂配置、提升可维护性与复用性。文章技术性强，重点实用，适合希望将 CLI 工具安全接入 AI 网关的开发者。

### C# 基础入门指南：从零开始学习 C# 编程

https://www.cnblogs.com/token-ai/p/20020485

文章介绍了C#及其应用场景，如桌面、Web(ASP.NET)、游戏、移动和云服务。说明了开发环境搭建步骤，包括下载 .NET SDK 和验证命令，列出常用 IDE：Visual Studio、VS Code、Rider。演示了创建和运行第一个控制台程序的完整命令和示例代码。概述了基本语法：变量与类型、var 推断、常量、字符串操作与 if-else 控制流。内容适合入门，技术深度有限且未提供引用，末尾示例被截断。

### NuGet下载量数据分析与.NET生态全景观察：从数据洞察技术演进

https://www.cnblogs.com/shanyou/p/20018119

本文基于AI与NuGet官方实时统计，沿增长轨迹、热门包生态、技术驱动、社区活跃与未来展望五个维度，系统解析NuGet周下载量自2019年约3亿增至2026年2月约54亿的原因。文章指出.NET Core将BCL拆分为大量NuGet包，令NuGet从可选工具变为基础设施，从而放大下载量与开发活动的映射。方法结合MVP张善友的纵向分析与nuget.org实时数据交叉验证，覆盖2019–2026年并关联版本发布、LTS策略、Native AOT与AI集成等驱动因素。作者以周下载量、TOP10包排行、Stack Overflow与GitHub数据评估生态健康并提出中短期演进判断。

### 数据去重：通过 C# 删除 Excel 中的重复行

https://www.cnblogs.com/jazz-z/p/20029050

本文介绍用 Free Spire.XLS for .NET 和 C# 编程删除 Excel 中的重复行。文章按步骤说明安装库、加载工作簿、确定数据范围、按 A 列 DisplayedText 分组、保留每组首行、收集重复行号并从后向前删除、最后保存结果。示例用 LINQ 简洁实现，实用且可直接运行。文章缺少异常处理、大文件性能优化、多列判重示例和参考链接。总体步骤清晰、可复现，但原创性与引用较弱。

### .NET 8 Web开发入门(三)：解构引擎——依赖注入(DI)与中间件管道

https://www.cnblogs.com/shenchuanchao/p/20008775/dotnet-8-web-development-part3-dependency-injection-middleware

文章为系列第三篇，讲解ASP.NET Core中的依赖注入与中间件。作者先说明为何用DI以消除紧耦合并便于测试。文中详解三种服务生命周期：Transient、Scoped、Singleton，并强调Scoped适用于单次HTTP请求。作者以性能监控为例，展示接口、实现和在Program.cs中以Scoped注册的实践。写作通俗易懂，适合初中级读者入门。文章有实战价值但中间件部分未展开，且未提供参考来源。

### AScript之匿名类型与动态类型

https://www.cnblogs.com/rockey627/p/20058232

文章介绍AScript开源C#动态脚本引擎中两种特殊数据类型：匿名类型和动态类型。匿名类型在编译时确定结构且属性只读，示例展示通过Script.AnonymousTypes和AnonymousTypeManager获取并在LINQ查询中使用。动态类型采用ExpandoObject，允许运行时添加属性，示例展示初始化器和动态赋值两种用法。文章附上源码仓库链接以便查阅实现细节。

### MewUI 项目：面向 NativeAOT 的超轻量级.NET GUI 架构、底层图形管线与性能演进

https://www.cnblogs.com/shanyou/p/20064719

MewUI是社区驱动的实验性.NET GUI框架，优先支持NativeAOT和Trimming。它用托管自绘引擎和双重抽象消除外部原生库依赖，将单文件体积分至3–4MB。框架舍弃WPF复杂样式与反射绑定，采用Fluent C#链式声明和强类型ObservableValue绑定。项目采用模块化、低耦合架构以便裁剪。文章横向比较了WinForms、WPF、Avalonia与MewUI，分析兼容性、体积、渲染引擎与依赖隔离等要点。该方案技术原创且及时，但仍为原型，实用性和生态成熟度有待验证。

### AnyDrop 一款自部署的内容共享工具

https://www.cnblogs.com/kop-elan/p/20065325

AnyDrop 是基于 .NET 10 与 Blazor 的自托管跨设备内容共享应用。它通过 SignalR 实时同步文字、图片、视频、任意文件与链接预览。功能包含主题分组、全文搜索、阅后即焚和归档。认证使用 JWT+Cookie，数据存储在 SQLite(EF Core)，界面用 Tailwind。项目提供 Docker Compose 与源码运行两种部署方式，并给出环境变量与启动步骤。文档实用，部署指引清晰，但技术深度与外部引用有限。

### 【EF Core】继承策略——TPH

https://www.cnblogs.com/tcjiaan/p/20061618

文章解释了 EF Core 的三种继承映射策略：TPH、TPT、TPC。TPH 将整个继承链映射到单表，并通过额外列区分类型。TPT 为每个类型建表，派生表只存自身字段，基类字段存基类表。TPC 为每个具体类型建表，派生表复制基类字段。文中以 BaseType 与 DeriveType 为例演示 OnModelCreating 配置，指出应在基类上调用 ToTable 与 HasKey，派生类仅注册实体。作者强调在 TPH 中不得在派生类配置表名或主键，否则会报错。

### 【Azure Developer】ASP.NET Framework 4.8 集成 Azure Application Insights SDK 完整指南

https://www.cnblogs.com/lulight/p/20055306

本文介绍在 ASP.NET Framework 4.8 项目中集成 Azure Application Insights SDK 的步骤与要点。作者建议使用 Microsoft.ApplicationInsights.Web 2.23.0，并说明该包自动引入的核心组件，包括 TelemetryClient、HTTP 自动追踪、依赖项追踪、性能计数器和分布式追踪关联。操作步骤包含在 Visual Studio 中通过 Install-Package 安装该 NuGet 包，并在生成的 ApplicationInsights.config 中配置 Connection String，文内给出中国区示例。文章实用且直接，但存在 HTML 实体残留，缺少具体代码示例和引用支持。

### AScript如何实现LINQ语法

https://www.cnblogs.com/rockey627/p/20065217

AScript 是开源的 C# 动态脚本解析执行引擎，支持自定义语法扩展。文章说明 LINQ 语句被编译为对 Queryable/Enumerable 扩展方法的调用，AScript 通过 AddFunc 注入这些方法并生成对应方法调用。示例展示在脚本中对 EF/SQLite 上的上下文执行 join 和 left join 并生成 SQL。实现要点是定义 QueryNode 节点以管理 from/where/join/group/orderby/select，维护变量父子关系并在编译或执行时构造表达式。内容对引擎开发者实用，但缺乏外部引用和更完整的实现细节。

### Git实战覆盖98%日常开发场景

https://www.cnblogs.com/yuxl01/p/19928139

文章用Visual Studio和SourceTree演示团队常用Git操作。覆盖创建分支、删除分支、合并分支、解决冲突、储藏(stash)、回滚等步骤。作者以.NET开发者视角用VS演示，同时兼顾其他语言。文中详细说明在两款工具中的具体点击与选项，讲解三方合并界面与冲突处理策略，建议新手避免轻易使用rebase。部分截图打马赛克但不影响理解。作者提供视频索取渠道。整体面向企业日常开发，实用性强，适合非命令行用户快速上手。

### 用ANTLR实现表达式词法和语法分析器

https://www.cnblogs.com/rrooyy/p/20040014

文章说明易元平台表达式需求与解析演进。旧方案用C#正则实现词法分析并给出源码，存在性能问题和对转义、负号等高级语法支持不足。新方案采用ANTLR生成器，平台使用3.1版本，并提到4.x更易用。文章展示问题与迁移方向，但缺少ANTLR语法示例、性能对比与测试细节。

### C#如何优雅处理引用类型的深拷贝

https://www.cnblogs.com/lmy5215006/p/20058060

文章讲解 C# 中浅拷贝與深拷贝差异。作者用真实故障引入场景，指出未深拷贝会导致原件被意外修改。说明 ICloneable 只有 Clone()，不保证浅或深拷贝，需由实现者决定。提供浅拷贝示例展示引用共享导致 Address 被同时修改。提供深拷贝示例展示对引用类型字段逐层 Clone，从而使副本与原件独立。文章实用且代码直观，但未涉及循环引用处理、性能或序列化等替代方案，也缺少引用文献或标准链接。

### 【Azure Relay】记录使用Azure Relay在通信中遇见侦听器(Listener)或发送端(Sender)断开时的异常日志 (Hybrid Connection by Websocket)

https://www.cnblogs.com/lulight/p/20064536

文章介绍Azure Relay中继原理及用HybridConnectionListener和HybridConnectionClient实现Listener与Caller的单对单通信。阐述网关创建中继、请求查找与转发、临时通道建立及消息双向转发流程。复现场景显示当Caller突然中断时，Listener日志会记录Microsoft.Azure.Relay.RelayException，内含System.Net.WebSockets.WebSocketException，提示远端在未完成关闭握手前关闭了WebSocket。作者说明若不捕获该异常，Listener进程会崩溃并退出。文章实用且流程清晰，但缺少异常处理建议和参考来源。

### .Net基于NetCoreKevin框架 AI 与 Hangfire 集成：实现AI智能自动任务调度

https://www.cnblogs.com/net-kevin-li/p/20056384

本文介绍在 NetCoreKevin 框架中将 AI 与 Hangfire 集成，实现智能周期任务调度。框架采用前后端分离，内置 RAG 检索增强、知识库与技能集成，并提供 HTTP、Python、Shell 等工具。架构分为 AI 工具层、任务服务接口 IKevinAITasksService 及基于 Hangfire 的 KevinAITasksService。KevinAITasksService 注入 IRecurringJobManager 与 JobStorage，使用 RunTask 执行并可接入 AI 处理。文中说明了 Hangfire 的 NuGet 安装、Startup/Program 注册示例与示意调用流程。源码托管于 GitHub 与 Gitee，适用于定时生成报告、数据同步和内容总结等自动化场景。

### OpenCode 对接实践：从独立进程到共享 Runtime 的架构演进

https://www.cnblogs.com/newbe36524/p/20012511

本文复盘 HagiCode 集成 OpenCode 的全流程实践与架构演进。项目从每会话独立进程切换到系统级共享 runtime，由 OpenCodeRuntimeCoordinator 管理启动、健康检查和重建。Provider 层通过 OpenCodeCliProvider 实现 IAIProvider 接口。使用 MonoSpecs 配置仓库，采用 plain Git 和 scripts/clone-repos.mjs 管理克隆。会话绑定持久化到 SQLite，保存 CessionId 与 OpenCode SessionId 映射以支持恢复。错误恢复由 ProviderErrorAutoRetryCoordinator 和 OpenCodeRetryableTerminalFailureClassifier 实现自动重试。还遇到 400 BadRequest 因外部端点复用缺少上下文导致失败。文章提供真实踩坑与设计决策供参考。

---

## 国际周报

**国际周报未更新**

## 今日人物

**道格拉斯·恩格尔巴特**(英语：Douglas Carl Engelbart，1925年1月30日—2013年7月2日)，美国工程师、发明家和人机交互先驱。他领导的研究团队发明了鼠标，并推动了超文本、群件、网络计算机和交互式计算的发展。1968年的“所有演示之母”集中展示了鼠标、窗口、超文本、视频会议和协同编辑等后来深刻影响个人计算的技术。

1997年，恩格尔巴特因“提出了交互式计算的未来愿景，并发明了帮助实现这一愿景的关键技术”获得图灵奖。

![道格拉斯·恩格尔巴特](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/douglas-engelbart.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

- 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
- .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
- 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。