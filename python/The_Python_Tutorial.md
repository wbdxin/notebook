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
        具备丰富的数据结构  
        支持大型程序的开发，优于shell和batch  
        提供错误检查机制，优于c  
        具备高级数据类型，例如弹性数组和字典，优于awk和perl  

    Python可以支持模块化编程，由此支持复用  
    并提供了大量的模块，以便构建应用是调用  
        例如：文件IO，网络socket，系统调用，GUI  

    Python是解释执行语言，利于节省编程时间，因为无需耗时编译链接  
    解释器可以交互，以便实践语言的特性，用于编写抛弃型应用，测试功能  

    Python程序比较紧凑，易读  
        高级数据类型使得可以单行表达复杂公式  
        代码块缩进对编码进行分组  
        无需变量参数声明  

    Python是易于扩展的，支持源码，二级制格式的扩展  

    学习语言的好方法是：使用它 

## 02 Using the Python Interpreter  

### 调用解释器  

    解释器安装路径  
    /usr/local/bin/python3.10  

    注意添加安装路径到shell的搜索路径  
        安装路径为可选，注意实际情况  

    windows下如果安装自Microsoft Store，python命令会生效  
    如果安装了py.exe Launcher，可以用py命令  

    运行python命令的方法可以参考：Excursus： Setting environment variables  

    退出解释器可以使用CTRL-d[unix]，CTRL-z[windows]  
    或者使用quit()命令  

    解释器的行编辑特征：  
        交互式编辑
        历史记录替换  
        代码补全  
        支持GNU Readline库  

    可以在解释器中输入ctrl-p，如果有beep声音，说明支持行编辑  
    如果无beep或屏幕输出^p,则不支持行编辑  

    解释器工作类似于unix shell  
        当通过链接到tty设备的标准输入调用解释器，则读入命令并交互执行  
        当使用文件作为参数或标准输入，则执行文件中的脚本  

    第二个执行解释器的途径是：python -c command [arg]...，  
    会执行command中的代码，类似shell的-c参数  
    因为python代码段经常包含空格或其他特殊字符，建议用单引号将command包括起来  

    部分python模块可以被用作脚本，  
    使用python -m module [arg]...,其中module的源码会被执行  

    通过在使用脚本前加上-i参数，可以进入交互模式  

    关于命令行选项，请参考Command Line and Environment  

### 参数传递  
    调用解释器命令行中的脚本名和后续的参数会作为字符串列表传递给sys模块中的argv变量  
    要访问这个列表，需要import sys  
    该列表长度最少为1  
    当无脚本名也无参数，argv[0]是空字符串  
    如果脚本名是-[标准输入],argv[0]被设置为-  
    当使用-c command格式，sys.argv[0]设置为-c  
    当-m被使用，sys.argv[0]设置为模块完整路径名  
    -c或-m后的参数放在sys.argv,交给命令或模块去处理  

### 交互模式  
    执行命令后解释器进入交互模式  
    prompts为>>>
    在继续行的prompts为...  
    第一个提示符会伴随欢迎信息，版本信息，版权  
    
    Python 3.10.1 (tags/v3.10.1:2cd268a, Dec  6 2021, 19:10:37) [MSC v.1929 64 bit (AMD64)] on win32
    Type "help", "copyright", "credits" or "license" for more information.
    >>>

    需要输入多行的情形如下：  
    >>> the_world_is_flat = True
    >>> if the_world_is_flat:
    ...     print("Be careful not to fall off!")
    ... 
    Be careful not to fall off!
    >>>
    
         