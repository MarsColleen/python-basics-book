# Python 语法

## 执行

正如我们在上一讲学到的那样，Python可以通过直接在命令行中编写代码来执行：

```python
>>> print("Hello, World!")
Hello, World!
```

或者我们可以在服务器上创建带有 .py 后缀的文件，通过命令行来执行它：

```text
C:\Users\Your Name>python myfile.py
```

## 缩进

缩进指在一行代码前的空格（一般四个空格或Tab）。  
在其他语言中，缩进仅为了提升代码的可读性，但在Python语言中，缩进十分重要。 Python使用缩进来表示一个代码块。

#### 实例

```python
if 5 > 2:
    print('Five is greater than two!')
```

如果你忽略了缩进，Python将会报错：

#### 实例

语法错误（Syntax Error）：

```python
if 5 > 2:
print('Five is greater than two!')
```

你可以决定缩进的长度，但一个缩进至少需要一个空格。

#### 实例

```python
if 5 > 2:
 print('Five is greater than two!')
if 5 > 2:
       print('Five is greater than two!')
```

你需要在同一个代码块中使用相同的缩进长度，否则Python会报错：

#### 实例

语法错误（Syntax Error）：

```python
if 5 > 2:
 print('Five is greater than two!')
      print('Five is greater than two!')
```

## 变量

在Python语言中，当你把一个值赋予一个名称，你就创建了一个变量。

#### 实例

Python中的变量：

```python
x = 5
y = 'Hello, World!'
```

Python没有关于声明变量的命令。 你稍后会在Python变量章节中学到更多关于变量的知识。

## 注释

Python中的注释就是对代码的解释与声明。 Python中，`#`是单行注释的符号。从`#`开始直到换行，`#`后面的内容都会视为注释，并被编辑器忽略。

#### 实例

Python中的注释：

```python
# 这是一条注释。
print('Hello, World!')
```

