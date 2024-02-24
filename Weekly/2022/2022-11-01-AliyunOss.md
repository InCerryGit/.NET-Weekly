---
Title: "2022-11-01: AWS App Runner now supports .NET managed runtime, AWS Toolkit for .NET Refactoring, Copy Nice"
Published: 2022/11/01 00:00
DestinationPath: 2022/11/01/updates.html
---
## 精选要闻
### .NET 7 NativeAOT比.NET单文件发布文件小80%
https://twitter.com/JamesNK/status/1584919726861737984?s=20&t=cOsB41s2cydu_Ibts4xnEw
AOT GRPC服务器应用程序比.NET运行时自包含的单文件发布小80%，目前只比Go稍大一点。
![image-10月第4期 10.24-10.30-221026094245473](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-10%e6%9c%88%e7%ac%ac4%e6%9c%9f+10.24-10.30-221026094245473-16673007959462.png)

由于.NET需要Jit编译，第一次请求需要编译很多代码，所以都比较耗时。通过NativeAOT以后，第一次请求响应时间比.NET默认快650%，和Go只相差12%。
![image-10月第4期 10.24-10.30-221026094510906](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-10%e6%9c%88%e7%ac%ac4%e6%9c%9f+10.24-10.30-221026094510906-16673008039633.png)
要知道.NET不是静态编译的平台，而且它在典型场景有着比Go更完善的特性和更高的性能，能在体积和第一次请求响应追上Go是非常不错的。**不过这并不是最终结果，因为.NET NativeAOT虽然可用，但是还未正式发布，期待后续的更新。**

## .NET8 新增新的AOT分层编译策略，DynamicPGO可达FullPGO性能
.NET8现在可以检测经常访问的AOT代码（并且重新jits它），一般来说只检测经常访问的代码 - 我们已经可以从中看到很好的好处（RPS🔼, Start-time🔽）🙃https://github.com/dotnet/runtime/pull/70941（已合并）。

![image-10月第4期 10.24-10.30-221028102145262](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-10%e6%9c%88%e7%ac%ac4%e6%9c%9f+10.24-10.30-221028102145262-16673008140834.png)

可以看到上图中红色箭头所示，RPS有明显提升，而Start-time也有明显的下降。

### Silky 微服务框架
https://github.com/liuhll/silky

在.NET平台下的微服务应用开发框架，支持微服务场景的诸多特性，如服务治理、RPC通信、链路跟踪、分布式事务等。


### 介绍一个免费、开源的.NET 分布式应用框架 - MassTransit
https://www.cnblogs.com/sheng-jie/p/MassTransit-NET-Distributed-Application-Framework.html

本文着重介绍了[MassTransit](http://masstransit-project.com/ "MassTransit")框架。它直译公共交通， 是由`Chris Patterson`开发的基于消息驱动的.NET 分布式应用框架，其核心思想是借助消息来实现服务之间的松耦合异步通信，进而确保应用更高的可用性、可靠性和可扩展性。

### C# RulesEngine 规则引擎：从入门到看懵
https://www.cnblogs.com/whuanle/p/16830333.html

本文介绍了微软开源的规则引擎库RulesEngine的特性和使用方法，其中包含很多代码实例，方便易懂。

### 是什么让.NET7的Min和Max方法性能暴增了45倍？
https://www.cnblogs.com/InCerry/archive/2022/10/28/how_to_use_simd_improve_dotnet7_min_max_performance.html

本文就通过.NET7中的一些pr带大家一起探索下.NET7的`Min()`和`Max()`方法是如何变快45倍的。

### .NET性能系列文章一：.NET7的性能改进
https://www.cnblogs.com/InCerry/archive/2022/10/24/net-performance-series-1-performance-improvements-in-net-7-fb793f8f5f71.html

.NET 7目前（17.10.2022）处于预览阶段，将于2022年11月发布。通过这个新版本，微软提供了一些大的性能改进。这篇 .NET性能系列的第一篇文章，是关于从.NET6到.NET7最值得注意的性能改进。

### 创建.NET程序Dump的几种姿势
https://mp.weixin.qq.com/s/ihXas9SwRyGTd26tVjhCPQ

本文介绍了生成一个.NET Dump 文件的多种方式。在 Windows、Linux 或 Azure 上有许多方法可以生成Dump文件。

### TensorFlow.NET 实战 - 为.NET开发者开启机器学习之旅
https://mp.weixin.qq.com/s/RY5GH948d1Xy7Q2Zeine6A

介绍在《TensorFlow.NET 实战 - 为.NET开发者开启机器学习之旅》这本书 -  .NET 生态上在人工智能领域有一个开源团队 SciSharp STACK ，他们为TensorFlow提供了 .NET Standard binding，旨在以C＃实现完整的Tensorflow API，允许 .NET开发人员使用跨平台的.NET Standard框架开发、训练和部署机器学习模型。 

### C#实现生成Markdown文档目录树
https://mp.weixin.qq.com/s/VGxEftueOWOecP9vpJvQmw

介绍了使用C#处理Markdown文档的方式和方法。

### 记一次 .NET 某娱乐聊天流平台 CPU 爆高分析
https://mp.weixin.qq.com/s/LuxA50zsDzxJbS3ehCuFjg

前段时间有位朋友加微信，说他的程序直接 CPU=100%，每次只能手工介入重启，让我帮忙看下到底怎么回事，哈哈，这种CPU打满的事故，程序员压力会非常大, 我让朋友在 CPU 高的时候抓 2 个 dump 下来，然后发给我分析。

## 主题

### AWS App Runner推出对PHP、Go、.Net和Ruby托管运行时的支持
https://aws.amazon.com/jp/about-aws/whats-new/2022/10/aws-app-runner-support-php-go-dot-net-ruby-managed-runtimes/

现在AWS App Runner支持多种语言的运行机制，包括.NET和Java。

AWS App Runner是一个系统，允许你通过准备带有源代码的镜像或配置文件，轻松构建、部署和运行你的应用程序。 作为一个运行时，ASP.NET 6被支持，作为一个例子，一个ASP.NET Core应用程序可以通过以下的配置文件来构建和部署。

```yaml
version: 1.0
runtime: dotnet6
build:
  commands:
    build:
      – dotnet publish -c Release -o out
run:
  command: dotnet out/HelloWorldDotNetApp.dll
  network:
    port: 5000
    env: APP_PORT
  env:
    – name: ASPNETCORE_URLS
      value: "http://*:5000"
```

### 介绍AWS Toolkit for .NET Refactoring，一个新的Visual Studio扩展。
https://aws.amazon.com/jp/about-aws/whats-new/2022/10/aws-toolkit-net-refactoring-visual-studio-extension/

一个名为AWS Toolkit for .NET Refactoring的Visual Studio扩展已经发布。

这是一个扩展，提供了为云环境更新遗留的.NET框架应用程序的功能。 编写.NET Core/.NET，扫描依赖性和API使用情况，改变IIS web.config的代码以在Linux下运行，并协助部署到AWS。

### 以适当的缩进方式复制 - Visual Studio Blog
https://devblogs.microsoft.com/visualstudio/copy-with-proper-indentation/

文章描述了一个实验性的Visual Studio扩展，允许以保持正确缩进的方式复制代码。

该扩展允许缩进，即使在复制一个嵌套代码块中间的代码块时也能保持一致。 当粘贴到消息应用程序、博客等时，这可以防止只有第一行失去缩进，而其余部分过度缩进的情况。

- [Copy Nice - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.CopyNice)

### .NET框架2022年10月累积更新预览 - .NET Blog
https://devblogs.microsoft.com/dotnet/dotnet-framework-october-2022-cumulative-update-preview/

.NET框架的2022年10月累积更新预览已经发布。

这个版本包含几个质量改进的更新，包括WPF。

## 文章、幻灯片
### 使AnimationEvent对CoreCLR垃圾收集器安全 | Unity Blog
https://blog.unity.com/technology/making-animationevent-safe-for-the-coreclr-garbage-collector

文章介绍了在用CoreCLR运行Unity时，如何将AnimationEvents与CoreCLR的GC整合并运行。

包括为提高速度而使其成为Blittable，重用GCHandle，以及修改它们，使其在Mono、IL2CPP中的运行速度与CoreCLR相同。

### 在Visual Studio 2022中使用的扩展 - tech.guitarrapc.cóm
https://tech.guitarrapc.com/entry/2022/10/27/023608

介绍Visual Studio 2022中可用扩展的文章。 它引入了各种扩展，从编辑器到显示构建状态等等。

### Blazor Wasm的现场演示现在可以使用 | &#x2B;&#x2B;C&#x2B;&#x2B;; // 不明飞行C博客
https://ufcpp.net/blog/2022/10/blazorwasmdemo/

一篇关于在Blazor WebAssembly中整理和重做工作演示的文章。

### 在.NET项目中，有6种方法可以在一个共同的位置设置相同的版本信息 | @jsakamoto
https://devadjust.exblog.jp/29404286/

本文介绍了从一个共同的位置设置一个解决方案中多个.NET项目的版本信息的方法。

文章介绍了六种设置常用设置的方法。

- Directory.Build.props
- 进口道具。
- 链接包含AssemblyFileVersion的源代码
- 从文件中导入
- 通过dotnet构建参数指定
- 在构建时通过环境变量进行规范

### OpenSearch的.NET客户端现在是GA，我打算使用它。
https://zenn.dev/shimat/articles/d2ae99acaf022f

关于Amazon OpenSearch（前身为Elasticsearch Service）的.NET客户端库的文章。

Elasticsearch 客户端库从 v7.14 开始就无法连接到 OpenSearch，所以一直在等待 OpenSearch 的客户端库。 现在已经发布的.NET版本的客户端库，以及它的使用和感受。

### 在ASP.NET Core 6.0中构建你自己的OAuth 2.0服务器和OpenId连接提供商
https://dev.to/mohammedahmed/build-your-own-oauth-20-server-and-openid-connect-provider-in-aspnet-core-60-1g1m

关于在.NET 6的ASP.NET Core中实现自己的OAuth 2.0服务器和OpenId Connect Provider的文章。

### 托管指针、Span、ref结构、C#11 ref字段和scoped关键字 - NDepend
https://blog.ndepend.com/managed-pointers-span-ref-struct-c11-ref-fields-and-the-scoped-keyword

这篇文章回顾并解释了从指针到Span、Ref结构和字段的一切。

### 自动发布.Net应用程序的版本
https://blog.antosubash.com/posts/automatic-version-and-release

关于如何使用Versionize工具在GitHub Actions中自动进行版本和发布的文章。

文章还讨论了如何使用Husky.Net对Git的pre-commit钩子中的注释进行提示。

### 学习系列：在Visual Studio中开始使用GitHub
https://devblogs.microsoft.com/visualstudio/learn-github-in-visual-studio-learning-series/

一篇关于使用Visual Studio学习GitHub的电子邮件系列的介绍性文章。

### LINQ的聚合函数在.NET7中为何如此之快的故事（或者说矢量化的难度） - Qiita
https://qiita.com/Kujiro/items/dc90366325fffcd3675d

一篇解释LINQ聚合函数（Sum、Max、Average）的具体实现的文章，这些函数在.NET 7中被加速了。

### Project Volterra和Windows开发工具包2023 - Shibayan Miscellaneous
https://blog.shibayan.jp/entry/20221027/1666807751

关于Windows开发工具包2023的评论文章。

### 我买了Windows开发工具包2023 | DevelopersIO
https://dev.classmethod.jp/articles/try-windows-dev-kit-2023-project-volterra/

一篇关于Windows开发工具包2023的评论文章，其中还讨论了像PowerShell和AWS工具如何工作。

### 在Razor Pages中与空引用类型作斗争
https://andrewlock.net/fighting-with-nullable-reference-types-in-razor-pages/

关于在Razor Pages中与空引用类型斗争的文章。

文章讨论了如何处理Razor页面，其中的值是从外部插入的，警告和不适当的抓取会增加NullReferenceException的可能性。 文章介绍了一些建议，包括使用C# 11的`required`，这在一定程度上可以缓解。

### 在C#中使用多线程的SQLite。
https://zenn.dev/kn64872/articles/90ae674d5332a7

文章探讨了在多线程环境下使用System.Data.SQLite的行为。

### 用Infer#杀死僵尸 "无回复 "崩溃 - .NET博客
https://devblogs.microsoft.com/dotnet/slaying-zombie-no-repo-crashes-with-infersharp/

一篇关于使用Infer#进行静态代码分析以检测难以发现的资源泄漏和安全问题的介绍性文章。

- [microsoft/infersharp: Infer#是一个用于C#的跨程序和可扩展的静态代码分析器。通过Facebook的Infer的功能，这个工具可以检测到空解引用、资源泄漏和线程安全违规。它还执行污点流跟踪，以检测关键的安全漏洞，如SQL注入。](https://github.com/microsoft/infersharp)

### 官方发布! @dotnet  目前的版本已被重新命名为 "标准期限支持"，这些变化已在网站上发布。
https://dotnet.microsoft.com/download/dotnet

目前的.NET非LTS版本已被重新命名为 "标准期限支持"，其变化已在网站上上线。

![image-20221101190029335](https://incerry-blog-imgs.oss-cn-hangzhou.aliyuncs.com/image-20221101190029335.png)

## 图书馆、资源库、工具

### corvus-dotnet/Corvus.UriTemplates:  低分配的URI模板解析和解决，支持Tavis.UriTemplates API
https://github.com/corvus-dotnet/corvus.uritemplates

一个分配较少的处理URI模板的库（RFC 6570）.

- [低分配高性能的C#来解决UriTemplate问题| endjin](https://endjin.com/blog/2022/10/high-performance-csharp-uritemplates)

## 版权声明

* InCerry 翻译与整理 : https://github.com/InCerryGit/WeekRef.NET/blob/master/input_zh-CN/2022/2022-11-01.md
* Myuki WeekRef : https://github.com/mayuki/WeekRef.NET/blob/master/input/2022/2022-11-01.md

**欢迎大家为.NET周报进行贡献，需要推广自己的文章或者框架、开源项目可以下方的项目地址提交Issue或者我的微信公众号私信。**

格式如下：

* 10~50字左右的标题
* 对应文章或项目网址访问链接
* 200字以内的简介，如果太长会影响阅读体验

https://github.com/InCerryGit/.NET-Weekly
