## 一月头条：C# 被评为2023年度编程语言！
在TIOBE指数的历史上，祝贺 C# 首次赢得了年度编程语言奖项！C# 已经是十大顶尖选手超过两个十年了，现在它正在迎头赶上四大语言，凭借一年内最大增幅（+1.43%）赢得了这个当之无愧的奖项。紧随其后的是Scratch（+0.83%）和Fortran（+0.64%）。C# 正在从Java那里夺取市场份额，并且在诸如Web应用后端和游戏（感谢Unity）等领域变得越来越受欢迎。C# 可以免费使用，并且以稳定的步伐发展，每个新版本都使语言表达能力更强。C# 来了就不会走，并且可能很快就会超过Java。

除了C#，去年TIOBE指数还有很多有趣的变化。Fortran和Kotlin成为了常驻前20名的选手，取代了长期以来的热门选择R和Perl。Fortran非常适合进行数字计算，拥有良好的库，并且在许多领域仍然是大学的宠儿。Kotlin是Java的易学/易写竞争者。有趣的问题是：哪些语言将在2024年进入TIOBE指数前20名？这很难预测。Julia在2023年短暂触及了TIOBE指数，但未能保持住这一位置。Julia语言和社区的成熟是获得第二次机会所需要的。我会把赌注放在Dart（搭配Flutter）和TypeScript上。后者已经在工业界广泛使用，但由于某些原因，它还没有在TIOBE指数中取得突破。让我们看看2024年会发生什么。-- TIOBE软件公司首席执行官 Paul Jansen

TIOBE编程社区指数是编程语言流行度的一个指标。该指数每月更新一次。评级基于全球范围内的熟练工程师数量、课程和第三方供应商。使用谷歌、必应、雅虎！、维基百科、亚马逊、YouTube和百度等流行搜索引擎来计算评级。请注意，TIOBE指数并不是关于最好的编程语言，或者编写代码行数最多的语言。

该指数可以用来检查你的编程技能是否仍然是最新的，或者在开始构建新的软件系统时做出关于应该采用哪种编程语言的战略决策。TIOBE指数的定义可以在这里找到。

https://www.tiobe.com/tiobe-index/

![image-20240107163602321](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240107163602321.png)

## 国内文章

### 马某 说c# 不开源，他是蠢还是坏?

https://www.cnblogs.com/shanyou/p/17946547

本文指出马某在视频中错误地称C#不开源且仅限于微软平台。实际上，自2014年起，C#已开源10年，包括编译器、工具集和标准库等，均在GitHub上以MIT协议公开。文章还提到龙芯中科.NET编译器团队的工作，他们针对LoongArch64架构优化了.NET生态，包括C#编译器和其他关键技术。此外，Avalonia UI在Linux桌面开发中有多个案例，尤其是在龙芯.NET平台上得到了重点支持。

### C#/.NET/.NET Core优秀项目和框架2023年12月简报

https://www.cnblogs.com/Can-daydayup/p/17944249

本文介绍了公众号“追逐时光者”定期分享的C#/.NET/.NET Core优秀项目和框架，包括项目介绍、功能特点和截图，并提供了源码地址。文中特别提到了WalkingTec.Mvvm框架，一个基于.net core的快速开发框架，支持多种前后端分离技术，并内置代码生成器；AutoMapper，一个.NET对象映射库，简化了对象映射的工作量；以及Masuit.Tools，一个全龄段友好的C#万能工具库，功能丰富，代码量小。公众号旨在为开发者提供高效的开发工具和框架资源。

### IIS通过ARR实现负载均衡

https://www.cnblogs.com/wei325/p/17939429

本文介绍了在Windows服务器上通过IIS实现负载均衡的方法。由于80和443端口被占用，无法使用nginx，故采用IIS。首先安装ARR和URL重写功能，创建三个网站：一个代理网站（8050端口）和两个服务网站（8051和8052端口）。设置好后，创建服务器场，配置站点健康检查和取消缓存。最后，通过URL重写规则将代理站端口的请求转发到负载均衡器，实现负载均衡。

### 确定了-C#是2023年度的编程语言！

https://www.cnblogs.com/Dotnet9-com/p/17950286

本文报告C#在2023年被评为年度编程语言，这是C#首次在TIOBE指数中获此殊荣。C#因在一年内增长了1.43%的市场份额而胜出，超过了Scratch和Fortran。C#正侵蚀Java的市场份额，在Web后端和游戏开发等领域越来越流行。C#是免费且开源的，每个新版本都在不断进步。TIOBE指数显示Fortran和Kotlin进入了前20名，而R和Perl被替代。尽管Julia在2023年曾短暂进入前20名，但未能保持。TIOBE指数每月更新，反映了编程语言的流行度，有助于了解技能是否过时或选择构建新系统的语言。

### 一个WPF版的Layui前端UI库

https://www.cnblogs.com/Can-daydayup/p/17940333

本文介绍了Layui-WPF，这是一个基于.NET后端开发的WPF版Layui前端UI样式库。WPF是一个创建富用户界面Windows应用的框架，而Layui是一款简约、易用的Web UI组件库。Layui-WPF项目的源代码和运行截图已展示，项目源码可在GitHub上查看，并鼓励给予Star支持。此外，该项目被收录在C#/.NET/.NET Core优秀项目和框架精选中，有助于.NET开发者了解行业动态和最佳实践。DotNetGuide技术社区提供.NET相关的学习资料和技术交流，欢迎开发者加入。

### 【ASP.NET Core】使用SignalR推送服务器日志

https://www.cnblogs.com/tcjiaan/p/17938449

本文描述了作者对产线机器人项目上位机启动流程的优化。原上位机启动缓慢，作者通过异步请求Web API、延迟连接PLC、简化窗口管理、替换日志和JSON处理库等措施，将启动时间缩短至秒级。此外，作者还改进了日志系统，最初计划将日志写入系统，后改为输出到文件，并通过Web API读取。最终，考虑到实时监控的需求和现场调试的便利，作者采用SignalR实时推送日志到上位机。这些改造显著提高了系统的效率和可用性。

### 实现一个事件总线

https://www.cnblogs.com/donpangpang/p/17939849

本文介绍了如何使用C#实现Event Bus，一种促进应用程序内部或跨组件事件通信的机制。通过定义IEvent和IAsyncEventHandler接口，以及IEventBus接口，实现了事件的发布和订阅功能。文章还展示了LocalEventBusManager类的实现，它使用Channel来存储和自动处理事件，从而实现了组件间的松耦合通信，提升了代码的可维护性和扩展性。GitHub仓库提供了完整代码。

### 【C# 技术】C# 常用排序方式

https://www.cnblogs.com/guojin-blogs/p/17938600

本文讲述了在C#中对数据排序的方法。对于基本数据类型，可直接使用Sort方法；自定义数据类型或排序规则则复杂。介绍了Sort方法的三种使用方式，包括默认排序、带比较函数的排序和自定义比较逻辑的排序。还提到了LINQ语句排序，包括原生LINQ和OrderBy方法。对于多条件排序，展示了使用Lambda表达式和LINQ语句的方法，前者通过定义委托函数实现，后者则更简单直观。

### Ef Core花里胡哨系列(10) 动态起来的 DbContext

https://www.cnblogs.com/donpangpang/p/17944918

本文介绍了如何动态管理Ef Core的DbContext。通过自定义DbContextBase类和动态生成不同AppId的DbContext，可以有效处理多子应用中动态实体更新追踪的性能问题。文章还展示了如何使用DbContextGenerator和DbContextContainer来生成和管理不同的DbContext实例，以优化数据库操作和提高性能。

### Freezable ---探索WPF中Freezable承载数据的原理

https://www.cnblogs.com/pandefu/p/17946312

本文探讨了如何在WPF中使用`Freezable`类实现`DataGridTextColumn`列的绑定隐藏。`Freezable`是`DependencyObject`的子类，可以在XAML中使用依赖属性进行绑定。文章首先回顾了`Freezable`的功能，然后通过自定义`Freezable`类和修改界面绑定方式，展示了如何在后台手动绑定列，以及如何通过`Freezable`实现数据的中转和属性变化通知。最后，通过`Code-Behind`代码的`InitDataGrid()`方法，完成了列的手动绑定。

### 构建 dotnet&amp;vue 应用镜像-&gt;推送到 Nexus 仓库-&gt;部署为 k8s 服务实践

https://www.cnblogs.com/morang/p/17938668/devops-docker-to-nexus-deploy-k8s-use

本文介绍了如何将.net core和vue项目（zhontai）打包成Docker镜像，并部署到Kubernetes（k8s）。首先需要准备k8s环境和相关中间件。文章详细描述了使用Docker打包应用镜像的流程，包括准备打包和运行所需的基础镜像，以及构建项目镜像的步骤。同时，提供了Nexus镜像仓库的安装和配置信息，以及如何将项目镜像推送到仓库。最后，介绍了如何部署前后端项目到k8s，并使用ingress解析域名到服务。

### 码农的转型之路-偶遇大佬情况或有变

https://www.cnblogs.com/yizhuqing/p/17939352

本文回顾了作者在23年最后一篇帖子的内容，并分享了最新的调研反馈，多数人对其工具的可行性和商业模式提出质疑。作者还描述了与两位业界朋友的交流，一位需要跨网络控制暖通系统，另一位是升鲜宝创始人余东升，希望开发WPF版本的分拣系统。尽管作者对余总的技术选择不认同，认为WPF开发成本高，但仍尊重不同意见，并探讨了原生与H5、APP开发的选择问题。

### dotnet-dump工具使用

https://www.cnblogs.com/lgxlsm/p/17944357

本文介绍了dotnet-dump工具，它是.NET Core官方提供的，用于生成和分析转储文件，帮助开发者诊断故障。在Linux上，根据系统类型使用yum或apt安装。安装dotnet-dump前需先安装dotnet-sdk。使用dotnet-dump collect命令生成转储文件，再用dotnet-dump analyze命令分析。分析时，可用SOS命令识别大内存对象，查找对象分布和应用根，有助于发现内存问题。分析生产环境的大文件时，需要较高的机器配置。

### 聊一聊 C# 的线程本地存储TLS到底是什么

https://www.cnblogs.com/huangxincheng/p/17940282

本文讲述了C#中的`ThreadStatic`属性，它是基于C++的线程本地存储机制。C#通过`ThreadStatic`将变量与线程绑定，实际上是CLR利用`ThreadLocalInfo`结构体在底层实现的。文章还介绍了Windows的两种TLS技术：动态TLS和静态TLS。C#使用的是静态TLS，它在编译时声明，在每个线程的堆上复制数据。静态TLS的数据存放在PE文件的.tls节点，并通过`_TEB.ThreadLocalStoragePointer`指向的数组管理。

### 助力项目快捷实现国际化，造个多语言轮子

https://www.cnblogs.com/fanshaoO/p/17944667

本文介绍了一个多语言项目管理工具，旨在简化和自动化多语言资源的处理。该工具支持自动翻译、资源共享、实时同步和多格式导出，通过API和SignalR实现资源的即时更新。它还提供.NET SDK接入，适用于多种应用场景，如后端国际化、Web和APP项目。项目开源，测试环境可供体验和反馈。

### 由浅入深理解C#中的事件

https://www.cnblogs.com/mingupupu/p/17946032

本文详细介绍了C#中事件的概念和使用方法。事件是一种特殊的委托，用于在对象间传递消息，它包含私有委托，只能添加、删除或调用处理程序。文章解释了发布者和订阅者的角色，以及事件处理程序的定义和触发事件的过程。通过示例代码展示了如何声明委托类型、事件、注册事件处理程序以及如何在发布者类中触发事件。订阅者类通过注册其方法到事件上，当事件被触发时，相应的方法会执行。

### Ef Core花里胡哨系列(7) 使用Ef Core也能维护表架构？

https://www.cnblogs.com/donpangpang/p/17942407

本文讲述了如何使用Ef Core的迁移功能来维护数据库表架构。通过创建Operation对象，Ef Core能够生成对应的Sql语句，减少了与特定数据库Sql语法的耦合。文章还介绍了两种使用Operation的方法：直接创建并填充Operation对象，以及类似于迁移文件的写法。这两种方法都需要引用相应的数据库提供程序，以生成和执行Sql语句。通过这种方式，Ef Core提供了一种灵活且高效的表架构维护手段。

### 在C#中，如何以编程的方式设置 Excel 单元格样式

https://www.cnblogs.com/powertoolsteam/p/17929835.html

本文介绍了如何使用GcExcel组件修改Excel单元格样式。包括文本颜色、边框、字体样式、对齐缩进、文本方向和旋转角度等。文本颜色可以突出重要数据，边框划分数据区域。字体样式包括加粗、斜体和下划线。对齐缩进调整段落格式，文本方向适用于特定语言，旋转角度有助于垂直文本显示。GcExcel通过IRange接口和相关属性实现这些功能，提高了Excel文件处理的效率和效果。

### 《实现领域驱动设计》—实体

https://www.cnblogs.com/afei-24/p/17920098.html

开发者在软件开发中往往先考虑数据属性和关系，而非领域概念，导致实体模型中getter和setter方法泛滥。实体是具有唯一标识和可变性的领域对象，可以追踪其变化。设计实体时，应关注其唯一标识和查找方式，而非属性和行为。实体的唯一标识有助于维持其身份，但不一定有助于查找匹配。创建实体标识的策略包括用户输入、程序生成、数据库生成和限界上下文决定。ORM工具如Hibernate处理实体标识时可能与领域模型冲突，可采用委派标识解决，通常隐藏于外界。层超类型是一种抽象基类，隐藏委派主键，所有实体都扩展自该基类，使客户端不关心委派标识。

### 【OpenCV】在MacOS上使用OpenCvSharp

https://www.cnblogs.com/guojin-blogs/p/17948569

本文介绍了OpenCV和OpenCvSharp的安装与配置过程。OpenCV是开源的计算机视觉库，支持多种编程语言和操作系统。OpenCvSharp是其在.Net平台的封装库。文章详细说明了在Mac OS上使用Visual Studio Code和.NET 6.0环境下，如何创建控制台项目、添加Nuget包，并通过示例代码测试OpenCvSharp库的功能，最终实现图像读取和处理。

### 【OpenCV】在 Mac OS 上使用 EmguCV

https://www.cnblogs.com/guojin-blogs/p/17945244

本文介绍了如何在Mac OS上使用EmguCV，一个跨平台的OpenCV .Net包装器。首先，使用Visual Studio Code和.NET 6.0框架设置编码环境。然后，通过dotnet指令创建并测试控制台项目。接着，添加Emgu.CV官方包和运行依赖包，并手动配置缺失的libcvextern.dylib文件。最后，通过编写代码测试应用，验证EmguCV的功能。

### Kernel Memory 入门系列：异步管道

https://www.cnblogs.com/xbotter/p/17941210/kernel_memory_async_pipeline

本文介绍了Kernel Memory的异步管道处理机制。异步管道允许文档在导入后立即返回，通过注册消息队列和后台任务，实现文档处理的异步化。文档保存在分布式文件存储中，消息队列负责传递消息，后台任务监听队列并触发处理流程。客户端可查询文档状态，从而提高了处理效率，避免了阻塞。

### 编写.NET的Dockerfile文件构建镜像

https://www.cnblogs.com/hejiale010426/p/17944627

本文讲解了如何为WebApi项目创建Dockerfile，以便使用Docker容器部署。首先，选择.NET 7.0 SDK作为基础镜像，并设置工作目录和暴露端口。接着，使用.NET SDK镜像构建项目，并将构建结果输出到指定目录。最后，从构建阶段的镜像中发布应用，并在最终镜像中配置启动命令，以运行.NET Core项目。

### Visual Studio 2022版本17.8中的实用功能

https://www.cnblogs.com/Can-daydayup/p/17948296

本文介绍Visual Studio 2022版本17.8的四个功能：保留大小写的查找替换、文本差异比较的摘要视图、多存储库限制提升至25个、代码搜索导航的状态栏结果计数。同时，提到DotNetGuide技术社区，它是.NET开发者的开源社区，提供学习资料、技术分享、项目推荐和招聘信息，旨在帮助开发者成长。

### aspnetcore使用websocket实时更新商品信息

https://www.cnblogs.com/morec/p/17947739

本文通过动图演示了效果，然后展示了获取商品目录的代码逻辑。代码中定义了一个API接口，用于查询商品信息，支持分页和按ID筛选。如果提供了ID，接口会返回对应的商品数据；如果没有提供ID，接口则返回所有商品的分页列表。

### 【Azure APIM】APIM 策略语句如何来设置多个Cookie值让浏览器保存

https://www.cnblogs.com/lulight/p/17946065

本文讨论了在APIM的`<return-response>`策略中设置多个Cookie值的问题。两种尝试方法：一是将多个Cookie值用分号拼接，二是使用多个set-header节点，但这两种方法都只能保存一个Cookie值。

### 日志记录升级(中间件全局日志)

https://www.cnblogs.com/zhang-3/p/17943024

本文讲述了如何在.NET中记录每个请求的日志并存入数据库。首先，通过实现IAsyncActionFilter接口创建一个日志记录过滤器，该过滤器能够捕获每个action方法的请求信息。然后，定义一个LogActionFilter类，它在action执行后记录操作详情，包括是否有异常、控制器、动作、请求路径和操作者等信息，并通过日志服务将日志信息异步存入数据库。最后，将这个过过滤器注入到全局过滤器中，以便自动应用于所有控制器的动作。

### ASP.NET Core 8 的内存占用可以更低吗？

https://www.cnblogs.com/shanyou/p/17929487.html

.NET 8引入了名为“动态适应应用程序大小”（DATAS）的服务器GC新特性，允许动态调整托管堆数量，以平衡吞吐量和内存占用。DATAS默认关闭，可通过环境变量或MSBuild属性启用。它适用于内存受限环境，如Docker容器，能在请求高峰自动增加堆数量，提高吞吐量，闲时减少内存使用。服务器GC与工作站GC不同，前者针对服务吞吐量优化，后者适用于客户端应用，频繁GC以减少延迟。DATAS结合了两者优势，动态调整以适应负载变化。要使用DATAS，需在.NET 8应用中设置相应配置，但不能与GCHeapCount选项同时使用。

### 记一次 .NET某股票交易软件 灵异崩溃分析

https://www.cnblogs.com/huangxincheng/p/17932438.html

本文分析了一个程序偶发性崩溃的问题。作者通过WinDbg工具的自动化分析命令发现，程序崩溃是由于栈上的安全检查值（cookie）被破坏，这通常是由栈溢出引起的。进一步分析指出，问题出现在`RtlAllocateLUnicodeString`函数，该函数在退出时检查到cookie被破坏，导致程序异常终止。作者还提到了电离辐射可能导致的bit翻转问题，但本例中的崩溃与此无关。

### 【类型转换】使用c#实现简易的类型转换(Emit，Expression，反射)

https://www.cnblogs.com/1996-Chinese-Chen/p/17932654.html

本文讨论了在ASP.NET MVC框架中使用EntityFramework时，通过SqlQuery方法查询数据转换效率低下的问题。作者尝试使用Emit和表达式树优化性能，最终通过DataCommand和DataReader实现硬赋值，提升了80%的性能。文章还分享了IL代码的学习经验，并提供了集合转换的示例代码，鼓励读者自行扩展功能。

### .NET开发中合理使用对象映射库，简化和提高工作效率

https://www.cnblogs.com/Can-daydayup/p/17925894.html

本文讲述了对象映射库的好处和AutoMapper的使用方法。对象映射库能减少重复代码，提高开发效率和代码质量。AutoMapper是.NET中的一个库，通过预定义映射规则，自动转换对象，简化了开发者的工作。文章以创建控制台应用为例，介绍了如何安装AutoMapper包，定义源对象和目标对象，并配置映射规则。这些步骤帮助开发者快速实现对象间的映射，提升开发效率。

### Net 高级调试之十五：经典的锁故障

https://www.cnblogs.com/PatrickLiu/p/17925615.html

本文是《Net 高级调试》系列的第十五篇，介绍了在C#项目调试中解决锁问题的方法，包括死锁、孤立锁、线程中止等问题。文章首先回顾了锁的实现逻辑，然后详细讲解了如何识别和处理这些锁问题，强调了深入理解Net框架底层对调试的重要性。调试环境包括Windows 10、Windbg Preview、Visual Studio 2022和Net Framework 4.8。文章还提到了源码调试的重要性，并举例说明了如何通过具体代码来验证所学知识。

### Taurus .Net Core 微服务开源框架：Admin 插件【4-8】 - 配置管理-Mvc【Plugin-Limit 接口访问限制、IP限制、Ack限制】

https://www.cnblogs.com/cyq1162/p/17934709.html

本文介绍了Taurus .Net Core微服务框架中的系统配置节点，包括接口访问限制、IP限制和Ack限制。系统配置提供了对内网IP、后台管理界面、自动化接口测试文档和微服务通讯的限制忽略选项。访问频率限制功能允许动态调整最大TCP连接数和设定特定时间内的最大请求次数。IP黑名单限制可同步到所有客户端应用。Ack验证增强了网络请求安全，要求客户端请求带上特定算法生成的ack头，后端验证其合法性和一次性使用。文章最后提到作者正在开发分布式事务插件。

### 从Redis读取.NET Core配置

https://www.cnblogs.com/zhaorong/p/aspnet-configuration-redis.html

本文讲述了如何在.NET Core应用中创建自定义配置源和提供程序，以从Redis读取配置。首先，.NET Core应用支持多种配置源，如json、xml、ini文件等，并可同时添加多个配置源。配置数据以键值对字典形式存储，键的格式为"Node1:Node2:abc"。Redis的Hash数据结构适合存储这种格式的配置数据。文章接着介绍了如何使用StackExchange.Redis包在.NET应用中实现Redis配置提供程序，包括安装NuGet包、创建RedisConfigurationProvider和RedisConfigurationSource类，以及如何读取和转换Redis中的配置数据。

### 01的token的年度总结

https://www.cnblogs.com/hejiale010426/p/17935796.html

本文作者是.NET爱好者token，来自湖南衡阳，曾与多位老乡交流，如李哥。他在.NET领域成长迅速，从Java转向.NET，逐渐深入开源社区。在实习期间，他通过阅读微软官方文档，不断提升自己，从三层架构到接触Abp框架，每次学习都是新挑战。他在开源社区贡献代码，如nanoframework和AvaloniaUI文档翻译，参与MASA Blazor组件库开发，并自创多个开源项目，如ChatGpt.Desktop和EarthChat。他还提供了几点建议给新手：找人带学习，设定目标，规划开源项目。过去一年，他学会了Blazor技术，录制教程，学习Avalonia框架，深入研究ABP框架和Openiddict库，并尝试结合React和openiddict重构授权中心。他掌握了多种技术栈，如React、Blazor、.NET等，并提供了联系方式和技术交流群。

### 记一次 .NET某工控 宇宙射线 导致程序崩溃分析

https://www.cnblogs.com/huangxincheng/p/17925800.html

本文分析了程序崩溃的原因，作者在知乎上看到一篇关于程序因宇宙射线或太阳耀斑导致bit位翻转而崩溃的文章，感到兴奋。通过Windbg工具分析，发现程序在后台垃圾回收标记阶段时，托管堆上出现坏对象，导致CLR执行引擎异常。进一步使用命令验证，确认了托管堆内存布局被破坏，特别是TreeNode.children的MethodTable不正确，导致CLR无法识别内存对象，从而引发崩溃。

### 在macOS中搭建.NET MAUI开发环境

https://www.cnblogs.com/jevonsflash/p/17937122

本文指导如何在macOS Monterey及以上版本电脑上，使用Visual Studio Code开发并调试MAUI项目。首先安装XCode13.3以上版本和Visual Studio Code，再安装.NET MAUI扩展和.NET 8。通过终端命令安装MAUI工作负载和Xcode命令行工具，以便调试iOS应用。对于Android应用，需下载并安装JDK，创建.NET MAUI项目，并构建项目以安装Android SDK。若需使用模拟器，需安装模拟器、镜像，并创建虚拟机。通过命令面板可创建新的Android模拟器，完成调试环境设置。

### 数据智慧：C#中编程实现自定义计算的Excel数据透视表

https://www.cnblogs.com/powertoolsteam/p/17925408.html

本文介绍了如何使用Java在GcExcel中为数据透视表添加计算项，以便进行自定义数据分析。通过五个步骤：加载工作簿、创建数据透视表、添加计算项、隐藏重复项和保存工作簿，可以将数据按需求分类汇总。例如，将订单状态分类为“完成”和“未完成”，并计算“未完成”状态的产品金额总和。计算项功能使数据透视表的分析更加灵活和深入。

### 使用C#如何监控选定文件夹中文件的变动情况？

https://www.cnblogs.com/mingupupu/p/17933098.html

本文介绍了如何在C#中使用FileSystemWatcher类监控文件夹变动。文章分为前言、效果展示、具体实现和总结四部分。具体实现包括界面设计和全部代码，界面设计简洁，代码部分展示了如何创建FileSystemWatcher实例、设置属性、注册事件处理函数，并通过FolderBrowserDialog让用户选择监控文件夹。监控事件包括文件改变、创建、删除和重命名，且支持子目录监控。

### Kernel Memory 入门系列：文档的管理

https://www.cnblogs.com/xbotter/p/kernel_memory_document_tag.html

本文介绍了Kernel Memory入门系列中文档的管理方法。通过Document对象，可以批量上传文件并管理，自定义DocumentId或使用系统生成的随机ID。使用Tag标记文档属性，如类型、来源等，便于后续检索时筛选。检索时，可通过Tag或DocumentId进行范围筛选，支持复杂的And和Or条件组合。文档更新时，指定DocumentId上传新文件即可自动替换。删除文档也通过DocumentId实现。此外，Index参数用于文档隔离，确保检索时的独立性。

### Json Schema简介和Json Schema的高性能.net实现库 LateApexEarlySpeed.Json.Schema

https://www.cnblogs.com/dotnet-diagnostic/p/17927879.html

本文介绍了Json Schema，一种用于描述Json数据结构和限制的声明式语言。它允许定义Json规则，确保数据格式一致性。Json Schema解决了复杂验证需求和动态Json结构问题，提供了标准化的Json理解和验证方法。文章还展示了如何使用.net库LateApexEarlySpeed.Json.Schema进行Json验证，包括验证失败时的详细输出信息。该库基于最新Json Schema草案，特点是高性能，使用System.Text.Json，通过官方测试套件验证。

### Kernel Memory 入门系列：自定义处理流程

https://www.cnblogs.com/xbotter/p/kernel_memory_custom_handler.html

本文介绍了Kernel Memory的自定义处理流程。用户可以通过实现`IPipelineStepHandler`接口来创建自定义Handler，以修改数据流程。自定义Handler可以访问和修改`DataPipeline`中的数据，还可以利用`IPipelineOrchestrator`来读写文件和获取基础组件。完成自定义Handler后，需要将其注册到Kernel Memory中，以便在Pipeline中使用。通过这种方式，用户可以根据需求定制文档预处理的步骤，实现更加灵活的数据处理流程。

### Kernel Memory 入门系列：生成并获取文档摘要

https://www.cnblogs.com/xbotter/p/kernel_memory_summaries.html

本文介绍了Kernel Memory入门系列，重点是如何生成和获取文档摘要。通过Kernel Memory，用户可以导入文档并指定Summary流程来生成摘要，该流程包括提取、总结、生成嵌入和保存记录等步骤。生成的摘要不是文档的分片，而是经过语言模型总结后的内容。检索摘要时，使用`SearchSummariesAsync`方法，通过文档过滤条件来获取。摘要生成和检索过程涉及数据类型标记和自定义筛选。此外，还可以自定义其他文章处理流程，如分类、关键词提取等。相关参考资料提供了更多信息和代码示例。

## 主题

### 发布版本 v2.60.0 · grpc/grpc-dotnet
https://github.com/grpc/grpc-dotnet/releases/tag/v2.60.0

### Visual Studio 2013 停用：对旧版本 Visual Studio 的支持提醒 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/visual-studio-2013-retirement-support-reminder-for-older-versions-of-visual-studio/

### 宣布推出适用于 .NET 的 Azure Migrate 应用程序和代码评估工具 - .NET 博客
https://devblogs.microsoft.com/dotnet/azure-migrate-app-and-code-assessment-tool-release/

## 文章、幻灯片等

### 使用 TensorFlow.NET 和 C# 重温“从实现中学习深度学习”（作者：@Nezura） - Qiita
https://qiita.com/C5D5E5/items/9de54719f853ef375e95

### 使用 SearchValues 提升 .NET 8.0 中的字符串搜索性能 | endjin
https://endjin.com/blog/2024/01/dotnet-8-searchvalues-string-search-performance-boost

### [C#]使用VS2022的源生成器简介
https://zenn.dev/mkmonaka/articles/8b9c1a87e35313

### 在 macOS/Linux 上本地运行包含本机库的 Azure Function 时出错
https://zenn.dev/karamem0/articles/2023_12_30_090000

### 使用 Visitor 模式消除基于类型的 switch 和 if 判断 - Qiita
https://qiita.com/toRisouP/items/d96a09fab827af17fb37

### F# 中更安全的递归 - .NET 博客
https://devblogs.microsoft.com/dotnet/safer-recursion-in-fsharp/

### 让我们看一下 Semantic Kernel v1.0.1 插件
https://zenn.dev/microsoft/articles/semantic-kernel-v1-003

### 什么是.NET Aspire？ - 概览 - 奇塔
https://qiita.com/takashiuesaka/items/f45e930ef296c5710acc

### 尝试使用 .NET Aspire - Qiita
https://qiita.com/takashiuesaka/items/8794f99b0bf3ce3c3106

### 部署 .NET Aspire - Qiita
https://qiita.com/takashiuesaka/items/3da744d0511f29270299

### 使用 .NET Aspire（使用 YARP）配置 Next.js + ASP.NET Core - Qiita
https://qiita.com/takashiuesaka/items/e167852af299a7b00939

### 将 Prometheus、Jaeger、Grafana 与 .NET Aspire 一起使用 - Qiita
https://qiita.com/takashiuesaka/items/4811e62aa52e39ed834c

### 在 Azure 中为 Windows 应用程序创建 CI/CD 环境：DevDrive 的效果如何？ - 奇塔
https://qiita.com/spc_ksudoh/items/42d7ab8ad27c475d011c

### 在 Visual Studio 中使用 Git 提高工作效率的一年 - Visual Studio 博客
https://devblogs.microsoft.com/visualstudio/a-year-of-making-you-more-productive-using-git-in-visual-studio/

### 在 .NET 中使用 PBKDF2 进行进化且强大的密码散列
https://dev.to/asimmon/evolutive-and-robust-password-hashing-using-pbkdf2-in-net-34pc

### 可删除优先级队列 - Qiita
https://qiita.com/saka_pon/items/7d42012e44978580a0c0

### 使用 perf 对 Linux 上的 .NET 应用程序进行紧急 CPU 使用情况分析的简短指南
https://igorexplains.medium.com/a-short-guide-to-urgent-cpu-usage-profiling-of-net-applications-on-linux-using-perf-1e0dbd1f0533

### .NET 9 中的新锁类型
https://steven-giesel.com/blogPost/d7f923b3-13ff-4ecc-8b8f-d847ae581f68

### .NET Native AOT 解释 - NDepend 博客
https://blog.ndepend.com/net-native-aot-explained/?WT.mc_id=link-twitter-isaacl

### IntelliSense 对 C# 12 新特性“主构造函数”的神圣支持 - xin9le.net

https://blog.xin9le.net/entry/2023/12/27/220943

### .NET Semantic Kernel v1.0 无法使用的子Handlebars模板的使用方法及注意事项
https://zenn.dev/microsoft/articles/semantic-kernel-v1-002

### .NET Semantic Kernel v1.0 已经发布了，所以我又回顾了一下。
https://zenn.dev/microsoft/articles/semantic-kernel-v1-001

### 使用 Quartz.NET 安排作业
https://zenn.dev/oyasumi731/articles/6611ecad604d41

### 了解 C# 线程、线程池和任务
https://zenn.dev/higty/articles/fea5f57cd1b1c2

### 使用 C# 序列化餐厅表格
https://blog.ploeh.dk/2023/12/25/serializing-restaurant-tables-in-c/

### [C#] 一个关于创建一个可以轻松快速地接收来自竞争性程序等的输入的库的故事 - Qiita
https://qiita.com/Kujiro/items/facad439eb0873748f87

### 如何在 C# 中成功创建方法链第 1 部分 - Qiita
https://qiita.com/dhq_boiler/items/61752b74db5f1fa6dfd5

### 在微服务架构中使用 Jaeger 和 OpenTelemetry 进行分布式跟踪
https://medium.com/@ebubekirdinc/distributed-tracing-with-jaeger-and-opentelemetry-in-a-microservices-architecture-62d69f51d84e

### 使用 C# 创建您自己的双端队列 - Qiita
https://qiita.com/YuHima03/items/e52fdebdf626192c4b1e

### 由于 OpenSilver 2.0 与 VB 兼容，我尝试显示 Hello World! - Qiita
https://qiita.com/yaju/items/8f210bcc90222fe8826f

### 在 Fluent UI Blazor 中使用开关的指南
https://zenn.dev/tomokusaba/articles/bec7719e8dc282

### 尝试使用语义内核获取天气
https://zenn.dev/tomokusaba/articles/6f56ea6556036e

### 使用 F# 进行汇编编程（基础知识）
https://zenn.dev/sayurin/articles/22989af1e3833d

### 使用 F# 进行汇编编程（准备）
https://zenn.dev/sayurin/articles/6768087198fd70

### 使用 F# 进行汇编编程（实用）
https://zenn.dev/sayurin/articles/fa986cfe698961

### C# Boost、DotNext 库第 2 部分 - Qiita
https://qiita.com/up-hash/items/10138710a9d7c9cba209

## 库、存储库、工具等。

### GitHub - KristofferStrube/Blazor.WebAuthentication：Web 身份验证浏览器 API 的 Blazor 包装器。
https://github.com/KristofferStrube/Blazor.WebAuthentication

https://x.com/kstrubeg/status/1740133676984246464?s=12&t=ggvrrZ7oLogHyNoIGNgjbw
## 网站、文档等
### 推文

https://x.com/sergiopedri/status/1740826434019434701?s=12

![image-20240107164013025](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240107164013025.png)

---

https://x.com/egorbo/status/1739696282686439519?s=12

![image-20240107164123427](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240107164123427.png)

---

https://x.com/steplyakov/status/1737895816050934101?s=12

![image-20240107164216271](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20240107164216271.png)


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