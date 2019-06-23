# errors
see built-in error types
```python
dir(__builtins__)
```
change error to output
```python
try :
    num1 = int(input('1:'))
    num2 = int(input('2:'))
    print(num1/num2)
except ZeroDivisionError :
    print('divided by 0 !')
```
print the error
```python
try :
    num1 = int(input('1:'))
    num2 = int(input('2:'))
    print(num1/num2)
except Exception as e :
    print(e)
```
fuck all the error
```python
# 一了百了
try :
    num1 = int(input('1:'))
    num2 = int(input('2:'))
    print(num1/num2)
except :
    print('stupid !')
```
have a saying at last if operated successfully (else)
```python
try :
    num1 = int(input('1:'))
    num2 = int(input('2:'))
    print(num1/num2)
except Exception as e :
    print(e)
else :
    print('ahhhh，that's good, that is good')
```
have a saying at last anyway (finally)
```python
try :
    num1 = int(input('1:'))
    num2 = int(input('2:'))
    print(num1/num2)
except Exception as e :
    print(e)
finally :  #无论如何都会被执行
    print('ahhhh，that's good, that is good')
```
