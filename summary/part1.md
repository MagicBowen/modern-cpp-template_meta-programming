# 模板的基础知识

C++是一门静态类型语言，我们在该语言中使用的所有变量都需要事先指定好类型，这样方便编译器帮我们预先捕捉各种类型错误，并且做更好的代码优化。但是这样以来，很多功能相同但是处理数据类型不同的代码，就得手动写多份。在没有模板之前，程序员要么通过预处理宏，要么通过把数据地址转成`void*`这种不安全的手段来消除上述重复。

为此C++引入模板机制。使用模板则可以在定义逻辑的时候不具体指定处理的数据类型，等到使用这段逻辑的时候再将类型传给模板。在C++中模板完全支持类型检查和作用域，因此它保持了静态语言的安全性，以及不会破坏编译器对代码的静态优化能力。

本节我们回顾模板的各种基础知识，在此过程中我们会着重提及后文中会用到和模板元编程相关的一些特性。另外，现代C++对模板新的发展，我们放在第三章单独讲述。
