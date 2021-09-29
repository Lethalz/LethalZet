# Type Conversion Operators

**C++** also has *four operators* for type conversion. They are known as **type conversion operators**:

1. static_cast
2. dynamic_cast
3. const_cast
4. reinterpret_cast

## static_cast conversion

*Syntax*:
`  static_cast < new_type > ( expression )		`

**Static Cast**: This is the *simplest* type of cast which can be used, It can also be called a **compile time cast**

It does things like *implicit conversions* between types (such as `int` to `float`, or pointer to void*), and it can also call *explicit conversion* functions (or implicit ones).

*Example* 
 ```cpp
 #include <iostream>
using namespace std;
int main()
{
    float f = 3.5;
    int a = f; // this is how you do in C
    int b = static_cast<int>(f);
    cout << b;
}
```
Output is 3 which undermines the built-in Hierarchical structure because of the line ` int b = static_cast<int>(f);`




