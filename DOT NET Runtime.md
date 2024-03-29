.NET Runtime可以简单理解为.NET应用程序的运行时环境。它在程序执行时提供了一系列系统服务和管理功能。

具体来说,.NET Runtime的作用包括:

1. 提供通用语言运行时环境([[Common Language Runtime (CLR)]])。这是所有.NET语言([[C Sharp Lang]], VB等)编译成中间语言([[Intermediate Language (IL)]])代码后,最终执行的地方。

2. 存储管理和垃圾回收。自动管理程序运行时的内存分配和释放。

3. 提供线程管理和线程池的服务。用于执行多线程程序。

4. 异常处理。提供TRY/CATCH块来方便处理异常。

5. 提供类型系统与反射的支持。允许通过类型信息动态创建对象、调用方法。

6. 提供核心.NET类库的支持。程序可以利用丰富的BCL类库快速开发。

7. 提供对aspx,.asmx的运行环境。支持部署和运行.NET Web应用。

8. 提供调试、性能分析和统计信息。方便跟踪和调优程序。

9. 提供安全检查和验证。如XML、代码访问安全检查。保护系统安全。

综上,.NET Runtime为程序的编译与运行提供了完整的框架支持和系统服务。它简化了开发,提高效率,是.NET应用得以顺畅运行的必须环境。可以看作一个完整的执行引擎。

.NET Runtime 中确实内置了 [[Common Language Runtime (CLR)]] 的功能。C#等语言编译成的 [[Intermediate Language (IL)]] 代码,终将由 [[Common Language Runtime (CLR)]] 来执行。

只是微软在命名和概念上,不再明确强调“[[Common Language Runtime (CLR)]]”,因为整个运行时的架构和内部细节发生了调整,想要向开发者暗示这是新的系统。

但简单来说 [[DOT NET Runtime]] 作为一个整体,承担了原来 [[Common Language Runtime (CLR)]] 的职责。它负责如下工作:

1. 提供语言中间码([[Intermediate Language (IL)]])的运行环境
2. 管理程序的内存分配、线程调度等
3. 提供核心服务如垃圾回收、异常处理等
4. 对 [[DOT Net]] 程序提供寻址和安全机制的支持

所以 C# 编译器生成 [[Intermediate Language (IL)]] 代码后,.NET Runtime 将对其进行即时(JIT)编译,然后执行结果。

这其中,仍然涉及虚拟机、线程池、垃圾回收等概念。只是微软通过新的 [[DOT NET Runtime]] 架构,改进和统一了这些功能的实现。

所以简单总结 [[DOT NET Runtime]] = [[Common Language Runtime (CLR)]] + 更多系统服务及改进。[[Common Language Runtime (CLR)]]的核心功能,现在都被整合入一个统一的模块中,也就是我们现在的 [[DOT NET Runtime]]