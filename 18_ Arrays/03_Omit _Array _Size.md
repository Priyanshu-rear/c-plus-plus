# C++ Omit Array Size <hr>

## Omit Array Size
In C++, you don't have to specify the size of the array. The compiler is smart enough to determine the size of the array based on the number of inserted values:
```c++
string cars[] = {"Volvo", "BMW", "Ford"}; // Three array elements
```
The example above is equal to:
```c++
string cars[3] = {"Volvo", "BMW", "Ford"}; // Also three array elements
```
However, the last approach is considered as "good practice", because it will reduce the chance of errors in your program.

### Omit Elements on Declaration
It is also possible to declare an array without specifying the elements on declaration, and add them later:

### Example
```c++
string cars[5];
cars[0] = "Volvo";
cars[1] = "BMW";
...
```