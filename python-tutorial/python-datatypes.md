# Python 数据类型
## 内置数据类型
在编程中，数据类型是一个很重要的概念。  
变量可以存储不同的数据类型，而不同的数据类型用途不一。  
Python默认有以下几种不同种类的数据类型：  

类别|数据类型
-|-
字符串|`str`
数字|`int`, `float`, `complex`
序列|`list`, `tuple`, `range`
映射|`dict`
集合|`set`, `frozenset`
布尔|`bool`
二进制|`bytes`, `bytearray`, `memoryview`


## 获取数据类型
你可以使用 `type()` 函数来获取一个对象的数据类型：
#### 实例
打印变量x的数据类型：
```python
x = 5
print(type(x))
```

## 设置数据类型
在Python中，当你将一个值赋给一个变量，它的数据类型就被设置了。
实例|数据类型
-|-
x = 'Hello World'|str
x = 20|int
x = 20.5|float
x = 1j|complex
x = ['apple', 'banana', 'cherry']|list
x = ('apple', 'banana', 'cherry')|tuple
x = range(6)|range
x = {'name' : 'John', 'age' : 36}|dict
x = {'apple', 'banana', 'cherry'}|set
x = frozenset({'apple', 'banana', 'cherry'})|frozenset
x = True|bool
x = b'Hello'|bytes
x = bytearray(5)|bytearray
x = memoryview(byte(5))|memoryview

## 设置指定数据类型
如果你想指定数据类型，你可以用对应的构造函数：

实例|数据类型
-|-
x = str('Hello World')|str
x = int(20)|int
x = float(20.5)|float
x = complex(1j)|complex
x = list(('apple', 'banana', 'cherry'))|list
x = tuple('apple', 'banana', 'cherry')|tuple
x = range(6)|range
x = dict('name'='John', 'age'=36)|dict
x = set(('apple', 'banana', 'cherry'))|set
x = frozenset(('apple', 'banana', 'cherry'))|frozenset
x = bool(5)|bool
x = bytes(5)|bytes
x = bytearray(5)|bytearray
x = memoryview(byte(5))|memoryview








学号|姓名|分数
-|:-:|-:
小明|男|75
小红|女|79
小陆|男|92


















<table>
    <tr>
        <td><a href="http://www.jd.com">123</a></td>
        <td><b>456</b></td>
    </tr>
    <tr>
        <td><i>123</i></td>
        <td><font color="#ff00ff">456</font></td>
    </tr>
</table>
