## Pascal

**Ваше имя:**

В заданиях ниже вам нужно написать, что компьютер выведет на экран после запуска программы. Писать можно прямо на этих листках справа от кода.

```pascal

A := 5 + 10;
writeln(A);

B := A / 2;
writeln(B);

C := B * 3 div 2;
writeln(C);

D := C mod 3;
writeln(D);

```
---

```pascal
A := 5;
B := 17;

if ((A + B mod 2) == 0) then
    writeln(A);
else
    if (((A + B) mod 3) == 0) then
         writeln(A * 2);
    else
        writeln(A * 3);
```
---
```pascal
weather := 22;
rain := 'no';

if (weather > 25) then
    writeln('го в футбол');
else
    if (weather > 20 and rain == 'no') then
        writeln('го гулять!');
    else:
        writeln('го в фортнайт!');
```

---
С какой вероятность программа выведет слово *джекпот*?:
```pascal

randomize;
if (random(100-1+1)+1 > 30) then
  writeln('джекпот');
else
  writeln('кот в мешке');
```
---

```pascal
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
```pascal
Randomize;
n := Random(10) + 1;
for i:= 1 to n do write('*');
```
---
```pascal
s := 0;
a := 0;
b := 1;
while (b < 13) do begin
    s := s + a;
    c := a;
    a := b;
    b := b + c;
end;
writeln(s);
```
---
```pascal
n := 6;
animals := ['cow', 'camel', 'pig', 'frog', 'horse', 'goat']
for i:= 1 to n do
    if (length(animals[i]) > 4) then
	for j := length(animals[i]) downto 1 do
        	writeln(animals[j]);
```
---
```pascal
matr := (
    (1, 2, 3),
    (1, 5, 2),
    (3, 2, 1));
p := 1;
n:= 3;
for i:=1 to n do begin
	sum := 0;
	for j := 1 to n do 
        	sum := sum + matr[i,j];
    	p := p *  sum;
end;
writeln(p);
```
---
```pascal
a := 5;
l := (a, a, a, a);
l2 := l;
l2[0] := 6;
writeln(l);
writeln(l2);
```

В следующих заданиях попробуйте написать код на листочке, не используя компьютер.

#### Маленькая, но гордая птичка!

Вы играли в Flappy Bird? В этой игре птичке нужно преодолевать препятствия, пролетая между двух преград. 

Вам нужно написать такую же игру, только пока без графики. В каждый момент времени вводятся три числа - границы проема и позиция птички по вертикали. Игра заканчивается, когда птица в проем не пролезает. Нужно вывести, сколько было набрано очков!

<table>
<tr><td>Ввод (жирный выделена координата птицы)</td><td>Вывод</td></tr>
<tr><td>
 1 <b>2</b> 3<br>
 4 <b>5</b> 6<br>
 6 <b>2</b> 9<br>
 </td><td>2</td></tr>
<tr><td>
 100 <b>101</b> 110<br>
 100 <b>100</b> 110
 </td><td>1</td></tr>
</table>

В первом примере птица успешно пролетела две "дырки", но на третий раз угодила в нижнюю стену. Во втором примере птица пролетела в первый проем, но затем врезалась в нижний край следующего.

#### Четные и нечетные

Вводится 20 чисел. Если их сумма четная - вывести все четные, а если нечетная - только нечетные.
