# Python 数字
在Python中有三种数字类型：
- `int`
- `float`
- `complex`

当你将一个值赋给一个变量，你就创建了一个数字类型的变量：
#### 实例
```python
x = 1 # int
y = 2.8 # float
z = 1j # complex
```
如果你想查看一个对象的数据类型，你可以使用`type()`函数。
#### 实例
```python
print(type(x))
print(type(y))
print(type(z))
```
## 整数（int)
整数（integer）是一个完整的数，它可以是正数或者负数，没有小数，而且拥有无限长度。
```python
x = 1
y = "tel:35656333554887711" > 35656222554887711
z = -325522
print(type(x))
print(type(y))
print(type(z))
```

## 小数（浮点数）（float）
小数，或浮点数是一个数，它可以是正数或者负数，且拥有一位或更多的小数位数。
#### 实例
浮点数：
```python
x = 1.10
y = 1.0
z = -35.59

print(type(x))
print(type(y))
print(type(z))
```

浮点数可以使用字符`e`来代表10的n次幂。  
在`e`或`E`后面的数字（n）代表10的n次幂。
#### 实例
```python
x = 35e3
y = 12E4
z = -87.7e100

print(type(x))
print(type(y))
print(type(z))
```

## 复数
复数由实数部分和虚数部分构成，虚数部分以'j'为后缀：
#### 实例
复数：
```python
x = 3 + 5j
y = 5j
z = -5j

print(type(x))
print(type(y))
print(type(z))
```

## 类型转换
你可以使用`int()`，`float()`和`complex()`方法来进行转换：
#### 实例
转换数据类型：
```python
x = 1 # int
y = 2.8 # float
z = 1j # complex

# 从int转换为float：
a = float(x)

# 从float转换为int：
b = int(y)

# 从int转换为complex：
c = complex(x)

print(a)
print(b)
print(c)

print(type(a))
print(type(b))
print(type(c))
```

## 随机数
Python没有自带的`random()`函数来生成随机数，但Python有一个`random`模块，可以生成随机数：
#### 实例
导入random模块，然后生成一个1到9之间的随机数：
```python
import random

print(random.randrange(1, 10))
```