**C# .NET 周刊｜2026年6月3期 2026-06-21 dotnet_week_26_6_3**

## 国内文章
### 5年，一个程序员是如何把私有化在线客服系统做到第一名的

https://www.cnblogs.com/sheng_chao/p/20627166

作者为独立开发者，五年持续维护升讯威在线客服与营销系统。近期签下大客户，经历近三个月的技术评估与压力测试。客户要求私有化无后门证明、压测在其环境中直接抽取性能数据、服务器带宽计算依据、OpenAPI 对接与合规验证等。作者使用 dotnet-counters 监测性能。项目数据包括 Docker 拉取 3.8K、私有化包 1211 次下载和近 2400 万次会话。作者强调先保证产品稳定可靠，再追求易用性与口碑。文中批评了一些不以用户为先的产品设计做法。

### .NET 程序在装有企业防水墙的电脑上运行报错：内存不足

https://www.cnblogs.com/zhuweisky/p/20629887

客户在Win10上运行傲瑞通时，点击联系人无法打开聊天窗口。排查发现企业防水墙将程序目录下PNG文件加密，Image.FromFile读取被修改的PNG时，GDI+抛出“内存不足”误导性错误。取消对图片文件夹的加密后，图标正常加载，程序恢复。根因是防水墙改写PNG二进制头，导致非标准图片文件被GDI+识别失败。建议把程序资源目录设为不加密或在程序中加入解密处理以避免此类异常。此问题涉及.NET的System.Drawing/GDI+图片解析。

### 终于！我造了个「AI代驾」级别的AutoBuilder，一键干掉80%的重复CRUD工作

https://www.cnblogs.com/weipt/p/20535238

AutoBuilder 是一款三合一生产力工具。它支持 MySQL、SQL Server、PostgreSQL 和 Oracle。它可一键生成实体、Repository、Service、Controller 并带 Swagger 注解。它能反向生成完整数据库设计文档并从 Swagger JSON 自动生成接口文档。示例以 C#/.NET 为主，兼容 ADO.NET 与 EF Core，代码模板可扩展并遵循 Clean Architecture。后续计划支持自定义模板、Java/Go 版本、Docker 部署和前端 CRUD 生成。该工具旨在消除重复劳动，加速项目启动与重构。

### C#摸鱼实录——IoC与DI案例详解

https://www.cnblogs.com/leaf-7-scouts/p/20633961

文章聚焦IoC与DI的实用用法。作者摒弃学院派冗长概念，强调能用就行。文中定义依赖、注入与依赖注入，配以C#示例代码。示例对比了直接new导致的强耦合与通过构造注入实现的松耦合。作者提到常见三种注入方式并以构造注入为主，但代码在中途截断。文末推荐了一个.NET依赖注入的视频教学。语气随意，偏实战与个人经验分享。

### C#实现控制台交互式操作

https://www.cnblogs.com/wucy/p/20469788/csharp-console-op

文章比较传统CLI与现代实时交互CLI，聚焦列表菜单与确认框两种终端组件。作者用C# Console实现动态选择界面，给出菜单数据与核心方法ShowSelectionMenu，并解释通过Console.ReadKey、光标隐藏与重绘实现上下键切换与回车确认。示例简洁可复用，适合Agent CLI场景开发。

### [MAF预定义的AIContextProvider-01]TextSearchProvider——RAG在MAF中的实现

https://www.cnblogs.com/artech/p/20585633/ai-context-provider-01

文章介绍ChatClientAgent作为核心AIAgent，构建与LLM交互的中间件管道。通过输入增强和输出增强改善模型输出。AIContextProvider集合位于管道中间，专门用于输入/输出增强。RAG被描述为典型的输入增强，并通过TextSearchProvider实现。文中先给出无RAG的OpenAI示例，说明模型因知识固化无法回答实时问题；再说明在AsAIAgent时添加TextSearchProvider并用SearchAsync注入相关新闻以实现RAG。示例基于OpenAIClient和MAF框架，但代码命名与实现细节需完善。

### kestrel 的 ssl 行为分析

https://www.cnblogs.com/kewei/p/20578940

作者在项目中用 CYarp 将 Kestrel 作为对外网关。更新 SSL 后浏览器正常但客户端设备无法信任证书。用 openssl 对比发现 Kestrel 返回的证书链缺一节，而 Nginx 正常。排查后作者发现 Kestrel 仅在 Endpoint+PEM 情形下能正确读取证书链，Default 配置或 PFX 情形存在缺陷，导致 https.ServerCertificateChain 为 null。作者通过手动设置 ServerCertificateChain 作为临时解决，并引用了 ASP.NET Core 的相关 issue 以说明该行为不一致的 BUG。

### [MAF预定义ChatClient中间件-09]MessageInjectingChatClient-赋予工具消息注入的能力

https://www.cnblogs.com/artech/p/20527914/chat-client-pipeline-09

文章说明MAF中ReAct循环由FunctionInvokingChatClient驱动，AIFunction结果被封装为角色为Tool的ChatMessage并加入对话历史，无法像LangChain工具返回结构化Command。作者演示通过MessageInjectingChatClient让工具在执行中注入Assistant消息以提示风险。示例为TransferMoney工具：从AIAgent.CurrentRunContext读取Session，若Session.StateBag未标记UserConfirmed，工具注入要求短信验证码的Assistant消息并返回已提交缓冲区的提示。示例展示了用OpenAIClient构建支持消息注入和AIFunction的Agent流程。

### OpenClaw.NET 上线 MetaSkills ：软件工程第一性原理的工业级实践

https://www.cnblogs.com/shanyou/p/20584467

文章以 OpenClaw.NET 的 MetaSkills PR 为例，基于 Fred Brooks 的《没有银弹》拆解软件三类复杂性。作者说明偶然困难通过抽象屏蔽，列举 HardenFilterAllowlist、依赖感知 DAG 引擎、Checkpoint 和 LLM 路由抽象如何简化底层细节。作者认为社会学困难可借开源与透明文档打破，突出 SKILL.md、迁移对照与 MIT 许可带来的可审计性。作者承认本质困难不可消除，主张用抽象释放认知带宽以正面应对并发与非确定性问题。文章结合具体 PR 展示实践价值与工程思路。

### OpenClaw.NET 重大更新：Goal 机制登场，让 AI Agent 不再"半途而废"

https://www.cnblogs.com/shanyou/p/20642014

OpenClaw.NET 推出会话级持久化 Goal 机制，解决大语言模型在多步骤任务中常“半途而废”的问题。该机制以六状态状态机为核心，配合 Token 预算、自动续跑引擎和智能阻塞检测，自动评估目标完成度并在必要时注入续跑提示。系统支持暂停、恢复、完成与阻塞状态，并在 CLI/TUI 中实时展示进度与状态。相关改动在 PR #154 中新增约 3,994 行代码和 16 个核心文件，覆盖数据模型、服务层、运行时集成与界面展示。该机制增强了 Agent 的自动化能力和可观测性，适用于复杂工程类任务场景。

### [MAF预定义的AIContextProvider-02]AgentSkillsProvider——将Agent Skills引入MAF

https://www.cnblogs.com/artech/p/20615379/ai-conext-provider-02

文章介绍Agent Skills概念，给出translator技能的Markdown定义与C#示例代码，展示AgentSkillsProvider与OpenAI客户端的整合。示例实用且易复现，有助快速上手。文章技术深度适中，但缺乏架构细节、性能、容错与安全讨论。表达总体清晰，可读性良好。原创性一般，紧跟LLM相关技术趋势。文章未提供引用或外部链接，影响可信度。

### 装了 30 个 Skills 之后，我才搞清楚哪些是在白浪费 context

https://www.cnblogs.com/uniqueDong/p/20534635

三个月前我把34个Skills装进~/.claude/skills/。Claude Code变聪明但变慢，经常触发无关Skill并浪费token。周末我研究四大Awesome仓库，把34减到11，加载更快且行为更可控。文章给出可用的过滤框架，指出生态巨大但质量参差：agentskillreport显示22% Skills未通过基本验证，52% token为非功能性文件。文中比较四大仓库定位，强调VoltAgent严格策展、适合与工具深度整合，并举出Microsoft按语言细分的.NET相关Skills。antigravity规模最大，提供Bundle和installer，便于按角色一键安装。文章侧重实用筛选和性能优化建议。

### OpenClaw.NET 祭出 TokenJuice：Agent 时代的"Token 瘦身引擎"，让 LLM 上下文不再膨胀

https://www.cnblogs.com/shanyou/p/20657325

文章描绘了夜间生产故障中 AI Agent 导致的 Token 泄露问题。它列举了 ANSI 码、冗余构建清单、重复进度行和完整 HTML 等噪音类型，分析了对话历史中 Token 二次方增长的成本。介绍了 OpenClaw.NET 与社区提交的 TokenJuice PR(21 次提交，+9555/-1469 行，276 文件)，目标是在送入 LLM 前用确定性规则压缩工具输出。TokenJuice 以 IToolResultInterceptor 插件形式运行，按规则过滤与精简日志，保留关键信息以显著降低 Token 消耗并提升响应速度。文章实践价值高且实现细节明确，但缺少外部评测数据与引用。

### [MAF预定义的AIContextProvider-03]ChatHistoryMemoryProvider——赋予Agent从经验中学习的能力

https://www.cnblogs.com/artech/p/20661262/ai-context-provider-03

本文指出LLM本身无状态，难以支持持续学习与演化，因而需要为Agent赋予记忆。短期记忆以Session实现多轮对话能力，长期记忆实现跨Session的信息共享，范围可面向用户、Agent或系统。作为AIContextProvider派生类，ChatHistoryMemoryProvider可按不同Scope保存对话历史，并在后续对话中作为上下文供Agent使用，从而实现基于经验的学习。文章给出C#示例，使用Azure OpenAI嵌入与InMemoryVectorStore，将用户偏好存入名为user_preference的向量集合，配合GetMenu和PlaceOrder工具实现个性化点餐。示例展示了在.NET环境中为Agent构建记忆的基本做法。

### 从 OpenClaw.NET 的 /loop 实现，看 Loop Engineering 如何从概念走向工程实践

https://www.cnblogs.com/shanyou/p/20666509

文章以 OpenClaw.NET 的 /loop PR 为例，解析 Loop Engineering 的技术本质。作者指出该 PR 用 1,033 行代码、11 个文件和 62 个通过的测试，实现了定时循环提示词注入，支持 '/loop 5m check CI status' 之类的命令。文章将 Agent Loop 定义为 Thought→Action→Observation 循环，强调模型在循环中自主决策。作者回顾了演进脉络：ReAct、AutoGPT、Agent SDK 到 Loop Engineering。文章将 Loop 抽象为公式：Cron(定时触发)+ 决策器(LLM)。作者认为 Loop 把人设为循环作者、把模型当子程序运行，强调真实工程实现胜过概念炒作。

### Microsoft Agent Framework 1.0 正式接棒，.NET AI 进入 Agent-Native 时代

https://www.cnblogs.com/shanyou/p/20681353

本文报道了2026年4月3日 Microsoft Agent Framework (MAF) 1.0 GA 发布，并指出 Semantic Kernel 1.77.0 已通过 PR 完成向 MAF 的迁移。文章解析了 MAF 的五层架构：Service Connectors、Abstractions、Kernel、Agent、Orchestration。作者说明 SK 的插件、提示词模板和向量存储功能被保留并作为基础层重定位，而原有的 Agent 抽象被 AIAgent 和 WorkflowBuilder 取代。文中提醒 AutoGen 与 SK 已进入维护模式，建议开发者将新功能与编排能力集中迁移到 MAF，以避免技术债务并利用跨语言企业级平台优势。

### HagiCode 中 AI 提交使用的提示词：设计思路与实现拆解

https://www.cnblogs.com/newbe36524/p/20666681

本文介绍 HagiCode 的 AI 提交提示词设计与实现。作者指出把未提交改动交给 AI 会遇到作者/提交者错误、风格不符、误推主干等问题。HagiCode 将提示词拆为 Handlebars 模板与 JSON 元数据。JSON 描述参数 schema，模板负责文本表述。每个 locale 使用独立的 .hbs/.json，以便本地化和示例定制。团队由 Scriban 迁移到 Handlebars.Net 提升性能，并兼顾布尔输出兼容性。该方案增强了前端自动渲染、参数化配置和提交安全性。文章实践性强但引用不足。

### 用 Orleans 搞定 AI 编程工作台的后台分布式难题

https://www.cnblogs.com/newbe36524/p/20681196

本文基于 HagiCode 项目，描述在单进程后台管理多种 AI CLI 工具与大量长周期会话时的分布式与状态管理难题。作者比较了无状态+Redis、Dapr/Akka.NET 与 Microsoft Orleans 三种选型，指出 Redis 带来序列化与锁复杂度，Dapr 的 sidecar 不适合桌面部署，Akka.NET 对长生命周期持久化支持不足。文章阐述 Orleans Virtual Actor 的自动激活/回收、IAsyncEnumerable 原生流式支持、[AlwaysInterleave] 与 [ResponseTimeout] 等特性如何简化并发、超时、流式输出和状态管理，从而在 HagiCode 场景中降低实现复杂度与运维成本。文章实战性强但缺少外部引用与性能数据。

### Pi Agent 对接实现：消息解析、重试与取消

https://www.cnblogs.com/newbe36524/p/20645406

本文讨论将 Pi CLI AI agent 接入 HagiCode 的实现。作者指出三大难点：私有事件流解析、失败重试语义和可中断长任务取消。架构拆为两层：底层 Hagicode.Libs 提供 ICliProvider，将 CLI 输出归一化为 CliMessage；上层 hagicode-core 提供 IAIProvider，将业务请求翻译为 provider 参数并输出流式 chunk。关键组件有 PiJsonEventMapper、归档式重试方案与 CliProcessManager。文章基于真实项目代码，说明了职责划分与实践权衡，提供可复用的对接策略。

### 【YFIOs】用C#开发硬件之设备上云

https://www.cnblogs.com/yefanqiu/p/20557501

本文以完整项目 YeFanIoTTest 展示如何将 YF3300-ESP32S3 通过 YFLink 协议经 MQTT 上传到叶帆物联网平台。文中列出所需 nanoFramework NuGet 包及版本，并说明各包功能，如 WiFi、MQTT、I2C、SHT30 传感器、Web 配网和日志。文章给出设备系统架构图，涵盖传感器、继电器、GPIO、驱动层与管理层。内容实用且工程导向，但缺少示例代码与外部引用，技术细节可更深入。

### OpenClaw.NET MetaSKILLs 系统深度解析：AI Agent 正在学会「自己给自己写技能」

https://www.cnblogs.com/shanyou/p/20614913

文章介绍了 OpenClaw.NET 在 PR #152 中新增的 MetaSkills 系统。作者以因重复加载技能说明导致 API 账单暴涨的场景开头。MetaSkill 将多个子 Skill 打包为可复用的工作流模板，下次只需调用模板即可按序触发技能、传参并处理异常。系统选用 Jinja2(.NET 移植版)描述流程。MetaSkill 可被复用、修改并能生成新 MetaSkill，具备自举能力。文章用乐高比喻其价值，并概述了五大核心模块，重点解决技能组织与上下文代价问题。


---

## 国际周报

## 话题

### C# Kaigi 2026 #csharpkaigi - fortee.jp
https://fortee.jp/csharpkaigi-2026/speaker/proposal/cfp

### 发布 3.0.0 · StackExchange/StackExchange.Redis
https://github.com/StackExchange/StackExchange.Redis/releases/tag/3.0.0

### AI驱动的MSBuild调查，使用Microsoft Binlog MCP服务器 - .NET博客
https://devblogs.microsoft.com/dotnet/msbuild-binlog-mcp-server/

### Windows 应用开发 CLI v0.3.2 — 捆绑支持、更智能初始化等 - #ifdef 窗户
https://devblogs.microsoft.com/ifdef-windows/windows-app-development-cli-v0-3-2-bundling-support-smarter-initialization-and-more/

### 通过包ID标准加强NuGet安全· 第75期 · NuGet/公告
https://github.com/NuGet/Announcements/issues/75

### 在不离开 Visual Studio - Visual Studio 博客的情况下审核拉取请求
https://devblogs.microsoft.com/visualstudio/review-pull-requests-without-leaving-visual-studio/

## 发布
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [4.0.268.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.268.0)、[4.0.269.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.269.0)、[4.0.270。 0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.270.0)， [4.0.271.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.271.0)， [4.0.272.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.272.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.ResourceManager.DataBox_1.1.2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataBox_1.1.2)，[Azure.ResourceManager.Dynatrace_ 1.2.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Dynatrace_1.2.1)，[Azure.ResourceManager.Elastic_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Elastic_1.1.1)，[Azure.ResourceManager.ElasticSan_1.2。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ElasticSan_1.2.1)，[Azure.ResourceManager.FrontDoor_1.4。 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.FrontDoor_1.4.2)，[Azure.ResourceManager.HealthBot_1.3。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.HealthBot_1.3.0)，[Azure.ResourceManager.IotFirmwareDefense_1.1。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.IotFirmwareDefense_1.1.1)，[Azure.ResourceManager.IotOperations_1.1。 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.IotOperations_1.1.0)，[Azure.ResourceManager.Kusto_1.6。 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Kusto_1.6.3)，[Azure.ResourceManager.MachineLearning_1.2。 4](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.MachineLearning_1.2.4)， [Azure.ResourceManager.Monitor.PipelineGroups_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Monitor.PipelineGroups_1.0.0)， [Azure.ResourceManager.Monitor.Workspaces_1.0. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Monitor.Workspaces_1.0.0)，[Azure.ResourceManager.MySql_1.2。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.MySql_1.2.1)，[Azure.ResourceManager.NetApp_1.16。 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.NetApp_1.16.1)，[Azure.ResourceManager.StorageMover_1.4. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.StorageMover_1.4.1)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.46.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.46.0)
- [dotnet/Orleans](https://github.com/dotnet/orleans)
    - [v10.2.0](https://github.com/dotnet/orleans/releases/tag/v10.2.0)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.AlloyDb.V1-1.15.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.AlloyDb.V1-1.15.0)， [Google.Cloud.Bigtable.V2-3.29. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Bigtable.V2-3.29.0)， [Google.Cloud.ConfidentialComputing.V1-1.12. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.ConfidentialComputing.V1-1.12.0)， [Google.Cloud.Firestore-4.3. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Firestore-4.3.0)， [Google.Cloud.OracleDatabase.V1-1.6. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.OracleDatabase.V1-1.6.0) [Google.Cloud.PubSub.V1-3.36.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.PubSub.V1-3.36.0)
- [微软/Aspire](https://github.com/microsoft/aspire)
    - [v13.4.4-release](https://github.com/microsoft/aspire/releases/tag/v13.4.4-release)， [v13.4.5](https://github.com/microsoft/aspire/releases/tag/v13.4.5)
- [microsoft/CsWin32](https://github.com/microsoft/CsWin32)
    - [v0.3.287](https://github.com/microsoft/CsWin32/releases/tag/v0.3.287)， [v0.3.296](https://github.com/microsoft/CsWin32/releases/tag/v0.3.296)
- [spectreconsole/spectre.console](https://github.com/spectreconsole/spectre.console)
    - [0.57.0](https://github.com/spectreconsole/spectre.console/releases/tag/0.57.0)
- [StackExchange/StackExchange.Redis](https://github.com/StackExchange/StackExchange.Redis)
    - [3.0.0](https://github.com/StackExchange/StackExchange.Redis/releases/tag/3.0.0)

## 文物、幻灯片等
### 你的JetBrains IDE专长现已登陆LinkedIn - JetBrains博客
https://blog.jetbrains.com/blog/2026/06/17/your-jetbrains-ide-expertise-now-on-linkedin/

### 即使在阿瓦洛尼亚UI 12 - Qiita也没有所有权证栏窗口
https://qiita.com/mifumi323/items/5aedc2c0abba3b7d302e

### 设计制造现场设备检查系统以提升Blazor能力的故事
https://zenn.dev/jodycraft/articles/65deec95c1b734

### CountAsync() 真的有必要吗？—— 搜索限制检查的替代方案 - Qiita
https://qiita.com/vayaci/items/da84f952ad73a420fdd9

### 让Visual Studio呈现你想要的样子 - Visual Studio博客
https://devblogs.microsoft.com/visualstudio/make-visual-studio-look-the-way-you-want/

### 你的第一个 Microsoft.UI.Reactor 应用
https://xaml.dev/post/your-first-microsoft-ui-reactor-app

### 当你无法用 netframework 构建 TUnit(net462 - net48)时的文章 - Qiita
https://qiita.com/juner/items/12800023c87eca4e5aba

### 我没有Mac，但用GitHub Actions生成macOS通用二进制文件
https://zenn.dev/j_sakamoto/articles/bd847ab518ec3c

### 试用GA GitHub Copilot SDK(.NET)
https://zenn.dev/microsoft/articles/github-copilot-sdk-dotnet-ga

### 2026年6月 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2026/06/12/dotinsights-june-2026/

### C# 和内存安全中的指针：Span vs. C# 16 unsafe - NDepend 博客
https://blog.ndepend.com/pointers-in-c-and-memory-safety-span-vs-c-16-unsafe/

### 我如何写出一个BGP服务器却没有失去理智
https://dev.to/vhex/how-i-wrote-a-bgp-server-and-didn't-lose-my-mind-16fc

## 库、仓库、工具等
### 快速失败 - Visual Studio 市场
https://marketplace.visualstudio.com/items?itemName=MadsKristensen.FailFast

---

## 今日人物

**罗纳德·李维斯特**(英语：Ronald Linn Rivest，1947年5月6日—)、**阿迪·萨莫尔**(英语：Adi Shamir，1952年7月6日—)与**伦纳德·阿德曼**(英语：Leonard Max Adleman，1945年12月31日—)，分别是美国、以色列和美国的密码学家与计算机科学家。他们共同发明 RSA 公钥密码系统，使安全密钥交换、数字签名和互联网加密通信得以广泛应用。

2002年，李维斯特、萨莫尔与阿德曼因“以巧妙贡献使公钥密码学在实践中可用”共同获得图灵奖。

![罗纳德·李维斯特、阿迪·萨莫尔与伦纳德·阿德曼](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/rsa-inventors.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

- 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
- .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
- 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。
