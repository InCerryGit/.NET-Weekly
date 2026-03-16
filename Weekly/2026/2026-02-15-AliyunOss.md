## 国内文章
### 追更 HelloGitHub 一整年，终于等到了这篇年度盘点

https://www.cnblogs.com/xueweihan/p/19596455

HelloGitHub在春节前举办了年度开源项目盘点，选出了2025年十大热门开源项目。入选项目根据社区用户的真实反馈如阅读、点赞、收藏与评论进行评估。本文分为年度十佳和分类精选，涵盖C/C++、C#、Go等多种类别。十大项目包括桌宠应用、游戏变速器、电子书阅读器等，均为开源且支持多平台。每个项目都附有用户评价和GitHub链接，鼓励读者参与互动，以提高项目的可见度与影响力。

### 从零开始:C#单文件AOT打包前后端分离项目

https://www.cnblogs.com/luojin765/p/19607043

本文介绍如何在.NET生态中使用C#实现单文件和AOT（Ahead-of-Time）编译，将前后端整合进一个可执行文件。首先，创建一个ASP.NET Core Web API项目，并将前端代码嵌入到项目中。接着修改.csproj文件，将wwwroot文件夹的所有文件设为嵌入资源。然后，通过EmbeddedFileProvider配置静态文件，使后端能够访问这些嵌入的文件。此外，设置页面路由，确保服务器能正确处理请求并返回嵌入的index.html。最后，文章展示了整个过程的简洁性和高效性，强调了无反射和无动态代码生成的优点。

### Dapper轻量级扩展库SmartDapper

https://www.cnblogs.com/mumaren/p/19593895

SmartDapper 是一个轻量级的 Dapper 扩展库，提供 SQL 生成、链式查询和多数据库支持。它默认使用参数化执行，降低 SQL 注入风险。用户可以使用 SQL 生成器创建查询并通过 Dapper 执行。示例中展示了如何定义实体类，以及如何使用扩展方法进行查询，支持列名映射和查询分页。基于简洁的 API，SmartDapper 提升了数据库操作的灵活性和安全性。

### dotnet Vortice 通过 Angle 将 Skia 和 DirectX 对接

https://www.cnblogs.com/lindexi/p/19593476

ANGLE是一个开源组件，能够将OpenGL ES API调用转换为DirectX的实际调用。文章介绍了使用ANGLE与DirectX的集成步骤，包括创建Win32窗口、初始化DirectX以及ANGLE，使用NuGet安装必要库。项目文件显示了所需的引用包。文章提供核心代码的概述以及完整的Program.cs文件，鼓励读者从文末下载完整代码。整体结构清晰，突出关键实现。该文与.NET相关，适合C#开发者。

### 一款开源、强大、简单易用的 .NET 假数据生成利器

https://www.cnblogs.com/Can-daydayup/p/19601424

本文介绍了一个用于 .NET 项目的假数据生成库Bogus。Bogus是基于faker.js开发的开源库，支持C#、F#和VB.NET等多种语言。它提供简单易用的API，可快速生成多种模拟数据，适用于单元测试、数据库填充、性能测试和API调试等场景。Bogus支持40多种语言区域本地化，能有效替代手动生成数据的方法。文章中还展示了如何创建控制台应用并安装Bogus，以及生成随机订单的示例代码。该库能极大地提高开发和测试的效率。

### C#/.NET/.NET Core优秀项目和框架2026年1月简报

https://www.cnblogs.com/Can-daydayup/p/19593194

文章介绍了每月推荐的几个C#/.NET/.NET Core优秀开源项目和框架。包括PicView、NanUI、Generative-AI-for-beginners-dotnet、XAML Studio和Codist。这些项目涵盖图像查看、WinForm应用开发、生成式人工智能课程、XAML设计工具以及Visual Studio插件，展示了技术的深度和实用性。每个项目都有详细介绍与源码链接，适合开发者使用。同时，文章及时更新，注重清晰明了地传达信息，排版友好。

### OData 协议的智能化语义互操作

https://www.cnblogs.com/shanyou/p/19601411

在企业数字化转型中，开放数据协议（OData）是关键技术。自2007年由微软推出以来，OData从私有规范发展为国际标准，旨在打破数据孤岛，提升数据共享价值。其设计遵循REST原则，支持简单性、增量构建和高可扩展性。实体数据模型（EDM）显式定义数据模型，确保语义互操作性。OData服务提供服务文档与元数据文档，支持客户端的自发现。这一协议让开发者专注于业务逻辑，而非底层技术细节，为构建现代API提供了最佳实践。

### AI工具实践日记（一）：在树莓派上搭建OpenClaw，一个后端开发者的真实踩坑记录

https://www.cnblogs.com/rsls/p/19606304

本文记录了作者在树莓派上部署OpenClaw的真实经历。这位后端开发者通过学习AI技术，探索将AI助手本地化运行。选择树莓派的原因包括数据隐私、硬件集成和自动化能力。作者详细描述了安装过程中的挑战，如Python和Node.js版本不兼容、权限问题和安装速度慢。作者提供了具体的解决方案，如配置环境和使用国内npm镜像。这篇文章真实且实用，适合有类似需求的开发者。

### 【EF Core】实体追踪——Entry中记录的数据

https://www.cnblogs.com/tcjiaan/p/19601119

文章讨论了Entity Framework Core中的EntityEntry对象及其功能，强调其在状态追踪中的重要性。通过示例实体Book类及其数据库上下文MyDb，展示了如何配置和保存实体，使用字典结构来存储属性值，并介绍了DetectChanges方法的作用。当从数据库查询数据并修改属性时，EF会自动跟踪变化，提高开发效率。文章明确适合初学者理解EF功能和数据库操作。

### MAF快速入门（15）Agent调试利器：DevUI

https://www.cnblogs.com/edisontalk/p/-/quick-start-on-maf-chatper15

本文介绍了DevUI，MAF开发中的交互式Web调试工具，帮助开发者可视化测试和调试AI代理。DevUI无需额外开发，支持在浏览器中对Agent进行测试和查看对话历史，优化了多Agent系统的调试过程。文中提供了创建DevUI示例的步骤，涉及到ASP.NET Core应用的配置和必要NuGet包的安装。这使得开发者能高效配置并启动调试环境，明确了解Agent的行为，提升开发体验。

### Linux Docker Compose 部署.NET+Vue+MySQL+Redis+Nginx 完整记录（亲测无坑）

https://www.cnblogs.com/huyong/p/19598103

本文介绍了Docker Compose的优势，特别是相较于单容器部署的高效性。使用Docker Compose可以一键启动或停止多个容器，集中管理所有配置，简化服务间通信，确保环境一致性，易于维护和迁移。此外，文章还提供了部署环境准备，包括系统要求、软件版本及本地准备文件，确保读者能顺利进行容器化部署。该方案非常适合包括后端、前端和数据库等多组件的中小型项目。

### 【译】Visual Studio 一月更新 —— 增强的编辑器体验

https://www.cnblogs.com/MeteorSeed/p/19600128

本月，Visual Studio推出一系列新功能，增强用户体验。包括快速滚动、支持中键滚动、富HTML格式复制粘贴、语法行压缩等。用户可以通过设置调整这些功能，如快速滚动速度和左侧边距。彩色代码补全功能提升了建议代码的可读性，用户可自定义外观。新功能允许点击部分接受补全，提高了代码编辑的灵活性。Markdown编辑器也优化了预览模式，提供更清晰的访问选项。这些功能目前在Insiders版本中可用，正式版即将发布。

### 8、SequenceInputStream的源码和Vector.class的一些函数说明（windows操作系统，JDK8）

https://www.cnblogs.com/Carey-ccl/p/19618752

文章深入解析了SequenceInputStream类的源码，通过UML图展示其关系，详细说明了如何顺序读取多个InputStream。文章阐述了构造函数的实现，如何处理输入流集合以及流的关闭操作。整体结构清晰，信息丰富，实用性强，适合学习C# .NET相关技术的开发者。文章引入的异常处理和可用性判断增强了代码的实用性和鲁棒性。注释中使用了专业术语，符合技术文章标准。该内容符合当前技术趋势，针对开发者的实际需求提供了具体的实现方案，具有较高的时效性和原创性。

### 拆解 OpenDeepWiki 的 Agent Skills 机制：从 SKILL.md 到 AI 工具调用的完整链路

https://www.cnblogs.com/token-ai/p/19598343

文章介绍了 OpenDeepWiki 的 Skill 扩展体系，主要阐述了 SKILL.md 文件的结构及其功能。Skill 是一组用于 AI Agent 的工具，遵循 agentskills.io 标准。核心 SKILL.md 文件包含元数据和 AI 提示，支持辅助脚本和静态资源。SkillConfig 实体处理元数据，确保格式和规范一致。该体系涉及到文件解析、数据持久化和工具注入等多个环节，展示了开发过程的各个方面。

### Docker Compose部署多.NET后端API+多Vue前端Web 完整记录（含多数据库扩展+实用场景，亲测无坑）

https://www.cnblogs.com/huyong/p/19607257

本文介绍了如何使用Docker Compose在CentOS上部署多个.NET 8后端API和Vue前端Web，解决了端口冲突和配置混乱问题。文章详细阐述了准备工作，包括服务器环境、软件版本、文件准备及基础配置。适用于小型项目和企业内部多环境部署，支持灵活扩展服务，且经过实际测试。本文希望能帮助其他开发者实现容器化部署，提供了详细的部署步骤与配置文件。由于内容丰富且实用，适合开发者参考与实施。

### Admin.NET开源版微服务改造记录

https://www.cnblogs.com/shiningrise/p/19612443

此文记录了Admin.NET项目的微服务改造过程，将其拆分为Admin.NET.Common和Admin.NET.Core两个项目。重构核心类库和工具类，提高模块化设计。通过配置AspireApp.AppHost，集成PostgreSQL，实现持久化和健康检查。同时设置共享目录，确保上传目录存在。利用Furion的Knife4j UI替代Aspire的Swagger UI，增强API文档展示。项目架构清晰，旨在提升系统的可维护性和扩展性。

### 【Azure App Service】32位 Windows App Service 最大能使用多少内存？

https://www.cnblogs.com/lulight/p/19613358

本文详细解答了 Windows-based Azure Web App（32位）的进程内存限制及托管模式下内存计算方式。32 位程序的理论内存上限为4GB，但默认用户态限制为2GB，特殊配置下可突破。In-Process 模式在同一进程中运行，内存共享，性能较高；Out-Of-Process 模式独立进程，内存计算分开。文中还讨论了多个虚拟目录的内存影响及SCM进程的内存计入情况。作者提供了监控方法，包括Azure Portal指标和Kudu进程管理器，便于用户了解内存使用情况。

### 基于DWS构建RAG框架生成行业调研报告

https://www.cnblogs.com/huaweiyun/p/19596583

本文介绍了基于DWS构建检索增强生成（RAG）框架的行业调研报告自动化生成过程。随着信息爆炸，生成高质量报告面临挑战。RAG通过结合信息检索和大语言模型提升生成效率和准确性。文章详细阐述了数据准备、检索优化和生成控制等关键环节。DWS 9.1.1.200支持多种AI功能，优化检索与生成流程。案例部分展示了如何从长文本资料中提取内容，构建数据库，实现报告生成。这一框架降低人工依赖，为组织提供及时、可靠的信息支撑，促进报告的快速迭代。

### 射线法判断一个坐标点（经纬度）是否在一个多边形区域内部

https://www.cnblogs.com/foury/p/19605235

本文探讨在GIS、无人机巡检和地图系统中，如何判断一个点是否位于某个多边形内。采用射线法，通过从待判断点向右绘制水平射线，统计其与多边形边的交点数。若交点数为奇数，则点在多边形内；若为偶数，则点在外部。文中提供了相应的C#代码实现，详细讲解了判断射线与多边形边相交的核心逻辑，通过布尔翻转实现最终判断，采用线性插值计算交点x坐标。这种方法有效解决了空间位置判断问题。

### 从零实现一个生产级 RAG 语义搜索系统：C++ + ONNX + FAISS 实战

https://www.cnblogs.com/charlee44/p/19609813

本文探讨语义化搜索的核心概念，强调传统关键词搜索的局限性。语义化搜索通过嵌入模型将文本转化为向量，使得相似语义的内容在向量空间中靠近。作者计划在资源受限的云服务器上实现一个高效的站内搜索功能，选择C++作为实现语言，以追求性能和资源效率。文章详细介绍了嵌入模型bge-small-zh-v1.5的特点及使用方法，强调其在内存占用和推理速度之间的平衡，适合生产环境的需求。

### MAF快速入门（16）用户智能体交互协议AG-UI（上）

https://www.cnblogs.com/edisontalk/p/-/quick-start-on-maf-chatper16

AG-UI是一个开放的智能体与用户交互协议，旨在优化AI应用界面。其特点包括实时响应、事件驱动架构和状态同步机制。AG-UI与MCP和A2A协议协同工作，分别对应用户界面、工具调用和Agent间合作。文章提供了AG-UI的使用步骤，包括创建ASP.NET Web应用和配置AG-UI服务。AG-UI通过提供清晰的架构组件，使开发者容易构建对话应用。整体内容技术深度高、实践性强，且语言清晰易懂。文章引用和更新力度适中。

### 【渗透测试】HTB靶场之Lock 全过程wp

https://www.cnblogs.com/DSchenzi/p/19618342

Lock是一台简单的Windows靶机，解题流程包括枚举Gitea仓库以找到个人访问令牌（PAT），利用该令牌在服务器上部署ASPX网页后门，获得初始立足点，再从mRemoteNG配置文件解密密码以获取新用户登录权限，最后利用PDF24程序中的本地提权漏洞获取SYSTEM权限的Shell。

### Avalonia.Controls.DataGrid自动合并列

https://www.cnblogs.com/kevin-Y/p/19600957

本文讨论了Winform的DataGridView如何通过线条和透明效果实现列合并。作者观察Avalonia.Controls.DataGrid的实现方式。借助AI，作者探索了如何在AddNewCellPrivate方法中修改数据单元的显示。文章指出DataGrid在使用中并不为每行创建新的DataGridCell，而是复用这些单元格。作者还分享了在EnsureGridLine方法中实现合并逻辑的过程，如何通过比较相邻行的内容来决定合并。文章提到在滚动时合并列可能出现空白的问题。


---

## 国际周报

**国际周报未更新**

## 今日人物

**罗伯特·恩卓·塔扬**（英语：Robert Endre Tarjan，1948年4月30日—），生于美国[加州](https://zh.wikipedia.org/wiki/加州)[波莫纳](https://zh.wikipedia.org/wiki/波莫纳_(加利福尼亚州))，计算机科学家，为1986年[图灵奖](https://zh.wikipedia.org/wiki/图灵奖)得主。他发现了解决[最近公共祖先](https://zh.wikipedia.org/wiki/最近公共祖先_(图论))（LCA）问题、[强连通分量](https://zh.wikipedia.org/wiki/Tarjan算法)问题、[双连通分量问题](https://zh.wikipedia.org/w/index.php?title=雙連通分量問題&action=edit&redlink=1)的高效算法，参与了开发[斐波那契堆](https://zh.wikipedia.org/wiki/斐波那契堆)、[伸展树](https://zh.wikipedia.org/wiki/伸展樹)，分析[并查集](https://zh.wikipedia.org/wiki/并查集)的工作。不少他发明的算法都以他的名字命名，以至于有时会让人混淆几种不同的算法。

![img1](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/S2WLpjoD3EDdPhHI3wGy3_1536x1024_20260308_034440_raw.jpg)

## C# .NET 交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET 性能优化经验的群组，主题包括但不限于：

* 如何找到.NET 性能瓶颈，如使用 APM、dotnet tools 等工具
* .NET 框架底层原理的实现，如垃圾回收器、JIT 等等
* 如何编写高性能的.NET 代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET 问题和宝贵的分析优化经验。**目前一群已满，现在开放二群。**可以加我 vx，我拉你进群: **ls1075** 另外也创建了 **QQ Group**: 687779078，欢迎大家加入。 