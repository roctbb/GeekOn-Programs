## Итоговый зачет по курсу "КМБ-1"

### Часть 1: Программирование на Python

Что будет выведено на экран в следующих программах:

```python
a = 10 / 4 * 2
b = 13 % 4 // 2
print((a + b) ** 3)
```
---
```python
a = [1, 2, 3]
for i in a:
    i += 2
print(a)

```
---
```python
for i in range(15,5,-3):
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
    if len(animal) > 3:
        print(animal[::2])
```
---
```python
sentence = "Мама мыла раму"
sentence = sentence.upper().replace("а", "у")
print(sentence[:2] + sentence[12:])
```
---
### ...
```python
d = {}
list = [1, 2, 3, 3, -45, 23, 6, 23, 3]
for elem in list:
    if elem in d.keys():
        d[elem] += 1
    else:
        d[elem] = 1
print(d[2])
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
    p += sum(l) // 2
print(p)
```

### Часть 2: Практика

1. Напишите фотофильтр, который находит средний цвет всех пикселей картинки и закрашивает картинку этим цветом.
2. Напишите веб-сервис, который будет показывать все сообщения, которые пользователи отправляют телеграм боту.

