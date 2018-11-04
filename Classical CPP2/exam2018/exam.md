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
####

```cpp
#include <iostream>
using namespace std;
const int N=10;
int func(int a)
{
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
using namespace std;
int func(int a)
{
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
void step(char * str)
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
