# Formatted output in CPP


C++ has special instructions that allow the user to control output attributes such
as spacing, decimal point precision, data formatting and other features.

To get access to these features you will need to put `#include <iomanip>` into your code header.

`cout << fixed`  Displays the output in decimal format rather than scientific notation.

`cout << showpoint;` Forcues all floating-point output to show a decimal point even if the values are whole numbers.

`cout << setprecision(2)` Rounds all floating point numbers to 2 decimal places. *can change the `2` for another number*


These are Examples of **Stream Manipulators**, the order in which they appear do not matter in the code. You can put them anywhere to recieve the formatted output.

**Spacing** is handled by an indication of the width of the field that the number , charater or string is to be placed it can be done with the `cout.width(n);`

`n` is the width size 

`setw(n)` is the more commonly used one.



For reference:

`cout << "Hi there\n"; cout << "Hi there" << endl;`

**Line Enders** 
