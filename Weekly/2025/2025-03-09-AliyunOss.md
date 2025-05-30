## 国内文章
### 记一次.NET内存居高不下排查解决与启示

https://www.cnblogs.com/huangsheng/p/18731382

本文讲述了一个ASP.NET Core gRPC服务迁移到Kubernetes后的内存管理问题。服务在K8s上遇到了高内存占用与副本扩展的问题，经过排查发现服务的内存请求设置正确，但未设定上限。压测显示内存长期维持在高位，虽然没有性能下降。使用dotnet-dump分析得出，LOH驻留类型的对象导致内存占用过高。调试过程中尝试多个GC调试方案，其中工作站GC模式有效减小了内存使用。但文章也警示不建议频繁手动调用GC，并讨论了K8s中请求与限制的配置重要性。

### SQL Server 2025 AI相关能力初探

https://www.cnblogs.com/CareySon/p/18753299/SQL_SERVER_2015_AI_New_Feature

本文讨论了SQLServer的演变及其与AI相关的向量数据库支持。作者回顾了SQLServer自2008年以来各版本新增功能，以适应市场趋势和技术需求。SQLServer2025引入了向量类型支持，允许存储高达1998维度的向量，并通过DiskANN技术实现高效相似度检索。向量数据库在AI应用中至关重要，能够显著提高向量搜索的计算效率，降低成本。这些新特性满足了当前数据管理和分析的需求，展示了SQLServer与时俱进的技术深度和实践意义。

### C#/.NET/.NET Core优秀项目和框架2025年2月简报

https://www.cnblogs.com/Can-daydayup/p/18758846

文章介绍了一系列C#和.NET相关的开源项目和框架，包括eShop、Bulk Crap Uninstaller、Netnr.Login、BYSerial、V-Control和Plotly.NET。这些项目展示了如何利用.NET技术构建现代应用，覆盖电子商务、应用卸载、OAuth2登录、串口调试、UI组件和交互式图表等多个领域。每个项目提供了源码和详细介绍，鼓励读者关注公众号获取更多信息。文章提供了丰富的资源和实用的指导。

### AI与.NET技术实操系列(二)：开始使用ML.NET

https://www.cnblogs.com/code-daily/p/18749505

本文探讨了机器学习及其在.NET环境中的应用，特别是ML.NET框架。ML.NET使.NET开发者更容易构建和部署机器学习模型。文章介绍了ML.NET的特点和优势，包括支持多种机器学习任务和无缝集成于.NET平台。通过具体的分类任务示例，读者将了解机器学习的基本流程，包括数据准备、特征工程、模型训练和评估。同时，文章也提及机器学习面临的挑战，如数据质量及伦理问题，旨在激发开发者在机器学习领域的探索兴趣。

### .NET 10首个预览版发布：重大改进与新特性概览！

https://www.cnblogs.com/Can-daydayup/p/18750340

.NET团队于2025年发布了.NET 10的首个预览版，此版本为长期支持(LTS)版本，提供三年支持。新特性包括运行时性能改进，降低虚方法调用的开销，增强JIT编译器的去虚拟化能力和对AVX10.2指令集的支持。类库方面新增功能支持非SHA-1证书指纹搜索，直接读取ASCII编码PEM文件，新扩展ISOWeek类简化周数计算，以及ZipArchive的性能和内存改进。OrderedDictionary的方法增强了元素索引的查找，JSON序列化功能也得到了加强。

### Linux系列：如何用 C#调用 C方法造成内存泄露

https://www.cnblogs.com/huangxincheng/p/18748086

本文介绍了在Linux平台上通过C#调用C语言的过程，强调了使用gcc编译生成共享库.so文件的重要性。通过代码示例，展示了如何在Linux中分配内存并编译共享库，具体说明了各个编译选项的含义和作用。作者强调了研究C#程序中的非托管内存泄露现象的必要性和实践意义。文章内容简洁明了，适合开发者学习和参考。

### 基于Microsoft.Extensions.AI核心库实现RAG应用

https://www.cnblogs.com/edisonchou/p/-/introduction-to-vector-rag-demo

本文介绍了如何基于Microsoft.Extensions.AI和VectorData构建RAG问答应用。以电商网站“易速鲜花”为例，文章讨论了向量存储和词嵌入的应用。核心是创建一个 AI 机器人，帮助员工解答政策性问题。文章详细描述了所用工具，包括LLM、Qdrant向量数据库及Ollama模型生成器。内容涵盖了必要的文件结构与代码示例，尤其是如何设计TextSnippet和TextSearchResult类以支持向量查询。整体结构清晰，内容实用，适合开发者参考与实施。文章具有较高的技术深度与实践性，跟进了最新技术趋势。

### .NET10 - 预览版1新功能体验(一)

https://www.cnblogs.com/hugogoos/p/18748741

.NET 10 预览版已发布，包含重要更新，如.NET Runtime、SDK、C#、ASP.NET Core和Blazor等。用户需下载.NET 10.0.0-preview.1 SDK，并确保Visual Studio 2022更新至最新版本。创建类库前需在VS中启用预览版SDK功能。C# 14 也随之发布，需设置属性以使用新功能。新特性包括field关键字简化属性访问器、支持未绑定的泛型类型的nameof表达式，以及对Span和ReadOnlySpan的新隐式转换，提升代码性能和安全性。

### AI与.NET技术实操系列 - 开篇

https://www.cnblogs.com/code-daily/p/18744841

本文探讨了人工智能(AI)在.NET平台中的应用，强调AI对软件开发者的重要性。AI涵盖机器学习、深度学习和自然语言处理等领域，推动了各行各业的创新与变革。特别是ML.NET为.NET开发者提供了构建和部署机器学习模型的工具。理解AI基础概念对掌握.NET中的AI应用至关重要。本文为有一定.NET经验的开发者提供指导，旨在展现AI与.NET结合的潜力和应用场景。

### 在 Aspire 项目下使用 AgileConfig

https://www.cnblogs.com/kklldog/p/18747156/aspire-agileconfig

.NET Aspire 是一组工具和包，用于构建可监控的生产应用。它通过 NuGet 包提升开发效率，支持现代应用开发中的服务整合。文章介绍了如何使用 AgileConfig。在使用 AgileConfig 时，需要通过 docker 命令启动服务端，设置必要的配置，然后添加客户端包。在 Aspire 项目中，读者可以直接运行服务，并通过简单配置链接 AgileConfig 服务，达到简化操作的目的。文章提供代码实例，展示如何配置 Aspire 项目。整体信息丰富，具备实践指导意义。

### [WinUI 3] 模仿 Visual Studio 的 Docking 控件

https://www.cnblogs.com/xymfblogs/p/18753956

WinUI 3 是微软推出的 UI 框架，支持 Win32 和混合开发，继承了 WPF 的特性。国内关注度低，应用有限。Uno Platform 基于 WinUI 3 API，支持跨平台运行，开发体验一致。WinUI.Dock 是一个基于 WinUI 3 的 Docking 控件，灵感来源于 AvalonDock 和 ImGui，支持 Uno Platform，但无法跨窗口拖动。项目仍在早期阶段，不建议用于生产环境。

### .NET MCP项目对比分析：MCPSharp、mcpdotnet与ModelContextProtocol.NET

https://www.cnblogs.com/shanyou/p/18748718

MCP协议由Anthropic推出，旨在大型语言模型与外部数据源的无缝集成。文章分析三个.NET项目：MCPSharp、mcpdotnet和ModelContextProtocol.NET。MCPSharp提供全面的服务器和客户端实现，易用的API和丰富文档，适合构建AI助手工具。mcpdotnet支持多种功能，并有良好的日志支持，兼容.NET 8.0以上。ModelContextProtocol.NET实现了标准输入输出，但部分功能仍在开发中，近期不活跃。三者均采用MIT许可证，MCPSharp和mcpdotnet社区活跃，ModelContextProtocol.NET相对低迷。若寻找功能丰富、社区支持的选项，MCPSharp更为合适。

### AI与.NET技术实操系列 - 开篇

https://www.cnblogs.com/Edison-Go/p/18744841

本文探讨了人工智能(AI)在.NET平台上的应用。随着AI技术的发展，掌握这些技术对开发者至关重要。首先介绍了AI的基础概念，涵盖机器学习、深度学习和自然语言处理等关键领域。机器学习通过数据学习模式，深度学习利用多层神经网络处理复杂任务，而自然语言处理使计算机理解人类语言。这些基础为.NET开发者在其平台上应用AI奠定了基础，ML.NET等工具支持开发者构建和部署机器学习模型，推动了智能应用的实现。

### AI与.NET技术实操系列(二)：开始使用ML.NET

https://www.cnblogs.com/Edison-Go/p/18749505

本文讨论了机器学习在.NET开发中的重要性，介绍了ML.NET作为微软推出的机器学习框架，降低了入门门槛。ML.NET支持多种机器学习任务，并提供易用的API。文章解释了机器学习的基本概念，包括监督学习与无监督学习，描述了模型的训练、评估和部署过程，强调高质量数据和算法选择的重要性，同时也提及了伦理和隐私问题。最后，本文通过实例引导开发者使用ML.NET构建分类模型，帮助他们理解机器学习的应用与挑战。

### AI与.NET技术实操系列(三)：在.NET中使用大语言模型(LLMs)

https://www.cnblogs.com/code-daily/p/18752589

本文探讨了大语言模型(LLMs)在.NET开发中的应用，以及如何通过OpenAI等API集成LLMs。首先定义了LLMs的概念和工作原理，介绍预训练和微调的过程。接着列举了LLMs的多种应用场景，如智能对话系统和机器翻译等。文章强调了LLMs为开发者带来的实际优势及其复杂性和数据隐私等挑战。通过示例任务构建聊天机器人，读者将理解LLMs的策略和开发流程，激励开发者在.NET环境中探索LLMs的潜力。

### 设计模式学习：2、状态模式实现订单状态流转

https://www.cnblogs.com/huangmingji/p/18755997

本文探讨电商支付模块中的状态流转，强调状态模式的重要性。订单经历待支付、支付中、支付成功/失败与退款处理的生命周期。不同状态有不同可执行操作，且状态转换需触发附加操作。传统的条件语句导致代码臃肿且维护难度加大，因此状态模式提供了更优解决方案。该模式通过研制状态接口和上下文类，简化状态管理，提升可维护性。具体实现展示了待支付和支付中状态的核心逻辑，确保状态转换自动化。全流程实现清晰并具有实践价值，适合电商应用场景。

### 终于写完轮子一部分：tcp代理 了，记录一下

https://www.cnblogs.com/fs7744/p/18759510

该文章讨论了作者计划使用C#开发一个网络代理的设想。文章明确说明了项目的目标，设计理念以及实现中的技术细节。作者借鉴了Kestrel和Yarp的相关处理逻辑，强调了多线程处理和跨平台适配的重要性。提到现有的限制，例如Dotnet不支持统一的跨进程socket转移API，影响热重启功能。项目已初步完成TCP部分，并逐步向UDP和HTTP协议扩展。提供了基本的使用说明和配置示例，整体内容清晰实用。虽然最终实现尚未完成，但框架设计已经初步成型。

### 跨平台Windows和Linux(银河麒麟)操作系统OCR识别应用

https://www.cnblogs.com/lsjwq/p/18747917

本文介绍了在Linux上安装Tesseract OCR引擎的详细步骤，包括下载、配置和测试等环节。首先提供了代码下载链接，并展示了OCR的运行效果。随后详细说明了如何下载tesseract和leptonica，以及如何在Linux环境下依次执行安装命令。同时，文章还讲解了如何配置环境变量和下载语言包，最后提供了测试安装成功与读取图片文字的代码示例，适合需要进行OCR识别的开发者参考。

### Linux系列：如何用heaptrack跟踪.NET程序的非托管内存泄露

https://www.cnblogs.com/huangxincheng/p/18757287

本文分析了在C#中调用C语言代码引发的内存泄露问题，尤其在Linux环境下的复杂性。文章通过案例展示了C和C#代码，并介绍了heaptrack工具的使用，以跟踪C/C++的内存分配情况。虽然heaptrack与C#关系不大，但它能够记录分配调用栈信息，分析内存使用情况。该文章提供了详细的技术背景和实用案例，适合对内存管理感兴趣的开发者。

### 重生之数据结构与算法----队列&amp;栈

https://www.cnblogs.com/lmy5215006/p/18748329

这篇文章介绍了数据结构的基本概念，重点讲解了栈和队列的定义及实现。栈遵循后进先出原则，通过链表实现，提供了入栈、出栈和查看栈顶的操作，效率为O(1)。队列遵循先进先出原则，同样通过链表实现，提供了入队和出队操作。文章通过代码示例直观展示了如何实现栈和队列，便于读者理解和应用。

### 重生之数据结构与算法----数组&amp;链表

https://www.cnblogs.com/lmy5215006/p/18736066

这篇文章探讨了数据结构和算法的基本概念，重点分析了数组和动态数组的特征。数组包括静态和动态两类，静态数组提供快速的随机访问，但在插入和删除时效率低下。动态数组解决了扩容和易用性的问题，但并未根本改善性能。文中给出了简单的动态数组实现示例，阐述了增、删、改、查的方法。整体分析提供了深入的理解，对于初学者和开发者具有很好的启发意义。

### 展开说说关于C#中ORM框架的用法！

https://www.cnblogs.com/chen233/p/18752092

Entity Framework(EF)是微软的ORM框架，分为EF 6和EF Core两个版本。EF 6专为.NET Framework设计，成熟稳定，支持复杂数据库操作，但性能不如EF Core。EF Core则为.NET Core和.NET 5+重设计，强调高性能、轻量级和跨平台支持。EF Core支持异步编程和模块化功能，持续更新。选择建议方面，基于.NET Framework的项目推荐EF 6，而基于.NET Core的项目应使用EF Core，以满足性能和跨平台需求。

### Windows 提权-MSSQL

https://www.cnblogs.com/kqdssheng/p/18757951

本文讨论了利用 MSSQL 服务器进行 Windows 权限提升的攻击方法。通过手动枚举数据库，破解凭证，以及执行 CMD 命令，展示了如何从数据库中获取敏感信息。文章结构清晰，包括搜寻 MSSQL 服务以及针对特权用户的攻击场景。虽然内容生成自翻译，校正与注释增强了理解，仍有进一步改进空间。整体技术深度和实用性较强但存在表述不够流畅的问题，未标明更新的文献资料。本文对 MSSQL 服务器的多种攻击手段进行了全面介绍，适合安全研究人员参考。

### 重生之数据结构与算法----哈希表

https://www.cnblogs.com/lmy5215006/p/18748028

文章详细介绍了哈希表的原理，包括哈希函数的运作方法、哈希冲突的成因与解决方案，及负载因子的概念。哈希函数将任意长度的输入转化为固定长度的输出，并讨论了注意生成正整数和避免太大数组的策略。拉链法和开放寻址法分别用于解决哈希冲突，文中也探讨了负载因子的影响及其在扩容过程中的作用。整体内容丰富，技术性强，适合对哈希表有一定了解的读者。语言清晰，例子直观，适合学习和应用。

### Windows 提权-PrintNightmare

https://www.cnblogs.com/kqdssheng/p/18753135

本文介绍了PrintNightmare漏洞及其利用方法，包括CVE-2021-34527(远程代码执行)和CVE-2021-1675(本地权限提升)。文章详细描述了如何远程和本地枚举Windows打印服务，并使用具体工具(如rpcdump.py和SharpPrintNightmare)进行漏洞利用。PrintNightmare影响几乎所有Windows版本，攻击者需要标准用户凭证。文中给出了创建恶意DLL和进行服务共享的步骤，清晰地展示了攻击过程和所需条件。总体上，文章具备技术深度并强调实用性，语言简练清晰。

### 重生之数据结构与算法----二叉树的遍历

https://www.cnblogs.com/lmy5215006/p/18740995

文章介绍了二叉树的基本概念和几种类型，如满二叉树、完全二叉树、平衡二叉树和二叉搜索树。每种树的特点及其实现方式都有详细说明。通过图示和代码示例，作者清晰地展示了如何使用链表和数组实现二叉树。此外，强调了理解二叉树对解决复杂数据结构的重要性。整体上，文章为读者提供了关于二叉树深入浅出的知识。内容结构严谨，易于理解，适合对数据结构感兴趣的读者。

### 非容器环境中使用Selenium，提升Chrome与ChromeDiver兼容性

https://www.cnblogs.com/chenyishi/p/18757021

在 Windows 环境下使用 Selenium 时，Chrome 和 ChromeDriver 版本不匹配是个常见问题。为避免此问题，建议下载指定版本的 Chrome 和 ChromeDriver 并将其放入项目的发布目录。在 .csproj 文件中配置，将 chrome-win64 目录包含到输出目录中。使用 C# 代码显式指定 Chrome 和 ChromeDriver 的路径。在运行时，Selenium 将使用这些指定版本，有效避免不兼容带来的错误。该方法提高了代码稳定性和可维护性。

### 分布式锁—2.Redisson的可重入锁

https://www.cnblogs.com/mjunz/p/18749444

本文介绍了Redisson可重入锁RedissonLock的实现和使用，包括创建RedissonClient实例、Lua脚本加锁逻辑、WatchDog机制、锁的互斥与释放等。首先在pom.xml中引入Redisson依赖，随后构建RedissonClient连接Redis Cluster，获取和使用可重入锁RLock。RedissonLock实现了Lock接口，并提供异步和响应式接口。文中强调了锁的超时管理，WatchDog可自动延长锁的有效期，有效避免了超时释放问题。最后总结了可重入锁源码的核心逻辑。

### AI与.NET技术实操系列(四)：使用Semantic Kernel和DeepSeek构建AI应用

https://www.cnblogs.com/code-daily/p/18757511

本文探讨了大型语言模型(LLMs)及其在智能应用开发中的重要性。微软的Semantic Kernel(SK)为.NET开发者提供了集成LLMs的工具。SK具备插件化和模块化设计，允许开发者定制AI应用。它简化了LLMs的调用，提供易用接口，支持多种模型。虽然使用SK需掌握一些基本概念，但它对新手和经验丰富的开发者均友好。文章展示了如何安装SK及其基础使用，促进开发者理解和应用这一工具。希望激励开发者探索AI应用的未来。 

### C# 中的“相等判断”

https://www.cnblogs.com/hihaojie/p/18761086/c-bk2f6

本文详细讨论了C#中不同的相等判断方式，包括双等号、Equals方法和其他特殊类型的相等比较。文章分析了基元类型、部分预定义值类型和引用类型在使用==运算符时的行为，并解释了它们在编译和运行时的工作原理。重点展示了基元类型的优化以及值类型和引用类型在相等判断中的不同处理。内容深入易懂，适合开发者理解C#相等判断的逻辑和实际应用场景。

### Windows编程----进程的当前目录

https://www.cnblogs.com/caoruipeng/p/18761238

本文讨论Windows API中进程的当前目录及其影响。创建文件时，如果路径不是全路径，Windows会获取进程的当前目录并拼接成全路径。通过GetCurrentDirectory函数可以获取当前目录示例，而通过CreateFile函数可以展示如何使用相对路径创建文件。运行结果表明，VS调试下与直接运行exe文件时的当前目录不同。此外，进程的当前目录可以通过SetCurrentDirectory函数修改，进一步增强文件操作的灵活性。

## 主题

### .NET 和 .NET Framework 2025 年 3 月服务发布更新 - .NET 博客
https://devblogs.microsoft.com/dotnet/dotnet-and-dotnet-framework-march-2025-servicing-updates/

### 新的、更简单的解决方案文件格式 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/new-simpler-solution-file-format/

### 引入对 SLNX 的支持，SLNX 是 .NET CLI 中一种新的、更简单的解决方案文件格式 - .NET 博客
https://devblogs.microsoft.com/dotnet/introducing-slnx-support-dotnet-cli/

### TypeScript 速度提高 10 倍 - TypeScript
https://devblogs.microsoft.com/typescript/typescript-native-port/

- [Anders Hejlsberg 回答 - 为什么去？ ·microsoft/typescript-go · 讨论 #411](https://github.com/microsoft/typescript-go/discussions/411#discussioncomment-12476218)

### 解锁对 Cloud Academy 的免费访问：Visual Studio 订阅者的新好处 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/cloud-academy-visual-studio-subscription-benefit/

### MongoDB EF Core Provider 现在支持 EF 9！
https://medium.com/@MongoDB/mongodb-ef-core-provider-now-supports-ef-9-62db9b89ce0d

### GPT-4o Copilot 代码完成模型现已在 Visual Studio 公共预览版中提供 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/gpt-4o-copilot-code-completion-model-available-now-in-visual-studio-public-preview/

## 发布
- [aws/aws-sdk-net](https://github.com/aws/aws-sdk-net)
    - [3.7.1000.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1000.0)、[3.7.1001.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1001.0)、[3.7.1002. 0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.1002.0)， [3.7.999.0](https://github.com/aws/aws-sdk-net/releases/tag/3.7.999.0)
- [Azure/azure-sdk-for-net](https://github.com/Azure/azure-sdk-for-net)
    - [Azure.Data.AppConfiguration_1.6.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Data.AppConfiguration_1.6.0)， [ Azure.ResourceManager.AlertsManagement_1.1.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.AlertsManagement_1.1.1)、[ Azure.ResourceManager.Analysis_1.1.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Analysis_1.1.1)、[ Azure.ResourceManager.AppComplianceAutomation_1.0.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.AppComplianceAutomation_1.0.1)、[ Azure.ResourceManager.ApplicationInsights_1.0.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ApplicationInsights_1.0.1)、[ Azure.ResourceManager.AppPlatform_1.1.2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.AppPlatform_1.1.2)、[ Azure.ResourceManager.Automanage_1.1.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Automanage_1.1.1)、[ Azure.ResourceManager.Automation_1.1.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Automation_1.1.1)、[Azure.ResourceManager.Billing_ 1.2.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Billing_1.2.1) [Azure.ResourceManager.BotService_1.1.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.BotService_1.1.1)，[Azure.ResourceManager.Cdn_1.3. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Cdn_1.3.1)，[Azure.ResourceManager.ChangeAnalysis_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.ChangeAnalysis_1.1.1)，[Azure.ResourceManager.Communication_1.2. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Communication_1.2.1)，[Azure.ResourceManager.Confluent_1.2. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Confluent_1.2.1)，[Azure.ResourceManager.CostManagement_1.0. 2](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.CostManagement_1.0.2)， [Azure.ResourceManager.DataBox_1.0. 4](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataBox_1.0.4)，[Azure.ResourceManager.DataBoxEdge_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataBoxEdge_1.1.1)，[Azure.ResourceManager.DataFactory_1.7. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataFactory_1.7.0)， [Azure.ResourceManager.DataLakeAnalytics_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataLakeAnalytics_1.1.1)，[Azure.ResourceManager.DataLakeStore_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataLakeStore_1.1.1)，[Azure.ResourceManager.DataShare_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DataShare_1.1.1)，[Azure.ResourceManager.DesktopVirtualization_1.3. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DesktopVirtualization_1.3.1)，[Azure.ResourceManager.DeviceProvisioningServices_1.2. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.DeviceProvisioningServices_1.2.1)，[Azure.ResourceManager.FrontDoor_1.3. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.FrontDoor_1.3.1)，[Azure.ResourceManager.Hci_1.2. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Hci_1.2.1)，[Azure.ResourceManager.Resources_1.9. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Resources_1.9.1)， [Azure.ResourceManager.Sphere_1.0. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Sphere_1.0.1)，[Azure.ResourceManager.StorageCache_1.3. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.StorageCache_1.3.1)，[Azure.ResourceManager.StorageMover_1.2. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.StorageMover_1.2.1)，[Azure.ResourceManager.Support_1.1. 1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.Support_1.1.1)，[Azure.ResourceManager.TrafficManager_1.1. 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.ResourceManager.TrafficManager_1.1.3) [Azure.Storage.Blobs_12.24.0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Blobs_12.24.0)，[Azure.Storage.Blobs.Batch_12.21. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Blobs.Batch_12.21.0)， [Azure.Storage.Common_12.23. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Common_12.23.0)， [Azure.Storage.Files.DataLake_12.22. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Files.DataLake_12.22.0)， [Azure.Storage.Files.Shares_12.22. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Files.Shares_12.22.0)， [Azure.Storage.Queues_12.22. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Azure.Storage.Queues_12.22.0)， [Microsoft.Azure.WebJobs.Extensions.EventGrid_3.4. 4](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebJobs.Extensions.EventGrid_3.4.4)， [Microsoft.Azure.WebJobs.Extensions.ServiceBus_5.16. 5](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebJobs.Extensions.ServiceBus_5.16.5)， [Microsoft.Azure.WebJobs.Extensions.SignalRService_ 2.0.1](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebJobs.Extensions.SignalRService_2.0.1)， [Microsoft.Azure.WebJobs.Extensions.Tables_1.3. 3](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Azure.WebJobs.Extensions.Tables_1.3.3)， [Microsoft.Extensions.Azure_1.11. 0](https://github.com/Azure/azure-sdk-for-net/releases/tag/Microsoft.Extensions.Azure_1.11.0)
- [DataDog/dd-trace-dotnet](https://github.com/DataDog/dd-trace-dotnet)
    - [v3.12.0](https://github.com/DataDog/dd-trace-dotnet/releases/tag/v3.12.0)
- [googleapis/google-cloud-dotnet](https://github.com/googleapis/google-cloud-dotnet)
    - [Google.Cloud.AIPlatform.V1-3.22.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.AIPlatform.V1-3.22.0)，[Google.Cloud.Audit-2.5. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Audit-2.5.0)，[Google.Cloud.Bigtable.Admin.V2-3.24. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Bigtable.Admin.V2-3.24.0)，[Google.Cloud.Bigtable.V2-3.16. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Bigtable.V2-3.16.0)、[Google.Cloud.Datastore.V1-4.15. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Datastore.V1-4.15.0)， [Google.Cloud.Dialogflow.Cx.V3-2.23. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Dialogflow.Cx.V3-2.23.0)， [Google.Cloud.Dialogflow.V2-4.26. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Dialogflow.V2-4.26.0)，[Google.Cloud.Filestore.V1-2.7. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Filestore.V1-2.7.0)、[Google.Cloud.Firestore-3.10. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Firestore-3.10.0)，[Google.Cloud.Firestore.V1-3.10. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Firestore.V1-3.10.0) [Google.Cloud.PubSub.V1-3.22.0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.PubSub.V1-3.22.0)，[Google.Cloud.PubSub.V1-3.23. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.PubSub.V1-3.23.0)，[Google.Cloud.Storage.V1-4.11. 0](https://github.com/googleapis/google-cloud-dotnet/releases/tag/Google.Cloud.Storage.V1-4.11.0)
- [grpc/grpc-dotnet](https://github.com/grpc/grpc-dotnet)
    - [v2.70.0](https://github.com/grpc/grpc-dotnet/releases/tag/v2.70.0)
- [microsoft/microsoft-ui-xaml](https://github.com/microsoft/microsoft-ui-xaml)
    - [winui3](https://github.com/microsoft/microsoft-ui-xaml/releases/tag/winui3/release/1.6.6)
- [microsoft/WindowsAppSDK](https://github.com/microsoft/WindowsAppSDK)
    - [v1.6.6](https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.6.6)

## 文章、幻灯片等
### System.Linq.Async 是 .NET 10 的一部分 - LINQ for IAsyncEnumerable
https://steven-giesel.com/blogPost/e40aaedc-9e56-491f-9fe5-3bb0b162ae94

### JetBrains Rider 中对游戏机的支持 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2025/03/14/support-for-game-consoles-in-jetbrains-rider/

### DevProxy 0.25 改进了配置管理，加入了 .NET Foundation
https://www.infoq.com/news/2025/03/devproxy-025-net-foundation/

### 如何使用 Notion 构建无头 CMS
https://zenn.dev/rendya/articles/notion-headless-cms-sample

### 【. NET8] 使用 MagicOnion 设置 API 服务器 - Qiita
https://qiita.com/inco-cyber/items/3253235a0a9d5fda2b1e

- [将 gRPC-Web 与 MagicOnion 结合使用 - Qiita](https://qiita.com/inco-cyber/items/74715318a7f40d819d64)

### 如何在 C# 中将 EventWaitHandle wait 转换为 Task 来解决混合问题(简单地在 Task 中等待会导致问题) - Qiita
https://qiita.com/spc_ksudoh/items/bff67ca86c878b106c92

### [C#] 使用 JsonExtensionData 处理动态属性
https://zenn.dev/shimiyu/articles/c89058684563d2

### 使用 DuckDB 读取 Excel 文件 - C#
https://zenn.dev/gkuroki/articles/dotnet-duckdb-excel-read

### [Discord] DSharpPlus - 琪塔
https://qiita.com/wrsmA/items/00b2b8ee085ac08761a4

### 比较字符串和数字 (.NET 10) - Qiita
https://qiita.com/h084/items/9ece2dfd6bb5bafaadb1

### 在 Windows 容器中的 IIS 中运行 ASP.NET Core 应用程序
https://andrewlock.net/running-an-aspnetcore-app-behind-iis-in-a-windows-container/

### 使用 EF Core 中的序列对 Id 以外的列进行自动编号 - Qiita
https://qiita.com/jun1s/items/0090dd0c4f56e63bd6a0

### 关于分发和更新 WPF 的_InnoSetup和 AutoUpdater.NET - Qiita
https://qiita.com/msms/items/223c30212d3458958001

### 更理解多线程调试 - Visual Studio Blog
https://devblogs.microsoft.com/visualstudio/make-more-sense-of-multithreaded-debugging/

### 你好 HybridCache！ 简化 ASP.NET Core 应用程序的缓存管理 - .NET 博客
https://devblogs.microsoft.com/dotnet/hybrid-cache-is-now-ga/

### [C#] 使用 UnsafeAccessor 属性的代码在运行时抛出 BadImageFormatException 异常
https://zenn.dev/j_sakamoto/articles/55676560cef8b2

### 用 C# 编写 .NET 垃圾回收器 - 第 5 部分
https://minidump.net/writing-a-net-gc-in-c-part-5/

### [C#] 关于集合表达式
https://zenn.dev/nuskey/articles/19b3c75b806dad
### 使用 AWS 开发工具包。 如果使用 Extensions.NETCore.Setup 3.7.x 进行初始化速度较慢，请使用 3.7.1 或为 DefaultsMode 指定 Standard
https://qiita.com/karuakun/items/cf7c334ec8156e4bfd63

### C# 14 中的新增功能
https://zenn.dev/ya46/articles/6fe156619d87b0

### [.NET 10 Preview 1] 看来 foreach 通过接口的性能会有所提升
https://zenn.dev/ya46/articles/bca4fa5e5ceca5

### Kyoto.cs #1 (2025/04/06 15：00〜)
https://kyotocs.connpass.com/event/348616/

## 库、存储库、工具等
### Cysharp/ZLinq：所有 .NET 平台和 Unity 的 Span 和 LINQ to SIMD 的零分配 LINQ、LINQ to Tree(FileSystem、Json、GameObject 等)。
https://github.com/Cysharp/ZLinq

### 推特
https://x.com/jcouv/status/1899508932068176238?s=12

![image-20250318205232696](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20250318205232696.jpg)

---

https://x.com/mkristensen/status/1900224976332218558?s=12

![image-20250318205257256](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20250318205257256.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET性能优化经验的群组，主题包括但不限于：

* 如何找到.NET性能瓶颈，如使用APM、dotnet tools等工具
* .NET框架底层原理的实现，如垃圾回收器、JIT等等
* 如何编写高性能的.NET代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我vx，我拉你进群: **ls1075** 另外也创建了**QQ Group**: 687779078，欢迎大家加入。