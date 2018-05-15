### Проверочная работа по программированию

Напишите, что будет выведено в результате работы следующих программ. **Не забудьте подписать работу.** Удачи! :)

```python
print(2 + 4)
print(5 / 2)
print(2 ** 3)
print(10 // 3)
print(7 % 3)
```
---

```python
a = 10
b = 15
c = b - a
print(c * 3)
```
---

Что надо ввести с клавиатуры, чтобы программа вывела 15?

```python
a = 3
b = int(input())
print(a * b // 2)
```
---
Приведите пример входных данных, на которых программа выведет *Поло*:
```python
a = int(input())
if a % 2 == 0 or a // 3 != 0:
  print("Марко")
else:
  print("Поло")
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
sentence = "Мама мыла раму"
sentence = sentence.lower().replace("м", "п")
print(sentence[:4] + sentence[10:])
```
---