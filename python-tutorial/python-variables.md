# Python 变量

## 变量
变量是储存值的“容器”。

## 创建变量
Python没有创建变量的特殊指令。
一旦你将一个值赋予给一个名称，你就成功创建了一个变量。

#### 实例
```python
x = 5
y = 'John'
print(x)
print(y)
```

变量没有任何类型限制，你甚至可以在创建变量之后改变它的数据类型。
#### 实例
```python
x = 4 # x是整数型
x = 'Sally' # x现在是字符串类型
print(x)
```

## 数据类型转换
如果你想声明一个变量的数据类型，可以通过数据类型转换来实现。
#### 实例
```python
x = str(3) # x现在是'3'
x = int(3) # x现在是3
x = float(3) # x现在是3.0
```

## 获取数据类型
你可以使用`type()`函数来获取一个变量的数据类型。
#### 实例
```python
x = 5
y = 'John'
print(type(x))
print(type(y))
```

## 单引号还是双引号？
字符串类型的变量可以用单引号或双引号来声明。
#### 实例
```python
x = "John"
# 与
x = 'John'
# 相同
```

## 区分大小写
变量名称区分大小写。
#### 实例
以下指令将会创建两个不一样的变量。
```python
a = 4
A = 'Sally'
# A不会覆盖a
```

## 变量名称
一个变量可以有一个很短的名字（比如x和y）也可以是一个更加具有描述性的名称（年龄，车的名字，总_容积）。以下是Python变量的命名规则：
- 一个变量名需要以一个字母或一个下划线开始
- 一个变量名不可以以一个数字开始
- 一个变量名只可以包含26个英文字母，10个数字以及下划线。
-  变量名区分大小写。（age, Age和AGE是三个不一样的变量名）

#### 实例
符合规则的变量名称：
```python
myvar = 'John'
my_var = 'John'
_my_var = 'John'
myVar = 'John'
MYVAR = 'John'
myvar2 = 'John'
```
#### 实例
不符合规则的变量名称：
```python
2myvar = 'John'
my-var = 'John'
my var = 'John'
```

## 多单词变量名
有多单词的变量名可能会很难阅读。
有几个技巧可以让它们的可读性大大增加。
### 驼峰命名法
除了第一个单词的首字母都大写：
```python
myVariableName = 'John'
```
### 帕斯卡命名法
所有单词的首字母都大写：
```python
MyVariableName = 'John'
```

### 蛇式命名法
每一个单词用下划线分隔开：
```python
my_variable_name = 'John'
```

## 给变量赋予多个值
### 多个值赋给多个变量
Python允许你在一行代码中将多个值赋给多个变量：
#### 实例
```python
x, y, z = 'Orange', 'Banana', 'Cherry'
print(x)
print(y)
print(z)
```
**注意**：值的数量必须和变量的数量相等，否则系统将会报错。

### 一个值赋给多个变量
你也可以在一行代码中将一个值赋给多个变量：
#### 实例
```python
x = y = z = 'Orange'
print(x)
print(y)
print(z)
```
### 拆分序列
如果你在一个列表，元组等序列中存有一些值，Python允许你将这些值赋给变量。这个操作叫做*拆分*。
#### 实例
拆分一个列表：
```python
fruits = ['apple', 'banana', 'cherry']
x, y, z = fruits
print(x)
print(y)
print(z)
```
你将会在拆分元组这个章节学到更多。

## 输出变量
Python的`print`函数经常被用来输出变量。
Python使用`+`字符来将字符串和变量组合在一起：

#### 实例
```python
x = 'awesome'
print('Python is' = x)
```

我们也可以用`+`字符来把变量与变量结合：
#### 实例
```python
x = 'Python is'
y = 'awesome'
z = x + y
print(z)
```

对于数字来讲，`+`字符充当一个数学运算符：
#### 实例
```python
x = 5
y = 10
print(x + y)
```
如果你试图将一个数字和一个字符串结合，Python将会报错：
#### 实例
```python
x = 5
y = 'John'
print(x + y)
```

## 全局变量
在函数之外（也就是以上所有例子）创建的一个变量是一个全局变量。
全局变量是任何人都可以使用的，无论是在函数之内还是在函数之外。

#### 实例
在函数外创建一个变量，然后在函数内使用它
```python 
x = 'awesome'

def myfunc():
    print('Python is ' + x)

myfunc()
```
如果在函数中创建一个同名的变量，那么该变量将是一个局部变量，而且只可以在该函数内使用。但全局变量依旧不变，它依旧是全局变量，而且值也是相同的。
#### 实例
在函数内创建一个与全局变量同名的局部变量
```python
x = 'awesome'

def myfunc():
    x = 'fantastic'
    print('Python is ' + x)

myfunc()

print('Python is ' + x)
```

### 创建全局变量的关键词
一般当你在函数内创建一个变量时，它将会是局部的，并且只可以在该函数内使用。
如果你想在一个函数内创建一个全局变量，你可以使用关键词`global`。

#### 实例
```python
def myfunc():
    global x
    x = 'fantastic'

myfunc()

print('Python is ' + x)
```
如果想在一个函数内更改一个全局变量的值，你也可以使用关键词`global`。
#### 实例
```python
x = 'awesome'

def myfunc():
    global x
    x = 'fantastic'

myfunc()

print('python is ' + x)
```