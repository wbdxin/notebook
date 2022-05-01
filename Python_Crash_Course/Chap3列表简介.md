## 列表是什么
    一系列特定顺序排列的元素，有值，有索引，差一规则
    listname = [item0,item1,...]
    exp:bicycles.py--->打印结果包括方括号

## 访问列表元素
    listname[index]
    改进bicycles.py--->print(bicycles[0])
    输出仅为字符串，不包含方括号

## 索引从0而不是1开始

## 使用列表中的各个值
    listname[index],也是obj，根据具体类型有对应的方法和函数

## 修改，添加和删除元素
### 修改列表元素
    listname[index] = new_value
    exp:motorcycles.py

### 在列表中添加元素
    在列表末尾添加元素
        listname.append(new_value)
        exp:改进motorcycles.py--->注销修改语句，增加append语句

    在列表中插入元素
        listname.insert(index,new_value)
        将new_value添加到index位置
    
    在列表中删除元素
        使用del语句删除元素
            del listname[index]
            需要指定待删除索引

        使用方法pop()删除元素
            lisntname.pop()--->弹出栈顶元素，此方法返回弹出元素的引用

        弹出列表中任何位置的元素
            listname.pop(index)--->弹出index位置的元素，此方法返回弹出元素的引用
        
        根据值删除元素
            使用方法remove()
            listname.remove(value)--->删除第一个值与value相同的元素，如果有多个，需要自行判断
        
## 组织列表
    使用方法sort()对列表进行永久性排序
        exp：cars.py
        sort()永久修改列表元素的顺序
        反序：listname.sort(reverse = True)
    
    使用函数sorted()对列表进行临时排序
        sorted(listname)
        sorted(listname,reverse=True)

    倒着打印列表:使用方法reverse()
        listname.reverse()
    
    确定列表长度，函数len()
        len(listname)

## 使用列表避免索引错误
    注意index从0开始
