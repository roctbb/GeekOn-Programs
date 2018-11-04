## Промежуточный зачет по курсу "Объектно-ориентированное программирование на С++"

#### 1. Сколько оперативной памяти занимают следующие структуры?

```cpp
int a;
const char b='a';
unsigned short mas[2048];
long long m[1024];
```

#### 2. Что будет выведено на экран в следующих программах?

```cpp
#include <iostream>

using namespace std;

void f1(int a) {
    a++;
}

void f2(int *mas) {
    mas[0]++;
}

int main() {
    int a = 1;
    f1(a);
    int mas[10];
    mas[0] = 1;
    f2(mas);
    cout << a << mas[0];
    return 0;
}
```

```cpp
#include <iostream>
using namespace std;
const int N=10;
int func(int a) {
   if (a%3==0)
       return 1;
   return a*func(a+2);
}
int main() {
   cout<<func(2);
   return 0;
}
```
```cpp
#include <iostream>
#include <cstring>
using namespace std;
void step(char * str) {
   for (int i=0; i<strlen(str); i++) {
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

#### 3. Теория и практика
**Теория:** Класс. Свойства и методы. Конструктор и деструктор.

```cpp
#include <iostream>
#include <cstdlib>

using namespace std;

class A {
    int a;
public:
    A(int _a) {
        a = _a;
        cout<<"A";
    }
    ~A() {
        cout<<"B";
    }
    void func() {
        cout<<a;
    }
};

int main()
{
    A a(1);
    cout<<"C";
    for (int i=0;i<2;i++) {
        A b(2);
        b.func();
        a.func();
    }
    cout<<"C";
    return 0;
}
```

**Теория:** Динамическая память и операции для работы с ней?

```cpp
#include <iostream>
using namespace std;
int main() {
    int a = 3;
    int b = 2;
    int * c;
    int * d;
    c = &a;
    d = &b;
    cout<<*c**d;

    int mas[10];

    for (int i=0; i<10; i++)
        mas[i] = i;
    int * mas1 = mas+9;
    for (int i=0; i<10; i++)
       cout<<*(mas1-i);
}
```
Сколько памяти будет утеряно?
```cpp
#include <iostream>
using namespace std;
int main() {
    for (int i=0; i<1024*1024*1024; i++)
        char * a = new char;
}
```
#### 4. Практика

Реализуйте структуру данных стэк, которая поддерживает три операции:
 - push - добавление элемента на вершину стэка
 - pop - возвращает верхний элемент и удаляет его
 - empty - возвращает true, если стэк пуст

Используйте шаблоны.

