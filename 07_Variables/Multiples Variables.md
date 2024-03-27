# C++ Declare Multiple Variables
## Declare Many Variables
To declare more than one variable of the **same type**, use a comma-separated list:

### Example
```c++
int x = 5, y = 6, z = 50;
cout << x + y + z;
```


## One Value to Multiple Variables
You can also assign the **same value** to multiple variables in one line:

### Example
```c++
int x, y, z;
x = y = z = 50;
cout << x + y + z;
```