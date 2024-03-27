# isinstance 函数的使用

isinstance() 是一个内置函数，用于检查一个对象是否是指定类或类型的实例。它的语法如下：
`isinstance(object, classinfo)`

1.object：要检查的对象。
2.classinfo：可以是一个类、类型（如 int、str、list 等），或者是一个包含类或类型的元组（用于检查对象是否属于元组中的任何一个类或类型）。

isinstance() 返回一个布尔值，如果 object 是 classinfo 类或类型的实例，返回 True；否则，返回 False。
以下是一些示例用法：

1.  检查一个整数是否是 int 类型的实例：

```python
x = 5
result = isinstance(x, int)  # 返回 True，因为 x 是 int 类型的实例
```

1.  检查一个字符串是否是 str 类型的实例：

```python
s = "Hello, World!"
result = isinstance(s, str)  # 返回 True，因为 s 是 str 类型的实例
```

1.  检查一个对象是否是多个类型中的任何一个：

```python
x = 5
result = isinstance(x, (int, str, list))  # 返回 True，因为 x 是 int 类型的实例
```

1.  检查一个对象是否是某个自定义类的实例：

`class MyClass:
pass`

`obj = MyClass()
result = isinstance(obj, MyClass)  # 返回 True，因为 obj 是 MyClass 类型的实例`

isinstance() 在编写灵活和健壮的代码时非常有用，因为它允许您根据对象的类型执行不同的操作或采取不同的控制流。这对于类型检查和多态性编程非常有帮助。
