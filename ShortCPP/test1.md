### Промежуточный зачет по курсу "Объектно-ориентированное программирование на С++"

Сколько оперативной памяти занимают следующие структуры?

```cpp
int a;
const char b='a';
unsigned short mas[2048];
long long m[1024];
```

Что будет выведено на экран в следующих программах?

```cpp
#include <iostream>
using namespace std;
int multiply(int a, int b)
{
   return a*b;
}
int main() {
   cout<<multiply(multiply(5,4), 3);
   return 0;
}
```

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
