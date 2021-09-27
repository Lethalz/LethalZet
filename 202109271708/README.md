# CPP Operators 

*Operators* are used to operate on Variables and constants. I may not remember all of these but it will be a good reference to get down what I understand.

## Arithmatic Operators

There are *five* Arithmatic operators:


|operator|	description|
|--------|--------------|
|+|	addition|
|-|subtraction|
| * |	multiplication|
|/|	division|
|%|	modulous|

The first four Arithmatic operators should come easy to use they are the same operators we use in everyday math.

The *Modulous* Operator , defined by the percentage symbol `%`, shows the remainder of a division of two values instead of the whole number.

## Assignment Operators

Assignment meaning we're assigning a value to a variable. For example `x = 5`; The assignment operation always takes place from right.

If a variable value changes later on in the statement it doesnt affect the previous statement:

```cpp
int main ()
{
  int a, b;         // a:?,  b:?
  a = 10;           // a:10, b:?
  b = 4;            // a:10, b:4
  a = b;            // a:4,  b:4
  b = 7;            // a:4,  b:7

  cout << "a:";
  cout << a;
  cout << " b:";
  cout << b;
}
```
There are also **Compound assignment** Operators that make the variable operate on itself, i know that sounds weird but let me show you:

```cpp
int main ()
{
  int a, b=3;
  a = b;
  a+=2;             // equivalent to a=a+2
  cout << a;
}
```

All of the **compound assignment** operators work the same as the one in the example above here is a table of the available operators: 
|operator| example | also |
|---------|---------|-------|
|=|	x = 5	x = 5	
|+=|	x += 3|	x = x + 3	|
|-=|	x -= 3|	x = x - 3	|
|*=|	x *= 3|	x = x * 3	|
|/=|	x /= 3|x = x / 3	|
|%=|	x %= 3|	x = x % 3	|
|&=|	x &= 3|	x = x & 3	|
|\|=|	x \|= 3|	x = x \| 3	|
|^=|	x ^= 3|	x = x ^ 3	|
|>>=|	x >>= 3|	x = x >> 3|	
|<<=|x <<= 3	|x = x << 3|

## Comparison Operators

Two code expressions can be compared using relational or comparison operators. For example, you can use it to know if two values are equal or if one is greater than the other.

The return value of a comparison is either true (`1`) or false (`0`).

These perators Work on Constants as well as Variables.
`a = 5 a == a` 


|Operator |Desc|
|---------|-----|
|==	|Equal to      |
|!=	|Not equal to|
|<	|Less than| 
|>	|Greater than|
|<=	|Less than or equal to|
|>=	|Greater than or equal to|

## Logical Operators 

Logical Operators are used to determine logic between variables and constants,

The operator `!` is the C++ operator for the Boolean operation NOT:

```cpp
!(5 == 5)   // evaluates to false because the expression at its right (5 == 5) is true
!(6 <= 4)   // evaluates to true because (6 <= 4) would be false
!true       // evaluates to false
!false      // evaluates to true 
```

**The logical AND operator (`&&`) returns `true` if both operands are true and returns `false` otherwise. 

The operands are implicitly converted to type `bool` before evaluation, and the result is of type bool.

```cpp
int main() {
   int a = 5, b = 10, c = 15;
   cout  << boolalpha
         << "The true expression "
         << "a < b && b < c yields "
         << (a < b && b < c) << endl
         << "The false expression "
         << "a > b && b < c yields "
         << (a > b && b < c) << endl;
         return 0;
  }
 ```
   
   The logical OR operator (`||`) returns the boolean value `true` if either or both operands is true and returns `false` otherwise. It's also the same as the AND operator and will convert the type to bool before evaluation.
   ```cpp
   int main() {
   int a = 5, b = 10, c = 15;
   cout  << boolalpha
         << "The true expression "
         << "a < b || b > c yields "
         << (a < b || b > c) << endl
         << "The false expression "
         << "a > b || b > c yields "
         << (a > b || b > c) << endl;
         return 0;
}
   ```
 







