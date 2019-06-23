# set
zip to combine
```python
a = [1,2,3]
b = [4,5,6]
print(set(zip(a,b)))
# get {(2, 5), (3, 6), (1, 4)}
```
counter realization
```python
p_dic1 = {}
for item in p_list :
    p_dic1[item] = p_dic1.get(item,0) +1
```
**dic.get()** 
dict.get(key, default = None)
if the key do not exist, return the second argument given

----
further see ai_programming/3.12/集合