# IOstream
  
**输入切割**(split() func)
```python
a , b = input().split()
a , b = input().split(',')
```
**自动判定** identify automatically
```python
a = eval(input())
# input -> '1,2,3.5'
# a = (1 , 2 , 3.5)
```
> 格式输出(format output)

```python
x,y = 3,5
print(x,y)
# get 3 5
```
seperate
```python
x,y = 3,5
print(x , y , sep = ',')
# get 3,5
```
without changing line
```python
list = [2,3,4,5,6]
for i in list[:-1]:
    print(i,',',end = ' ')
print(list[-1])
# get 2 , 3 , 4 , 5 , 6
```
format
```python 
x,y = 3,5
print('x=%d,y=%d'%(x,y))
# get x=3,y=5
```
change line within arg
```python
print('x=%d,y=%d \nhhhhhhh'%(x,y))
```
保留小数(save dots)
```python
z = 2.237237
print('the result is %.2f.'%z)
```
control white space
```python
print('the result is %10.2f.'%z)
# 格式对齐，表示占多少列
# get: the result is       2.24.
```
with many arguments to fill
```python
print('x = {0:d},z={1:.2f}'.format(x,z)) 
#1 表示format中位置
```
----
further see ai_programming/3.12/3.12 集合