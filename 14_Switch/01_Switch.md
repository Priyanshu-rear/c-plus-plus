# C++ Switch 
<hr>

## C++ Switch Statements
Use the `switch` statement to select one of many code blocks to be executed.

Syntax
```c++
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```
This is how it works:<br>
* The `switch` expression is evaluated once <br>
* The value of the expression is compared with the values of each `case` <br>
* If there is a match, the associated block of code is executed <br>
* The `break` and `default` keywords are optional, and will be described later in this chapter<br>
The example below uses the weekday number to calculate the weekday name:

### Example 
```c++
int day = 4;
switch (day) { 
  case 1:
    cout << "Monday";
    break;
  case 2:
    cout << "Tuesday";
    break;
  case 3:
    cout << "Wednesday";
    break;
  case 4:
    cout << "Thursday";
    break;
  case 5:
    cout << "Friday";
    break;
  case 6:
    cout << "Saturday";
    break;
  case 7:
    cout << "Sunday";
    break;
}
// Outputs "Thursday" (day 4)
```
## The break Keyword
When C++ reaches a break keyword, it breaks out of the switch block. <br>

This will stop the execution of more code and case testing inside the block.<br>

When a match is found, and the job is done, it's time for a break. There is no need for more testing.<br>

A break can save a lot of execution time because it "ignores" the execution of all the rest of the code in the switch block.

## The default Keyword
The `default` keyword specifies some code to run if there is no case match:

Example
```c++
int day = 4;
switch (day) {
  case 6:
    cout << "Today is Saturday";
    break;
  case 7:
    cout << "Today is Sunday";
    break;
  default:
    cout << "Looking forward to the Weekend";
}
// Outputs "Looking forward to the Weekend"```