# CPP Strings

A **`string`** variable is a collection of chars surrounded by double quotes

`string curse = "fuck"`

### String Concatenation

The `+` operator can be used between strings to add them together to make a new string. This is called *concatenation*:

```cpp
string firstName = "John ";
string lastName = "Doe";
string fullName = firstName + lastName;
cout << fullName; 
```

add a space with quotes (" ")
```cpp
string firstName = "John";
string lastName = "Doe";
string fullName = firstName + " " + lastName;
cout << fullName;
```

You could append its faster than the + operator
`string fullName = firstName.append(lastName);`

### Length

If you need to know the length of a string you can use the `length() function`

`string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
cout << "The length of the txt string is: " << txt.length();`

Notice, the format for the `length` function is `STRING_NAME.LENGTH();`

### Access Strings 

You can access specific characters in a string with square brackets after the string name `[]`
```cpp
string myString = "Hello";
cout << myString[0];
// Outputs H
```
***Note:*** String indexes start with 0: [0] is the first character. [1] is the second character, etc.

## Getline

Alot of times when working with `cin >>` to read strings youll have a hard time because of the way it handles **whitespace** (blank spaces, tabs, indents ,line breaks)

When the `cin` function is reading numeric data leading whitespace is ignored and the read continues until a non numeric character is encountered.

When `cin` is reading non numeric data or data defined as a string it still skips leading white spaces but since it encountered that whitespace within the string it will stop.

Example

```cpp

string firstname 
cin >> firstname
cout << firstname
```

if my first name were mary lou it would only out-put `Mary`

**`getline(cin, STRING_NAME)`** Is important because it include spaces it doesnt ignore the white space and stop inputing the string to the computer.




