# list
### list analysis
```python
a = [x*x for x in range(10)]
```
```python
a = [x**2 for x in range(10) if x **2 < 50]
```
```python
a = [(x+1,y+1) for x in range(2) for y in range(2)]
```
```python
lst1 = ['ass','shit','fuck']
lst2 = [2,3,4]
m = [(a,b) for a in lst1 for b in lst2]
```
delete completely
```python
lst.remove()
```
**caution**
```python
lst = [1,2,4,3,5]
for x in lst :
    if x % 2 == 0:
        lst.remove(x)
print(lst)
# get [1,4,3,5]

# 问题：指针删除完元素下移，然而删除一个对象后下一个元素顶上，故出问题
lst = [1,2,4,3,5]
for x in lst[:] :
    if x % 2 == 0:
        lst.remove(x)
print(lst)
get [1,3,5]
```
### generater
``` python
(x**2 for x in range(10) if x**2 < 50)
# get <generator object <genexpr> at 0x1100b8840>
```
### jieba
```python
poem = '生活可能美满，可能悲伤，生活常常让你吃屎'
import jieba
s = list(jieba.cut(poem))
# get cut sentence
```
word counter
```python
import collections
collections.Counter(s)
```
[counter realization](/chapter_1/set.md)

further see ai_programming/3.19/3.19



