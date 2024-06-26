# C++ Access Strings
## Access Strings
You can access the characters in a string by referring to its index number inside square brackets `[]`.

This example prints the **first character** in **myString:**

### Example
```c++
string myString = "Hello";
cout << myString[0];
// Outputs H
```

>**Note:** String indexes start with 0: [0] is the first character. [1] is the second character, etc.

This example prints the **second character** in **myString:**

### Example
```c++
string myString = "Hello";
cout << myString[1];
// Outputs e
```


## Change String Characters
To change the value of a specific character in a string, refer to the index number, and use single quotes:

### Example
```c++
string myString = "Hello";
myString[0] = 'J';
cout << myString;
// Outputs Jello instead of Hello
```