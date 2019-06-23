# string

**重复子串 repeat** 
```python
'5'*2000 #2000个5
```
**倒序 reverse**
```python
s = '12321'
s == s[::-1]
```
**读入列表 read list**
```python
s = eval(input())
# eval 可输入类似‘[1,4,2,3]’
```
**查看保留名 reserved namespace**
```python
import keyword
print(keyword.kwlist)
```
**数据地址 address**
```python
a = 5
b = 5
id(a) == id(b)
# 判定为True
# 小整形会重复利用空间
```
**取余 residual**
```python
28.31 % 4
# 对float型也适用
```
**链式赋值（从右向左依次运算）**
```python        
a = 1
b = a = a + 1
# b = 2 ; a = 2
```   
**查找 list find**
```python
str(i).find(str(x)) == -1
# 找不到
```

----
further see ai_programming/2.26
