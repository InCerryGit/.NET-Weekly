## 专题 - NanoFramework项目案例

如果有时间，我会在周报中加入一些专题和项目案例的分享，本周就是讨论.NET NanoFramework项目案例的专题，在讨论 NanoFramework 的典型案例之前，让我们先回顾一下 .NET 在嵌入式领域的历史。

2007年，.NET Micro Framework（.NET MF） 问世，作为一个针对单片机和资源受限设备的轻量级 .NET 实现。.NET MF 实现了基本的 .NET 功能集，支持 C# 和嵌入式系统编程。这使得开发人员能够在小型设备上充分利用 .NET 的便捷性和可靠性，并与各种硬件轻松兼容。

然而，随着硬件技术的不断发展和嵌入式领域对资源的需求增长，.NET MF 开始暴露出其限制，这促使了 NanoFramework 的诞生。NanoFramework 继承了 .NET Micro Framework 的优点，加入了现代 C# 特性，提高了性能，扩展了硬件支持，从而满足嵌入式开发领域的需求。

回到我们的案例，NanoFramework 成功应用于智能家居控制系统项目中，实现了实时监控和控制家庭设备的功能。NanoFramework 提供了高效的开发过程、紧凑的代码实现和跨平台适应性等多种优势，使得该项目易于扩展，功能强大。

通过了解 .NET 在嵌入式领域的发展历程，我们可以看到 NanoFramework 是这一领域技术持续突破的代表。尽管 .NET Micro Framework 不再更新，但 NanoFramework 持续推进嵌入式系统的发展和创新。

原文链接：https://nano.tokengo.top/docs/home/

### 【案例一】CSA Engineering AG 在使用 .NET nanoFramework

**公司**：[CSA Engineering AG](https://www.csa.ch/)

作为一家工程服务提供商，CSA Engineering AG 为医疗技术、客运交通和工业领域开发客户定制的硬件和软件解决方案。最近，CSA 与其中一家客户共同开发了一种以 STM32F4 微控制器为主要硬件组件、以 .NET nanoFramework 作为软件基础的通用嵌入式平台。其结果是所谓的 M4MCU-Board。

#### M4MCU-Board

对于这两个应用程序，以下关键需求非常重要：

- 广泛的通信功能，特别是远程访问的 TCP/IP，以及用于连接到 PLC 和工业传感器的 CAN 和 ModBus
- 可用的文件系统和处理较大数据文件的能力，以及实现现场配置的便利性，特别需要 USB 主机和 SD 卡功能
- 使用 C# 代码和所有公开可用的 .NET 类库，因为客户和 CSA 已经拥有大量现有代码。此外，为了提供高效的开发环境，嵌入式部分（M4MCU）和计算机应用程序可以使用相同的编程工具
- 实现安全可靠的远程软件更新功能

开发的 M4MCU-Board 通过以下组件满足了这些关键需求：

- 搭载 Cortex-M4 STM32F427 微控制器，具有 256kB 的 SRAM 和 1MB 的闪存
- 8MB SDRAM 和 8MB 闪存的外部存储
- SD 卡槽用于存储配置数据和大文件
- LED、按钮和一些通用输入输出（GPIO）用于一般交互
- 通信接口：
  - 1x USB 设备
  - 1x USB 主机
  - 1x 以太网 RJ45
  - 1x CAN
  - 1x RS485

![M4MCU-Board](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/M4MCU-503b25d7d39863e3c886eab2558cc758.jpg)

此外，还实现了多个软件功能，例如使用 Visual Studio 进行开发、部署和调试，使用 NaCl 算法进行数据加密，远程软件更新，支持 SSL/TLS、CAN、ModBus 等多种通信协议，以及使用看门狗进行软件监视。

将 .NET nanoFramework 移植到我们自己的硬件平台花费了一些时间，并需要在嵌入式软件开发方面的深入知识。但最终，.NET nanoFramework 可以成功引入，并为产品应用提供了一种舒适的开发方式，结合了一套全面的功能。

M4MCU-Board 和 .NET nanoFramework 已

经在以下应用中使用。

#### 应用程序 1：联合热电厂单元的智能网关

这些发电机同时产生热能和电能。为了优化目的，需要设置多个控制参数，例如点火时机或空燃比。这些参数必须可由维护工程师访问，无论是在发电机本身的本地访问，还是通过互联网，因为其中一些发电机安装在非常偏远的位置。此外，还记录和发送特征数据和错误信息供公司持续分析工厂效率。其中一个重要的特征数据是废气中的氮氧化物浓度。为了连续监测此值，之前的模型中也提供了一个独立单元作为改装套件。所有描述的任务都是通过使用 M4MCU-Board、.NET nanoFramework 作为基础和 C# 产品应用程序来实现的。

![M4MCU DIN 轨壳体](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/M4MCU_Housing-f3d323051a5aa91cf6323e14dd418bd7.png) *M4MCU 安装在符合 DIN 轨标准的壳体内*

![应用程序 1 中的 M4MCU](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/M4MCU_SmartGateway-0e5db9685ebec3cc5f68d17c8dc34cc7.png) *应用程序 1：智能网关（用黄色圈标出）安装在联合热电厂控制柜中*

##### 应用程序 2：展览吸引产品的控制和通信电子设备

该产品是一个 8x8x8 的 LED 立方体，用于显示文本和动画，从而吸引展览访客的注意力。LED 立方体可以进行配置，选择动画，并且操作员可以在前端进行状态监控。在后台，我们基于 Azure 产品的物联网后端正在运行。使用 M4MCU-Board、.NET nanoFramework 作为基础和 C# 产品应用程序，实现与物联网后端的通信（通过 MQTT）、动画/播放列表的转换和存储，以及通过 SPI 激活 LED。

![应用程序 2 中的 M4MCU（硬件）](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/LED-Cube-HW-1-c0186aab539cca7d4fccf6bf927dd279.png) *应用程序 2：由 M4MCU-Board 控制的 LED 立方体*

![应用程序 2 中的 M4MCU（前端）](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/LED-Cube-Application-3-64dd7e520d5d37f07316ea3654b5eb9b.png) *应用程序 2：LED 立方体配置前端界面*

### 【案例二】油田监测

**公司**: [OrgPal远程遥测](https://www.orgpal.com/)

**应用行业**: 油田

**[产品网站](https://www.orgpal.com/solutions-tank-level-monitoring)**

能源领域的服务和运营需要合规、准确和频繁的监测。对于石油和天然气公司来说，挑战在于找到一种经济实惠、可靠的系统，而并非所有的遥测系统都是相同的。

[扎恩·格利戈洛夫](https://www.linkedin.com/in/zan-gligorov-bb03a752)，[OrgPal远程遥测](https://www.orgpal.com/)的首席执行官，解释了他们的选择背后的原因。

我们的目标是创建一个现代化、简单易用的设备，可以轻松与北美各个油田中从最现代化到已有的数百个传感器进行集成。我们的硬件实现了这些目标，但我们需要一个优秀的固件来匹配它，而nanoFramework就使这成为可能。

许多解决方案使用来自许多制造商的不同组件来集成一个解决方案，导致成本高昂，维护选项更加昂贵。这种技术在设计上并不兼容，只是功能上相容，而且由于它们部署在偏远的恶劣环境中，几乎没有或者根本没有地面通信和电力供应，随着时间的推移，维护成本非常高昂。

由于nanoFramework功能丰富且易于使用，占用空间小（适用于微小的MCU），我们的解决方案在行业中具有最低的能源消耗。我们能够使用高功率的STM32 MCU，集成了完整的带天线的卫星、内置闪存/文件系统、USB、蜂窝网络支持、RTC等等，打造出一个功能强大的远程测量系统，并且能耗低。

基于PalThree的解决方案将是该行业的颠覆者。

请查看下面的照片。

![停放区的储罐](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/oil-tank-palthree-00-ebdf42754c483a03253b020a411ee211.jpg) *停放区的储罐*

![带有PalThree的储罐的近景](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/oil-tank-palthree-01-0291d4ea5c94f510d3e3249010aa3deb.jpg) *带有PalThree的储罐的近景*

![安装了PalThree的储罐在沙漠中部署](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/oil-tank-palthree-02-4404e4f0f66a5cefefbd3c5c05a32feb.jpg) *安装了PalThree的储

罐在沙漠中部署*

![为PalThree供电的太阳能电池板](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/oil-tank-palthree-03-2f283293d2835e23cfe777d43ca5c54e.jpg) *为PalThree供电的太阳能电池板*

![产品外壳中的PalThree](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/palthree-close-up-01e9da0a133e05c4e7e098399919ad11.jpg) *产品外壳中的PalThree*

### 【案例三】太阳能电厂远程监控与控制

**公司**: [Neshtec](https://neshtec.eu/)

**应用行业**: 太阳能电厂

Neshtec首次在一个项目中使用了他们自己新开发的硬件平台Neshtec-Control。该硬件平台基于STM32F7微控制器，并在.NET nanoFramework上运行。在该项目中，Neshtec-Control用于实现一个安装在污水处理厂的小于100千瓦峰值功率的光伏太阳能系统与能源供应商之间的接口。

借助Neshtec-Control，能源供应商可以远程监控系统，并进行控制，例如设置性能规范或进行紧急停机。这与Azure相连接，使得Neshtec能够执行自己的电厂监控和远程软件更新。

Neshtec-Control进行的接口转换在Modbus和IEC 60870-5-104这两种通信协议之间进行。Neshtec-Control具有模块化结构，因此可以通过.NET nanoFramework在应用层上抽象地使用不同的I/O模块，以满足项目的特定需求。结合框架的高可靠性和信息安全功能，这提高了Neshtec项目在成本和实施时间方面的效率。

请查看下面的照片。

![电厂的鸟瞰图](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/solar-plant-00-fd53439aa9781badc510b85031cd735c.png) 

*电厂的鸟瞰图*

![系统图示](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/solar-plant-diagram-00-174fe371239d5d878f4dbbc3350e76ec.png) 

*系统图示*

## 国内文章

###  ASP.NET Core 6框架揭秘实例演示[36]：HTTPS重定向

https://www.cnblogs.com/artech/p/17414159.html

HTTPS是确保传输安全最主要的手段，并且已经成为了互联网默认的传输协议。不知道读者朋友们是否注意到当我们利用浏览器（比如Chrome）浏览某个公共站点的时候，如果我们输入的是一个HTTP地址，在大部分情况下浏览器会自动重定向到对应HTTPS地址。这一特性源于浏览器和服务端针对HSTS（HTTP Strict Transport Security）这一HTTP规范的支持。ASP.NET利用HstsMiddleware和HttpsRedirectionMiddleware这两个中间件提供了对HSTS的实现。（本文提供的示例演示已经同步到《[ASP.NET Core 6框架揭秘-实例演示版](https://www.cnblogs.com/artech/p/inside-asp-net-core-6.html)》）

###  各个语言运行100万个并发任务需要多少内存？

https://www.cnblogs.com/InCerry/p/memory-consumption-of-async.html

在这篇博客文章中，我深入探讨了异步和多线程编程在内存消耗方面的比较，跨足了如Rust、Go、Java、C#、Python、Node.js 和 Elixir等流行语言。

不久前，我不得不对几个计算机程序进行性能比较，这些程序旨在处理大量的网络连接。我发现那些程序在内存消耗方面有巨大的差异，甚至超过20倍。有些程序在10000个连接中仅消耗了略高于100MB的内存，但另一些程序却达到了接近3GB。不幸的是，这些程序相当复杂，功能也不尽相同，因此很难直接进行比较并得出有意义的结论，因为这不是一个典型的苹果到苹果的比较。这促使我想出了创建一个综合性基准测试的想法。

### 由C# yield return引发的思考

https://www.cnblogs.com/wucy/p/17443749.html

 当我们编写 C# 代码时，经常需要处理大量的数据集合。在传统的方式中，我们往往需要先将整个数据集合加载到内存中，然后再进行操作。但是如果数据集合非常大，这种方式就会导致内存占用过高，甚至可能导致程序崩溃。

  C# 中的`yield return`机制可以帮助我们解决这个问题。通过使用`yield return`，我们可以将数据集合按需生成，而不是一次性生成整个数据集合。这样可以大大减少内存占用，并且提高程序的性能。

  在本文中，我们将深入讨论 C# 中`yield return`的机制和用法，帮助您更好地理解这个强大的功能，并在实际开发中灵活使用它。

### 如何自动转发接收的请求报头？ 

### https://www.cnblogs.com/artech/p/HeaderForwarder.html

了解OpenTelemetry的朋友应该知道，为了将率属于同一个请求的多个操作（Span）串起来，上游应用会生成一个唯一的TraceId。在进行跨应用的Web调用时，这个TraceId和代表跟踪操作标识的SpanID一并发给目标应用，W3C还专门指定了一份名为Trace Context的标准，该标准确定了一个名为trace-parent的请求报头来传递TraceId、（Parent）SpanID以及其他两个跟踪属性。其实我们的应用也可能会使用到分布式跟踪这种类似的功能，我们需要在某个应用中添加一些“埋点”，当它调用另一个应用时，这些埋点会自动添加到请求的报头集合中，从而实现在整个调用链中自动传递。为了实现这个功能，我创建了一个名为HeaderForwarder（[Github](https://github.com/jiangjinnan/HeaderForwarder)）的框架。本文不会介绍HeaderForwarder的设计，仅仅介绍它的使用方式，有兴趣的朋友可以查看源代码。

### 如何兼顾性能+实时性处理缓冲数据？

https://www.cnblogs.com/artech/p/batcher.html

我们经常会遇到这样的数据处理应用场景：我们利用一个组件实时收集外部交付给它的数据，并由它转发给一个外部处理程序进行处理。考虑到性能，它会将数据存储在本地缓冲区，等累积到指定的数量后打包发送；考虑到实时性，数据不能在缓冲区存太长的时间，必须设置一个延时时间，一旦超过这个时间，缓冲的数据必须立即发出去。看似简单的需求，如果需要综合考虑性能、线程安全、内存分配，要实现起来还真有点麻烦。这个问题有不同的解法，本文提供一种实现方案。

###  .NET 创建无边框的跨平台应用

https://www.cnblogs.com/hejiale010426/p/17440603.html

在创建了`Photino`应用程序以后我们发现它自带了一个标题栏，并且非常丑，我们现在要做的就是去掉这个很丑的自带标题栏，并且自定义一个更好看的，下面我们将用`Masa Blazor`提供的模板去进行实战。

### 如何让Task在非线程池线程中执行？

https://www.cnblogs.com/artech/p/DedicatedThreadTaskScheduler.html

Task承载的操作需要被调度才能被执行，由于.NET默认采用基于线程池的调度器，所以Task默认在线程池线程中执行。但是有的操作并不适合使用线程池，比如我们在一个ASP.NET Core应用中承载了一些需要长时间执行的后台操作，由于线程池被用来处理HTTP请求，如果这些后台操作也使用线程池来调度，就会造成相互影响。在这种情况下，使用独立的一个或者多个线程来执行这些后台操作可能是一个更好的选择。

### 一个.Net强大的Excel控件，支持WinForm、WPF、Android【强烈推荐】

https://www.cnblogs.com/chingho/p/17455791.html

这是一个开源的表格控制组件，支持Winform、WPF和Android平台，可以方便的加载、修改和导出Excel文件，支持数据格式、大纲、公式计算、图表、脚本执行等、还支持触摸滑动，可以方便地操作表格。

总的来说是一个可以快速构建、具有高性能、良好交互、美观的UI表格控件。

### .NET Core 程序实现 Windows 系统 Development、Staging、Production 三种环境的无感部署

https://www.cnblogs.com/czzj/p/DSPConfig.html

日常开发中，程序的环境切换是相当频繁的了，如果不同环境中的某些参数不同，那就需要每次编辑之前手动进行修改，比较麻烦，效率低下。

本文将以 .NET Core WebAPI 项目的配置方法为例，分步骤实现根据环境变量的配置参数，自动读取对应配置文件中的特殊参数值，从而达到 Development、Staging、Production 三种环境的无感部署。

### C#/VB.NET：如何从 PowerPoint 演示文稿中提取文本

https://www.cnblogs.com/Carina-baby/p/17440477.html

在学习或者日常工作中，有时我们需要把幻灯片的东西整理成文字，而从 PowerPoint 演示文稿中一张一张的整理手动复制粘贴，整个过程会非常费精力且耗时。那么怎么样才能比较轻松且快速地提取PowerPoint中的文字呢?今天这篇文章就将为你介绍如何通过编程方式提取PowerPoint中的文字，文章最后附有C#/VB.NET代码以及效果图，希望对你有所帮助。

### Linux 上的 .NET 崩溃了怎么抓 Dump

https://www.cnblogs.com/huangxincheng/p/17440153.html

训练营中有朋友问在 Linux 上如何抓 crash dump，在我的系列文章中演示的大多是在 Windows 平台上，这也没办法要跟着市场走，谁让 .NET 的主战场在**工控** 和 **医疗** 呢，上一张在 合肥 分享时的一个统计图。

## 主题

### 【英文】宣布使用新的 CLI 工具更新 .NET 升级助手！- .NET 博客
https://devblogs.microsoft.com/dotnet/upgrade-assistant-cli/

.NET 升级助手工具的控制台版本已更新。

新版本的升级助手工具现在具有与 Visual Studio 扩展相同的优势。

### 【英文】Avalonia UI v11 的第一个候选版本现已发布！
https://dev.to/avalonia/first-release-candidate-of-avalonia-ui-v11-now-available-34c8

Avalonia UI v11 候选版本现已发布。

由于存在主要的 API 更改和重大更改，我们正在通过尝试 RC 来寻求反馈。

- [版本 11.0.0 候选版本 1.1 AvaloniaUI/Avalonia](https://github.com/AvaloniaUI/Avalonia/releases/tag/11.0.0-rc1.1)

### 【英文】宣布 devtunnel CLI 的公共预览版
https://techcommunity.microsoft.com/t5/azure-developer-community-blog/announcing-the-public-preview-of-the-devtunnel-cli/ba-p/3823131

Dev Tunnel 工具命令行版本的公共预览版现已推出。

Dev Tunnel 提供了一种可以像 ngrok 一样从外部本地访问的机制，它内置于 Visual Studio 2022 中，但它也将作为命令行工具提供。

## 文章、幻灯片等
### 在 NET 中使用 Elasticsearch 和 NEST
【英文】https://medium.com/@lucasgarciaz2018/using-elasticsearch-and-nest-in-net-9821f64cfa76

了解如何使用 Elasticsearch .NET 客户端。

文章还提到了 NEST，这是一种高级操作。

### 【英文】使用 ASP.NET Core TestServer 处理 JWT 身份验证 | Jason Mitchell
https://json.codes/posts/dotnet/handling-jwt-authentication-with-aspnetcore-testserver/

单元测试 ASP.NET Core 应用程序时如何在测试服务器上处理 JWT 身份验证。

### 【英文】如何在 C# 中构建共享库并从 Java 代码中调用它
https://medium.com/@sixpeteunder/how-to-build-a-shared-library-in-c-sharp-and-call-it-from-java-code-6931260d01e5

如何使用 NativeAOT 创建 C# 共享库并从 Java 调用它。

### 【英文】了解 Dapr 工作流引擎和 .NET 中的创作工作流 | Diagrid
https://www.diagrid.io/blog/authoring-dapr-workflows-in-dotnet

如何在 .NET 中实施 Dapr Workflow 工作流和活动。

### 【英文】Blazor 中 JSInterop 的类型化异常 - Kristoffer Strube 的博客
https://kristoffer-strube.dk/post/typed-exceptions-for-jsinterop-in-blazor/

如何通过将异常转换为 .NET 端的唯一异常类型来处理 Blazor JavaScript 互操作中 JavaScript 端发生的异常。

### 【英文】使用 CommunityToolkit 在 .NET MAUI 中进行语音识别 - .NET 博客
https://devblogs.microsoft.com/dotnet/speech-recognition-in-dotnet-maui-with-community-toolkit/

.NET MAUI Community Toolkit 的 Speech-to-Text 功能的介绍性文章。

### 【英文】迭代您的欢迎体验反馈 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/welcome-feedback/

引入在 Visual Studio 预览版中引入的新欢迎页面（启动时用于项目选择、创建等的屏幕）。

新的欢迎页面现在可以显示更多元素、响应速度更快、处理 MRU 列表等。

### 【日文】.NET + AvaloniaUI制作日记⑦（ChatGPT API客户端应用：终章）
https://zenn.dev/jun_murakami/articles/a2a30d11efd14a

制作记录（最后一集）详细说明了我在使用 Avalonia UI 创建 ChatGPT 客户端应用程序时学到的知识。

### 【日文】[C#] 尝试使用源代码生成器 - Qiita
https://qiita.com/dsyuuto/items/4c13cc2234980a906863

一篇关于创建生成嵌入 Git 信息的代码的源代码生成器的文章。

### 【英文】为您的 ASP.NET Core Web API 创建 Microsoft Power App - Visual Studio 博客

https://devblogs.microsoft.com/visualstudio/create-a-microsoft-power-app-for-your-asp-net-core-web-api/

介绍使用 ASP.NET Core Web API 创建 API 的过程，支持连接到 Power App 和创建在 Visual Studio 2022 17.6 预览版 2 中添加的自定义连接器。

### 【英文】在 JetBrains Rider 中使用实时模板升级 | .NET 工具博客
https://blog.jetbrains.com/dotnet/2023/05/30/level-up-with-live-templates-in-jetbrains-rider/

了解有关利用 Rider 的实时模板的更多信息。

本文介绍了什么是实时模板、如何创建它们以及如何共享它们。

### 【英文】在您的 .NET 应用程序中正确执行 AES 加密
https://propertyguru.tech/doing-aes-encryption-correct-in-your-net-application-5d66168b5b44

了解如何在 .NET 应用程序中进行 AES 加密。

本文还涉及简单的密钥轮换等内容。

### 【英文】并发 B+ 树 — ConcurrentSortedDictionary c#/.net
https://medium.com/@mkrebser/concurrent-b-trees-concurrentsorteddictionary-c-net-f7c1c2a84141

基于 B+ 树中的 ConcurrentDictionary 的 ConcurrentSortedDictionary 实现细节的讨论。

- [mkrebser/ConcurrentSortedDictionary：ConcurrentSortedDictionary 在 (c#, .NET 7) 中的实现。它是使用并发 B+Tree 实现的](https://github.com/mkrebser/ConcurrentSortedDictionary)

### 【英文】C# worker 服务和 Kubernetes Liveness 探测
https://medium.com/@james.matson_64120/c-worker-services-and-kubernetes-liveness-probes-538c6839bbb5

如何在工作服务（控制台应用程序或 BackgroundService）中为 Kubernetes 实现 liveness 探测。

### 【英文】Serilog 日志记录和 EF Core 日志记录
https://dev.to/karenpayneoregon/serilog-logging-and-ef-core-logging-25hm

如何使用 Serilog 记录 Entity Framework Core。

### 【英文】获取 .NET 库项目以输出依赖程序集
https://weblog.west-wind.com/posts/2023/May/29/Getting-NET-Library-Projects-to-Output-Dependent-Assemblies

关于如何输出依赖程序集作为库的输出。

正常用例不需要依赖程序集本身，但在某些情况下，例如插件，也需要依赖程序集。

### 【英文】如何在 .NET 中检测全球化不变模式 - Gérald Barré
https://www.meziantou.net/detect-globalization-invariant-mode-in-dotnet.htm

检测是否在全球化不变模式下运行的技术。

### 【英文】HTTP 连接池的艺术：如何优化连接以获得最佳性能 - 开发人员支持
https://devblogs.microsoft.com/premier-developer/the-art-of-http-connection-pooling-how-to-optimize-your-connections-for-peak-performance/

云服务访问高峰期间端口耗尽导致错误的示例和连接池作为对策。

### 【英文】使用 Github 操作将您自己的 Nuget 包发布到 Github Nuget Registry。
https://pasinduprabhashitha.medium.com/publish-your-own-nuget-packages-to-github-nuget-registry-with-github-actions-939b07e8b6f5

有关如何将 NuGet 包发布到 GitHub 的包注册表的说明。

### 【英文】.NET 微优化和重构技巧 - NDepend
https://blog.ndepend.com/net-micro-optimization-and-refactoring-trick/

介绍了在将字符串用作字典中的键时如何使用“StringComparer.Ordinal”仅在 .NET Framework 上加速它，以及如何使用 ReSharper 的模式替换功能对其进行重构。

## 库、存储库、工具等。
## 站点、文档等
### 推特

**wasmtime 现在包括 WASI-http 规范和一个在 .NET 中调用 WASI-http 的示例实现**

https://twitter.com/brendandburns/status/1664684609924378625?s=12

![image-20230607221130076](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230607221130076.png)

---

**将 .NET 8 Native AOT 结果添加到 AWS Lambda .NET 演示应用程序的基准测试中。**

https://twitter.com/plantpowerjames/status/1663601337945280512?s=12

![image-20230607221152484](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20230607221152484.png)


## 版权声明

* 国内板块由 InCerry 进行整理 : https://github.com/InCerryGit/WeekRef.NET
* 其余内容来自 Myuki WeekRef，由InCerry翻译（已获得授权） : https://github.com/mayuki/WeekRef.NET

**由于笔者没有那么多时间对国内的一些文章进行整理，欢迎大家为《.NET周报-国内文章》板块进行贡献，需要推广自己的文章或者框架、开源项目可以下方的项目地址提交Issue或者在我的微信公众号私信。**

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

如果提示已经达到200人，可以加我微信，我拉你进群: **lishi-wk**

另外也创建了**QQ群**，群号: 687779078，欢迎大家加入。 
