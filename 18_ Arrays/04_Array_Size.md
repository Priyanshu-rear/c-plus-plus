# C++ Array Size <hr>
## Get the Size of an Array
To get the size of an array, you can use the sizeof() operator:

### Example
```c++
int myNumbers[5] = {10, 20, 30, 40, 50};
cout << sizeof(myNumbers);
```
Result:

20
Why did the result show `20` instead of `5`, when the array contains 5 elements?

It is because the `sizeof()` operator returns the size of a type in **bytes**.

You learned from the<u> Data Types chapter</u> that an `int` type is usually 4 bytes, so from the example above, 4 x 5 (4 bytes x 5 elements) = **20 bytes**.

**To find out how many elements an array has**, you have to divide the size of the array by the size of the data type it contains:

### Example
```c++
int myNumbers[5] = {10, 20, 30, 40, 50};
int getArrayLength = sizeof(myNumbers) / sizeof(int);
cout << getArrayLength;
```
Result:

5

## Loop Through an Array with sizeof()
In the Arrays and Loops Chapter, we wrote the size of the array in the loop condition (`i < 5`). This is not ideal, since it will only work for arrays of a specified size.

However, by using the `sizeof()` approach from the example above, we can now make loops that work for arrays of any size, which is more sustainable.

Instead of writing:
```c++
int myNumbers[5] = {10, 20, 30, 40, 50};
for (int i = 0; i < 5; i++) {
  cout << myNumbers[i] << "\n";
}
```
It is better to write:

### Example
```c++
int myNumbers[5] = {10, 20, 30, 40, 50};
for (int i = 0; i < sizeof(myNumbers) / sizeof(int); i++) {
  cout << myNumbers[i] << "\n";
}
```
Note that, in C++ version 11 (2011), you can also use the <u>"for-each" loop </u>:

### Example
```c++
int myNumbers[5] = {10, 20, 30, 40, 50};
for (int i : myNumbers) {
  cout << i << "\n";
}
```
It is good to know the different ways to loop through an array, since you may encounter them all in different programs.