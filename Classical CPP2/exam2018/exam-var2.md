## Промежуточный зачет по курсу "Объектно-ориентированное программирование на С++"

### Задание 1
**Теория:** Массивы в С++.

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

### Задание 2
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

### Задание 3
**Теория:** Динамическая память и операции для работы с ней.

Сколько памяти будет утеряно?
```cpp
#include <iostream>
using namespace std;
int main() {
    for (int i=0; i<1024*1024*1024; i++)
        char * a = new char;
}
```
#### Задание 4

Реализуйте структуру данных стэк, которая поддерживает три операции:
 - push - добавление элемента на вершину стэка;
 - pop - возвращает верхний элемент и удаляет его;
 - empty - возвращает true, если стэк пуст.

Используйте шаблоны.

