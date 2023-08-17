# python
> Written with [StackEdit](https://stackedit.io/).
python中有一种特殊的元组叫做命名元组，命名元组可以构建自己的数据结构。python中的namedtuple用以构建只有少数属性但是没有方法的对象
```python
from collections import namedtuple
# 命名元组对象student_info
student_info = namedtuple('stud_info','name, id, gender, age, score')
# 使用student_info对象对studinf进行赋值
studinf = student_info(name = 'xiaowang', id = '00001', gender = 'male', age = 22, score = 99)
print("name:{}, id:{}, gender:{}, age:{}, score:{}".format(studinf[0],studinf[1],studinf[2],studinf[3],studinf[4]))
```
```python 
from collections import namedtuple
# 命名元组对象student_info
student_info = namedtuple('stud_info','name, id, gender, age, score')
# 使用student_info对象对studinf进行赋值
studinf = student_info(name = 'xiaowang', id = '00001', gender = 'male', age = 22, score = 99)
print("name:{}, id:{}, gender:{}, age:{}, score:{}".format(studinf.name,studinf.id,studinf.gender,studinf.age,studinf.score))
```
python 中随机抽取一个元素的函数：
```python 
from random import choice
choice(deck)
```
python中的格式化输出方法
-   `{!r}`就是使用format语法时候的`%r`。因此，我们只需要关注`%r`就好。
- `%r`表示的用repr()处理；类似于的`%s`表示用str()处理一样。
其含义就是，转成解释器可以理解的部分。
比如，数字，就变成str；str就变成带有引号的str
在实际实现的时候是调用其内部的__repr__函数进行实现的

另一种格式化输出的方式是使用.format

<!--stackedit_data:
eyJoaXN0b3J5IjpbNDUwMDcxMTk5LC0xMDUxODI0NDU5LDEyMD
k1OTA3MDgsMTg1OTcyNjkxXX0=
-->