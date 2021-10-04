# CPP USER INPUTS AND DATA TYPES

`cin` is a predefined variable that reads data from the keyboard with the extraction operator (`>>`).

The name `cin` refers to the standard input stream (pronounced “see-in,” for “char-
acter input”)

In the following example, the user can input a number, which is stored in the variable x. Then we print the value of x:

Example
```cpp
int x; 
cout << "Type a number: "; // Type a number and press enter
cin >> x; // Get user input from the keyboard
cout << "Your number is: " << x; // Display the input value
```
----

**Creating a Simple Calculator**

```cpp
int x, y;
int sum;
cout << "Type a number: ";
cin >> x;
cout << "Type another number: ";
cin >> y;
sum = x + y;
cout << "Sum is: " << sum;

```
Can be used to input more than one value, one after another:

```cpp
cin >> height >> width
```
Order is very important the first value entered goes to the first variable.

An *object* is a region of memory with a type that specifies what kind of
information can be placed in it. A named object is called a *variable*.

A statement that introduces a new name into a program and sets aside memory
for a variable is called a *definition*

`cin` does that here with `first_name`

```
int main()
{
    cout << "Please enter your first name (followed by 'enter'):\n";
    
    string first_name;  // first_name is a variable of type string
    cin >> first_name;  // read characters into first_name
   
   cout << "Hello, " << first_name << "!\n";
```

## DATA TYPES

a variable in C++ must be a specified data type:

```cpp
int myNum = 5;               // Integer (whole number)
float myFloatNum = 5.99;     // Floating point number
double myDoubleNum = 9.98;   // Floating point number
char myLetter = 'D';         // Character
bool myBoolean = true;       // Boolean
string myText = "Hello";     // String
```

|Data Type| Size | Description|
|----------|-----|-------------|
|int	|4 bytes|	Stores whole numbers, without decimals|
|float	|4 bytes	|Stores fractional numbers, containing one or more decimals. Sufficient for storing 7 decimal digits|
|double	|8 bytes	|Stores fractional numbers, containing one or more decimals. Sufficient for storing **15** decimal digits|
|boolean	|1 byte	|Stores true or false values|
|char	|1 byte	|Stores a single character/letter/number, or ASCII values
|void | 2/4/8 Bytes| Valueless *will learn later*|


# NUMBERS, BOOLEANS , CHARACTERS AND STRINGS

## Numeric Types
Use `int` when you need to store a whole number without decimals, like 35 or 1000, and `float` or `double` when you need a floating point number (with decimals), like 9.99 or 3.14515.


```cpp
int myNum = 1000;  // This is a integer(whole)
cout << myNum;

float myNum = 5.75; // This is a float jiggla
cout << myNum;

double myNum = 19.99; // This is a Double
cout << myNum;
```
### `Float` VS `Double`

The precision of a floating point value indicates how many digits the value can have after the decimal point. 

The precision of float is only six or seven decimal digits, while double variables have a precision of about 15 digits. 

**Therefore it is safer to use double for most calculations.**

## Boolean Types

A boolean data type is declared with the bool keyword and can only take the values true or false. 
When the value is returned, true = 1 and false = 0.

Example
```cpp
bool isCodingFun = true;
bool isFishTasty = false;
cout << isCodingFun;  // Outputs 1 (true)
cout << isFishTasty;  // Outputs 0 (false)
```

## Character Types 

The `char` data type is used to store a single character. The character must be surrounded by single quotes, like 'A' or 'c':

```cpp
char myGrade = 'B';
cout << myGrade;
```

you can use ASCII values to display certain characters:
```cpp
char a = 65, b = 66, c = 67;
cout << a;
cout << b;
cout << c;
```

This code would still print out ABC:

```cpp
int main () {
  char stan = 65, b = 66, c = 67;
  cout << stan;
  cout << b;
  cout << c;
  return 0;
}
```
[ASCII TABLE REFERENCE](https://www.w3schools.com/charsets/ref_html_ascii.asp)


## STRING TYPES

The string type is used to store a bunch of characters (text). This is not a built-in type, but it behaves like one in its most basic usage. 
String values must be surrounded by double quotes:

```cpp
string greeting = "Hello";
cout << greeting;
```

**To use strings, you must include an additional header file in the source code, the `<string>` library:**
```cpp
// Include the string library
#include <string>

// Create a string variable
string greeting = "Hello";

// Output string value
cout << greeting;
```


[Cout,Identifiers,constants](https://github.com/Lethalz/LethalZet/tree/main/202109231850.)


[NEXT>>](https://github.com/Lethalz/LethalZet/tree/main/202109252207)






