**C# .NET 周刊｜2026年7月1期 2026-07-05 dotnet_week_26_7_1**

## 国内文章
### .NET 10 的正则性能现在什么水平？我拿它和 Go、Python、C++、PCRE2 测了一轮

https://www.cnblogs.com/sdcb/p/21057904/dotnet-regex-perf

作者为原文补上 .NET 对比，把测试开源并用合成数据保证可复现。数据为约1GB、4.6M行的JSON字符串，约5%命中，固定种子。测试了10种实现，包括MSVC/GCC std::regex、PCRE2(含JIT)、Python、Go，以及.NET 的 Plain、Compiled、GeneratedRegex 和 NonBacktracking。结果显示在此数据集上 .NET 10 的 GeneratedRegex 最快。作者强调结论受合成数据和单一模式影响，故有限制，且公开了代码和数据生成脚本以便复现和扩展。

### 在 .NET 上构建超大托管数组

https://www.cnblogs.com/hez2010/p/20979630/build-a-very-large-array-in-dotnet

文章解析 .NET 数组受 int 限制的问题，提出 BigArray<T> 方案。作者用 .NET 8 的 InlineArrayAttribute 把每个物理元素做成固定内联块，从而扩展逻辑元素数量。方案支持引用类型、连续托管内存、由 GC 管理并兼容 NativeAOT。文章列出实现细节与权衡，指出块大小受值类型 65535 字节限制。论述技术性强且实用，缺少外部引用与性能实测。

### 一套基于 .NET 10 + Vue 3 构建、高颜值、前后端分离的企业级多租户中后台管理系统

https://www.cnblogs.com/Can-daydayup/p/20958904

XiHan.BasicApp 是一套开源(MIT)的 .NET 10 + Vue 3 企业级多租户中后台管理系统。后端遵循 DDD 与 CQRS，应用服务通过动态 API 暴露为 REST。系统内置完整的身份认证、RBAC+ABAC 权限、多租户管理、代码生成、审计日志与系统设置。前端采用 Vue 3 + TypeScript，提供移动端友好界面和现代 UI。项目强调高性能、模块化、跨平台与可扩展性，适合作为 B2B SaaS 与 .NET+Vue 全栈实践的起点。

### 《HelloGitHub》第 123 期

https://www.cnblogs.com/xueweihan/p/20898733

HelloGitHub 是一个每月更新的开源项目合集。它精选 GitHub 上有趣且入门友好的项目，覆盖 C、C#、C++、Go、JavaScript 等语言。示例包括 Linux 键位映射工具 keyd、轻量 TLS 库 mbedtls、C# 桌面便签 PaperTodo、体素引擎 luanti、老旧平板手写笔记 SpeedyNote、古诗词 API、斗地主终端游戏、团队密码管理器 gopass、零代码认证 tinyauth、无服务 CMS emdash 和前端文件管理 r2-web。文章实用且分类清晰，便于快速选取学习或使用的项目。

### Winform 能用 Native AOT 吗？—TDS 项目实战尝试

https://www.cnblogs.com/luojin765/p/20959578

文章记录将中等复杂度的 WinForms 项目 TDS 迁移到 .NET Native AOT 的实战。作者说明 AOT 的限制，如不支持 Assembly.LoadFile、System.Reflection.Emit 等，并提到 SDK 抛出的 NETSDK1175 警告。改动包括升级到 net10.0-windows、开启 PublishAot，并用 SuppresswinformTrimError 跳过 SDK 拦截。最终生成约 20MB 的单文件 exe，大多数功能可用，COM 支持是主要短板。作者认为对小工具很适合，但不建议直接用于生产环境。

### .NET 8 与 .NET 9 支持终止倒计时：开发者需要了解什么

https://www.cnblogs.com/shenchuanchao/p/21064641/dotnet-8-9-end-of-support-countdown-november-2026

文章译自微软公告，指出 .NET 8 与 .NET 9 将于 2026-11-10 同时终止支持。文章说明 .NET 8 为 LTS、本应三年支持却与 STS 的 .NET 9 对齐，微软建议升级到 .NET 10(LTS，支持至 2028-11)。作者认为对齐简化管理但削弱 LTS 含金量，并可能推动更快迁移。文章警示安全、合规及依赖链风险，并建议尽快评估和迁移以规避风险。作者呼吁提供更平滑的升级路径或延长 LTS 支持以减轻版本疲劳。

### C# GeneratedRegex：面向对象语言的"底层性能突围

https://www.cnblogs.com/shanyou/p/21098868

文章论证在需编译期代码生成、底层内存控制与向量化场景中，C# 是唯一在语言、运行时与编译器层面同时提供完整支持的面向对象语言。以 .NET GeneratedRegex 为例，编译期把正则生成为 C# 代码，消除解释器开销并获得 JIT/AOT 优化。文章列出 SIMD、缓存行对齐、分支预测与零拷贝等优化维度。文章比较 C#/Java/Go/C++/Rust 能力，强调 C# 的 struct、`Span<T>` 与 Source Generators 可实现零分配的高性能抽象。论述技术性强且及时，但缺乏引用支持。

### 当 AI 不再只是"说话"：OpenClaw.NET 率先原生支持 MCP Apps

https://www.cnblogs.com/shanyou/p/20943627

MCP Apps 是 Anthropic 于 2026 年发布的 MCP 扩展，允许工具返回可嵌入对话窗口的交互式 UI。MCP Server 提供前端资源并注册工具，Host 在客户端创建 iframe 并中转所有通信，View 在 iframe 内渲染界面并反向调用 Server。设计采用渐进增强，不支持渲染的客户端仍接收纯文本。OpenClaw.NET 在 PR #168 为 .NET 率先实现原生 MCP App 支持，推动 .NET 开发者构建可交互的 AI 仪表盘。架构强调安全性和可审计性。

### 基于Blazor实现的光伏设备调试软件

https://www.cnblogs.com/known/p/20979852

文章介绍基于 Blazor WebAssembly 和 .NET 10 的纯浏览器端光伏跟踪支架调试工具。软件通过 Web Bluetooth 在浏览器建立 BLE GATT 连接，并以 Modbus RTU over BLE 完成参数读写与控制。架构列出运行时、前端框架、存储、PWA 打包与主要服务实现(蓝牙封装、Modbus、设备管理、主题与本地化)。采用单页应用与动态组件切换不同产品页面，支持无安装、跨平台和浏览器即用。文中给出设备连接流程与 Service UUID 等实现细节。总体技术实用且及时，但部分实现细节与引用不足。

### WebSocket 快速入门教程(附示例源码)

https://www.cnblogs.com/shenchuanchao/p/20932272/websocket-quick-start-tutorial-source-code

本文系统介绍 WebSocket 原理、握手与数据帧格式，并演示浏览器前端 API。文章提供 C# 服务端三种实现(ASP.NET Core、Fleck、HttpListener)，包含心跳、重连与安全扩展。作者附完整源码，便于快速构建实时应用。技术深度与工程实用性较高，但引用不足，原创性一般。

### .NET CORE 认证模块-Cookie、JWT 与自定义 Scheme

https://www.cnblogs.com/yuxl01/p/20679054

文章讨论在不构建身份认证中心时采用 Cookie 与 JWT 的取舍。文中建议系统性学习 OIDC 与 OAuth2.0。详细比较了无状态与有状态 Cookie 认证的流程、优缺点和部署影响。指出 .NET Core 默认使用无状态 Cookie，解释服务端不存会话的特性以及有状态会话在踢人、即时撤销场景的必要性。并给出在 Program 中注册身份认证服务及配置 DefaultAuthenticateScheme、DefaultChallengeScheme 和 RequireAuthenticatedSignIn 的实现思路，提示在需要时可切换为会话存储以应对 Cookie 大小或强制下线需求。

### AI 时代的设备所见即用

https://www.cnblogs.com/lindexi/p/20943982

作者设想让个人AI助手直接操控任意设备。通过在设备上预装一个名为“设备连接器”的程序，实现靠近即连、无配对、自动发现与能力声明。连接器向AI提供设备身份与能力清单，执行AI下发的结构化指令或本地Agent理解自然语言并执行。说明书会随使用累积经验动态更新，支持OTA场景适配与异常恢复。设备端采用C# .NET跨平台实现，AI端先做薄壳验证并逐场景落地。目标是让用户只需与自己的AI对话，由AI替用户处理设备操作与故障恢复。

### 我变成了 AI 的打字猴子——以及我为什么写了一个禁止 AI 写代码的工具

https://www.cnblogs.com/daibitx/p/21146747

作者讲述让 AI 代写 C# 代码导致生产线死锁的真实案例。系统为 C# 后台服务，使用 System.Threading.Channels、OPC UA 回调和 SqlBulkCopy。急停触发大量传感器并发写入，Channel 被写满，OPC 回调线程在 WaitToWriteAsync 同步重试阻塞，OPC 会话断开，消费者永远等待，导致死锁和人工抄单。作者指出 AI 能拼出语法正确的代码，但无法理解执行模型和系统语义。作者因此变成“按 Tab 的打字猴子”，丧失对代码的掌控与手感。

### 你的 AI Agent 会在服务器上"修仙"——OpenClaw.NET 长持久会话技术解读

https://www.cnblogs.com/shanyou/p/21127247

文章指出当前大多数 AI Agent 采用无状态架构，导致会话重启即丢失。OpenClaw.NET 的 PR #174 引入完整的 Agent 生命周期管理，包含热路径缓存与冷路径持久化、后台执行、启动自愈、检查点和 Token 审计等机制。核心设计是“会话是状态，不是线程”，SessionManager 将执行上下文与会话数据解耦，内存用 ConcurrentDictionary 做热缓存，未命中则通过 IMemoryStore(默认 SQLite)双检锁加载回内存并按 LastActiveAt 淘汰。该方案提升持久性与并发性能，但 SQLite 在多实例下写锁成瓶颈，生产环境建议换 PostgreSQL 或 MySQL。

### 在Visual Studio里用原版Copilot交互，烧DeepSeek等国模的Token，让微软和深度求索都为你打工

https://www.cnblogs.com/egreen/p/21136292

作者分享一个能在 Visual Studio 中替换 Copilot 后端模型的工具。作者指出 Copilot 模型选择少且费用高，因此开发了一个开箱即用的工具，保持原版 Copilot 的交互体验但可切换为国产模型如 DeepSeek、千问、GLM、MiniMax 等，只要模型兼容 OpenAI 接口即可接入。工具专为 VS 和 WinForm/WPF 开发者设计，配置简单免费，作者承诺持续维护并提供下载与QQ群 390485182。作者邀请 C# WinForm 开发者试用并反馈。

### 远程部署工具ZEQP-PSDeploy

https://www.cnblogs.com/liuju150/p/21146087/ZEQP-PSDeploy

该项目提供基于PowerShell的一键部署工具。它通过PSSession远程连接服务器，支持HTTP(5985)和HTTPS(5986)并演示Get-Credential与ConvertTo-SecureString用法。安装只需git clone并以管理员运行Install.ps1。工具可自动编译并发布到远程IIS站点或Windows服务，示例包含dotnet publish(net8.0)和node yarn构建命令。还支持直接同步文件并可压缩传输。主要命令包括Start-DeployIIS、Start-DeploySvc和Start-DeployFile。仓库示例清晰，适合CI/CD和运维自动化部署场景。

### Surging AI Agent 完整产品介绍

https://www.cnblogs.com/fanliang11/p/20980032

本文介绍AgentForge(DevAgent)，一款深度集成Surging微服务引擎的本地.NET智能体。它通过engine-cli提供自然语言问答并输出结构化JSON配置。它能全自动执行微服务流水线：生成模块、编译、部署。实现基于C#的LLamaSharp离线推理，进程内存约5.5G，适配政务和金融内网场景。文中给出DevAgentSupportProvider示例，展示插件挂载、RAG知识库和多智能体提示词注册。技术细节明确且实用，但缺乏外部引用和性能对比数据。

### 淘宝的木鱼小程序下架后，我自己用 uniapp 写了一个

https://www.cnblogs.com/farb/p/21132879

作者九年后回归，复盘独立开发“睡眠木鱼”产品。因淘宝小程序下架且不支持后台播放，作者用 uni-app 3.0(Vue3+TS)实现微信小程序与 Android App，后端选用熟悉的 ASP.NET Core + Kestrel 提高开发效率。文章详细列出 uni-app 在音频后台播放、API 差异、BackgroundAudioManager 与 InnerAudioContext 冲突、安卓需前台服务保活、低端机解码问题及 MP3/OGG 双格式策略等实战坑。作者实现统一 AudioManager、事件总线状态管理和对象存储音频，强调真机早测与包体大小限制等上架要点。产品已覆盖微信小程序和 Android，iOS/鸿蒙在研。


---

## 国际周报

## 话题

### SkiaSharp 4.0 来了：宣布首个稳定版本 - .NET 博客
https://devblogs.microsoft.com/dotnet/skiasharp-4-0-stable/

- [宣布SkiaSharp 4.0](https://platform.uno/blog/announcing-skiasharp-4-0/)

### WSL容器现已公开预览
https://devblogs.microsoft.com/commandline/wsl-container-is-now-available-for-public-preview/

### Visual Studio 六月更新 - 跟踪使用情况，信任你的工具 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-june-update-track-your-usage-trust-your-tools/

### .NET 8 和 .NET 9 将于 2026 年 11 月 10 日结束支持 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-8-9-end-of-support/

## 精选
### Kaigi 2026 in C# 招标(讨论)现已开放
https://fortee.jp/csharpkaigi-2026/speaker/proposal/cfp

我们现正接受[C# Kaigi 2026](https://csharpkaigi.net/)的提案征集(CfP)，该活动将于2026年9月19日星期六在台场的docomo R&D OPEN LAB举行。 直到2026年7月5日星期日。

## 发布
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [4.0.277.0](https://github.com/aws/aws-sdk-net/releases/tag/4.0.277.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.ResourceManager.NetApp_1.17.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.NetApp_1.17.0)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.48.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.48.0)
- [dotnet/诊断](https://github.com/dotnet/diagnostics)
    - [v10.0.731102](https://github.com/dotnet/diagnostics/releases/tag/v10.0.731102)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.Datastore.V1-5.2.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Datastore.V1-5.2.0)， [Google.Cloud.Dialogflow.V2-4.31. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Dialogflow.V2-4.31.0)， [Google.Cloud.NetworkManagement.V1-2.21. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.NetworkManagement.V1-2.21.0)， [Google.Cloud.Tools.SecretManagerHelper-1.0. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Tools.SecretManagerHelper-1.0.0)
- [StackExchange/StackExchange.Redis](https://github.com/StackExchange/StackExchange.Redis)
    - [3.0.11](https://github.com/StackExchange/StackExchange.Redis/releases/tag/3.0.11)

## 文物、幻灯片等
### 当我试图用纯WASM读取Access文件时，Codex让我“停下”。
https://zenn.dev/clavisflow/articles/dd31102c818910

### Wasm 移动事件源源：尝试 C# 和 Rust 域代码
https://zenn.dev/jtechjapan_pub/articles/sekiban-wasm-runtime-public-container

### 在 Microsoft Agent Framework 中尝试 LoopAgent
https://zenn.dev/yy7613/articles/6baa8e35e1df54

### 如何用MassTransit Saga应对事件驱动的比赛条件
https://zenn.dev/pksha/articles/2088c13ac89ca6

### 封闭类层级：探索 .NET 11 预览版 - 第四部分
https://andrewlock.net/exploring-the-dotnet-11-preview-4-closed-class-hierarchies/

### MCP 超越聊天窗口：在 CI 中构建诊断 - .NET 博客
https://devblogs.microsoft.com/dotnet/mcp-build-diagnostics-workflows/

### 让继承的控制器路由在 ASP.NET 核心中工作
https://weblog.west-wind.com/posts/2026/Jun/30/Getting-Inherited-Controller-Routes-to-work-in-ASPNET-Core

### ReactiveProperty.R3 已发布
https://zenn.dev/okazuki/articles/reactiveproperty-r3-overview

### 尝试在GitHub Copilot应用的画布上显示 ASP.NET Core Blazor WASM
https://zenn.dev/microsoft/articles/ghc-app-canvas-blazor

### 尝试使用 Microsoft Agent Framework 与本地 LLM 第16部分(持久实体状态)
https://zenn.dev/yy7613/articles/d15b00c266c36d

### 使用 Aspire 构建本地后台验证环境
https://zenn.dev/ryoku4/articles/ad4ff452832bbf

### Microsoft 代理框架中的代理技能介绍——从 C# 学习实现模式示例
https://zenn.dev/microsoft/articles/agentframework-agentskill-01

### 用C#编写.NET垃圾回收器 - 第10部分：终结者
https://minidump.net/writing-a-net-gc-in-c-part-10/

### Windows上使用WinApp CLI的.NET应用打包和包身份 - .NET博客
https://devblogs.microsoft.com/dotnet/packaging-dotnet-apps-winapp/

### 用 .NET 创建大型托管数组 - Qiita
https://qiita.com/hez2010/items/a464dc85421c5360d818

### [Blazor + Syncfusion] 关于在 SfDialog - Qiita 中创建删除确认对话的想法
https://qiita.com/af-dev-hub/items/9dd635b1ec0a006f1598

### 用 GitHub Actions 自动化你的 Visual Studio 扩展构建 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/automating-your-visual-studio-extension-builds-with-github-actions/
### 迁移中的C# - Microsoft代理框架 | 杰西·利伯蒂
https://jesseliberty.com/2026/06/28/migrating-c-microsoft-agent-framework/

### 创建双用途的 Windows 图形界面和控制台应用程序
https://weblog.west-wind.com/posts/2026/Jun/23/Creating-Dual-Use-Windows-GUI-and-Console-Applications

## 库、仓库、工具等
### GitHub - actbit/AstFirst
https://github.com/actbit/AstFirst

- [[C#] 仅通过写类创建语言 — 解析器生成器 AstFirst 介绍 (1) 制作科学计算器 - Qiita](https://qiita.com/Binary_number/items/6997bfe07fe74ae33bef)

---

## 今日人物

**文特·瑟夫**(英语：Vinton Gray Cerf，1943年6月23日—)与**罗伯特·卡恩**(英语：Robert Elliot Kahn，1938年12月23日—)，是美国计算机科学家和互联网架构先驱。他们共同设计 TCP/IP，确立不同计算机网络互联的核心机制，为现代互联网奠定技术基础。

2004年，瑟夫与卡恩因“在互联网互联领域的开创性工作，包括设计和实现互联网基础通信协议 TCP/IP，并在网络领域发挥卓越领导作用”共同获得图灵奖。

![文特·瑟夫与罗伯特·卡恩](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/cerf-kahn.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

- 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
- .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
- 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。
