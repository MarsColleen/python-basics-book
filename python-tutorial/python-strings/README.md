# Python 字符串
## 字符串
Python中的字符串可以被单引号包裹，也可以被双引号包裹。  
`'hello'` 和 `"hello"` 其实是一样的。
你可以通过 `print()` 函数来输出一个字符串：

#### 实例
```python
print('hello')
print("hello")
```
## 将一个字符串赋给一个变量
将字符串赋给一个变量与其他类型相同，先写上变量名，加上等号，最后在等号后面加入字符串：

#### 实例
```python
a = 'hello'
print(a)
```

## 多行字符串
你可以通过使用三引号来创建一个多行字符串：

#### 实例
你可以用三个单引号：
```python
a = '''this
is
a
multiline
string'''
print(a)
```
#### 实例
或者三个双引号：
```python
a = """this
is
a
multiline
string"""
print(a)
```
**注意**：在结果中，换行符被插入到与代码相同的位置。

## 字符串是数组
就像其他流行的编程语言一样，Python中的字符串是表示unicode字符的字节数组。  
但是，Python没有一个字符数据类型，一个单独的字符就是一个长度为1的字符串。  
中括号可以被用来访问字符串中的一个元素。

#### 实例
获取索引为1的字符串（记住，第1个字符的索引为0）：
```python
a = 'hello, world!'
print(a[1])
```

## 循环出一个字符串
因为字符串为数组，我们可以使用 `for` 循环来循环出一个字符串中的字符。

#### 实例
循环出'banana'中的字符：
```python
for x in 'banana':
    print(x)
```

## 字符串的长度
你可以使用 `len()` 函数来获取字符串的长度。

#### 实例
`len()` 函数返回了字符串的长度：
```python
a = 'hello, world!'
print(len(a))
```

## 检查某个字符是否在字符串中
我们可以使用关键词 `in` 来检查某个字符或关键词是否在某个字符串中。

#### 实例
检查"free"是否在以下文字中：
```python
txt = 'The best things in life are free!'
print('free' in txt)
```
你也可以使用 `if` 表达式：

#### 实例
如果'free'在字符串中，执行print：
```python
txt = 'The best things in life are free!'
if 'free' in txt:
    print("Yes, 'free' is present.")
```

## 检查是否**不**
可以使用关键词 `not in` 来检查某个关键词/字是否**不**在某个字符串中。

#### 实例
检查'expensive'是否**不**在以下文本中：
```python
txt = 'The best things in life are free!'
print('expensive' not in txt)
```

你也可以使用 `if` 表达式：

#### 实例
如果'expensive'不在字符串中，执行print：
```python
txt = 'The best things in life are free!'
if 'expensive' not in txt:
    print("No, 'expensive' is NOT present.")
```
