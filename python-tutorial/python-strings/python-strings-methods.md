# Python String Methods
## 分割字符串
你可以通过使用特定的语法来分割字符串。
声明起始位置与结束位置，中间加上一个分号，这样就可以输出一个字符串的一部分。

#### 实例
获取从索引为2到索引为5的字符（不包括5）：
```python
b = 'Hello, World!'
print(b[2:5])
```

**注意**：第一个字符的索引为0。

### 从头开始分割
如果将开始位置留空，那么系统会自动从第一个字符开始分割：

#### 实例
获取从头到索引为5的字符（不包括5）：
```python
b = 'Hello, World!'
print(b[:5])
```

### 分割至结尾
如果将结束位置留空，那么系统会自动分割至结尾：

#### 实例
获取从索引为2到结尾的字符：
```python
b = 'Hello, World!'
print(b[2:])
```

### 用负数分割
如果使用负数来代表字符的位置，那么分割将从字符串的最后开始：

#### 实例
获取字符：
从："World"中的"o"（位置-5）
到："World"中的"d"（位置-2，但并不包含它）
```python
b = 'Hello, World!'
print(b[-5:-2])
```
## 更改字符串
Python有很多能在字符串上使用的内置方法。

### 变为大写

#### 实例
`upper()`方法将字符改为大写：
```python
a = 'Hello, World!'
print(a.upper())
```

### 变为小写

#### 实例
`lower()`方法将字符改为小写：
```python
a = 'Hello, World!'
print(a.lower())
```

### 去除多余空格
多余空格指在字符前/后面的空格，通常情况下，你需要将它去除。

#### 实例
`strip()`方法去除字符前/后的多余空格：
```python
a = ' Hello, World! '
print(a.strip())
# 这将返回'Hello, World!'
```

### 替换字符

#### 实例
`replace()`方法将一个字符替换为另一个：
```python
a = 'Hello, World!'
print(a.replace('H', 'J'))
```

### 分割字符串
`split()`方法将返回一个序列，分割好的字符串将是序列的项。（可以指定分隔符）

#### 实例
```python
a = 'Hello, World!'
print(a.split(','))
# 这将返回['Hello', ' World!']
