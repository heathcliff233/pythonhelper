# function
## lambda
different from list analysis  
**map**
```python
lst = [1,2,3,4,5]
print(list(map(lambda x : x**2 , lst)))
# get [1,4,9,16,25]
```
```python
def foo(x):
    return x**2
print(list(map(foo,lst)))
# get [1,4,9,16,25]
```
```python
list(map(eval , ['1.2','3.4']))
# get [1.2 , 3.4]
```
```python
list(map(lambda x : x.upper(),['nju','pku']))
# get ['NJU','PKU']
```
**filter**
```python
print(list(filter(lambda x : x%2 == 0 , lst)))
# get [2,4]
```
**reduce**
```python
from functools import reduce
reduce(lambda x,y : x+y , lst)
# get 15
```
## func area
```python
x = 3 
def faQ():
    print(x * 2)
    x = 5
    print(x * 2)
faQ()
# get UnboundLocalError
# local variable 'x' referenced before assignment
```
```python
x = 3 
def faQ():
    global x
    print(x * 2)
    x = 5
    print(x * 2)
faQ()
# get 6 10
```
further see ai_programming/3.26/3.19补充

