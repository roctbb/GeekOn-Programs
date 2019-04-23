## Самостоятельная работа по программированию на Python

**Ваше имя:**

В заданиях ниже вам нужно написать, что компьютер выведет на экран после запуска программы. Писать можно прямо на этих листках.

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
---

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
---
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

---

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

```python
def my_func(a):
  print('*' * a)
  
my_func(1)
my_func(2)
my_func(3)
```

---

Будет ли работать эта программа? Если нет, то как ее исправить?
```python
def my_func():
  a += 15
  
a = 5
my_func()
print(a)
```
---
```python
v = int(input())
s = "Вася любит {0}"
if v and not True:
    print(s.format("кодить"))
elif v or True:
    print(s.format("спать"))
else:
    print(s.format("гулять"))
```
---
```python
for i in range(1,10,2):
    print("*" * i)
```
---
```python
s = 0
a = 0
b = 1
while b < 13:
    s += a
    c = a
    a = b
    b = b + c
print(s)
```
---
```python
animals = ['cow', 'camel', 'pig', 'frog', 'horse', 'goat']
for animal in animals:
    if len(animal) > 4:
        print(animal[::-1])
```
####

---
```python
sentence = "Мама мыла раму"
sentence = sentence.lower().replace("м", "п")
print(sentence[:4] + sentence[10:])
```
---
```python
matr = [
    [1, 2, 3],
    [1, 5, 2],
    [3, 2, 1]
]
p = 1
for l in matr:
    p *= sum(l)
print(p)
```
---
```python
a = 5
l = [a, a, a, a]
l2 = l
l2[0] = 6
print(l)
```
---
```python
a = [1, 2, 3]
for i in a:
    i += 2
print(a)
```
