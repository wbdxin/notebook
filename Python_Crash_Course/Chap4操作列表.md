## 编历列表
    for item_var in list_name:
        code block
    
    在循环后执行一些操作
        循环后的代码与for语句取齐
    
    避免缩进错误
        注意python通过缩进来确定代码的作用域
    
            忘记缩进
            忘记缩进额外的代码行
            不必要的缩进
            循环后不必要的缩进
            遗漏了冒号

## 创建数值列表
    使用函数range()
        for value in range(start,end,step):
            code
        注意生成的数字序列对象取值范围为:[start,end)

    使用range()创建数字列表
        list(range(start,end,step))
    
    对数字列表执行简单的统计计算
        min()
        max()
        sum()
    
## 列表解析
    [var_express for var in range(start,end,step)]

## 使用列表的一部分
    listname[start_index:end_index]
        注意：切片取值范围[start_index:end_index)

        负数返回离列表末尾相应距离的元素

    遍历切片
        for var in list_name[start_index:end_index]:
            code block
    
    复制列表
        list_name = list[:]

## 元组
    tuples_name = (item0,item1...)
        元组元素不可编辑，但整个元组可以重新定义

    遍历元组
        for var in tuples_name:
            code block
    
## 格式设置指南
    PEP8
    缩进：使用4个空格
    行长：不超过80字符
    空行：分割逻辑单元