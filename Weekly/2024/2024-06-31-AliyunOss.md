.NET周刊【6月第5期 2024-06-30】dotnet_week_24_6_5
## 国内文章
### 呼吁改正《上海市卫生健康信息技术应用创新白皮书》 C# 被认定为A 组件 的 错误认知

https://www.cnblogs.com/shanyou/p/18264292

近日，《上海市卫生健康“信息技术应用创新”白皮书》发布，提到医疗信创核心应用适配方法及公立医院信息系统。文章中对C#/.NET平台的分类存在错误，C#/.NET不应被归类为A组件。文中详细介绍了C#从1.0到12的版本历程，并解释了C#及.NET平台的标准化和开源情况。指出C#自2014年起属于开源项目，版权归.NET基金会，使用宽松的开源协议，且不受美国出口管理条例限制，不存在断供问题。

### .NET 高效灵活的API速率限制解决方案

https://www.cnblogs.com/1312mn/p/18264444

FireflySoft.RateLimit 是基于 .NET Core 和 .NET Standard 构建的限流库，支持多种限流算法和策略，如固定窗口、滑动窗口、漏桶和令牌桶。其支持分布式系统，通过 Redis 实现数据共享和同步。该库还注重易用性和性能优化，提供简洁明了的 API 和丰富的示例代码。开发者可以快速将其集成到 Web API 和中间件中，实时跟踪限流情况，并动态更改规则。它能够适应各种限流场景，保护系统免受恶意请求和过载请求的侵害。

### CAP 8.2 版本发布通告

https://www.cnblogs.com/savorboard/p/18268210/cap-8-2

CAP 8.2 版本主要支持消费者独立并行执行，并在订阅者中增加更多控制消息头的行为。CAP 作为处理微服务和分布式系统中分布式事务的开源项目，此次增强了消息处理的灵活性和效率。新增特性包括 CapSubscribe 新增 GroupConcurrent 参数，实现订阅组间的并行度设置，并移除了 UseDispatchingPerGroup 配置项。同时，CapHeader 可以指定 callbackName 参数来控制补偿事务，更好地应对不同场景需求。

### C#语言编写的仅有8KB大小的简易贪吃蛇开源游戏

https://www.cnblogs.com/Can-daydayup/p/18274313

文章介绍了一款由C#编写的8KB大小的简易贪吃蛇开源游戏SeeSharpSnake，项目文件和脚本提供多种构建配置。文章详细说明了不同版本大小的构建方法，并提供了项目源码地址和相关链接。本文也宣传了DotNetGuide技术社区，鼓励开发者参与和分享。

### .NET使用CsvHelper快速读取和写入CSV文件

https://www.cnblogs.com/Can-daydayup/p/18266135

本文介绍了在.NET中使用CsvHelper开源库快速实现CSV文件读取和写入的方法。首先，介绍了CSV文件的基本概念，然后创建了一个控制台应用，并通过NuGet安装CsvHelper库。接着，定义了一个StudentInfo类，展示了如何写入和读取CSV文件的数据。最后提供了项目源码地址和更多信息的参考链接。

### 【译】Visual Studio 2022 - 17.10 性能增强

https://www.cnblogs.com/MeteorSeed/p/18254356

Visual Studio 2022 17.10 更新带来了多项性能改进。Windows Forms 设计器加载速度提升了30%-50%。Razor/C# 着色速度提升了25%。解决方案加载速度提升了10%。通过减少加载的 dll 数量，提高了低端机器的性能。用户反馈对工具改进至关重要，团队鼓励通过多种平台分享使用体验和建议。

### 为什么不推荐使用Linq?

https://www.cnblogs.com/VAllen/p/18268012/why-not-recommend-using-linq

在性能敏感型和追求零内存分配的应用中，不推荐使用Linq。通过Benchmark测试，使用Linq的性能和内存分配较差。用传统循环方法性能更优。即使优化后的Linq代码，性能差距依然明显。

### 在C#中进行单元测试

https://www.cnblogs.com/ZYPLJ/p/18270869

本文讲解了C#语言中如何进行单元测试，详细描述了单元测试的定义、作用和实施步骤。通过一个示例项目详细阐述了如何使用依赖注入创建和测试GreetingService类，使用xUnit和Moq框架模拟对象进行测试。包括项目的搭建、接口创建、类实现和测试流程三个主要部分。

### 无业游民写的最后一个.net有关项目框架

https://www.cnblogs.com/morec/p/18276172

文章讨论两种不同的开发模式。一种是按照DDD方式，根据业务需求模块化开发，不依赖公共框架，提高效率。另一种是基于公共框架的开发模式，业务人员只需编写业务代码。通过三个模块（业务模块、主机、基础模块）进行分层，业务模块以DLL形式提供给主机。文中展示了在仓储层和服务层中的通用方法，以及通过扫描assembly在主机注册服务。

### 一款开源、免费、现代化风格的WPF UI控件库 - ModernWpf

https://www.cnblogs.com/Can-daydayup/p/18268865

文章介绍了开源的WPF UI控件库ModernWpf，适用于.NET Framework 4.5+、.NET Core 3+和.NET 5+。它提供现代化控件和主题，使桌面应用程序拥有现代外观，支持浅色和深色主题。文章还提到项目的安装和源码地址，并邀请开发者加入DotNetGuide技术社区。

### [WPF]用HtmlTextBlock实现消息对话框的内容高亮和跳转

https://www.cnblogs.com/czwy/p/18273976

本文介绍了如何在WPF中实现能够局部高亮文字并支持链接跳转的消息对话框。通过HtmlTextBlock控件，支持有限HTML标签，可以展示高亮文字且实现链接跳转功能。通过修改消息对话框中的内容区域替换为HtmlTextBlock，并绑定Html内容属性，实现了目标功能。文章还提供了关键代码示例，修正了在跳转链接时的问题。

### 在WPF中使用WriteableBitmap对接工业相机及常用操作

https://www.cnblogs.com/yxllxy/p/18269391

这篇文章介绍了如何使用WPF中的WriteableBitmap类处理工业相机的图像，与WinForm中的Bitmap处理方法进行了对比，说明了图像接收、显示、像素操作和保存的具体步骤。特别强调了WPF中WriteableBitmap使用的两个缓冲区的操作方式，以及不同像素格式之间的转换问题。

### .NET下 支持大小写不敏感的JSON Schema验证方法

https://www.cnblogs.com/dotnet-diagnostic/p/18261226

本文讨论了在JSON数据验证中应对属性名大小写敏感问题的两种解决方案：一种是利用JSON Schema中的patternProperties关键字，另一种更优雅的解决方案是使用.NET库Lateapexearlyspeed.Json.Schema中的扩展选项PropertyNameCaseInsensitive。文中详细讲解了如何配置和使用该选项来实现属性名大小写无关的JSON Schema验证。

### 聊一聊 C# 弱引用 底层是怎么玩的

https://www.cnblogs.com/huangxincheng/p/18272869

该文通过讲述和对dump文件的分析，探讨了WeakReference在程序卡死中的影响，并深入研究了WeakReference的两种模式（弱短和弱长）及GCHandleType在垃圾收集中的作用。结合代码示例，说明了弱引用如何在不同场景下影响对象的复活与垃圾回收。文中还分析了coreclr源码，进一步解释了GCHandleType的工作机制。

### .net入行三年的感想回顾

https://www.cnblogs.com/jiaozai891/p/18273915

作者分享了三年工作经历，从初入职场的医疗公司，到智能制造公司，以及最后的楼下公司。总结了技术成长过程，建议新手不要进入门槛低的工控行业，并鼓励多方位发展。特别感谢曾经帮助过他的老大哥，表示将来也会传递这种帮助。

### 【译】VisualStudio.Extensibility 17.10：用 Diagnostics Explorer 调试您的扩展

https://www.cnblogs.com/MeteorSeed/p/18247891

VisualStudio.Extensibility 的 17.10 版本增强了调试体验和远程 UI 特性，新增了用户提示方法和改进的查询 API。通过 Diagnostics Explorer 工具，开发者可以调试和配置扩展，监控实时事件日志，优化激活约束。支持在 UI 中利用 XAML 资源，简化 UI 开发。使用新的 API，扩展用户可选择文件或目录。更改项目查询 API，允许开发者跟踪项目变动。此版本旨在提高扩展的开发速度、性能和可靠性。

### 【译】了解17.10 GA 中最新的 Git 工具特性

https://www.cnblogs.com/MeteorSeed/p/18270065

Visual Studio 版本控制团队发布新特性，提高开发和团队协作的生产力。新特性包括 AI 支持编写提交消息和拉取请求描述，增强拉取请求创建体验。使用 GitHub Copilot 生成提交注释和描述，需要激活订阅和启用 Git 预览功能。更新提交消息缩短输出内容。在 Commit Details 窗口中添加解释功能，使提交内容更易理解。可在 Create a Pull Request 窗口中使用工作项链接创建拉取请求。开发者社区的反馈对改进 Visual Studio 工具极为重要。

### 【WPF】根据选项值显示不同的编辑控件（使用DataTemplateSelector）

https://www.cnblogs.com/tcjiaan/p/18274217

ZWT先生的店卖拆片机，提供修改电机转向和转速的服务。因调速器笨重、不便，老周用串口和数据库解决方案简化操作。参数界面需增删改查，多种控件在动态布局中应用。老周采用ListBox、DataTemplate及DataTemplateSelector实现不同控件的动态呈现，解决了参数验证等问题。文章最后简述了拆片机背景。

### 在WPF中使用着色器

https://www.cnblogs.com/ggtc/p/18273658

本文介绍了CPU与GPU在编程方面的类比，包括二进制文件、指令、助记符、高级语言及其编译器、API和运行时环境等对比。文章还详细讲解了在3DS Max中如何编写和预览HLSL着色器的步骤，并提供了示例代码。最后，文章介绍了WPF中像素着色器的编写与使用的具体做法。

### C# pythonnet(1)_传感器数据清洗算法

https://www.cnblogs.com/KarlAlbright/p/18261015

文章展示了如何将Python代码转换为C#代码，完成数据清洗任务。Python使用pandas进行数据读取和处理，而C#使用CsvHelper、pythonnet等库进行相似操作，并调用Python库进行绘图。

### C# pythonnet(1)_传感器数据清洗算法

https://www.cnblogs.com/Cxiaoao/p/18261015

Python代码和C#代码示例展示了如何利用Pandas库和CsvHelper及pythonnet执行数据清洗操作。Python部分读取CSV数据，检测并删除异常值，最后保存清洗后数据。C#部分创建控制台程序，使用CsvHelper读取CSV，调用Python代码检测删除异常值，并绘制数据图表。

### WPF/C#：如何实现拖拉元素

https://www.cnblogs.com/mingupupu/p/18270547

这篇文章介绍了如何在WPF Canvas中实现拖放功能。通过描述xaml页面和C#代码，详细讲解了如何使用PreviewMouseLeftButtonDown、PreviewMouseMove和PreviewMouseLeftButtonUp事件处理鼠标操作，实现拖放效果。文章中还解释了隧道事件、装饰器 (Adorner) 的概念，并展示了创建和应用装饰器的过程。

### C#中关于 object,dynamic 一点使用心得

https://www.cnblogs.com/mjxxsc/p/18272628

文章介绍了 .NET 中 object 和 dynamic 类型的区别，及其在 WebAPI 接口中的应用。示范了如何使用 object 和 dynamic 接收前端传来的不确定类型数据，并通过示例代码展示了构建和解析复杂 JSON 对象的方法。文章还涵盖了一些基础知识和技巧，有助于处理结构不定的数据。

### WPF 做一个超级简单的 1024 数字接龙游戏

https://www.cnblogs.com/lindexi/p/18264294

本文介绍了一个简单的游戏开发。游戏规则是将数字放入列表，相同的数字会合并。本文提供了开发的详细步骤，包括如何使用用户控件和数据绑定来实现功能。代码示例和界面设计也详尽描述。

### 探索Semantic Kernel内置插件：深入了解HttpPlugin的应用

https://www.cnblogs.com/ruipeng/p/18266195

本文介绍了Semantic Kernel中的HttpPlugin插件及其应用。首先简要回顾了前一章的内容，然后详细解释了HttpPlugin的构造函数及其使用方法，包括如何通过HttpClient进行自定义操作。接着说明了插件的四种基本HTTP请求功能：GetAsync、PostAsync、PutAsync和DeleteAsync。文章还列举了安装必要的NuGet包和两种插件注册方式，并提供了一些实战示例，如GET和POST请求的测试代码。

### WPF/C#：BusinessLayerValidation

https://www.cnblogs.com/mingupupu/p/18267222

业务层验证在软件应用程序的业务逻辑层进行，确保数据符合业务规则，维护数据完整性和一致性。在WPF中实现业务层验证可使用IDataErrorInfo接口，提供自定义错误信息。通过在类中实现此接口，可在用户界面显示详细错误信息，帮助用户纠正输入错误。此外，WPF触发器用于在特定条件满足时改变控件外观或行为，包括属性触发器、数据触发器和事件触发器等。

### Fake权限验证小例子

https://www.cnblogs.com/aoximin/p/18258862

本地测试时，使用swagger调试时填写token不便，可通过伪造权限验证来解决。在.net框架下，通过自定义验证方案实现Fake验证。在FakeAuthenticationOptions中加入ClaimsIdentity，伪造用户信息。在FakeAuthenticationHandler中处理认证，生成ticket并注入认证结果，绕过Challenge和Forbidden。最后，将认证方案封装成中间件，便于注入和使用。

### WPF网格类型像素着色器

https://www.cnblogs.com/ggtc/p/18275543

文章讨论在WPF下使用像素着色器实现不同网格和效果的方法。通过调整纹理坐标和使用数学函数，如ceil、sin、round，生成各种网格效果，包括二分网格、四分网格、二值化网格和动态网格。最后扩展到线框网格和鼠标操控的小球视觉效果，提供具体代码示例。

## 主题

### 版本 2.8.0 · StackExchange/StackExchange.Redis
https://github.com/StackExchange/StackExchange.Redis/releases/tag/2.8.0

StackExchange.Redis 2.8.0 已发布。

此版本包括对 X509 证书链的额外检查、命令完整性检查模式以及对读取流中最后一条消息的支持。

### ReSharper 2024.1.4 和 Rider 2024.1.4 的错误修复现已推出 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/06/24/resharper-rider-2024-1-4/

ReSharper 和 Rider 2024.1.4 已发布。

此版本修复了多个错误，例如错误和死锁。

### 加入我们的 .NET Aspire 开发者日 – 提升您的云原生技能 - .NET 博客
https://devblogs.microsoft.com/dotnet/join-us-for-dotnet-aspire-developers-day/

关于 2024 年 7 月 23 日举办名为 .NET Aspire 开发者日的直播活动的公告。


## 文章、幻灯片等
### OWIN（.NET 的开放式 Web 界面）幕后花絮
https://dev.to/rasulhsn/behind-the-scenes-of-owin-open-web-interface-for-net-523d

历史和 OWIN 是什么，ASP.NET Core 的最初想法。

### 使用 .NET Upgrade Assistant 进行代码评估 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/code-assessment-with-net-upgrade-assistant/

了解如何使用 .NET Upgrade Assistant 评估您的升级。

本文涵盖了 Visual Studio 和 CLI 工具的分析，以及报告输出和共享。

### 探索生成的代码：T[]、SpanT 和不可变集合：集合表达式的幕后 - 第 3 部分
https://andrewlock.net/behind-the-scenes-of-collection-expressions-part-3-arrays-span-of-t-and-immutable-collections/

解释编译器如何扩展集合表达式。本文解释了数组、Span<T>、IEnumerable 和 Immutable 集合的行为。

### 检查 Xunit 中的成员数据中发生小数点到 Int 等转换时的行为 - Qiita
https://qiita.com/hatobeam75/items/163f398d8f87b4309d96

关于使用 MemberData 将测试数据传递给参数时需要类型转换的情况下的行为。

### 使用 Datadog 检测 .NET 凿刻的 Docker 镜像
https://medium.com/@vandonr/instrumenting-net-chiseled-docker-images-with-datadog-00b1db18f4b9

如何基于 Chiseled Ubuntu 设置 .NET Docker 映像以进行 Datadog 跟踪。

### ASP.NET Core 模型和 Razor 视图的 HTML5 验证
https://khalidabuhakmeh.com/html5-validation-for-aspnet-core-models-and-razor-views

如何使用浏览器的内置表单验证而不是默认的客户端输入验证。

本文介绍如何使用FinBuckle.HTML5Validation包。

### 如何使用 C# 正确遵循 OAuth 身份验证流程
https://dotneteers.net/how-to-use-c-to-properly-follow-oauth-authentication-flows/

了解如何实施 OAuth 身份验证流程。

### Kubernetes 和 ASP.NET Core 中的真正优雅关闭
https://dev.to/arminshoeibi/real-graceful-shutdown-in-kubernetes-and-aspnet-core-2290

如何优雅地关闭 Kubernetes 上的 ASP.NET Core 和通用主机应用程序。

文章还介绍了如何处理由于与 Ingress Controller 之间的间隙而需要额外延迟的情况。

### .NET Aspire NuGet 是云服务依赖项吗？
https://haacked.com/archive/2024/06/27/dotnet-aspire/

故事是这样的：.NET Aspire 就像云服务的 NuGet 包依赖项。

## 活动

### 使用 Blazor+ 低代码实现 .NET 资产现代化 (2024/07/04 13:30~)
https://codeer.connpass.com/event/319762/

## 库、存储库、工具等。

### ruccho/Disposify：使用 IDisposables 订阅 C# 事件！https://github.com/ruccho/Disposify

允许使用 IDisposable 管理事件订阅的源生成器。

- [[C#] 使用 IDisposable 订阅事件](https://zenn.dev/ruccho/articles/dc6f82771cf650)

## 网站、文档等
### 推文
https://x.com/filipnavara/status/1806291214884303064?s=12

![image-20240702220817327](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240702220817327.png)

---

https://x.com/jcouv/status/1805629757436084669?s=12

![image-20240702220907654](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240702220907654.png)

## 版权声明

* 国内板块由 InCerry 进行整理 : https://github.com/InCerryGit/.NET-Weekly
* 其余内容来自 Myuki WeekRef，由InCerry翻译（已获得授权） : https://github.com/mayuki/WeekRef.NET

**由于笔者没有那么多时间对国内的一些文章进行整理，欢迎大家为《.NET周刊-国内文章》板块进行贡献，需要推广自己的文章或者框架、开源项目可以下方的项目地址提交Issue或者在我的微信公众号私信。**

格式如下：

* 10~50字左右的标题
* 对应文章或项目网址访问链接
* 200字以内的简介，如果太长会影响阅读体验

https://github.com/InCerryGit/.NET-Weekly

## .NET性能优化交流群

相信大家在开发中经常会遇到一些性能问题，苦于没有有效的工具去发现性能瓶颈，或者是发现瓶颈以后不知道该如何优化。之前一直有读者朋友询问有没有技术交流群，但是由于各种原因一直都没创建，现在很高兴的在这里宣布，我创建了一个专门交流.NET性能优化经验的群组，主题包括但不限于：

* 如何找到.NET性能瓶颈，如使用APM、dotnet tools等工具
* .NET框架底层原理的实现，如垃圾回收器、JIT等等
* 如何编写高性能的.NET代码，哪些地方存在性能陷阱

希望能有更多志同道合朋友加入，分享一些工作中遇到的.NET性能问题和宝贵的性能分析优化经验。**目前一群已满，现在开放二群。**

如果提示已经达到200人，可以加我微信，我拉你进群: **ls1075**

另外也创建了**QQ群**，群号: 687779078，欢迎大家加入。 

![image-20230703203249615](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230703203249615.png)