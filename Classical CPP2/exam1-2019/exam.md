## Промежуточный зачет по курсу "Объектно-ориентированное программирование на С++"

### Задание 1 (16 баллов)

Сколько памяти занимают следующие структуры?

```cpp
int a;
const char b='a';
unsigned short mas[2048];
long long m[1024];
```


### Задание 2 (12 + 12 + 12 баллов)  

Что будет выведено на экран?


```cpp
#include <iostream>
#include <cstdlib>

using namespace std;

class Dog {
protected:
    int hunger;
public:
    Dog(int _hunger) {
        hunger = _hunger;
    }
    void voice() {
        for (int i=0; i<hunger; i++)
            cout<<"wow ";
    }

};
class Wolf:public Dog {
public:
    Wolf (int a) : Dog (a*2) {

    }
    void voice() {
        cout<<"a";
        for (int i=0; i<hunger; i++)
            cout<<"u";
    }
};

int main()
{
    Dog A(2);
    Wolf B(4);
    A.voice();
    B.voice();
    return 0;
}
```
---

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
---
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

### Задание 3 (15 баллов)

Реализуйте класс так, чтобы код начал работать...

```cpp
int main() {
    Line A (3,4);

    A.show(); // 3x + 4 = y

    cout<<A.checkPoint(0, 0)<<endl; // false: 3*0 + 4 != 0;
    cout<<A.checkPoint(2, 10)<<endl; // true: 3*2 + 4 == 10;

    return 0;
}
```

### Задание 4 (25 баллов)

Реализуйте структуру данных очередь, которая поддерживает три операции:
 - push - добавление элемента в конец очереди;
 - pop - возвращает первый элемент в очереди и удаляет его;
 - empty - возвращает true, если очередь пуста;
 
Критерии оценивания:

* **5 баллов** - можно добавлять в очередь ограниченное количество элементов;
* **5 баллов** - можно создать очередь для любого типа данных (шаблоны);
* **5 баллов** - при попытке достать элемент из пустой очереди выкидывается исключение;
* **5 баллов** - когда память заканчивается, размер очереди увеличивается автоматически;
* **5 баллов** - эффективное использование памяти (кольцевой буффер: если при отсутствии места в конце массива есть свободное место в начале, используются ячейки в начале).

