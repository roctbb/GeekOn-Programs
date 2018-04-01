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
    c = a
    a = b
    b = c
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
### Часть 2: Практика

#### 2048

В игре 2048 на поле появляются двойки, которые можно объединять друг с другом, получая четвёрки (по одной из двух двоек). Четверки можно объединять в восьмерки и так далее. Напиши программу, которая будет выводить максимальное число, которое можно получить из заданного количества двоек.

**Ввод:** n - количество доступных двоек.

**Вывод:** какое максимальное число можно получить от объединения n двоек.

<table>
<tr><td>Ввод</td><td>Вывод</td></tr>
<tr><td>2</td><td>4</td></tr>
<tr><td>3</td><td>4</td></tr>
<tr><td>12</td><td>16</td></tr>
</table>



