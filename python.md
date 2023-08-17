# python
> Written with [StackEdit](https://stackedit.io/).
python中有一种特殊的元组叫做命名元组，命名元组可以构建自己的数据结构
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
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTg1OTcyNjkxXX0=
-->