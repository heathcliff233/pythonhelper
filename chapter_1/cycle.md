# cycle
for as iterator 作为迭代器
```python
lst = [1,3,5,7]
x = iter(lst)
next(x)
```
realization of for loop
```python
x = iter([1,2,3])
while True :
    try:
        print(next(x))
    except StopIteration:
        break
```
while/for else
```python
for i in range(1,10,2):
    if i % 5 == 0 :
        print('bingo')
        break
else:
    print(i)
```
----
further see ai_programming/3.12/循环、for循环内部