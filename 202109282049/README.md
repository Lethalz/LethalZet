# Expressions in CPP

An **expression** is a sequence of *operators* and their *operands*, that specifies a computation.


### PEMDAS

Expresssions in cpp follows algebraic *Order of Operations*:

1. Anything grouped in parentheses is top priority
2. Unary negation (example: –8)
3. Multiplication, Division and Modulus * / %
4. Addition and Subtraction + –'


Which leads to being able to use **algebraic expressions** in cpp!

*For example*:

**Normally**: 4y(3-2)y+7  

**CPP**:`4 * y * (3-2) * y + 7`



There are several predefined math library routines that are contained in the
`cmath` library. 

In order to use these we must have the `#include <cmath>` direc-
tive in the header.

Included in this library is `pow(number,exp)` This is how we deal with *exponants* in CPP

`2^3` would be written as `pow(2,3)`

`5^9` would be written as `pow(5,9)`


**Square roots** are handled by `sqrt(n)`

square root 9 would be written as `sqrt(9)`
