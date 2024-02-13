Common Intermediate Language (CIL),也被称为 Microsoft Intermediate Language (MSIL) 或 [[Intermediate Language (IL)]], 是 [[DOT Net]] 框架管理代码的关键组成部分。

CIL是一种低级语言,介于源代码和机器码之间。它是一种跨语言的汇编语言,无与平台和源语言无关。

[[C Sharp Lang]]、VB等托管语言会被编译成CIL代码,而不是直接编译成机器码。这个CIL代码随后在运行时由公共语言运行库(CLR)进行就地编译(JIT)来生成原生CPU指令。

CIL的主要优点有:

1. 跨语言 - 不同语言(C#、VB等)都可以编译成同一个CIL指令集。
2. 跨平台 - CIL代码可以在不同处理器和操作系统上运行。
3. JIT和优化 - CIL可在运行时进行JIT (即时)编译来优化性能。
4. 安全可靠 - CIL系统可以确保类型安全,内存安全,异常处理等。
5. 元数据和反射 - CIL包含丰富的元数据来支持高级运行时服务。

所以CIL是 [[DOT NET Framework]] 语言和运行库之间的桥梁,是 [[DOT NET Framework]] 管理执行过程的关键。它为语言和开发者提供了重要服务和保障。