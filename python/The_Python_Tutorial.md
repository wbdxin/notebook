## 00The Python Tutorial

易于使用，强大的编程语言  
拥有高效的数据结构和简单但有效的面向对象编程途径  
优雅的语法和动态数据类型，配合原生的解释执行，使其成为脚本和快速应用开发方面的理想语言，而且支持多平台

Python解释器和扩展库以二进制或源码方式，在以下站点共享  
www.python.org  
其中大部分也可以自由分发  
该站点也包含指向很多第三方自由模块/程序/工具/文档的链接  

Python解释器可以通过C或C++[或可被c调用的语言]扩展功能和数据类型  
Python也适合作为定制化应用的阔转语言  

模块和标准对象的说明，参考The Python Standard Library  
标准的语言定义，参考The Python Language Reference  
使用c/c++写扩展，参考Extending and Embedding the Python Interpreter和Python/C API Reference Manual  

本教程未覆盖全面内容的全部细节，甚至一些通用/常用的特征  
而是注重Python值得关注的特征  
会提供好的编程习惯和风格  
通过学习可以读/写python模块和程序，并具备学习深入关于标准库的内容

## 01Whetting Your Appetite

适用于需要自动化/定制化处理的程序  
使用c/c++/java库进行开发，编写-编译-测试-重编译的循环耗时较长  
如果是为测试任务编写测试数据是更无趣且耗时的  
有时编程需要调用其他语言，但有不值得实现个完整的语言环境  

相比较unix shell或windows batch文件，擅长操作文本不擅长gui  
c/c++/java擅长gui但开发耗时，即便是很小的程序  
Python易于使用，跨平台，适合快速开发  

Python简单但是真正的编程语言  
- 具备丰富的数据结构  
- 支持大型程序的开发，优于shell和batch  
- 提供错误检查机制，优于c  
- 具备高级数据类型，例如弹性数组和字典，优于awk和perl  

Python可以支持模块化编程，由此支持复用  
并提供了大量的模块，以便构建应用是调用  
- 例如：文件IO，网络socket，系统调用，GUI  

Python是解释执行语言，利于节省编程时间，因为无需耗时编译链接  
解释器可以交互，以便实践语言的特性，用于编写抛弃型应用，测试功能  

Python程序比较紧凑，易读  
- 高级数据类型使得可以单行表达复杂公式  
- 代码块缩进对编码进行分组  
- 无需变量参数声明  

Python是易于扩展的，支持源码，二级制格式的扩展  

学习语言的好方法是：使用它  

## 02 Using the Python Interpreter  