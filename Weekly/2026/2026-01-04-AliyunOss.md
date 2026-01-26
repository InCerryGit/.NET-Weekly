## 国内文章
### 2026年，让.NET再次伟大

https://www.cnblogs.com/msdeveloper/p/19427679/make-dotnet-great-again-2026

文章探讨了将.NET SDK纳入操作系统的战略意义，认为这将推动开发生态的变革。.NET 10支持单文件运行，降低了开发门槛，提高了运行效率。文章列举了多种应用场景，以及各类开发语言生态的工具链现状。强调通过集成.NET SDK，Windows和Linux将变得更加开发者友好，从而促进.NET的普及和使用。文章提供了清晰的逻辑和具体的案例，突显了.NET的统一性和高效性。总之，文章在技术深度和实用性方面具有很高的价值。

### 所有64位WinForm应用都是Chromium浏览器（2）

https://www.cnblogs.com/sunhui/p/19415298

该文章介绍了如何将WinForm应用与Chromium浏览器结合。通过实现Chromium Tab Group绑定，WinForm窗体中的控件可以动态与Web页面交互。文章强调，使用DHTML和Javascript技术，开发者可以实现动态内容生成。Creator Runtime作为无主进程的Chromium浏览器，允许WinForm应用以浏览进程的方式运行，具备多进程架构。这种结合赋予WinForm应用新的能力，拓展了Web生态系统的边界。

### 从 ABP 到 CleanDDD：关于软件长期演进的一些思考

https://www.cnblogs.com/aishangyipiyema/p/19425837

本文探讨了CleanDDD相较于ABP在软件长期演进中的优势。作者指出，现代系统不仅要快速交付，还要易于维护和演进。CleanDDD通过集中业务规则、明确层次结构、优化代码维护，降低了人员流动带来的风险。它关注系统在多次需求变更后仍能稳定运行，强调了结构清晰、模块边界明确的重要性。此外，CleanDDD提高了开发效率，适应AI编码需求。文章指出ABP适合快速交付，但在长期项目中可能面临架构老化等问题。总体上，这是一次对软件架构深刻的反思和对比。

### 让WinForms再次伟大

https://www.cnblogs.com/xdesigner/p/19438384/Make_WinForms_Great_Again

全球约有300万至500万WinForms开发者，60%至80%的应用需现代化改造，其中40%至60%优先选择Web化迁移。Blazor WebAssembly因可重用C#代码和跨平台能力而受欢迎。许多WinForms应用依赖GDI+进行复杂绘图，迁移时需重写较多代码，导致企业面临高成本风险。本项目旨在将WinForms应用迁移到Blazor平台，降低修改量至10%以内，从而降低成本和风险。全球待迁移市场估算规模在275亿至1,100亿美元之间。

### Slickflow.NET 工作流引擎关于AI大模型的应用实践

https://www.cnblogs.com/slickflow/p/19424636

Slickflow.NET 是一个基于 .NET 的开源工作流引擎，3.5.0 版本引入 AI 大模型能力，具有文生流程图、图片分类识别和 RAG 增强检索三大特性。文生流程图允许用户用自然语言生成符合 BPMN 2.0 的流程图，显著降低设计门槛。技术实现依赖通义千问，核心在于系统提示词设计，以确保 AI 准确理解需求并生成目标输出。通过 BpmnApiClient 类，系统与大模型 API 交互，实现请求构建和响应处理，确保功能高效可靠。这些创新为工作流引擎应用带来了革命性变化。

### 如何设计易维护、低学习成本的飞书.NET SDK组件

https://www.cnblogs.com/mudtools/p/19426326

本文探讨如何通过特性驱动架构和编译时代码生成，实现易于维护、低学习成本的企业级HTTP API。强调设计理念的重要性，指出逻辑清晰和风险可控是维护的核心。通过源代码生成，减少样板代码，提升开发效率。提出关注点分离原则，确保业务逻辑与HTTP通信解耦，并且支持模块化集成。文章结构清晰，涵盖架构设计理念、核心特性实现、服务注册架构等内容，便于读者理解和应用这些技术。

### 基于SqlSugar开发框架的基础上快速开发H5端的移动应用

https://www.cnblogs.com/wuhuacong/p/19420561

本文介绍了基于SqlSugar开发框架实现快速开发H5端移动应用的过程。文章首先强调了数据库设计的重要性，规范命名和字段使用有助于管理。接着，文章讨论了使用代码生成工具提高开发效率，生成后端基础代码和整合项目文件。最后，讨论了Vant4与Vue3结合的H5前端开发，强调该框架轻量且可定制，适合移动端应用开发。整体内容对开发者有实用参考价值。

### 字符编码知多少(一)

https://www.cnblogs.com/lmy5215006/p/19000023

这篇文章深入探讨了字符编码的历史与演变。从最初的ASCII编码开始，到ISO 8859-1，再到GB2312等多字节字符编码，作者揭示了每种编码的优缺点。ASCII只能表示有限的英文字符，无法满足其他语言需求。为解决这一问题，各国制定了本地化编码，如GB2312与GBK，旨在覆盖更多汉字。文章通过代码示例展示了不同编码的实际效果，特别是编码不匹配时出现的乱码问题。作者强调了编码混乱带来的国际化困难，提出了对兼容性的关注。整体内容详实，适合技术人员参考。

### 【踩坑】Roslyn 5与VS2022——不散的红色浪线

https://www.cnblogs.com/oberon-zjt0806/p/19429665

本文讨论了Visual Studio 2022与Roslyn 5.0的兼容性问题，重点提到IntelliSense在构建过程中可能无法正常工作。若要在Visual Studio中使用代码分析服务，需确保NuGet包Microsoft.CodeAnalysis的版本为4.x。博文中还给出了解决MSBuild错误的方法，包括关闭有误文件并重新生成解决方案。接着，作者介绍了源代码生成器的基本用法，给出了具体代码示例，内容涉及如何创建一个简单的生成器，以及如何配置项目。

### CodeSpirit 开发环境搭建及启动指南

https://www.cnblogs.com/codelove/p/19392132

本指南提供了搭建CodeSpirit低代码框架开发环境的步骤，支持Windows、macOS和Linux操作系统。安装需要.NET 10 SDK、Visual Studio 2026或VS Code以及Docker Desktop。文中详细说明了如何下载和安装这些工具，并通过Git克隆CodeSpirit项目。在项目启动阶段，Aspire自动管理依赖服务，包括MySQL、Redis、RabbitMQ、GreptimeDB和Seq，用户仅需进入相应目录运行应用即可。这一过程简单明了，适合开发者快速上手。文章更新至2025年12月，确保信息的时效性。

### 【译】Visual Studio —— 为现代开发的速度而打造

https://www.cnblogs.com/MeteorSeed/p/19417404

Visual Studio 2026 代表微软在开发工具领域的重大进步，通过每月和年度更新提升了软件开发的持续性和可靠性。新IDE支持快速创新，提供高兼容性以保证项目顺利运行，同时支持多种构建工具和组件，允许团队根据自身需求选择更新节奏。Insiders 和 Stable 频道为用户提供了体验新功能的机会和稳定版本的更新，确保用户能够获得最新技术和支持，而不影响现有环境的运行。这一新方法旨在让开发者在稳定和创新之间找到平衡，推动现代化开发进程。

### 如何在.NET系统中快速集成飞书任务分配能力

https://www.cnblogs.com/mudtools/p/19415554

文章探讨了企业在数字化转型中面临的挑战，以及通过飞书等工具实现跨部门协作的必要性。传统系统往往导致信息孤岛，沟通效率低下，任务进展不明。而飞书API为传统系统提供了连接，提升了实时性与协作性，支持企业快速整合信息，优化工作流程。强调了.NET平台可靠性，适合企业级集成。通过实际案例，揭示了传统工单系统中的信息传递困境，强调推进协作的重要性与工具支持的价值。

### PowerDotNet平台化软件架构设计与实现系列（18）：商品管理平台

https://www.cnblogs.com/jeffwongishandsome/p/goods-platform-design-and-implement.html

该文章探讨电子商务核心的商品系统，分享了个人对PowerDotNet重写商品平台的经验。作者强调了商品管理的重要性，随着电商发展的复杂性，商品系统设计变得愈加重要。文章回顾了多个电商业务类型与个人在商品管理方面的积累。还分析了AI工具在代码优化中的作用，指出良好设计依赖扎实编码基础。作者分享了商品概念界定的复杂性，尤其在多个相关系统之间的整合。整体上，文章具备深度与实用性。

### Perigon.CLI 10.0 重磅发布【AspNetCore开发模板和辅助工具】

https://www.cnblogs.com/msdeveloper/p/19430150/perigon-10-announce

Perigon.CLI 10.0正式发布，旨在提升开发者的生产力和开发体验。它围绕Aspire/AspNetCore/EF Core等技术栈，提供项目脚手架、代码生成器及命令行工具。新版本的操作界面由Angular改为Blazer server，项目结构更加简化，增加了多租户、多数据库及多语言支持。未来将集中于提升生产力、性能和生态，计划每年更新，鼓励社区参与。官方文档提供使用指南。

### MAF快速入门（9）多路分支路由工作流

https://www.cnblogs.com/edisontalk/p/-/quick-start-on-maf-chatper09

本文详细介绍了在MAF中使用switch-case实现多分支路由的技巧。针对现实工作中多个决策条件的需求，作者通过企业内部邮件检测案例展示了如何利用switch-case增强代码的可维护性。文章通过示例代码对比了传统的if-else与switch-case的接口使用方法，强调了后者在新增分类时的便利性。此外，文章还提供了.NET控制台应用程序的准备工作和API配置，以便读者进行实践。这篇文章适合希望提升MAF开发技能的开发者。

### CodeSpirit 多语言国际化使用指南（Beta）

https://www.cnblogs.com/codelove/p/19417730

CodeSpirit 框架支持前后端多语言国际化，提供中英文双语功能，应用于 .NET 资源文件与 AMIS locale。其特性包括双语支持、系统多级配置、类型安全和动态切换。通过 Settings 组件，用户可无缝切换语言，且无需修改数据库结构。快速开始部分说明如何在 Controller 中使用本地化服务，包括抛出本地化异常及 DTO 的多语言验证特性。这一更新显著提高了应用的可用性，增强了用户体验。

### 【译】Copilot Profiler Agent —— 分析任务交由 AI，应用性能不受影响

https://www.cnblogs.com/MeteorSeed/p/19434707

Visual Studio 2026发布了Copilot Profiler Agent，帮助分析和优化代码性能。它结合了GitHub Copilot的功能与性能分析器，支持自然语言提问，识别热点路径，发现优化机会。文章通过对CsvHelper开源项目的基准测试演示其功能。用户可以通过Copilot生成基准测试，Copilot会询问安装分析器的NuGet包，并根据已有基准测试生成新模型。此外，用户可对测试进行调整，实现性能改进。

### MAF快速入门（10）循环工作流

https://www.cnblogs.com/edisontalk/p/-/quick-start-on-maf-chatper10

本文介绍了在MAF中实现循环与自我修正工作流的方法。通过构建“生成→审核→修复”的闭环，确保AI产出的内容符合企业质量标准。文中使用了WorkflowBuilder来添加循环边，并以电商客服中心为案例，展示了自动迭代的工作流配置。其中提到的关键依赖包包括Microsoft.Agents.AI.OpenAI等。此外，定义了数据传输模型，使得质检结果能结构化输出。整体思路清晰，案例实用，适合买家进行学习和应用。

### Serilog 日志库简单实践（四）消息队列 Sinks（.net8）

https://www.cnblogs.com/hnzhengfy/p/19191039/Serilog_MQSinks

本文介绍了Serilog日志库的消息队列Sinks及其实践，尤其侧重于Kafka和RabbitMQ的应用。Serilog.Sinks.Kafka能够将结构化日志数据发送到Kafka，利用其高吞吐量优势，适合处理大量日志数据。文章详细列出了在Windows上安装Kafka的步骤，包括Java环境的安装和Kafka配置的修改。作者强调了KRaft模式的使用，对Kafka的配置文件做了说明。整体内容紧扣分布式系统中的日志处理，适合开发者参考。

### 【Azure Web App】Github Action部署Jar包到App Service报400错误

https://www.cnblogs.com/lulight/p/19439653

文章描述了在使用GitHub Action部署Azure App Service时遇到的400错误。该错误表示无法将JAR包部署到配置为Tomcat的应用服务中。作者通过修改堆栈为Java SE成功解决了问题。此外，文章提到Kudu的开源代码，进一步验证了对JAR包的强制限制。提供了解决方案和背景信息，内容清晰且具有实用性。

## 今日人物

**史蒂芬·亚瑟·库克**（英语：Stephen Arthur Cook，1939年12月14日—）是一名[美国](https://zh.wikipedia.org/wiki/美國)[计算机科学家](https://zh.wikipedia.org/wiki/計算機科學家)，[计算复杂性理论](https://zh.wikipedia.org/wiki/計算複雜性理論)的重要研究者。

1971年，在他的论文《定理证明程式的复杂性》（*The Complexity of Theorem Proving Procedures*），他整理了[NP完备性](https://zh.wikipedia.org/wiki/NP完備)的目标，亦产生了[库克定理](https://zh.wikipedia.org/wiki/庫克定理)——[布尔可满足性问题](https://zh.wikipedia.org/wiki/布爾可滿足性問題)是NP完备的证明。

1982年，库克获得[图灵奖](https://zh.wikipedia.org/wiki/图灵奖)。因为其论文开启了NP完备性的研究，令这个领域于之后的十年成为计算机科学中最活跃和重要的研究。

库克现为[多伦多大学](https://zh.wikipedia.org/wiki/多倫多大學)的计算机科学和数学系教授。

![img-1](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/dtgE_1cPFtd9m2UR6E_YW_1536x1024_20260126_140335_raw.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

* 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
* .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
* 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。