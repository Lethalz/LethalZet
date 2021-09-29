# Data Type Conversion

C++ allows us to *convert* data of one type to that of another.

**There are two types of type conversion in C++**:

1.Implicit Conversion

2.Explicit Conversion (also known as **Type Casting**)

### Implicit Type Conversion

Whenever an *integer* and a *floating-point* variable or constant are mixed in an operation, the integer is
changed **temporarily** to its equivalent floating.

This automatic conversion is called **implicit type coercion**.

```cpp
// Working of implicit type-conversion

#include <iostream>
using namespace std;

int main() {
   // assigning an int value to num_int
   int num_int = 9;

   // declaring a double type variable
   double num_double;
 
   // implicit conversion
   // assigning int value to a double variable
   num_double = num_int;

   cout << "num_int = " << num_int << endl;
   cout << "num_double = " << num_double << endl;

   return 0;
}
```
Both of the Variables end up being 9 but the num_int gets converted to a double which switch to the `double` variable.

This also works *vice versa*. If the `double` was say `9.99` and you put it into a declared `int` variable you would on get 9 as an output.

Because we are dealing with a **Hierarchical system** when it comes to *data type conversions* the conversion from one data type to another is prone to data loss. 

This happens when data of a *larger* type is converted to data of a *smaller* type.


### Explicit Conversion

When the user *manually* changes data from one type to another, this is known as **explicit conversion**. 

This type of conversion is also known as **type casting** or **Manual Conversion**.

**Three Types**: 

1. C-style type casting (also known as cast notation)
2. Function notation (also known as old C++ style type casting)
3. Type conversion operators

Type conversions can be made explicit (by the programmer) by using the
following Code.

#### C-style Type Casting

This type of casting is favored by the *C programming language*. It is also known as **cast notation**.

Syntax:

`(data_type)expression;`

*Example*:
```cpp
// initializing int variable
int num_int = 26;

// declaring double variable
double num_double;

// converting from int to double
num_double = (double)num_int;
```


#### Function-style Casting

I can also use the `function` like notation to cast data from one type to another.
*Syntax*:
`data_type(expression);`

*Example*

```cpp
// initializing int variable
int num_int = 26;

// declaring double variable
double num_double;

// converting from int to double
num_double = double(num_int);
```

#### Type Casting

```cpp
#include <iostream>

using namespace std;
int main() {
    // initializing a double variable
    double num_double = 3.56;
    cout << "num_double = " << num_double << endl;

    // C-style conversion from double to int
    int num_int1 = (int)num_double;
    cout << "num_int1   = " << num_int1 << endl;

    // function-style conversion from double to int
    int num_int2 = int(num_double);
    cout << "num_int2   = " << num_int2 << endl;

    return 0;
}
  ```
  
  We used both the *C style* type conversion and the *function-style* casting for type conversion and displayed the results. 
  
  Since they perform the same task, both give us the **same output**.
  
  
 [Type Conversion Operators](https://github.com/Lethalz/LethalZet/tree/main/202128092136)

