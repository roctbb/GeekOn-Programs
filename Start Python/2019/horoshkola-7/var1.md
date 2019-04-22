### Самостоятельная работа

**Ваше имя:**

В заданиях ниже вам нужно написать, что компьютер выведет на экран после запуска программы. Писать можно прямо на этих листках.

**Задание 1: арифметические операции**

```python

A = 5 + 10
print(A)

B = A / 2
print(B)

C = B * 3 // 2
print(C)

D = C % 3
print(D)

E = D ** 2
print(E)
```

**Задание 2: условия**

```python
A = 5
B = 17

if A + B % 2 == 0:
    print(A)
elif (A + B) % 3 == 0:
    print(A * 2)
else:
    print(A * 3)
```

**Задание 3: еще условия**

```python
weather = 22
rain = "no"

if weather > 25:
    print("го в футбол")
else:
    if weather > 20 and rain == "no":
        print("го гулять!")
    else:
        print("го в фортнайт!")
```

**Задание 4: Рандом**

С какой вероятность программа выведет слово *джекпот*?:
```python
import random
if random.randint(1,100) > 30:
  print("джекпот")
else:
  print("кот в мешке")
```
# .
---

**Задание 5: Функции**

```python
def my_func(a):
  print('*' * a)
  
my_func(1)
my_func(2)
my_func(3)
```

**Задание 6: Еще функции**

Будет ли работать эта программа? Если нет, то как ее исправить?
```python
def my_func():
  a += 15
  
a = 5
my_func()
print(a)
```


