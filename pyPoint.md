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
- *: 解析数组与元祖，**： 解析字典
- &}- ： 集合的与或非
- from itertools import groupby： 集合的groupby
- from collections import defaultdict: 也可以实现集合的groupby, 指定字典value的类型，例如：x=defaultdict(list)，通过x[key].append(row)
- item for item in lise if item is vaild: 此语法来实现集合的filter功能
- item if item >0 else defaltValue for item in list: 指定默认值filter集合
- filter 类: 实现集合过滤功能 
- {key: value for key, value in source.items() if condition}：过滤字典source

## package

- fnmatch：Unix Shell通配符匹配
- re: 正则匹配
- urllib：http请求
- collections-namedtuple: 命名元祖
- collections-ChainMap: 字典合并
- os： 系统操作
- operator：操作接口，例如：getkey = itemgetter（“key”）,返回一个可以被调用的函数，从集合中获取key的值，sorted(list, key=getkey)，按照key对list进行排序
- heapq： 堆，一个集合放入堆中，可以方便的获取到最大或最小的n条记录
- itertools： 利用迭代器的函数工具，例如：

```
count(start=0, step=1) --> start, start+step, start+2*step, ...
cycle(p) --> p0, p1, ... plast, p0, p1, ...
repeat(elem [,n]) --> elem, elem, elem, ... endlessly or up to n times
```
