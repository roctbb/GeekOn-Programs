## Вступительные испытания на второй семестр обучения 

### Программирование на Python

Что будет выведено на экран в следующих программах:

```python
a = 10 / 4 * 2
b = 13 % 4 // 2
print((a + b) ** 3)
```
---
```python
def strangeMultiply(a, b):
    result = a * (b + 2)
    return result

c = strangeMultiply(2, strangeMultiply(3, 4))
print(c)
```
---
```python
for i in range(0, 5):
    print(" " * (4 - i) + "#" * (2 * i + 1))
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
sentence = "Do you know the way to the library?"
sentence = sentence.replace("the", "de").upper()
print(sentence[:18] + sentence[-1])
```
---
На диске в папке с программой лежит файл text.txt с следующим текстом:

```
python 1 - сб и вс, 18:00
python 2 - сб, 14:00
С++ - вс, 14:00
Frontend&Backend - сб и вс, 14:00
```

```python
with open('text.txt', 'r') as file:
    text = file.read()
words = text.split(' ')
counter = {}
for word in words:
    if word not in counter:
        counter[word] = 1
    else:
        counter[word] = counter[word] + 1
print(counter['python'])
```
---
```python
matr = [
    [1, 2, 3],
    [1, 0, 2],
    [3, 2, 1]
]
p = 0
for l in matr:
    p += sum(l)
print(p)
```
