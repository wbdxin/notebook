## 运行hello_world.py时发生的情况

    .py说明需要调用python解释器解释执行
    python解释器读取全部代码
    词法分析

## 变量

    python中一切皆对象
    变量保留对象的引用

## 变量的命名和使用

    1.只能包含数字，字母和下划线
    2.数字不能用于开头
    3.不能包含空格
    4.不能和保留字重复
    5.慎用形近字符
    6.python使用变量时，严格检查变量名的拼写一致性，但不强调所使用单词本身的正确性

## 字符串

    被引号括起来的字符序列
    引号可以是单双三引号，三引号可以包含换行
    
## 方法修改字符串大小写
    strobj.upper()
    strobj.lower()
    strobj.title()

## 合并字符串
    +

## 制表符或换行符来添加空白
    \n
    \t
    \n\t

## 删除空白
    strobj.strip()
    strobj.rstrip()
    strobj.lstrip()

## 使用字符串时避免语法错误
    注意字符串边界符和字符串中引号的区分

## 数字
    整数: +，-，*，/，**    
    浮点数: 带小数点，注意包含的小数位数可能不确定

## 使用函数str()避免类型错误
    str(intobj)

## 注释
    \# 单行注释
    三引号：多行注释
    当一段代码有多种选择，请写注释
    import this: python 之禅
    The Zen of Python, by Tim Peters

    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!