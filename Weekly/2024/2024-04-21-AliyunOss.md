## 国内文章

### 他来了他来了，.net开源智能家居之苹果HomeKit的c#原生sdk【Homekit.Net】1.0.0发布，快来打造你的私人智能家居吧

https://www.cnblogs.com/hezp/p/18142099

三合是一位不喜欢动态编程语言的开发者，对集成米家智能家居到苹果HomeKit的现有开源解决方案不满意。因为遇到了稳定性问题以及个人编程偏好的问题，他决定使用C#创建自己的智能家居解决方案。在一番研究后，三合开发了两个SDK【MiHome.Net】和【Homekit.Net】，后者已在GitHub上发布。文中介绍了如何用Homekit.Net模拟智能设备，如开关和温度传感器，并将其添加到苹果的家庭App中，让用户通过代码控制其状态。

### .NET开源强大、易于使用的缓存框架 - FusionCache

https://www.cnblogs.com/Can-daydayup/p/18142045

大姚介绍了一个基于.NET的开源缓存框架FusionCache，该框架支持多种缓存策略，如内存、分布式、HTTP、CDN、浏览器和离线缓存，拥有缓存防崩溃、超时处理、安全故障转移等特性，并支持同步/异步操作、事件通知等功能。文章还演示了创建控制台应用来使用FusionCache，并提供了框架的GitHub链接供读者学习交流。此外，项目还被收录在C#/.NET/.NET Core优秀项目和框架精选中，作者鼓励开发者提交推荐项目。

### WPF/C#实现图像滤镜优化方案：打造炫目视觉体验！

https://www.cnblogs.com/qingxi11/p/18138196

该项目通过GPU渲染实现了C#/WPF中的图像滤镜效果，克服了传统CPU渲染在批量图像处理时的性能瓶颈。作者参照Shazzam Shader Editor编写HLSL像素着色器，生成所需的文件，并添加到类库以便在WPF项目中使用。项目用到了CommunityToolkit.Mvvm库、AduSkin样式库，并且构建了一个模块化的项目结构，支持操作区的定制化和特效的动态调整。文章提供了详细的项目实现细节和前台代码示例。

### .NET8中的Microsoft.Extensions.Http.Resilience库

https://www.cnblogs.com/vipwan/p/18138649

该文章继续讨论.NET中如何实现服务发现及弹性机制。介绍了从.NET Core 2.1开始引入的Microsoft.Extensions.Http.Polly库，并对比了该库与.NET 8及之后版本中新引入的Microsoft.Extensions.Http.Resilience库的性能差异。文章详细展示了如何使用两个库实现重试和熔断策略，并且强调了Microsoft.Extensions.Http.Resilience在性能和内存使用上的优势以及如何通过配置文件灵活配置策略。

### WPF随笔收录-实时绘制心率曲线

https://www.cnblogs.com/liulangg/p/18139940

该项目中介绍了如何在客户端实时显示心率曲线图，具体通过模拟心率监测设备数据，使用定时器推送模拟数据和自定义控件绘制心率曲线，实现了曲线的实时更新和移动。文中简要说明了绘制过程，并提供了代码链接供进一步学习。

### CAP 8.1 版本发布通告

https://www.cnblogs.com/savorboard/p/18139824/cap-8-1

CAP 8.1版本发布，增添新的配置项支持并调整了功能，包括重新默认为串行发送消息，支持MongoDB事务的Session Handle指定，添加异步事务API，AzureServiceBus配置Correlation header等。破坏性改变包括移除NATS DeliverPolicy配置项和默认改为串行发布消息。CAP是一个开源的分布式事务和EventBus项目，有广泛的社区支持和应用。

### 记一次 .NET某炉膛锅炉检测系统 崩溃分析

https://www.cnblogs.com/huangxincheng/p/18140261

一位朋友的工控软件频繁崩溃，作者通过WinDbg分析了崩溃的dump文件，发现崩溃发生在后台对象标记的bgc线程。通过执行!verifyheap命令，确认了托管堆损坏。进一步分析发现24号线程触发了一个前台GC，导致38号bgc线程抛出执行引擎异常，最终导致程序崩溃。

### 一个.NET开源的功能丰富、灵活易用的 Windows 窗口增强神器

https://www.cnblogs.com/Can-daydayup/p/18136924

SmartSystemMenu是一款开源的.NET Windows窗口增强工具，可提供窗口和进程信息展示、窗口操作、截图和文件管理、窗口管理等多种功能，适用于Windows XP SP3及更高版本，支持x86和x64系统，需要.NET Framework 4.0环境。它的源代码和安装包可在GitHub上获取，同时该项目被收录于C#/.NET/.NET Core优秀项目和框架精选清单中。此外，文章还推荐了DotNetGuide技术社区，这是一个.NET开发者技术交流平台。

### .NET开源免费的跨平台框架 - MAUI（附学习资料）

https://www.cnblogs.com/Can-daydayup/p/18147747

.NET MAUI是一款基于MIT许可的免费和开源的跨平台框架，支持C#和XAML语言开发Android、iOS、macOS和Windows系统的本地应用。它是Xamarin.Forms的更新和扩展，提供改进的性能和可扩展性，可以共享代码和UI布局，支持特定平台的定制。典型用户包括使用Visual Studio和C#有跨平台开发需求的开发者。开发.NET MAUI应用需要Visual Studio 2022的指定版本。其优点在于跨平台性、本地用户体验、项目管理便捷和现有技术栈的利用；缺点包括性能可能有损失、平台特定功能的限制、学习成本和社区支持相对较少。

### 【Nano Framework ESP32篇】WS2812 彩色灯带实验

https://www.cnblogs.com/tcjiaan/p/18138995

这篇文章介绍了如何在物联网项目中使用 LED 灯带，特别是借助 ESP32 模块和 WS2812 驱动 IC 来控制灯带的每个灯珠。作者也解释了可以通过 SPI 方式和 RMT 方式来驱动 WS2812，提到了使用 Nano Framework 使得编程变得简洁。文章还包括了一段示例代码，展示如何用 RMT 方式驱动 WS2812，并分享了硬件组装部分的一些建议。

### 一个.NET内置依赖注入的小型强化版

https://www.cnblogs.com/coredx/p/18138360

.NET生态中内置依赖注入容器虽然好用，但不支持开放泛型服务的服务工厂类型转发，作者通过研究决定继承ServiceDescriptor并扩展功能来解决这个问题。文章中还宣传了作者的新书《C#与.NET6 开发从入门到实践》。文章详细介绍了TypedImplementationFactoryServiceDescriptor类来支持从自定义工厂获取服务类型，且自定义工厂新增了Type参数传递类型信息功能。

### WPF随笔收录-DataGrid固定右侧列

https://www.cnblogs.com/liulangg/p/18140748

本文解释了在WPF项目开发中，如何自定义DataGrid控件以固定表格的右侧列。作者首先提到默认的DataGrid不支持固定右侧列，然后介绍了一个基于第三方库HandyControl及微软MVVM库的自定义控件MyDataGrid，展示了通过RightFrozenCount依赖属性和滚动同步代码使右侧列固定的方法。

### 物联网浏览器(IoTBrowser)-整合机器学习yolo框架实现车牌识别

https://www.cnblogs.com/yizhuqing/p/18140050

该文章探讨了AI技术在.Net平台的应用，作者通过研究ML.NET这一开源的机器学习框架来实现图像的分类和目标检测。初始尝试使用Visual Studio插件和Vott进行图片标注和训练，但效率低下并伴随问题。最终采用了使用Python训练yolo模型，并将其导出为onnx格式在.Net环境下调用的方法。文章详细介绍了车牌识别的步骤，并集成到IoTBrowser中，同时提供了C#和JavaScript的调用代码示例，并介绍了支持的文件格式和协议。

### .NET Emit 入门教程：第六部分：IL 指令：9：详解 ILGenerator 指令方法：运算操作指令（指令篇结束）

https://www.cnblogs.com/cyq1162/p/18133417

本文介绍了.NET中的运算操作指令和其他IL指令，例如参数加载与存储、类型转换、方法调用等，运算操作指令包括算术、逻辑、位操作和比较，用于动态代码生成中的数学运算、比较和位操作。文中列举了指令如Add、Sub、And、Or、Shl等，并通过示例代码展示了其在ILGenerator中的使用方法。

### 如何将 ASP.NET Core MVC 项目的视图分离到另一个项目

https://www.cnblogs.com/kklldog/p/18147090/split-mvc-view-to-another-project

本文介绍了如何在ASP.NET Core MVC项目中，将视图分离到另一个Razor类库项目以提高模块化程度。分离步骤包括：创建Razor类库项目并配置项目文件、将视图文件复制到新项目、在主项目中添加对新项目的引用、配置Razor视图引擎查找新项目视图的路径、调整静态资源的引用路径。文章旨在为需要在SSR场景中提升首屏加载速度的开发者提供指导。

### 使用纯c#在本地部署多模态模型，让本地模型也可以理解图像

https://www.cnblogs.com/gmmy/p/18146496

文章介绍了作者使用更新版本的llamasharp（0.11.1）实现了对llava-v1.6多模态大模型的本地部署和图像理解的过程。文章中作者分享了模型理解图像的结果，指出了其智能和速度上的局限性，并提供了改用CUDA版本以加快推理速度的方法。文章还详细展示了如何加载和部署多模态模型的源代码，以及执行推理的核心代码，并分享了一些遇到的问题，最后将更新的项目代码放在GitHub供兴趣者下载。

### Asp-Net-Core开发笔记：使用alpine镜像并加入健康检查

https://www.cnblogs.com/deali/p/18147029

本文介绍了如何使用docker优化部署AspNetCore应用，首先通过添加健康检查和修改docker-compose文件来实现服务的健康监测。其次，作者建议使用基于alpine的镜像来减少镜像大小。需要注意的是，在alpine环境下发布应用时，应选择linux-musl-x64运行时，以兼容alpine内置的musl libc。本文还计划介绍一个名为「IdentityServerLite」的项目。

### C#开发的PhotoNet看图软件 - 开源研究系列文章 - 个人小作品

https://www.cnblogs.com/lzhdim/p/18133842

作者近日忙于编程，并分享了自己使用C#开发的图片浏览管理器应用。文章中介绍了软件的使用方法，包括如何使用图片管理器浏览和设置壁纸，以及如何注册软件为默认的图片类型打开工具。此外，博文提供了项目的目录结构、详细的源码介绍、运行界面展示和源码下载链接。作者指出，该应用还可以进一步增加管理功能和窗体大小调整等特性。

### async/await 贴脸输出，这次你总该明白了

https://www.cnblogs.com/JulianHuang/p/18137189

这篇技术文章探讨了.NET中async/await的实现，及其背后的状态机概念。作者提到从初学者到高阶的难度梯度，引入了如何在Go语言中实现状态机，并将其概念运用到.NET中，即展现了状态机如异步操作的核心。文章最后以.NET编程语言中的async和await为例，详细阐述了状态机的运行过程。

### .NET Emit 入门教程：第六部分：IL 指令：8：详解 ILGenerator 指令方法：类型转换指令

https://www.cnblogs.com/cyq1162/p/18133303

本文主要介绍了.NET中的类型转换指令，包括强制类型转换、隐式类型转换和数值类型转换三个类别。文中通过示例代码展示了如何在IL代码级别使用castclass、isinst、box、unbox、unbox_any及conv系列指令进行类型转换。这些指令为.NET运行时提供了灵活性，使代码能够在不同数据类型间转换。

### 实战指南：使用 xUnit 和 ASP.NET Core 进行集成测试【完整教程】

https://www.cnblogs.com/ruipeng/p/18141877

ASP.NET Core支持集成测试，与单元测试不同，集成测试可以同时评估多个应用组件及其交互，确保数据库、文件系统和网络等组件功能正常。集成测试推荐用于重要基础结构，其他场景优先考虑单元测试。通过使用内置的内存中测试服务器TestServer，集成测试可以模仿应用在生产环境的行为。集成测试的建立需要创建测试项目、配置测试服务器客户端、执行排列-操作-断言流程及报告结果。文中还介绍了利用Microsoft.AspNetCore.Mvc.Testing包和WebApplicationFactory类简化集成测试的设置，以及测试环境的配置方法。

### Bogus 实战：使用 Bogus 和 EFCore 生成模拟数据和种子数据【完整教程】

https://www.cnblogs.com/ruipeng/p/18138134

本文介绍了在xUnit单元测试中结合xUnit.DependencyInject使用依赖注入的方法，并展示了如何使用Bogus库创建模拟数据以及EFCore生成种子数据。Bogus是一个.NET下的假数据生成器，具有丰富的数据类型支持、可重复性、易用性、内置规则、灵活性和社区支持。文章通过示例展示了Bogus生成测试数据的过程，并提供了单元测试成功的证明。还介绍了Bogus的国际化特性，包括各种地区设置和语言的支持。

### 简单写一个eventbus

https://www.cnblogs.com/aoximin/p/18068563

本文介绍了eventbus，一个基于发布订阅模式的开源框架，用于简化不同程序组件间的通信，实现松耦合连接。作者先定义了IEventBus接口及其发布、订阅、启动消费消息的方法，然后展示了IntegrationEvent类包含的基本信息，如唯一id和发生时间。后面作者解释了泛型接口和非泛型接口的设计目的，并演示了一个基于内存的eventbus实现——InMemoryEventBus，最后提到了InMemoryEventBusClient作为与外部连接的组件。

### WPF/C#：让绘制的图形可以被选中并将信息显示在ListBox中

https://www.cnblogs.com/mingupupu/p/18145295

本文介绍了如何在WPF应用程序中绘制矩形形成表格，并为表格中的单元格添加行列信息。文中详述了创建矩形、为单元格添加文本信息，以及实现单元格选中与取消选中的具体编码过程。同时，文章还使用了字典来关联每个矩形单元格与其信息，并介绍了如何使用ListBox类及其ObservableCollection的继承类SelectedRects来处理选中单元格的信息。

### 基于Material Design风格开源、易用、强大的WPF UI控件库

https://www.cnblogs.com/Can-daydayup/p/18136908

大姚分享了一款基于Material Design风格的WPF UI控件库MaterialDesignInXamlToolkit，这是一个开源、免费、易用且功能强大的库，可帮助开发者在C#和VB.Net中创建Material Design风格的UI。WPF框架专为Windows桌面应用开发，支持丰富的UI功能。项目的运行和查看方式被说明，并附上了项目源码地址。此外，这个控件库已被收录到C#/.NET/.NET Core的优秀项目和框架精选中。最后，文章提到DotNetGuide技术社区，它是.NET开发者的技术交流平台。

### 使用WebApi+Vue3从0到1搭建《权限管理系统》:二、搭建JWT系统鉴权

https://www.cnblogs.com/cyzf/p/18143537

该视频为《WebApi+Vue3搭建权限管理系统》系列之搭建JWT系统鉴权，讲解了如何在appsettings.json中配置JWT鉴权属性，创建JwtSettingModel模型与配置文件解析帮助类ConfigurationHelper，并在Startup.cs中编写鉴权代码。配置包括发行人、订阅人、过期时间、秘钥算法等。鉴权代码设置了TokenValidationParameters参数，保证了令牌的安全性。

### 记一次栈溢出异常问题的排查

https://www.cnblogs.com/anxin1225/p/18138704

开发环境下的服务程序不断崩溃，作者开启崩溃自动dump并分析，发现是栈溢出异常。通过打印堆栈，定位到问题代码，发现错误在一个对象的隐式转换操作中，由于返回了错误的类型，触发了无限递归。作者建议检查所有相关代码，表明仅凭常规方法难以找到问题，而windbg为问题排查提供了关键帮助。

### 实战指南：使用 xUnit.DependencyInjection 在单元测试中实现依赖注入【完整教程】

https://www.cnblogs.com/ruipeng/p/18134907

本文介绍了如何在xUnit项目中使用Xunit.DependencyInjection进行依赖注入的实战操作，包括安装NuGet包、创建测试类、配置依赖注入容器，并对Sample.Repository进行单元测试。文章还讲述了如何通过Startup.cs配置测试依赖和服务，以及CreateHostBuilder、ConfigureHost、ConfigureServices和Configure几个关键方法的使用。最后，演示了在StaffRepositoryTest单元测试类中如何通过构造函数获取依赖项。

### 如何实现数据库数据到Abp vnext实体对象的同步？以及代码生成工具

https://www.cnblogs.com/DinAction/p/18144756

在EF Core的Code First方式中，数据库直接操作的变更需同步到项目代码。首先可用Scaffold-DbContext命令从数据库生成实体模型和DBContext。其次，手动编写代码实现存储过程映射。应尽量通过迁移保持结构一致性。ABP vNext框架社区开发了代码生成工具，如NameIsBad/abp-vue、WuLex/AbpVnextGenerator和neozhu/abpvnextsmartcodegenerator，用于从数据库生成领域模型代码，可加快在ABP项目中的集成。选用这些工具前，需检查其更新情况和社区反馈。

### 【Azure Developer】.Net 简单示例 &quot;文字动图显示&quot; Typing to SVG

https://www.cnblogs.com/lulight/p/18139143

本文介绍了如何通过.NET Core WEBAPI项目生成SVG动图。文章首先解释了SVG图片和动画的基本概念，然后提供了一步步创建API的教程。通过设置Content-Type为image/svg+xml并输出定制的SVG代码，可以实现将文字转换为动画效果的SVG图片。实验部分展示了通过传递参数来动态生成内容的完整代码示例。

### .Net与AI的强强联合：AntSK知识库项目中Rerank模型的技术突破与实战应用

https://www.cnblogs.com/xuzeyu/p/18148685

AntSK是一个结合了.NET和AI技术的开源离线AI知识库项目，最近加入了Rerank模型来提高查询能力。它采用向量匹配技术，并针对传统方法中的局限性引入重排技术以优化搜索结果。AntSK支持Python混合编程，增强了.NET开发者的AI开发能力。新模型可通过pythonnet实现.NET与Python的集成，并优化了下载模型的流程以方便国内用户。

### 【Azure APIM】列举几种在APIM 策略中的主动生产的错误语句

https://www.cnblogs.com/lulight/p/18141734

本文介绍了在Azure API管理服务(APIM)配置诊断日志并制造错误的三种方法。首先是通过return-response策略返回指定错误码，但错误信息没有被记录。第二种方法是定义变量并直接抛出异常，还结合重试策略使错误多次出现，有助于调试。第三种是设置错误域名造成DNS解析错误，错误信息被详细记录。最后，在Log A Workspace中验证这些错误，确保第二种和第三种方法能够有效记录错误日志。

### 【ESP32 IDF】用RMT控制 WS2812 彩色灯带

https://www.cnblogs.com/tcjiaan/p/18147955

老周在.NET Nano Framework中展示了如何控制WS2812灯带，并批评了目前很多物联网和AI教程仅仅提供代码，而不讲解背后的原理，缺乏实际编程学习，特别是对于C语言的深入理解。接着，老周详细解释了ESP32的RMT功能，如何用32位数据来描述一次脉冲周期，每个周期分为两个16位的部分，对应高电平和低电平的持续时间。他强调了.Net Nano Framework使用的IDF版本与新版存在差异，但原理相似，且表示将适配新版的IDF，并简化了分频的概念，更易于新手理解。

### aop 阶段性概况

https://www.cnblogs.com/aoximin/p/18134418

文章首先解释了面向切面编程(AOP)的概念及其解决的问题，例如在多个方法中执行相同的后续操作时，如何通过AOP减少重复工作、降低出错率并增加代码优雅性。然后聚焦于AOP的滥用情况，并解释了日志和验证为何被接纳，而其他操作可能导致代码逻辑偏离本意。接着，文章讨论了实现AOP的两种技术：字节码操作和代理技术，分别列出了各自的优缺点。通过UserService的代码示例，展示了如何使用代理技术实现AOP功能。

### 使用归一化盒过滤器对图像进行平滑处理

https://www.cnblogs.com/mingupupu/p/18147819

本文介绍了归一化盒过滤器在OpenCV中用于图像平滑处理的原理与应用。归一化盒过滤器通过计算像素邻域的平均值来实现平滑效果，虽然可以去噪，但会导致图像模糊。文章通过3*3核的示例代码展示了如何自行实现这一过程，并与OpenCV自带函数的效果做了对比。最后提到自己实现的方法可以扩展适用于其他大小的核。

### C#判断窗体是否被遮挡 - 开源研究系列文章

https://www.cnblogs.com/lzhdim/p/18122548

作者之前发布了关于托盘窗体显示与隐藏的文章，但发现最大化时隐藏功能异常，于是研究并修正了窗体遮挡判断的代码。此次更新干净简洁，在博客园园友的协助下，添加了特殊窗体处理功能，使得操作类得到完善。文章描述了项目目录、源码介绍、操作类与主窗体的使用，且提供了源码下载链接。建议那些需要最大化窗体操作的用户，通过实际调试找出被遮挡坐标，并修改操作类中的特殊窗体坐标。

### Taurus.MVC 性能压力测试（ap 压测 和 linux 下wrk 压测）：.NET 版本

https://www.cnblogs.com/cyq1162/p/18135830

本文介绍了在相同电脑环境下对Taurus.MVC框架进行的.NET版本与.NET Core版本性能的对比压测。测试项目在Windows 11和IIS环境下进行。文章记录了不同并发级别下的请求每秒（qps）结果，在单线程和8线程下进行了简单接口返回的测试，并在8线程下测试了含数据库读取操作的接口。测试显示，.NET版本在8线程简单接口测试时qps为6277，高于.NET Core 8线程时的5765；同样的并发下，读数据库接口的qps为6031，也高于.NET Core 8的5470。

### winform之在主窗体中不显示子窗体的菜单栏

https://www.cnblogs.com/wuchen9527/p/18147718

本技术文章介绍了在MDi窗体中嵌入子窗体后不显示菜单栏的问题及其解决方案。在遇到主界面的子界面过多而影响程序运行效率后，决定采取MDi窗体，并发现子窗体显示时会出现菜单栏问题。通过重写WndProc方法，并处理WM_NCCALCSIZE消息，达到只计算工作区域大小，解决了问题，移除了菜单栏。作者提出了改进后的代码，并展示了实现效果。

### 【译】宣布在 Visual Studio 17.10 预览2中为 ARM64 架构提供 SSDT

https://www.cnblogs.com/MeteorSeed/p/18133834

Visual Studio 17.10预览版2为ARM64架构推出SQL Server Data Tools (SSDT)，提供SQL项目管理、模式比对、数据对比、查询编辑、表设计、数据库属性编辑和对象重构等功能。安装步骤涉及下载安装器，在可用选项中选择预览版本安装SSDT和其他组件，然后在Visual Studio创建数据库项目。Microsoft 提供反馈链接以优化Visual Studio并邀请开发者参与改进。

### WPF基础：在Canvas上绘制图形

https://www.cnblogs.com/mingupupu/p/18137691

Canvas是WPF中用于布局子元素的面板控件，它能够通过指定属性在二维空间中绝对定位元素，非常适合于绘图应用或精准UI布局。本文提供了在Canvas中绘制矩形、圆和多边形的示例代码，既包括XAML的定义方式，也涉及了C#代码的实现。这些示例展示了如何使用Canvas及其子元素的属性，如Width、Height和Fill等，以及如何通过Canvas.SetLeft和Canvas.SetTop方法来定位这些图形。

### c#采用toml做配置文件的坑过

https://www.cnblogs.com/liqi/p/18148138

这篇文章讨论了C#中使用TOML文件的经验，提到了通过Nett库读取和更新TOML文件中的数据，例如布尔、字符串、整型、双精度浮点数、时间偏移和时间跨度值。作者在尝试用Update函数修改float类型时遇到精度问题，发现Nett库中没有float类型的更新方法，导致数据精度丢失。因此作者建议在读取非整数类型时使用double类型，避免使用float，以免遇到类似问题。

### C#的窗体假关闭操作例子 - 开源研究系列文章

https://www.cnblogs.com/lzhdim/p/18120185

文章介绍了如何在C#程序中实现窗体的假关闭效果，即用户点击关闭按钮时，窗体不是真正的关闭，而是隐藏。文中提供了源代码和项目结构的简要说明，并附有源码下载链接。建议读者根据自己的需求，适当扩展该示例应用。

### C#使用PaddleOCR进行图片文字识别✨

https://www.cnblogs.com/mingupupu/p/18124485

PaddlePaddle是百度开发的深度学习平台，其开源光学字符识别工具PaddleOCR支持多语言文本检测和识别。PaddleSharp是飞桨针对C#开发者的深度学习库，使其能在C#环境中应用深度学习功能。同时提供的Winform界面设计可通过简单代码实现图片文字识别，示例演示了如何利用PaddleOCR和OpenCV进行中文文本识别，并将结果展示在界面上。

### .NET MAUI开源免费的UI工具包 - Uranium

https://www.cnblogs.com/Can-daydayup/p/18127902

《Uranium: .NET MAUI的免费UI工具包》一文介绍了UraniumUI, 一种基于.NET MAUI的开源免费UI框架，用于构建跨平台的现代应用程序界面。文章提供了安装指导、项目源码地址，解决了安装中可能遇到的问题，并分享了运行效果截图。同时，文章鼓励读者参与到DotNetGuide技术社区，以及向优秀项目和框架精选提交PR。

### 一个库帮你快速实现EF Core数据仓储模式

https://www.cnblogs.com/Can-daydayup/p/18120034

大姚分享了EF Core Generic Repository通用仓储库的使用方法，以便于.NET开发者简化数据仓储模式的实现工作。该库提供了.NET Core和.NET项目的支持，并集成了数据库事务、多种查询模式及单元测试等特点。示例代码展示了如何新建项目、安装库、创建类和上下文，以及如何进行CRUD操作。

### Taurus.MVC 性能压力测试（ap 压测 和 linux 下wrk 压测）：.NET Core 版本

https://www.cnblogs.com/cyq1162/p/18124330

最近Taurus.MVC更新优化后进行了性能压测。在.NET Core版本中，使用旧电脑（i5-9400 CPU、6核逻辑处理器、16G内存）运行基于.NET8的程序，通过ab工具在Windows 11环境下进行了不同参数的单接口压测。单线程测试时关掉日志后QPS可达3595，双线程达到5765。尽管CPU负载达到极限，测试显示关闭控制台日志的确可以提升性能。未来测试将继续关闭控制台日志，而接口也会调整为更常规的输出，以便更深入分析框架的性能。

### consul：啥？我被优化没了？AgileConfig+Yarp替代Ocelot+Consul实现服务发现和自动网关配置

https://www.cnblogs.com/xdq-zh/p/18122481

一位开发者为了优化微服务应用，准备弃用现有的ocelot+consul网关组合，改用agileConfig+yarp方案。他想通过agileConfig自动注册服务，并动态配置yarp代理来简化部署流程。通过查阅博客园文章，他成功实现了用代码动态配置yarp代理的方法，并给出了相关代码实现。

### C#的AOP（最经典实现）

https://www.cnblogs.com/dotnet-college/p/18128903

本文介绍了.NET领域面向横切面编程(AOP)的概念和实现方法。文章首先以一个GetInfo函数的示例说明了常规编程的限制，随后阐述AOP技术如何通过拦截方法，修改参数和返回值来实现程序解耦。文中通过横切面拦截主程序的方式，步骤性介绍了如何在Visual Studio中利用DeveloperSharp平台创建AOP程序，包括主程序、横切面程序的制作和配置文件的设置。着重说明了横切面程序可以在主程序执行前后进行自定义处理，以及配置文件可以简化程序变动时的处理流程。

### .NET服务发现(Microsoft.Extensions.ServiceDiscovery)集成Consul

https://www.cnblogs.com/vipwan/p/18129361

Microsoft.Extensions.ServiceDiscovery的preview5更新提供了服务注册和发现功能，并且可以简单地通过配置文件和代码集成，其中包括Config、DNS和YARP三种默认Provider。示例代码展示了如何配置appsettings.json支持服务发现，以及如何在ASP.NET Core应用中使用服务发现去模拟服务端接口和测试。此外，文章还介绍了如何扩展一个Consul服务发现Provider，包括实现IServiceEndPointProvider接口和HostNameFeature。

### [MAUI]集成富文本编辑器Editor.js至.NET MAUI Blazor项目

https://www.cnblogs.com/jevonsflash/p/18133608

本文介绍了如何将基于Web的所见即所得富文本编辑器Editor.js集成到.NET MAUI应用中。Editor.js由CodeX团队开发，可实现只读切换以及明/暗主题切换等功能。文中详细说明了获取Editor.js资源文件的方法，包括从源码构建和从CDN获取两种方式。此外，介绍了如何创建.NET MAUI Blazor项目，并将所需JavaScript和CSS文件拷贝到项目中以实现跨平台功能，最后说明了如何创建视图控件。

### .NET Emit 入门教程：第六部分：IL 指令：7：详解 ILGenerator 指令方法：分支条件指令

https://www.cnblogs.com/cyq1162/p/18130979

本文介绍了.NET Emitted编程中的分支条件指令，包括条件跳转指令、无条件跳转指令和Switch分支等。分支条件指令帮助实现了程序中的条件判断和控制转移，如beq、bgt、brtrue等，功能与高级语言中的控制结构类似，对理解和提升.NET Emit编程非常有帮助。

### 学习Source Generators之打包成Nuget使用

https://www.cnblogs.com/fanshaoO/p/18128770

本文介绍了如何将从Swagger生成实体类的Generator打包成Nuget包以便使用。首先要修改项目文件以生成Nuget包并避免作为库依赖项，还需要设置对第三方组件的依赖（例如Newtonsoft.Json）。然后编译项目生成nupkg文件，并将其上传到nuget.org。用户可以通过Nuget包管理器安装。安装后，用户需要将swagger.json文件复制过来并设置为AdditionalFiles，并修改包属性，以便在项目中使用。

### Asp .Net Core 系列：集成 Refit 和 RestEase 声明式 HTTP 客户端库

https://www.cnblogs.com/vic-tory/p/18130002

.NET平台没有Feign的直接端口，但有Refit、RestEase和feign.net等类似框架。Refit和RestEase通过定义接口描述HTTP API，并支持各种HTTP方法和异步操作。Feign.net基于.NET Standard 2.0实现类似Feign的接口。文章还展示了如何在ASP.NET Core中集成和使用Refit，包括通过NuGet安装包，创建接口定义远程API调用，以及在Startup.cs中将其注入服务。

### .NET Aspire预览5版本 发布

https://www.cnblogs.com/shanyou/p/18127925

2024年4月11日发布的.NET Aspire预览5版本，增加了对AWS的支持并优化了Azure服务，引入多项新功能如拆分Aspire.Hosting包、应用模型优化、状态更新、Visual Studio集成增强和安全性提升。新增功能包括重命名扩展方法以适配更多云服务、支持非安全传输、仪表板自定义资源状态更新、提高容器资源配置持久性、自动生成密码、Docker构建参数传递等。还改进了Azure资源和数据库管理工具，如添加Azure事件中心、NATS、Seq、SignalR、AI Search以及集成多种数据库管理系统。

### 一步一步实现 .NET 8 部署到 Docker

https://www.cnblogs.com/Earen/p/18132270

本文主要介绍了在操作系统CentOS 8下通过Docker部署应用的具体步骤。其中涵盖安装Docker、准备Dockerfile和launchSettings.json配置文件、上传源码到服务器、构建Docker镜像以及创建和运行Docker容器的详细操作。最后还提及了如何查看容器信息和检查接口是否可以正常访问。

### C#开发的绑定类型默认应用例子 - 开源研究系列文章

https://www.cnblogs.com/lzhdim/p/18118276

文章介绍了如何使用C#开发一个图片浏览工具，并解决了将该工具设置为图片扩展名默认应用以及解除绑定默认应用的问题。作者通过研究注册表操作并参考CSDN帖子中的函数实现了该功能，并提供了详细的项目目录、源码介绍、运行界面展示、使用介绍和源码下载链接。作者还建议读者根据实际需要对代码进行扩展应用，以适用于Windows 11系统。

### 【Nano Framework ESP32 篇】刷入 nanoCLR 固件以及相关问题

https://www.cnblogs.com/tcjiaan/p/18132688

老周分享了他在智能插座和远程控制项目中使用Nano Framework的经验。他认为Nano Framework比MicroPython更好用，并推荐官方的idf作为ESP32开发的框架。他还介绍了怎样正确安装idf，并批评了国产芯片的SDK问题，指出乐鑫做得不错。此外，他提到了.NET的nanoff工具用来刷固件的方便性，并详述了如何使用乐鑫官方工具和固件进行ESP32_S3的刷写过程。

### Blazor OIDC 单点登录授权实例7 - Blazor hybird app 端授权

https://www.cnblogs.com/densen2014/p/18014332

本文介绍了在Blazor应用中实现基于OpenID和OAuth2标准的单点登录功能，重点放在了Blazor WebAssembly(WASM)和不同平台的整合。内容包含了用于Google和码云Gitee登录的Blazor WASM示例，以及多个Blazor OIDC单点登录实例，如配置身份验证服务、登录信息组件、服务端管理组件、部署授权以及在不同客户端如Winform和Blazor hybird app的授权实现。文章提到了源码以及如何建立Blazor WinForms项目，并详细阐述了相关的库引用、引入授权的主要代码和配置OidcClient的关键步骤。

### Avalonia中的自绘控件

https://www.cnblogs.com/chenyishi/p/18123765

Avalonia UI框架中的自绘控件允许开发者完全控制渲染逻辑，实现高度自定义的UI元素。自绘控件具有高度自定义性、性能优化、跨平台一致性和可集成第三方图形库的优势。它们适用于自定义图表、游戏动画、特殊效果和专业工具等多样的应用场景。文章还通过示例代码展示了如何创建自绘控件并自定义事件，如何在Avalonia框架内定义和注册自定义事件，以及如何处理UI的绘制和用户交互。

### C#实现的下拉多选框，下拉多选树，多级节点

https://www.cnblogs.com/zhenzaizai/p/18120526

本文介绍了一个基于Telerik控件封装的下拉多选框和下拉多选树控件。开发者需要引用Telerik相关的dll库来使用该控件。控件支持父节点和子节点选择，代码中还提供了控件的样式定制功能，包括背景色、边框色和箭头按钮颜色等。

### 掌握 xUnit 单元测试中的 Mock 与 Stub 实战

https://www.cnblogs.com/ruipeng/p/18130083

本章介绍了在单元测试中模拟对象的概念，强调了Fake、Stub与Mock之间的区别。Fake是一个泛称，可以是Stub或Mock；Stub用于替代依赖项提供固定行为，而Mock则用于验证代码行为确保按预期执行。同时，启动了一个引入EFCore仓储模式的WebApi Controller实战项目，用于后续章节演示。

### 【译】新的 MSBuild 编辑体验

https://www.cnblogs.com/MeteorSeed/p/18123735

为了让.NET开发人员更好地理解和编辑MSBuild项目文件，发布了一个实验性的MSBuild编辑器。这个编辑器对MSBuild文件中的XML元素、属性、项和元数据提供了快速信息和深入链接，并支持智能感知、跳转到定义、查找引用等功能。编辑器还包含了针对NuGet包、语言文化等的特殊支持，能及时发现问题并提供了类型系统验证。MSBuild编辑器支持自定义schema，使得NuGet包作者可以为用户提供更好的编辑体验。这款编辑器目前只支持Visual Studio，但正在开展工作以支持Visual Studio Code。

### Avalonia中的布局

https://www.cnblogs.com/chenyishi/p/18128275

Avalonia是一个支持C#和XAML开发桌面应用的跨平台.NET UI框架。其中，Alignment决定元素在Panel内的对齐方式，Margin控制元素间的外距离，Padding调整元素内部间隔。通过这些属性和Panel，可以创建复杂界面。例如StackPanel内部的按钮通过Margin和Padding设置间隔，HorizontalAlignment调整对齐。常用Panel包括StackPanel、DockPanel等，它们有特定的布局特点，如Grid Panel用于表格布局，其中子元素可通过Grid.SetRow和Grid.SetColumn进行定位。

### Visual Studio 2022插件的安装及使用 - 编程手把手系列文章

https://www.cnblogs.com/lzhdim/p/18113429

文章介绍了如何在Visual Studio 2022中安装及使用CodeMaid插件，该插件用于代码格式化和处理。作者介绍了打开扩展窗口、查找和管理扩展，重点讲述了CodeMaid的配置和使用方法，还提供了自己的配置文件供读者下载。使用CodeMaid时，可以通过快捷键Ctrl+S保存代码文本时自动格式化处理，也可以对全部文件进行一次性处理。最后，作者预告了后续会有C#的Dll程序集类库编程的教程。

### .NET 9 预览版 3 发布

https://www.cnblogs.com/shanyou/p/18134625

.NET 9预览版3发布，带来多项性能和功能提升。主要改进包括TimeSpan.From新重载、PersistableAssemblyBuilder类支持运行时生成程序集、异常处理优化等。更新还包括内联性能提升、终端记录器改进。除了.NET核心组件更新，其他领域如.NET数据、EF Core、.NET MAUI和ASP.NET Core也有所增强。用户可通过安装.NET 9 SDK和相应的开发工具来体验这些新特性。详细信息和安装包可在GitHub上找到。

### 学习Source Generators之了解Source Generators的应用场景

https://www.cnblogs.com/fanshaoO/p/18130928

本文介绍了.NET生态系统中Source Generators的多种应用场景，包括自动代码生成、元数据处理、性能优化、支持DSL、代码分析验证和跨语言交互。Source Generators可以在编译时根据源代码生成额外代码，减少重复代码工作，避免运行时开销，提高性能和可维护性。文章推荐了一个用于学习的仓库。

### TensorRT C# API 项目更新 (1)：支持动态Bath输入模型推理

https://www.cnblogs.com/guojin-blogs/p/18125829

NVIDIA® TensorRT™ 是一款支持高效深度学习推理的 SDK，基于 NVIDIA CUDA® 技术，可以在 NVIDIA GPU 上运行且显著提高执行速度。TensorRT 兼容多种框架，通过量化和模型优化降低延迟，增强了对动态输入模型的支持。目前它提供了 C++ 和 Python 接口，而为了实现在 C# 中调用 TensorRT，开发了 C# API，并在最新的 2.0 版本中解决了数据传输问题，提高了使用便捷性和功能性。项目和应用源码已在 Github 上提供。

### Redis Stack功能介绍及redis-om-dotnet使用示例

https://www.cnblogs.com/yswenli/p/18129891

Redis Stack是一套产品，目的是简化开发人员使用Redis及其模块的体验。它包含Redis Stack Server、RedisInsight工具和各种语言的Redis Stack Client SDK。这些组件使得开发者能够更有效地构建基于Redis的应用程序。Redis Stack服务器集成了多个模块并支持Redis 6.2及Redis 7.0版本。开发者可以轻松地下载、安装并迁移现有数据到Redis Stack。它的各个组件都有其对应的开源许可，不会取代开源Redis，而是为其增加更多功能。

### 【译】使用最新预览版查看您的拉请求注释

https://www.cnblogs.com/MeteorSeed/p/18120861

Visual Studio 17.10预览版2新推出了直接在工作文件中查看GitHub和Azure DevOps拉取请求注释的功能。开发者可以在17.10预览2或更高版本中登录GitHub或Azure DevOps帐户，并开启Pull Request Comments功能体验。使用时，用户查看活动文件中的注释并进行导航，但不能查看已删除的文件或不受支持的文件类型。目前存在文中提及用户名显示为id的错误。微软寻求反馈以优化此功能，计划增加如在diff视图中查看注释等功能。鼓励开发者通过开发者社区提供反馈。

### .NET Emit 入门教程：第六部分：IL 指令：6：详解 ILGenerator 指令方法：方法调用指令

https://www.cnblogs.com/cyq1162/p/18113161

本文介绍了.NET中的方法调用指令，重点解释了Call和Callvirt指令的用途和区别，并讨论了Calli指令在委托调用中的应用。文章详述了这些指令在动态代码生成、AOP等方面的应用，帮助读者深入理解.NET平台的方法调用机制，并加强对ILGenerator的使用熟练度。

### 【译】Visual Studio 中的 GitHub Copilot：2023年回顾

https://www.cnblogs.com/MeteorSeed/p/18130331

Visual Studio通过集成GitHub Copilot，利用AI技术帮助开发者提高工作效率，管理代码库，分析异常，生成代码注释等。新功能包括内联聊天视图、斜杠命令提示意图、上下文变量优化作用域、分析修复测试失败和异常、自动见解分析工具、重命名建议、生成提交信息及断点表达式的智能感知等，尤其针对C#代码提供强化支持。这些特性可在Visual Studio 17.9及以上版本体验，旨在提高编码效率，简化开发流程。

### 创建型模式-设计模式

https://www.cnblogs.com/afei-24/p/18081931

创建型设计模式强调对象实例化的灵活性，通过封装类的信息和隐藏实例化细节来提高系统与具体类的独立性。这些模式可以是静态或动态配置，有时它们彼此竞争有时互补。文章通过迷宫构建示例解释了创建型模式，介绍了迷宫的基本组成和代码实现，并通过定义MazeGame类展示了一个创建迷宫的方法。

### 【译】如何在 Visual Studio 中安装 GitHub Copilot

https://www.cnblogs.com/MeteorSeed/p/18120119

GitHub Copilot是一个用AI帮助编程的工具，能在多种语言和框架中工作，并可学习用户代码和偏好。在Visual Studio中使用GitHub Copilot前需要GitHub账户、GitHub Copilot订阅和Visual Studio 2022 17.6或以上版本。安装包括下载扩展、运行安装程序、登录GitHub账户等步骤。GitHub Copilot用于代码补全，而GitHub Copilot Chat用于通过聊天界面解答编码问题。两者均提升开发效率但通过不同方式互动。

### gRPC入门学习之旅（六）

https://www.cnblogs.com/chillsrc/p/18132594

本文介绍了如何在Visual Studio 2022中创建gRPC服务，并实现了客户端对gRPC服务的https和http调用。内容详细解释了使用Demo.Grpc.Cmd项目和Demo.GrpcService项目，通过生成gRPC类文件及编码方式来启动和调用服务端，详细展示了如何配置和运行gRPC环境，以实现客户端和服务端的交互。

### Godot UI线程，Task异步和消息弹窗通知

https://www.cnblogs.com/gclove2000/p/18130874

本文介绍了在Godot环境下如何处理全局消息、线程安全和IOC注入，并展示了如何进行消息窗口的搭建及最简单的消息提示功能的实现。文章中提及了Godot的UI线程限制和通过C#工程化开发解决方案，以及通过使用ColorRect和VBoxContainer节点来创建UI元素，并且演示了如何通过复制节点来快速加载多个相同的UI组件。

## 主题

### .NET 9 预览 3 · dotnet/core · 讨论 #9271
https://github.com/dotnet/core/discussions/9271

.NET 9 Preview 3 已发布。

此版本向 TimeSpan.From* 添加了重载，添加 PersistableAssemblyBuilder 来存储动态生成的程序集，加快异常处理速度，内联共享泛型的运行时查找，并支持终端记录器（“dotnet”命令），这包括（输出）的可用性增强。

其他更改包括对 ML.NET Tokenizer 的增强以及始终使用 ActivatorUtilities.CreateInstance 的 ActivatorUtilitiesConstructor 属性。

### .NET 2024 年 4 月更新 – .NET 8.0.4、7.0.18、.NET 6.0.29 - .NET 博客
https://devblogs.microsoft.com/dotnet/april-2024-updates/

.NET 8.0.4、7.0.18、6.0.29 发布。

此版本是 2024 年 4 月的更新，包含多个错误修复以及 WPF 中权限提升漏洞的修复。

### ReSharper 2024.1：改进了集合、集合表达式和一次性资源的处理、新的程序集差异工具窗口等 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/04/09/resharper-2024-1/

ReSharper 2024.1 已发布。

此版本包括改进对集合表达式的支持、解析集合更改、生成格式化成员（例如“ISpanFormattable”）、改进对异步方法中 Disposable 的支持、改进对 Razor 的支持以及用于解决方案范围分析的高资源利用率模式、速度。重构的改进等等。

其他更改包括添加程序集差异视图以及使 SALIF 成为命令行工具的默认输出格式。

### Rider 2024.1：更好的调试、性能监控和游戏开发体验 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/04/09/rider-2024-1/

Rider 2024.1 已发布。

此版本添加了监视工具窗口，以在调试时显示内存使用情况和 CPU 使用情况、集合可视化工具、步骤时间显示、Blazor WebAssembly 的热重载、编辑器中的冻结行显示、新更新的项目对话框，包含类似于 ReSharper 的增强的 C# 支持。

其他变化包括对 Unity 的 Odin Inspector、.NET Aspire 插件的支持以及 AI 助手的分拆。

### dotCover、dotMemory、dotPeek 和 dotTrace 2024.1 已推出！
https://blog.jetbrains.com/dotnet/2024/04/09/dotnet-tools-241-release/

dotCover、dotMemory、dotPeek、dotTrace 2024.1 已发布。

- dotMemory 2024.1
    - 桌面MAUI应用程序支持
    - 支持冻结对象堆 (FOH)
    - Linux 和 macOS 上的新视图（类似的保留、Sunburst 对话框）
    - 在 macOS 上指定应用程序包 `.app` 而不是可执行文件的选项
    - 使用 JetBrains Rider 在 macOS 运行配置中进行分析。支持的框架：`net7.0-macos`、`net8.0-macos`
- dotTrace 2024.1
    - 桌面MAUI应用程序支持
    - UI预设（特定应用程序的UI显示配置）
    - 在 macOS 上指定应用程序包“.app”而不是可执行文件的选项
    - 使用 JetBrains Rider 在 macOS 运行配置中进行分析。支持的框架：`net7.0-macos`、`net8.0-macos`、`net7.0-maccatalyst`、`net8.0-maccatalyst`、`Xamarin.Mac`
- dotCover 2024.1
    - MAUI覆盖率分析（仅适用于.NET 7或更高版本的WinUI桌面应用程序）
    - 改进了代码覆盖率突出显示
- dotPeek 2024.1
    - 新的独立装配差异工具窗口
    - 支持WebAssembly中的WebCIL包格式

### 版本 1.5.2 - Windows 应用程序 SDK 的稳定通道发行说明 - Windows 应用程序
https://learn.microsoft.com/en-us/windows/apps/windows-app-sdk/stable-channel#version-152-15240404000

Windows App SDK 1.5.2 已发布。

此版本包含多个错误修复并添加了与小部件相关的 API。

- [发布 Windows App SDK 1.5.2 (1.5.240404000) · microsoft/WindowsAppSDK](https://github.com/microsoft/WindowsAppSDK/releases/tag/v1.5.2)

### .NET Aspire 预览版 5 - .NET Aspire
https://learn.microsoft.com/ja-jp/dotnet/aspire/whats-new/preview-5

.NET Aspire 预览版 5 已发布。

此版本包括包拆分、各种 API 更改、仪表板改进、从 Visual Studio Code C# DevKit 启动、对 Azure 事件中心、NATS 和 Seq 等组件的支持、增强的 Azure 支持以及添加的 AWS 支持。

### MSTest SDK 简介 - 改进的配置和灵活性 - .NET 博客
https://devblogs.microsoft.com/dotnet/introducing-mstest-sdk/

关于基于 MSBuild Project SDK 的 MSTest SDK 的公告。

提供包含 MSTest 必要配置的项目 SDK 提供默认值并简化使用。

### 宣布 pl/dotnet 版本 0.99（测试版）
https://www.postgresql.org/about/news/announcing-pldotnet-version-099-beta-2838/

pl/dotnet 0.99（测试版）已发布。

pl/dotnet 是一种向 PostgreSQL 添加 C#/F# 支持的机制，允许您在 .NET 中编写函数和过程。根据基准测试，C#/F# 是最快的过程语言 (PL/*)。提供 PostgreSQL 许可证。

## 文章、幻灯片等
### 使用 Dev Proxy 在 .NET 中构建和测试弹性应用程序 - .NET 博客
https://devblogs.microsoft.com/dotnet/build-test-resilient-apps-dotnet-dev-proxy/

介绍如何使用Dev Proxy模拟开发调用外部API时出现性能下降、错误、速率限制等问题。

### 如何在 Visual Studio 中使用 GitHub Copilot Chat - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/how-to-use-github-copilot-chat-in-visual-studio/

了解如何将 GitHub Copilot Chat 与 Visual Studio 结合使用。

本文介绍了使用 Copilot Chat 转换代码时的操作和预览。

### 探索集合和数据表 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2024/04/15/exploring-collections-and-datatables/

隆重推出 Rider 2024.1 中内置的集合可视化工具。

它涉及过滤、搜索以及使用新的集合可视化工具以图表格式显示等功能。

### 使用 .NET 8 简化容器构建和发布 - .NET 博客
https://devblogs.microsoft.com/dotnet/streamline-container-build-dotnet-8/

如何在 .NET 8 中使用 dotnet 命令构建和发布容器映像。

这篇文章涵盖了简单的用法、更改发行版以及凿刻/额外的图像。

### 如何使用 FakeLogger 测试日志记录
https://dev.to/canro91/how-to-test-logging-with-fakelogger-4dgc

如何在 Microsoft.Extensions.Diagnostics.Testing 中使用 FakeLogger 进行测试。

### .NET Aspire 仪表板是在本地开发期间可视化 OpenTelemetry 数据的最佳工具
https://anthonysimmon.com/dotnet-aspire-dashboard-best-tool-visualize-opentelemetry-local-dev/

如何在独立于 .NET Aspire 的本地开发中使用 .NET Aspire 仪表板作为 OpenTelemetry 的仪表板### 使用 Blazor Web App + ASP.NET Core Identity 中的自定义用户声明实现身份验证和授权
https://zenn.dev/hat_kotap/articles/421e9bc3419aa8

了解如何使用 Blazor Web App 和 ASP.NET Core Identity 实现身份验证和授权。

### Entity Framework Core 8 中对您的应用程序有用的功能
https://dateo-software.de/blog/entity-framework-8

介绍 Entity Framework Core 8 的有用功能。

文章涵盖原始集合映射、复杂类型、JSON 列和 Sentinel 值。

### 当输出超过错误日志时中断/中断 Visual Studio 的备忘录 - Qiita
https://qiita.com/kokeiro001/items/ee6221153ed868f77733

关于输出错误日志时中断调试器的想法。文章介绍了Serilog中的一个实现示例。

### 使用 Renovate 在 .NET 项目中自动更新 NuGet 包版本范围
https://dev.to/asimmon/automated-nuget-package-version-range-updates-in-net-projects-using-renovate-15il

如果在使用 Renovate 更新 NuGet 包版本时将版本指定为范围，该怎么办。


### 分析部署到应用服务的 .NET 应用的响应延迟 - Qiita
https://qiita.com/georgeOsdDev@github/items/166d9ed85c1effc648e8

介绍对部署到 Azure 应用服务的 .NET 应用程序执行性能分析的要点和工具。

- [分析部署到应用服务的 .NET 应用的响应延迟第 2 部分 - Qiita](https://qiita.com/georgeOsdDev@github/items/825bbc63679472248e1a)

### 使用带有语义内核的 JSON 模式
https://zenn.dev/microsoft/articles/semantic-kernel-v1-005

如何将 OpenAI API 的 JSON 模式（一种允许您接收 JSON 格式的答案的模式）与语义内核结合使用。

### TreatWarningsAsErrors 和 warnnaserror 不一样
https://dev.to/asimmon/treatwarningsaserrors-and-warnaserror-are-not-the-same-4h9c

关于 .csproj 中的 `TreatWarningsAsErrors` 和 `dotnet build` 中的开关 `-warnaserror` 之间的区别。

### 介绍 Visual Studio 中的新 Copilot 体验 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/introducing-the-new-copilot-experience-in-visual-studio/

介绍 Visual Studio 17.10 Preview 3 中 GitHub Copilot 相关功能的集成。

从 Visual Studio 17.10 开始，GitHub Copilot 和 Copilot Chat 已统一并作为 Visual Studio 组件的一部分提供。

### [C#]在服务器端验证Android收据的签名 - Qiita
https://qiita.com/simoyama2323/items/cdbb45031bbef405bd25

如何执行 Google Play 收据验证。

### [C#] RAG 和聊天代码示例，使用 AOAI 和 Azure AI 搜索以及 Azure.AI.OpenAI 包
https://zenn.dev/jtechjapan_pub/articles/cf284df0a1c693

使用 Azure.AI.OpenAI 与 Azure OpenAI 进行 RAG 和 Azure AI 搜索的聊天示例演练。

### 尝试使用 Dapr - 状态管理版 - Qiita
https://qiita.com/takashiuesaka/items/713499c531095d5687c2

如何在 Dapr 中使用状态管理服务。

本文还介绍了启动 Redis 的步骤、如何从 .NET 应用程序使用它以及如何将其与 .NET Aspire 链接。

### [C#] 如何在 Visual Studio 2022（.NET Framework 2.0 或更高版本）中使用旧版 .NET Framework - Qiita
https://qiita.com/diontools/items/b193ae8394161fc26698

如何在 Visual Studio 2022 中启用未正式支持的 .NET Framework。

### 并行开发 Aspire 和 Azure Functions 项目
https://zenn.dev/jtechjapan_pub/articles/d51d86c3105634

关于结合.NET Aspire和Azure Functions的项目开发配置。

### 注意使用与EF Core中MySQL的UUID_TO_BIN、BIN_TO_UUID相同的格式
https://zenn.dev/hikarin/articles/6964d684573076

如何在Entity Framework Core中将Guid转换为MySQL的`UUID_TO_BIN`、`BIN_TO_UUID`

### Visual Studio 的新解决方案格式 slnx - kkamegawa 的博客
https://kkamekawa.hatenablog.jp/entry/2024/04/12/051622

关于 Visual Studio 2022 17.0 Preview 3 中添加的新的基于 XML 的解决方案格式 .slnx。

## 活动

### 会议目录 | Microsoft Build | 2024 年 5 月 21 日至 23 日 | 西雅图
https://build.microsoft.com/en-US/sessions

Microsoft Build 的会议将于 5 月 21 日举行。

### 与 Stephen Toub 一起深入探讨 LINQ
https://www.youtube.com/watch?v=xKr96nIyCFM


Scott Hanselman 和 Stephan Toub 解释了 LINQ 实现。

### 让我们学习 .NET：容器（日语）
https://www.youtube.com/watch?v=PFUy3W-FeAY


## 网站、文档等
### 推文
https://x.com/dave_dotnet/status/1778501853312934200?s=12

![image-20240424211638903](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240424211638903.png)

## 版权声明

* 国内板块由 InCerry 进行整理 : https://github.com/InCerryGit/WeekRef.NET
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
