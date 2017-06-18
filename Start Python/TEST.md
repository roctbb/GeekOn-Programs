## Промежуточный зачет по прикладному программированию на Python

### Часть 1: Программирование на Python

Что будет выведено на экран в следующих программах:

1. ```python
a = 10 / 4 * 2
b = 13 % 4 // 2
print((a + b) ** 3)
```

2. ```python
v = int(input())
s = "Вася любит {0}"
if v and not True:
    print(s.format("кодить"))
elif v or True:
    print(s.format("спать"))
else:
    print(s.format("гулять"))
```

3. ```python
for i in range(1,10,2):
    print("*" * i)
```

3. ```python
s = 0
a = 0
b = 1
while b < 13:
    s += a
    a, b = b, a + b
print(s)
```

