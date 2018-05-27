### Задание 1

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

# .
# .

### Задание 2

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
# .
# .
# .
# .

### Прямая
```cpp
int main() {
    Line A (3,4);

    A.show(); // 3x + 4 = y

    cout<<A.checkPoint(0, 0)<<endl; // false: 3*0 + 4 != 0;
    cout<<A.checkPoint(2, 10)<<endl; // true: 3*2 + 4 == 10;

    return 0;
}
```

### Кошкин дом
```cpp
int main() {
    Cat Masha;
    Masha.setHunger(3);
    
    Dog Bobik;
    Bobik.setHunger(2);
    
    Masha.say(); // meow meow meow
    Bobik.say(); // bark bark
}
```
