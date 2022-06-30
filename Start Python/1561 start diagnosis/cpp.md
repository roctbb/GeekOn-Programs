## Python

**Ваше имя:**

В заданиях ниже вам нужно написать, что компьютер выведет на экран после запуска программы. Писать можно прямо на этих листках справа от кода. Для краткости `int main`
в примерах опущен.

```cpp

int A = 5 + 10;
cout << A << endl;

double B = (double) A / 2;
cout << B << endl;

int C = B * 3 / 2;
cout << C << endl;

int D = C % 3;
cout << D << endl;
```
---

```cpp
int A = 5;
int B = 17;

if (A + B % 2 == 0) {
    cout << A;
}
else if ((A + B) % 3 == 0) {
    cout << A * 2;
}
else {
    cout << A * 3;
}
```
---
```cpp
int weather = 22;
string rain = "no";

if (weather > 25) {
    cout << "lets play football!";
}
else {
    if (weather > 20 and rain == "no") {
        cout << "lets walk under rain!";
    } 
    else {
        cout << "lets play dota 2!";
    }
}
```

---
С какой вероятность программа выведет слово *джекпот*?

```cpp
srand(time(0));
if (rand() % 100 > 30) {
    cout << "jackpot!";
}
else {
    cout << "just a can with cucumbers!";
}
```
---

```cpp

void my_func(int a) {
    cout << "Ocean is shaking " << a << endl;
}

int main() {
    my_func(1);
    my_func(2);
    my_func(3);
}
```
---
```cpp
int v;
cin >> v;

if (v && !1) {
    cout << "Vasya likes coding";
}
else if (v || 1) {
    cout << "Vasya likes to sleep";
}
else {
    cout << "Vasya likes to walk";
}
```
---
```cpp
int s = 0;
int a = 0;
int b = 1;
while (b < 13)
{
    s += a;
    int c = a;
    a = b;
    b = b + c;
}
    
cout << s;
```
---
```cpp
void step(char str[255])
{
   for (int i=0; i<strlen(str); i++)
   {
       str[i] = str[i]+1;
   }
}
int main() {
   char a[] = "abba";
   step(a);
   cout<<a;
   return 0;
}

```
---
```cpp
void f1(int a)
{
   a++;
}
void f2(int& b)
{
   b++;
}
int main() {
   int a = 1;
   f1(a);
   f2(a);
   cout<<a;
   return 0;
}

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
