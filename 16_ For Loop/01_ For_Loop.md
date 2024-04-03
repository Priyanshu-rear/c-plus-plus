# C++ For Loop <hr>

## C++ For Loop
When you know exactly how many times you want to loop through a block of code, use the `for` loop instead of a while `loop`:

### Syntax
```c++
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
```
Statement 1 is executed (one time) before the execution of the code block. <br>

Statement 2 defines the condition for executing the code block. <br>

Statement 3 is executed (every time) after the code block has been executed. <br>

The example below will print the numbers 0 to 4:

### Example
```c++
for (int i = 0; i < 5; i++) {
  cout << i << "\n";
}
```
#### Example explained
Statement 1 sets a variable before the loop starts (int i = 0).

Statement 2 defines the condition for the loop to run (i must be less than 5). If the condition is true, the loop will start over again, if it is false, the loop will end.

Statement 3 increases a value (i++) each time the code block in the loop has been executed.

## Another Example
This example will only print even values between 0 and 10:

### Example
```c++
for (int i = 0; i <= 10; i = i + 2) {
  cout << i << "\n";
}
```
## Nested Loops
It is also possible to place a loop inside another loop. This is called a `nested loop`.

The "inner loop" will be executed one time for each iteration of the "outer loop":

### Example
```c++
// Outer loop
for (int i = 1; i <= 2; ++i) {
  cout << "Outer: " << i << "\n"; // Executes 2 times

  // Inner loop
  for (int j = 1; j <= 3; ++j) {
    cout << " Inner: " << j << "\n"; // Executes 6 times (2 * 3)
  }
}
```
## The foreach Loop
There is also a "**for-each loop**" (introduced in C++ version 11 (2011), which is used exclusively to loop through elements in an array (or other data sets):

### Syntax
```c++
for (type variableName : arrayName) {
  // code block to be executed
}
```
The following example outputs all elements in an array, using a "**for-each** loop":

### Example
```c++
int myNumbers[5] = {10, 20, 30, 40, 50};
for (int i : myNumbers) {
  cout << i << "\n";
}
```
**Note**: Don't worry if you don't understand the example above. You will learn more about arrays in the <ins>C++ Arrays chapter</ins>.