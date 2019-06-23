# object oriented
class object
```python
class Dog(object):
    '''
    ahhhh，that's good that is good
    '''
    def setName(self,name):
        self.name = name
    def greet(self):
        print('fuck%s'%self.name)
if __name__ == "__main__" :
    dog = Dog()
    dog.setName('Jack')
    print(dog.name)
    dog.greet()
```
自动调用 \__init__
```python
class Dog(object):
    '''
    ahhhh，that's good that is good
    '''
    def __init__(self,name):
        self.name = name
    def greet(self):
        print('fuck%s'%self.name)
if __name__ == "__main__" :
    dog = Dog('Jack')
    print(dog.name)
    dog.greet()
```
## 继承 heritage
### 子类
```python
class barkingdog(Dog):
    def bark(self):
        print('barking')
if __name__ == '__main__':
    dog = barkingdog('bili')
    dog.greet()
```
### 子类重写
```python 
class barkingdog(Dog):
    def bark(self):
        print('barking')
    def greet(self):
        print('that is good %s'%self.name)
if __name__ == '__main__':
    dog = barkingdog('bili')
    dog.greet()
```
super
(get father class)
```python 
class MyParentClass():
def __init__(self, x, y):
pass

class SubClass(MyParentClass):
def __init__(self, x, y):
super().__init__(x, y)
```
private 
```python
class P:
    def __init__(self,name):
        self.__name = name
x = P('Jack')
x.__name
# get an error
x._P__name
# get 'Jack'
```

