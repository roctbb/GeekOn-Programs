## Промежуточный зачет по прикладному программированию на Python

### Часть 1: Программирование на Python

Что будет выведено на экран в следующих программах:

```python
a = 10 / 4 * 2
b = 13 % 4 // 2
print((a + b) ** 3)
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
    a, b = b, a + b
print(s)
```
---
```python
animals = ['cow', 'camel', 'pig', 'frog', 'horse', 'goat']
for animal in animals:
    if len(animal) > 4:
        print(animal[::-1])
```
---
```python
sentence = "Мама мыла раму"
sentence = sentence.lower().replace("м", "п")
print(sentence[:4] + sentence[10:])
```
---
```python
d = {}
list = [1, 2, 3, 3, -45, 23, 6, 23, 3]
for elem in list:
    if elem in d.keys():
        d[elem] += 1
    else:
        d[elem] = 1
print(d[3])
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
### Часть 2: Теория

1. Что такое условный оператор? Как он записывается на блок-схеме и в коде? Объединение условий с условной операторе.
3. Чем цикл while отличается от for? Зачем нужна команда break?
1. Что такое список? Чем он отличается от словаря? Как добавить новый элемент в список? В словарь?

