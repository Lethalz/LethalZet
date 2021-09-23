# CPP First Day notes


The cout object, together with the << operator, is used to output values/print text:

Example

```cpp
#include <iostream>
using namespace std;

int main() {
  cout << "Hello World!";
  return 0;
}
```

Two `\n` characters after each other will create a blank line:

Example
```cpp
#include <iostream>
using namespace std;

int main() {
  cout << "Hello World! \n\n";
  cout << "I am learning C++";
  return 0;
}
```

Another way to insert a new line, is with the `endl` manipulator

## Comments and Variables

Single-line comments start with two forward slashes (`//`).

Any text between `//` and the end of the line is ignored by the compiler!

// ALL OF THIS IS IGNOREDD

---

Variables are containers for storing data values.

In C++, there are different types of *variables* (defined with different keywords), for example:

* int - stores integers (whole numbers), without decimals, such as 123 or -123
* double - stores floating point numbers, with decimals, such as 19.99 or -19.99
* char - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
* string - stores text, such as "Hello World". String values are surrounded by double quotes
* bool - stores values with two states: true or false

**To create a variable, you must specify the type and assign it a value:**

```type variable = value;```

*Type* could be any one of the data types such as `Int`.

*Variable* is the container for your value you can name it anything thats not a key word in Cpp 
***Also a Variable Cannot begin with a number or anything special Has to begin with (a..z,A..Z) Or an underscore***

### Quick Tip 

You can also declare a variable without assigning the value, and assign the value later:

Example 

```cpp
int myNum;
myNum = 15;
cout << myNum;
```

To declare more than one variable of the same type, use a comma-separated list:

Example

```cpp
int x = 5, y = 6, z = 50;
cout << x + y + z;
```

## Identifiers 

All C++ variables must be identified with unique names.

These unique names are called identifiers.

Identifiers can be short names (like `x` and `y`) or more descriptive names (age, sum, totalVolume).

**Note: It is recommended to use descriptive names in order to create understandable and maintainable code:**

Example
```cpp
// Good
int minutesPerHour = 60;

// OK, but not so easy to understand what m actually is
int m = 60;
```

## Constants

When you do not want others (or yourself) to override existing variable values, use the `const` keyword (this will declare the variable as "constant", which means **unchangeable and read-only**):

Example
```cpp
const int myNum = 15;  // myNum will always be 15
myNum = 10;  // error: assignment of read-only variable 'myNum'
```
***NOTE: You should always declare the variable as constant when you have values that are unlikely to change:***

Example
```cpp
const int minutesPerHour = 60;
const float PI = 3.14;
```


