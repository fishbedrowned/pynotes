## 技巧

- dir(对象)： 查看对象类型所具有的方法以及属性，eg:dir("test")
- help(方法)： 查看方法的使用, eg:dir("test".replace)
- 法则：可以用于多种类型的通用性操作都是以内置函数或者表达式的形式出现的，eg:len(X),X[0]。但是类型特定的操作是以方法调用的形式出现的，eg:aString.upper()
- 字符串模式匹配：import re, re.match().group(indexOfResult)
- 内置类型：

```
数值型：int float complex
序列：（iterable）
str,unicode,tuple,list,bytearray,buffer,xrange
集合：set,fronzeset
映射：dict
文件： file
布尔值：True,False
可调用对象
```


- 迭代协议：在内存中物理存储的序列，或一个在迭代操作情况下每次产生一个元素的对象

## point

- range(*(5,10,2)) : *解析tuple为参数，range(start, stop, step)
- &}- ： 集合的与或非
- from itertools import groupby： 集合的groupby
- from collections import defaultdict: 也可以实现集合的groupby, 指定字典value的类型，例如：x=defaultdict(list)，通过x[key].append(row)
- item form item in lise if item is vaild: 此语法来实现集合的filter功能
