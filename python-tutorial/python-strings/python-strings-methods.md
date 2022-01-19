# Python String Methods
## 字符串
在Python中，字符串前后需要加上单引号或者双引号。
`'hello'`与`"hello"`是一样的。
你可以通过`print()`函数来展示一个字符串：

#### 实例
```python
print("Hello")
print('Hello')
```

## 将一个字符串赋给变量
要想将字符串赋给一个变量，你需要先输入变量名，接上一个等号，最后加上字符串：

#### 实例
```python
a = 'Hello'
print(a)
```

## 多行字符串
你可以使用三引号来将一个字符串赋给一个变量：

#### 实例
你可以用三个双引号：
```python
a = """I felt my heart shatter
As I was hearing your chatter
Between loving you sweet and loving you bitter
I wouldn't prefer the latter."""
print(a)
```

#### 实例
或者三个单引号：
```python
a = '''I felt my heart shatter
As I was hearing your chatter
Between loving you sweet and loving you bitter
I wouldn't prefer the latter.'''
print(a)
```
*注意：在输出的结果中，字符串的断行与代码中保持一致。*

## 循环输出一个字符串
因为字符串是？？，我们可以通过`for`循环输出一个字符串。

#### 实例
```python
for x in 'banana':
    print(x)
```

## 字符串长度
你可以通过使用`len()`函数来获取一个字符串的长度。

#### 实例
`len()`函数输出一个字符串的长度：
```python
a = 'Hello, World!'
print(len(a))
```

## 检查字符串
你可以通过使用`in`关键词来检查一个字符串中是否包含一个指定的字符或短语。

#### 实例
```python
txt = 'The best things in life are free!'
print('free' in txt)
```

也可以搭配`if`条件句来使用：

#### 实例
```python
txt = 'The best things in life are free!'
if 'free' in txt:
    print('Yes, free is present.')
```

## 检查一个字符是否不在字符串中
如果想检查一个特定的字符或短语是否*不*在字符串中，可以使用关键词`not in`。

#### 实例
```python
txt = 'The best things in life are free!'
print('expensive' not in txt)
```

也可以搭配`if`条件句来使用：

#### 实例
```python
txt = 'The best things in life are free!'
if 'expensive' not in txt:
    print('No, expensive is NOT present.')
```
